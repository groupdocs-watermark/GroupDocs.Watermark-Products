---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:49
draft: false

lang: it
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Libreria di filigrane Node.js | filigrane dei documenti"
head_description: "La soluzione Node.js protegge i documenti aziendali con filigrane di testo e immagini. Sono supportati i formati più diffusi come PDF, Word, Excel, PowerPoint."

############################# Header ############################
title: "Accesso alla tecnologia di filigrana in Node.js tramite Java soluzioni"
description: "Proteggi la tua proprietà intellettuale e previeni le copie non autorizzate con questa soluzione Node.js. Consente agli utenti di aggiungere facilmente filigrane ai documenti aziendali in vari formati, tra cui PDF, Word, Excel, PowerPoint, immagini ecc."
words:
  for: "per"

actions:
  main: "Usa NPM per scaricare gratuitamente"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.watermark"
  alt: "Licenze"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
  title: "Pronto per iniziare?"
  description: "Prova le funzioni GroupDocs.Watermark gratuitamente o richiedi una licenza"

release:
  title: "Rilasciata la versione {0}"
  notes: "Scopri cosa c'è di nuovo"
  downloads: "Download"
  link: "https://releases.groupdocs.com/watermark/nodejs-java/"

code:
  title: "Aggiungi filigrana a PDF con TypeScript"
  more: "Altri esempi"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.watermark"
  content: |
    ```javascript {style=abap}

    // Istanzia Watermarker passando il percorso PDF
    let loadOptions = new PdfLoadOptions();
    let watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Personalizza le opzioni della filigrana
    let textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Applica filigrana al documento PDF
    watermarker.add(textWatermark);

    // Salva il documento dei risultati
    watermarker.save("result.pdf");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark a colpo d'occhio"
  description: "Libreria TypeScript Node.js per la filigrana"
  features:
    # feature loop
    - title: "Filigrana del file Node.js"
      content: "Proteggi i tuoi documenti aziendali con GroupDocs.Watermark for Node.js via Java. Aggiungi testo, immagini, diagrammi o allegati e-mail come filigrane in vari formati di file."

    # feature loop
    - title: "Personalizza le filigrane per le tue esigenze"
      content: "GroupDocs.Watermark for Node.js via Java offre ampie opzioni di personalizzazione per le filigrane. La messa a punto degli stili di testo (grassetto, corsivo, font) e delle proprietà delle immagini (rotazione, ecc.) consente di personalizzare l'elaborazione dei documenti."

    # feature loop
    - title: "Supporto completo per i formati"
      content: "GroupDocs.Watermark for Node.js via Java si integra perfettamente con un'ampia gamma di formati di file, tra cui: PDF, MS Office come Word, Excel, PowerPoint, immagini come JPEG, PNG, GIF, BMP, Visio diagrammi, e-mail ecc. Potenzia l'elaborazione dei documenti per raggiungere gli obiettivi aziendali."

    # feature loop
    - title: "Potente ricerca e aggiornamento della filigrana"
      content: "Ottieni e aggiorna le filigrane esistenti nei documenti con filigrana. Modifica testo, stile, contenuto dell'immagine o rimuovili completamente. GroupDocs.Watermark for Node.js via Java offre un'ampia gamma di elaborazione delle filigrane."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indipendenza dalla piattaforma"
  description: "GroupDocs.Watermark for Node.js via Java si integra facilmente con vari sistemi operativi e gestori di pacchetti."
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
    GroupDocs.Watermark for Node.js via Java consente di elaborare una vasta gamma di formati di file. [Esplora l'elenco completo](https://docs.groupdocs.com/watermark/java/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Node.js via Java: Set di funzionalità"
  description: "Potenzia una solida sicurezza dei documenti attraverso la filigrana programmatica. Supporta diversi formati di file, tra cui: PDF, DOCX, XLSX, PPTX e formati di immagine (PNG, JPG, ecc.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Controllo preciso della filigrana"
      content: "Manipola con precisione le filigrane aggiungendole o rimuovendole da sezioni specifiche, interi documenti o singoli allegati e forme all'interno di diversi formati di file."

    # feature loop
    - icon: "watermark_style"
      title: "Personalizzazione dell'aspetto della filigrana"
      content: "Esercita un controllo dettagliato sull'estetica della filigrana modificando attributi come colore, carattere, opacità, rotazione e posizionamento all'interno del documento."

    # feature loop
    - icon: "hidden_print"
      title: "Stampa PDF Watermark"
      content: "Implementa una filigrana invisibile durante la normale visualizzazione dei documenti ma che diventa evidente solo durante il processo di stampa, migliorando la sicurezza dei documenti in modo discreto."

    # feature loop
    - icon: "image_only"
      title: "Filigrana specifica per immagini"
      content: "Filigrana immagini specifiche all'interno di un documento utilizzando la nostra soluzione. Scegli di incorporare le filigrane in una sezione designata (ad esempio, pagina, diapositiva) o nell'intero documento."

    # feature loop
    - icon: "image_frame"
      title: "Filigrana per immagini a più fotogrammi"
      content: "Applica le filigrane in modo selettivo a fotogrammi specifici all'interno di un formato di immagine a più fotogrammi, garantendo un controllo granulare sul posizionamento della filigrana."

    # feature loop
    - icon: "attachments"
      title: "Protezione completa dei contenuti"
      content: "Estendi la protezione a vari elementi del documento, come gli allegati all'interno dei documenti Excel e le forme delle immagini all'interno delle presentazioni, fornendo un ulteriore livello di sicurezza."

    # feature loop
    - icon: "pdf_objects"
      title: "Filigrana avanzata in PDF"
      content: "Filigrana diverse aree di PDF s, tra cui Bleed Box, Art Box, Crop Box, Trim Box ecc."

    # feature loop
    - icon: "doc_background"
      title: "Filigrana dell'immagine di sfondo"
      content: "Gestisci le filigrane all'interno delle immagini di sfondo di fogli di calcolo e presentazioni, offrendo opzioni di personalizzazione aggiuntive per le misure di sicurezza visiva."

    # feature loop
    - icon: "unreadable_characters"
      title: "Filigrana di testo con caratteri illeggibili"
      content: "Utilizza caratteri illeggibili all'interno delle filigrane di testo incorporate nelle presentazioni, rafforzando la sicurezza rendendo l'estrazione di filigrane non autorizzata molto più difficile."

    # feature loop
    - icon: "watermark_text_search"
      title: "Ricerca avanzata con filigrana"
      content: "Utilizza funzionalità di ricerca complete per individuare le filigrane all'interno dei documenti in base a parametri specifici o combinando vari criteri, consentendo un recupero e una gestione efficienti."

    # feature loop
    - icon: "watermark_image_search"
      title: "Rilevamento della filigrana di immagini simili"
      content: "Trova immagini con filigrana simili all'interno di documenti che assomigliano visivamente a un'immagine sorgente."

    # feature loop
    - icon: "document_info"
      title: "Estrazione programmatica delle informazioni sui documenti"
      content: "Estrai metadati importanti a livello di programmazione, inclusi i dettagli di configurazione della pagina e altre informazioni sui documenti per i formati di file supportati."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Esempi di codice"
  description: "Scopri gli esempi di codice che mostrano le funzionalità comuni di GroupDocs.Watermark for Node.js via Java"
  items:
    # code sample loop
    - title: "Filigrana un documento con un'immagine"
      content: |
        Sfrutta GroupDocs.Watermark for Node.js via Java per migliorare la sicurezza dei documenti aggiungendo filigrane alle immagini. Per saperne di più: [Filigrane dell'immagine](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Come proteggere il file con la filigrana dell'immagine.">}}
        ```javascript {style=abap}
        // Carica il documento sorgente su Watermarker
        let watermarker = new Watermarker("document.pdf");
        
        // Specifica il percorso di un'immagine con filigrana
        let watermark = new ImageWatermark("watermark.jpg");

        // Proteggi il file e salvalo
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Cerca e modifica filigrane esistenti"
      content: |
        GroupDocs.Watermark for Node.js via Java consente di gestire le filigrane dei documenti. Seleziona le filigrane, modifica le loro proprietà. Scopri come: [Modificare le filigrane](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Ricerca e modifica delle filigrane.">}}
        ```javascript {style=abap}   
        // Carica il documento sorgente
        let watermarker = new Watermarker("document.pdf");

        // Cerca filigrane da aggiornare
        let searchCriteria = new TextSearchCriteria("test", false);                               
        let watermarks = watermarker.search(searchCriteria); 

        // Aggiornare le proprietà desiderate
        watermarks.forEach((watermark)
        {  
            watermark.setText("New Text");
        }

        // Salva il documento modificato in un percorso specificato
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
