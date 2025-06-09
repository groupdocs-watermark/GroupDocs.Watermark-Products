
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:30
draft: false
lang: it
format: Xlsx
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Rileva Filigrane nei File Excel XLSX"
head_description: "Trova rapidamente filigrane nascoste utilizzando GroupDocs.Watermark for Python via .NET nei documenti Excel."

############################# Header ############################
title: "Trova Filigrane nei Fogli XLSX" 
description: "Cerca e gestisci facilmente le filigrane con GroupDocs.Watermark for Python via .NET."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica da PyPi gratuitamente"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Cosa Può Fare GroupDocs.Watermark for Python via .NET?"
    link: "/watermark/python-net/"
    link_title: "Scopri di più"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET semplifica la gestione delle filigrane utilizzando Python. Aggiungilo ai tuoi progetti Python per rilevare, aggiornare o rimuovere filigrane in vari formati come Word, Excel e PDF.

############################# Steps ############################
steps:
    enable: true
    title: "Rileva le Filigrane di Xlsx Utilizzando Python"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/python-net/)** facilita la rilevazione delle filigrane in diversi tipi di documenti aziendali. Aggiungi questo strumento al tuo progetto Python per abilitare le funzionalità di rilevamento delle filigrane.
      
      1. Per iniziare, inizializza la classe **Watermarker** e carica il tuo documento Xlsx utilizzando un percorso di file, uno stream di file o un array di byte. Questo prepara il file per la ricerca delle filigrane.
      2. Per restringere la ricerca, utilizza la classe **SearchCriteria**. Per le filigrane di immagini, fornisci un'immagine di esempio. Per il testo, imposta dettagli come font, dimensione, colore o altri attributi correlati.
      3. Chiama il metodo **Search** dall'istanza di **Watermarker** per avviare la ricerca. Restituisce un elenco di elementi di filigrana trovati su cui lavorare.
      4. Con l'elenco degli elementi di filigrana, puoi rimuoverli o modificarli secondo necessità. Ad esempio, potresti voler aggiornare la loro dimensione o testo.
   
    code:
      platform: "python-net"
      copy_title: "Copia"
      install:
        command: |
        command: "pip install groupdocs-watermark-net"
        copy_tip: "clicca per copiare"
        copy_done: "copiato"
      links:
        #  loop
        - title: "Altri esempi"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
        #  loop
        - title: "Documentazione"
          link: "https://docs.groupdocs.com/watermark/python-net/"
          
      content: |
        ```python {style=abap}
        # Cerca i filigrane di testo all'interno di XLSX
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Crea un'istanza di Watermarker utilizzando il percorso di XLSX
        with gw.Watermarker("input.xlsx") as watermarker:

            # Utilizza le impostazioni di ricerca per trovare le filigrane
            search_criteria = gwss.TextSearchCriteria("Watermark text", False)
            possible_watermarks = watermarker.search(search_criteria)

            # Gestisci i risultati delle filigrane trovate
            print("\nFound {0} possible watermark(s).".format(len(possible_watermarks)))
       
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "Rilevazione Avanzata delle Filigrane in Python con GroupDocs.Watermark"
  description: "Esplora potenti opzioni di ricerca delle filigrane nell'API GroupDocs.Watermark, progettata per l'uso in progetti Python."
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "Ricerca di Filigrane in Python"
  features:
    # feature loop
    - title: "Rilevamento delle Filigrane Veloce e Semplice"
      content: "Utilizza GroupDocs.Watermark per trovare rapidamente le filigrane nel tuo codice Python. Il motore di ricerca intelligente ti aiuta a localizzare le filigrane con efficienza."

    # feature loop
    - title: "Trova Filigrane Specifiche con Precisione"
      content: "Proteggi i tuoi file trovando filigrane in base a colore, dimensione o posizione. GroupDocs.Watermark semplifica la configurazione dei filtri di ricerca in Python."

    # feature loop
    - title: "Strumenti Python per un Controllo Completo delle Filigrane"
      content: "Aggiungi GroupDocs.Watermark alle tue app Python per cercare, ispezionare e monitorare l'uso delle filigrane. Ottimo per audit, branding o protezione dei contenuti."
      
  code_samples:
    # code sample loop
    - title: "Esempio Python: Flusso Completo di Rilevazione delle Filigrane"
      content: |
        Scopri come utilizzare GroupDocs.Watermark in Python per cercare attraverso i documenti, gestire più formati e utilizzare filtri complessi.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # Imposta la tua app Python e carica il documento
        load_options = gwos.SpreadsheetLoadOptions()
        with gw.Watermarker("source.xlsx", load_options) as watermarker:

            # Definisci che tipo di filigrana cercare
            criteria = gwss.ImageColorHistogramSearchCriteria("watermark.png")
            criteria.MaxDifference = 0.5
            criteria.bins_count = 2

            # Esegui la ricerca e raccogli i dati delle filigrane
            possible_watermarks = watermarker.search(criteria)

            # Utilizza le informazioni trovate per ulteriori passi come rimozione o revisione
            print("Found {0} possible watermark(s).".format(len(possible_watermarks)))        
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Pronto per iniziare?"
  description: "Prova le funzioni GroupDocs.Watermark gratuitamente o richiedi una licenza"
  items:
    #  loop
    - title: "PyPi scarica"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      color: "red"
        #  loop
    - title: "Licenze"
      link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Rileva Filigrane nei Tipi di File Supportati"
    exclude: "XLSX"
    description: "Utilizza GroupDocs.Watermark for Python via .NET per rilevare filigrane in diversi tipi di documenti con facilità."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/python-net/search//pdf/"
          description: "Formato documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/python-net/search//word/"
          description: "MS Word e documenti Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/python-net/search//excel/"
          description: "MS Excel e fogli di calcolo Open Office"

        # format loop 4
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/search//powerpoint/"
          description: "MS PowerPoint e presentazioni Open Office"

        # format loop 5
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/python-net/search//docx/"
          description: "Documento XML aperto Microsoft Word"
          
        # format loop 6
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/python-net/search//pptx/"
          description: "PowerPoint Presentazione XML aperta"
          
        # format loop 7
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/python-net/search//xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"

        # format loop 8
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/python-net/search//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/python-net/search//xls/"
          description: "Cartella di lavoro Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/python-net/search//ppt/"
          description: "PowerPoint Presentazione 97-2003"

        # format loop 11
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/python-net/search//rtf/"
          description: "Formato RTF"

---