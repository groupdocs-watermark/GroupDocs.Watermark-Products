
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:20
draft: false
lang: it
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Sblocca Excel I segreti delle filigrane dei fogli di calcolo"
head_description: "Scopri la potenza di GroupDocs.Watermark for Node.js via Java per recuperare facilmente le filigrane dai documenti."

############################# Header ############################
title: "Rivela le filigrane nascoste nei Excel fogli di calcolo" 
description: "Scopri le filigrane nascoste nei tuoi documenti con GroupDocs.Watermark for Node.js via Java."
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Ottieni da NPM"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java Informazioni di base"
    link: "/watermark/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       Sblocca il potenziale di GroupDocs.Watermark for Node.js via Java nella gestione delle filigrane su Node.js via Java. Genera, aggiorna, ottieni ed elimina facilmente filigrane da vari formati di file, tra cui PDF, Word, Excel, PowerPoint e altro ancora.

############################# Steps ############################
steps:
    enable: true
    title: "Ottieni in modo efficiente filigrane nei file Excel con GroupDocs.Watermark"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** semplifica il processo di recupero delle filigrane incorporate in vari formati di documenti aziendali. Integra perfettamente GroupDocs.Watermark nelle tue applicazioni Node.js via Java per potenziarle con solide funzionalità di rilevamento della filigrana.
      
      1. Per sfruttare le funzionalità di GroupDocs.Watermark, crea un'istanza della classe **Watermarker** e fornisci il percorso del file Excel, il flusso di file o il flusso di byte come input. Questa azione carica il documento per l'analisi della filigrana.
      2. Per l'identificazione mirata della filigrana, utilizzare l'oggetto **SearchCriteria**. Specificare un'immagine per individuare filigrane di immagini simili. In alternativa, per le filigrane testuali, definire il contenuto del testo, le proprietà del carattere, gli attributi del colore e altri parametri rilevanti per affinare i criteri di ricerca.
      3. Utilizza il metodo **Search** dell'oggetto **Watermarker** per avviare il processo di rilevamento della filigrana all'interno del documento caricato. Questa funzione restituisce una raccolta di oggetti che rappresentano potenziali filigrane, consentendo un'ulteriore elaborazione.
      4. La raccolta recuperata di oggetti filigrana ti offre molte possibilità. Puoi rimuovere filigrane indesiderate o modificarne le proprietà. Cambia contenuto, sposta una filigrana su una pagina e molto altro.
   
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

        // Ottieni l'elenco delle filigrane di testo per EXCEL

        // Istanzia la classe Watermarker
        const watermarker = new groupdocs.watermark.Watermarker("input.xslx");
        
        // Ottieni filigrane in base ai criteri del testo
        const searchCriteria = new groupdocs.watermark.TextSearchCriteria("test", false);
        const watermarks = watermarker.search(searchCriteria);

        // Utilizza le informazioni sulle filigrane
        console.log(`Found ${watermarks.getCount()} possible watermark(s).`);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Semplifica la ricerca della filigrana con GroupDocs.Watermark in Node.js"
  description: "Impara a implementare funzionalità avanzate di ricerca con filigrana nelle tue applicazioni Node.js con GroupDocs.Watermark, ottimizzando la gestione dei documenti entro Node.js via Java."
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "Cerca filigrane in Node.js"
  features:
    # feature loop
    - title: "Rilevamento avanzato della filigrana in Node.js"
      content: "Utilizza GroupDocs.Watermark per migliorare la tua capacità di rilevare e identificare le filigrane in qualsiasi formato di documento. Effettua ricerche in modo efficiente utilizzando sofisticate opzioni di filtro."

    # feature loop
    - title: "API Node.js per ricerche personalizzate con filigrana"
      content: "Personalizza le tue operazioni di ricerca con la nostra API Node.js. Trova le filigrane specificando parametri dettagliati come posizione, opacità e tipo di contenuto, ottimizzando i flussi di lavoro dei documenti."

    # feature loop
    - title: "Recupero e analisi efficienti delle filigrane"
      content: "Con GroupDocs.Watermark, estrai e analizza rapidamente le filigrane da vari documenti. La nostra API supporta il recupero rapido, aiutandoti a mantenere la conformità e la coerenza del marchio."
      
  code_samples:
    # code sample loop
    - title: "Esempio Node.js: ricerca efficiente con filigrana"
      content: |
        Scopri come utilizzare Node.js con GroupDocs.Watermark per cercare filigrane in diversi tipi di documenti, dimostrando l'uso di criteri di ricerca dinamici per risultati precisi.
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Inizializza l'ambiente Node.js e carica il documento di destinazione
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  Imposta le query di ricerca utilizzando criteri flessibili per trovare filigrane specifiche
            const criteria = new groupdocsWatermark.TextFormattingSearchCriteria();
            criteria.setForegroundColorRange(new groupdocsWatermark.ColorRange());
            criteria.getForegroundColorRange().setMinHue(-5);
            criteria.getForegroundColorRange().setMaxHue(10);
            criteria.setBackgroundColorRange(new groupdocsWatermark.ColorRange());
            criteria.getBackgroundColorRange().setEmpty(true);
            criteria.setFontName("Arial");
            criteria.setMinFontSize(19);
            criteria.setMaxFontSize(42);
            criteria.setFontBold(true);
  
            //  Esegui la ricerca e raccogli le filigrane che soddisfano i criteri
            const watermarks = watermarker.search(criteria);

            //  Elabora e analizza i risultati per determinare le azioni necessarie
            console.log(`Found ${watermarks.getCount()} possible watermark(s).`);
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
    title: "Esplora diversi formati"
    exclude: "EXCEL"
    description: "Scopri, recupera e gestisci le filigrane in diversi formati di file con facilità."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/get//pdf/"
          description: "Formato documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/nodejs-java/get//word/"
          description: "MS Word e documenti Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/get//excel/"
          description: "MS Excel e fogli di calcolo Open Office"

        # format loop 4
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/get//powerpoint/"
          description: "MS PowerPoint e presentazioni Open Office"

        # format loop 5
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/get//docx/"
          description: "Documento XML aperto Microsoft Word"
          
        # format loop 6
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/get//pptx/"
          description: "PowerPoint Presentazione XML aperta"
          
        # format loop 7
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/get//xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"

        # format loop 8
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/get//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/get//xls/"
          description: "Cartella di lavoro Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/get//ppt/"
          description: "PowerPoint Presentazione 97-2003"

        # format loop 11
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/get//rtf/"
          description: "Formato RTF"

---