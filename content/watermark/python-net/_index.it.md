---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:49
draft: false

lang: it
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"
    # supported_platforms loop
    - title: "Python"
      tag: "python-net"

############################# Head ############################
head_title: "Python Libreria di filigrane | Filigrane dei documenti"
head_description: "Python protegge i documenti aziendali con filigrane di testo e immagini. Sono supportati formati di file come PDF, Word, Excel e PowerPoint."

############################# Header ############################
title: "Accedi alla tecnologia di filigrana di Python via .NET"
description: "Proteggi i tuoi dati e previeni la copia non autorizzata con questa soluzione Python. Aggiungi facilmente filigrane ai documenti aziendali in vari formati, tra cui PDF, Word, Excel, PowerPoint, immagini, ecc."
words:
  for: "per"

actions:
  main: "Scarica PyPi gratuitamente"
  main_link: "https://pypi.org/project/groupdocs-watermark-net/"
  alt: "Licenze"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
  title: "Pronto per iniziare?"
  description: "Prova le funzioni GroupDocs.Watermark gratuitamente o richiedi una licenza"

release:
  title: "Rilasciata la versione {0}"
  notes: "Scopri cosa c'è di nuovo"
  downloads: "Download"
  link: "https://releases.groupdocs.com/watermark/python-net/"

code:
  title: "Aggiungi filigrana al PDF utilizzando Python"
  more: "Altri esempi"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
  install: "pip install groupdocs-watermark-net"
  content: |
    ```python {style=abap}

    import groupdocs.watermark as gw
    import groupdocs.watermark.watermarks as gww
    import groupdocs.watermark.options.pdf as gwop
    import groupdocs.watermark.common as gwc

    # Istanzia Watermarker passando il percorso PDF
    pdf_lo = gwop.PdfLoadOptions()
    with gw.Watermarker("source.pdf", pdf_lo) as watermarker:
        options = gwop.PdfArtifactWatermarkOptions()

        # Personalizza le opzioni della filigrana
        text_watermark = 
            gww.TextWatermark("Approved", gww.Font("Arial", 8.0))
        text_watermark.horizontal_alignment = 
            gwc.HorizontalAlignment.RIGHT

        # Applica filigrana al documento PDF
        watermarker.add(text_watermark, options)

        # Salva il documento dei risultati
        watermarker.save("result.pdf")

    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark a colpo d'occhio"
  description: "Libreria Python per la filigrana"
  features:
    # feature loop
    - title: "Python Filigrana del documento"
      content: "Proteggi i tuoi dati sensibili con GroupDocs.Watermark for Python via .NET. Inserisci testo o immagini in vari formati di file come filigrane."

    # feature loop
    - title: "Personalizza filigrane"
      content: "Molte opzioni di personalizzazione sono disponibili in GroupDocs.Watermark for Python via .NET. Imposta gli stili del testo (grassetto, corsivo, carattere) o le proprietà dell'immagine come dimensioni o rotazione per ottimizzare la filigrana del documento."

    # feature loop
    - title: "Supporto dei formati di file più diffusi"
      content: "GroupDocs.Watermark for Python via .NET supporta un'ampia gamma di formati di file, inclusi PDF, documenti MS Office come Word, Excel, PowerPoint e immagini come JPEG, PNG, GIF, BMP, diagrammi Visio, e-mail, ecc. Migliora l'elaborazione dei documenti per soddisfare le esigenze del business obiettivi."

    # feature loop
    - title: "Ricerca e aggiornamento filigrana"
      content: "Recupera e aggiorna le filigrane inserite nei documenti. Modifica lo stile del testo, il contenuto dell'immagine o rimuovili completamente. GroupDocs.Watermark for Python via .NET offre un'ampia gamma di funzionalità di elaborazione della filigrana."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indipendenza dalla piattaforma"
  description: "GroupDocs.Watermark for Python via .NET si integra perfettamente con vari sistemi operativi e gestori di pacchetti."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Formati di file supportati"
  description: |
    GroupDocs.Watermark for Python via .NET ti consente di elaborare una vasta gamma di formati di file. [Esplora l'elenco completo](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formati Microsoft Office e OpenDocument
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### Immagini e grafica
        * **Formati di immagine più diffusi:** BMP, JPG, JPEG, PNG
        * **Immagini multipagina:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### Altro
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "Funzionalità di GroupDocs.Watermark for Python via .NET"
  description: "Rafforzare la sicurezza dei documenti attraverso la filigrana programmatica. Elabora diversi formati di file tra cui PDF, DOCX, XLSX, PPTX e formati di immagine (PNG, JPG, ecc.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Controllo preciso della filigrana"
      content: "Gestisci con precisione le filigrane aggiungendole o rimuovendole da sezioni specifiche, interi documenti o singoli allegati e forme all'interno di diversi formati di file."

    # feature loop
    - icon: "watermark_style"
      title: "Personalizza l'aspetto della filigrana"
      content: "Esercita un controllo capillare sull'estetica della filigrana modificando attributi come colore, carattere, opacità, rotazione e posizionamento all'interno del documento."

    # feature loop
    - icon: "hidden_print"
      title: "Stampa filigrana PDF"
      content: "Aggiungi filigrane nascoste ai normali documenti che diventano visibili solo durante il processo di stampa, migliorando la sicurezza dei documenti in modo discreto."

    # feature loop
    - icon: "image_only"
      title: "Filigrana di immagini specifiche"
      content: "Filigrana immagini specifiche all'interno di un documento utilizzando la nostra soluzione. Incorpora filigrane in una sezione designata (ad esempio, pagina, diapositiva) o nell'intero documento."

    # feature loop
    - icon: "image_frame"
      title: "Filigrane di immagini multistrato"
      content: "Aggiungi filigrane con precisione a fotogrammi specifici all'interno di un formato immagine multi-fotogramma, ottenendo un controllo granulare sul posizionamento della filigrana."

    # feature loop
    - icon: "attachments"
      title: "Protezione completa dei contenuti"
      content: "Estendi la protezione a vari elementi del documento come allegati all'interno di documenti Excel e forme di immagine all'interno delle presentazioni, fornendo un ulteriore livello di sicurezza."

    # feature loop
    - icon: "pdf_objects"
      title: "Filigrana PDF avanzata"
      content: "Filigrana su diverse aree dei PDF, tra cui Bleed Box, Art Box, Crop Box, Trim Box, ecc."

    # feature loop
    - icon: "doc_background"
      title: "Filigrana dell'immagine di sfondo"
      content: "Gestisci le filigrane all'interno delle immagini di sfondo di fogli di calcolo e presentazioni, offrendo opzioni di personalizzazione aggiuntive per le misure di sicurezza visiva."

    # feature loop
    - icon: "unreadable_characters"
      title: "Filigrana di testo con caratteri illeggibili"
      content: "Utilizza caratteri illeggibili all'interno delle filigrane di testo incorporate nelle presentazioni, rafforzando la sicurezza rendendo l'estrazione non autorizzata delle filigrane molto più complessa."

    # feature loop
    - icon: "watermark_text_search"
      title: "Ricerca avanzata di filigrane"
      content: "Utilizza funzionalità di ricerca complete per individuare le filigrane nei documenti in base a parametri specifici o combinando vari criteri."

    # feature loop
    - icon: "watermark_image_search"
      title: "Rilevamento filigrana immagine simile"
      content: "Trova immagini di filigrana simili all'interno di documenti che assomigliano visivamente a un'immagine di origine."

    # feature loop
    - icon: "document_info"
      title: "Analizzare le informazioni del documento"
      content: "Estrai i dati essenziali del documento come l'impostazione della pagina per ulteriori analisi."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Esempi di codice"
  description: "Esplora esempi di codice che mostrano le funzionalità comuni di GroupDocs.Watermark for Python via .NET."
  items:
    # code sample loop
    - title: "Filigrana un documento con un'immagine"
      content: |
        Utilizza GroupDocs.Watermark for Python via .NET per proteggere i documenti aggiungendo filigrane alle immagini. [Ulteriori informazioni](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Come proteggere il file con la filigrana dell'immagine.">}}
        ```python {style=abap}

        # Carica il documento sorgente su Watermarker
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Specifica il percorso di un'immagine con filigrana
            watermark = groupdocs.watermark.watermarks.ImageWatermark("watermark.jpg")
            watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwgroupdocs.watermark.common.VerticalAlignment.CENTER

            # Proteggi il file e salvalo
            watermarker.add(watermark)
            watermarker.save("result.pdf")
       
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Cerca e modifica filigrane esistenti"
      content: |
        GroupDocs.Watermark for Python via .NET ti consente di gestire le filigrane dei documenti. Seleziona filigrane e modifica le loro proprietà. [Scopri come](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Ricerca e modifica delle filigrane.">}}
        ```python {style=abap}

        # Carica il documento sorgente
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Cerca filigrane da aggiornare
            search_criteria = groupdocs.watermark.search.searchcriteria.TextSearchCriteria("annotation", False)
            watermarks = watermarker.search(search_criteria)
            
            # Aggiornare le proprietà desiderate
            for watermark in watermarks:
                watermark.text = "passed"

            # Salva il documento modificato in un percorso specificato
            watermarker.save("result.pdf")


        ```
        {{< /landing/code >}}

---
