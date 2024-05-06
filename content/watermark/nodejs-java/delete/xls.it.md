
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:44
draft: false
lang: it
format: Xls
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Rimozione precisa delle filigrane nei XLS fogli di calcolo"
head_description: "GroupDocs.Watermark offre un controllo granulare sull'eliminazione di filigrane specifiche."

############################# Header ############################
title: "Filigrane XLS specifiche per l'obiettivo" 
description: "Rimuovi selettivamente le filigrane indesiderate preservando quelle desiderate con GroupDocs.Watermark."
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica a NPM gratuitamente"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark consente agli sviluppatori di selezionare ed eliminare filigrane specifiche all'interno dei documenti. Questo controllo granulare garantisce una modifica precisa dei documenti, consentendo di rimuovere filigrane obsolete o irrilevanti mantenendo al contempo le informazioni cruciali. GroupDocs.Watermark si integra perfettamente con l'ambiente .NET, semplificando l'eliminazione delle filigrane per vari formati di file.

############################# Steps ############################
steps:
    enable: true
    title: "Elimina facilmente filigrane da Xls con Node.js via Java"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/nodejs-java/)** semplifica il processo di rimozione delle filigrane dai documenti aziendali. Migliora la tua applicazione Node.js via Java integrando perfettamente la nostra libreria e seguendo questi semplici passaggi:
      
      1. Avvia il processo istanziando la classe principale, **Watermarker**, con il documento Xls. La nostra versatile API elabora senza problemi i documenti, forniti come flusso o percorso locale.
      2. Sfrutta **SearchCriteria** per individuare con precisione le filigrane da risolvere. Utilizza vari parametri come immagini, testo o funzionalità di formattazione per perfezionare la ricerca. Quanto più dettagliati saranno i tuoi criteri, tanto più accurati saranno i tuoi risultati.
      3. Esegui il processo di rimozione sull'elenco delle filigrane dei documenti recuperate tramite la ricerca. Eliminali senza sforzo dal documento.
      4. Dopo aver eliminato con successo le filigrane, salva in modo sicuro il documento risultante come file locale o flusso di byte, preservandone l'integrità.
   
    code:
      platform: "net"
      copy_title: "Copia"
      install:
        command: "npm i @groupdocs/groupdocs.watermark"
        copy_tip: "clicca per copiare"
        copy_done: "copiato"
      links:
        #  loop
        - title: "Altri esempi"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
        #  loop
        - title: "Documentazione"
          link: "https://docs.groupdocs.com/watermark/nodejs-java/"
          
      content: |
        ```javascript {style=abap}

        // Elimina la filigrana dell'immagine nel documento XLS

        // Ottieni Watermarker passando il percorso XLS come argomento
        const watermarker = new groupdocs.watermark.Watermarker("input.xls");
        
        // Cancella filigrane di immagini in base ai criteri di ricerca
        const searchCriteria = 
            new groupdocs.watermark.ImageDctHashSearchCriteria("logo.png");
        const watermarks = watermarker.search(searchCriteria);
        watermarks.clear();

        // Salva il file elaborato
        watermarker.save("output.xls");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Node.js via Java API per la rimozione della filigrana | GroupDocs.Watermark"
  description: "Integra la nostra API Node.js via Java per rimuovere facilmente le filigrane dai documenti, migliorando la chiarezza e l'estetica dei documenti. Personalizzata per ambienti Node.js via Java, questa API è perfetta per le applicazioni che devono elaborare e presentare documenti puliti e privi di filigrane."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "Rimuovi filigrana"
  features:
    # feature loop
    - title: "Rimozione semplificata della filigrana per Node.js via Java"
      content: "La nostra API offre strumenti semplificati per la rimozione delle filigrane progettati specificamente per le applicazioni Node.js via Java, che consentono agli sviluppatori di migliorare la leggibilità dei documenti e l'aspetto professionale senza codifiche complesse."

    # feature loop
    - title: "Node.js via Java Pulizia della filigrana in batch"
      content: "Sfrutta la possibilità di cancellare le filigrane da più documenti in una volta sola con la nostra funzione di elaborazione in batch. Ciò è particolarmente utile per le applicazioni che devono gestire flussi di documenti di grandi dimensioni in modo rapido ed efficiente."

    # feature loop
    - title: "Modifica flessibile della filigrana tramite Node.js via Java"
      content: "Regola, modifica o rimuovi completamente le filigrane utilizzando i nostri strumenti di modifica flessibili. Questa funzionalità consente a Node.js via Java sviluppatori di adattare l'elaborazione dei documenti a specifiche esigenze aziendali o richieste dei clienti, garantendo risultati ottimali."
      
  code_samples:
    # code sample loop
    - title: "Eliminare le filigrane dell'intestazione del foglio di calcolo"
      content: |
        Questo esempio mostra come eliminare le filigrane inserite nelle intestazioni XLSX
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Carica la cartella di lavoro del foglio di calcolo
            const loadOptions = new groupdocsWatermark.SpreadsheetLoadOptions();
            const watermarker = new groupdocsWatermark.Watermarker("source.xlsx", loadOptions);

            //  Ottieni l'elenco delle sezioni dell'intestazione
            const content = watermarker.getContent(groupdocsWatermark.SpreadsheetContent.class);
            const sections = content.getWorksheets().get_Item(0).getHeadersFooters()
                .getByOfficeHeaderFooterType(groupdocsWatermark.OfficeHeaderFooterType.HeaderPrimary).getSections();
  
            //  Eliminare le filigrane dalle intestazioni
            for (const section of sections.getInnerList().toArray()) {
                section.setScript(null);
                section.setImage(null);
            }

            //  Salva cartella di lavoro cancellata
            watermarker.save("result.xlsx");
            watermarker.close();

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Pronto per iniziare?"
  description: "Prova le funzioni GroupDocs.Watermark gratuitamente o richiedi una licenza"
  items:
    #  loop
    - title: "NPM scarica"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licenze"
      link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Eliminazione precisa in tutti i formati"
    exclude: "XLS"
    description: "Scegli come target filigrane specifiche in diversi tipi di documenti con GroupDocs.Watermark."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/delete//pdf/"
          description: "Formato documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/nodejs-java/delete//word/"
          description: "MS Word e documenti Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/delete//excel/"
          description: "MS Excel e fogli di calcolo Open Office"

        # format loop 4
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/delete//powerpoint/"
          description: "MS PowerPoint e presentazioni Open Office"

        # format loop 5
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/delete//docx/"
          description: "Documento XML aperto Microsoft Word"
          
        # format loop 6
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/delete//pptx/"
          description: "PowerPoint Presentazione XML aperta"
          
        # format loop 7
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/delete//xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"

        # format loop 8
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/delete//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/delete//xls/"
          description: "Cartella di lavoro Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/delete//ppt/"
          description: "PowerPoint Presentazione 97-2003"

        # format loop 11
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/delete//rtf/"
          description: "Formato RTF"

---