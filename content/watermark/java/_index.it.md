---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:29
draft: false

lang: it
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

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

############################# Head ############################
head_title: "Java Watermark Library | aggiungere filigrane ai documenti"
head_description: "Software nativo Java per aggiungere e manipolare filigrane di testo e immagini in PDF, Word, Excel, presentazioni, Visio diagrammi, e-mail e file di immagini."

############################# Header ############################
title: "Implementa facilmente la filigrana dei documenti nei progetti Java"
description: "Migliora le tue applicazioni Java con la possibilità di aggiungere filigrane ai file utilizzando la libreria GroupDocs.Watermark. La nostra API offre filigrane personalizzabili per un'ampia gamma di formati di file popolari."
words:
  for: "per"

actions:
  main: "Download gratuito da Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "Licenze"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java/"
  title: "Pronto per iniziare?"
  description: "Prova le funzioni GroupDocs.Watermark gratuitamente o richiedi una licenza"

release:
  title: "Rilasciata la versione {0}"
  notes: "Scopri cosa c'è di nuovo"
  downloads: "Download"

code:
  title: "Filigrana PDF tramite Java"
  more: "Altri esempi"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-watermark</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Istanzia Watermarker passando il percorso PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Personalizza le opzioni della filigrana
    TextWatermark textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Applica filigrana al documento PDF
    watermarker.add(textWatermark);

    // Salva il documento dei risultati
    watermarker.save("result.pdf");
    watermarker.close();
      
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark a colpo d'occhio"
  description: "Libreria progettata per aggiungere filigrane utilizzando le tecnologie Java"
  features:
    # feature loop
    - title: "File con filigrana tramite Java"
      content: "Proteggi i tuoi documenti aziendali utilizzando GroupDocs.Watermark for Java. Aggiungi testo, immagini, diagrammi o allegati e-mail come filigrane in vari formati di file."

    # feature loop
    - title: "Personalizza le filigrane per esigenze specifiche"
      content: "GroupDocs.Watermark for Java offre ampie opzioni di personalizzazione per le filigrane. Modifica gli stili del testo (grassetto, corsivo, carattere) e le proprietà dell'immagine (rotazione, ecc.) per adattare il processo di filigrana ai tuoi obiettivi specifici."

    # feature loop
    - title: "Supporto per un ampio formato"
      content: "GroupDocs.Watermark for Java si integra perfettamente con un'ampia gamma di formati di file, tra cui: PDF, Microsoft Office (Word, Excel, PowerPoint), immagini (JPEG, PNG, GIF, BMP), Visio diagrammi ed e-mail. Migliora la sicurezza dei documenti su diversi tipi di file."

    # feature loop
    - title: "Ricerca e gestione delle filigrane senza sforzo"
      content: "Gestisci in modo efficiente le filigrane esistenti all'interno dei documenti. Individua filigrane specifiche, modificane il testo, lo stile o le immagini o rimuovile completamente. GroupDocs.Watermark for Java semplifica il flusso di lavoro per le filigrane."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indipendenza dalla piattaforma"
  description: "GroupDocs.Watermark for Java supporta diversi sistemi operativi e gestori di pacchetti."
  items:
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Formati di file supportati"
  description: |
    GroupDocs.Watermark for Java consente l'elaborazione di un'ampia gamma di formati di file. [Vedi l'elenco completo](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Java: Caratteristiche"
  description: "Proteggi i tuoi file aggiungendo filigrane. Supporta vari formati tra cui PDF, documenti Office e immagini."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Filigrana dei file"
      content: "Aggiungi o rimuovi filigrane da sezioni specifiche o interi documenti per vari formati di file supportati."

    # feature loop
    - icon: "watermark_style"
      title: "Personalizzazione della filigrana"
      content: "Personalizza l'aspetto della filigrana con opzioni come colore, carattere, rotazione e altro ancora."

    # feature loop
    - icon: "hidden_print"
      title: "Filigrana di stampa nascosta per PDF"
      content: "Aggiungi una filigrana che appare solo quando si stampa un documento PDF."

    # feature loop
    - icon: "image_only"
      title: "Filigrana selettiva delle immagini"
      content: "Filigrana tutte le immagini all'interno di una specifica sezione, pagina, diapositiva o intero documento."

    # feature loop
    - icon: "image_frame"
      title: "Filigrana su cornici di immagini specifiche"
      content: "Applica filigrane a fotogrammi specifici all'interno di un'immagine con più cornici."

    # feature loop
    - icon: "attachments"
      title: "Filigrana, allegati e forme"
      content: "Aggiungi filigrane a tutti gli allegati nei documenti Excel o a tutte le forme di immagine in Presentazioni."

    # feature loop
    - icon: "pdf_objects"
      title: "Allineamento della filigrana in PDF"
      content: "Allinea le filigrane alle diverse aree di un documento PDF, tra cui Bleed Box, Art Box, Crop Box e Trim Box."

    # feature loop
    - icon: "doc_background"
      title: "Filigrana per immagini di sfondo"
      content: "Aggiungi o rimuovi la filigrana dell'immagine di sfondo ai fogli di calcolo o alle presentazioni."

    # feature loop
    - icon: "unreadable_characters"
      title: "Protezione con caratteri illeggibili"
      content: "Proteggi le presentazioni utilizzando una filigrana di testo con caratteri illeggibili."

    # feature loop
    - icon: "watermark_text_search"
      title: "Cerca filigrane"
      content: "Ottieni l'elenco delle filigrane presentate nel file, utilizzando vari parametri tra cui le espressioni regolari."

    # feature loop
    - icon: "watermark_image_search"
      title: "Trova filigrane di immagini simili"
      content: "Individua le filigrane delle immagini che assomigliano a un'immagine specifica."

    # feature loop
    - icon: "document_info"
      title: "Estrai informazioni sul documento"
      content: "Ottieni vari dati del documento come l'impostazione della pagina per i formati di file supportati."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Esempi di codice"
  description: "Esplora esempi di codice che illustrano le funzionalità tipiche di GroupDocs.Watermark for Java"
  items:
    # code sample loop
    - title: "Filigrana un documento usando un'immagine"
      content: |
        Utilizza GroupDocs.Watermark for Java per migliorare la sicurezza dei documenti aggiungendo filigrane alle immagini. Per saperne di più: [Filigrane dell'immagine](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Come proteggere il file con la filigrana dell'immagine.">}}
        ```csharp {style=abap}
        // Carica il documento sorgente su Watermarker
        Watermarker watermarker = new Watermarker("document.pdf");
        
        // Specifica il percorso di un'immagine con filigrana
        ImageWatermark watermark = new ImageWatermark("watermark.jpg");

        // Proteggi il file e salvalo
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Modifica filigrane"
      content: |
        GroupDocs.Watermark for Java ti consente di gestire le filigrane esistenti all'interno dei documenti. Individua le filigrane specifiche e [modificane le proprietà](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Ricerca e modifica delle filigrane.">}}
        ```csharp {style=abap}   
        // Carica il documento sorgente
        Watermarker watermarker = new Watermarker("document.pdf");

        // Cerca filigrane da aggiornare
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);                               
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);                             

        // Aggiornare le proprietà desiderate
        for (PossibleWatermark watermark : watermarks)                                                           
        {  
            watermark.setText("New Text");
        }

        // Salva il documento modificato in un percorso specificato
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
