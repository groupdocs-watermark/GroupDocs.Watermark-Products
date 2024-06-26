
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
head_title: "Aggiorna le filigrane per i fogli di calcolo Excel"
head_description: "Aggiorna le filigrane nei fogli di calcolo di vari formati usando GroupDocs.Watermark for Node.js via Java. Arricchisci le tue Node.js via Java applicazioni."

############################# Header ############################
title: "Rivoluziona la filigrana dei fogli di calcolo usando Node.js via Java" 
description: "Prova la potenza di GroupDocs.Watermark for Node.js via Java. Proteggi i tuoi documenti aziendali con varie filigrane. Aggiorna le dimensioni, l'allineamento, l'angolo di rotazione, la posizione della filigrana, ecc."
subtitle: "GroupDocs.Watermark for Node.js via Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download gratuito di NPM"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "libreria GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java è una soluzione completa per la gestione delle filigrane utilizzando l'ambiente Node.js via Java. Con questo strumento, gli sviluppatori possono eseguire facilmente operazioni come aggiungere, modificare, cercare e rimuovere filigrane dai documenti in vari formati di file, tra cui PDF, Microsoft Word, Excel, PowerPoint, Visio, e-mail e formati di immagine. GroupDocs.Watermark supporta tutti i principali sistemi operativi e le versioni di Node.js.

############################# Steps ############################
steps:
    enable: true
    title: "Aggiorna filigrane in EXCEL tramite Node.js via Java"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** fornisce agli sviluppatori di Node.js via Java una solida API per l'aggiornamento programmatico delle filigrane all'interno di vari documenti EXCEL. Questa guida descrive il processo:
      
      1. Avvia il processo fornendo il tuo file EXCEL come argomento al costruttore della classe **Watermarker**. A seconda delle tue richieste, il file può essere fornito come flusso o riferimento a una posizione su disco locale.
      2. Successivamente, sfrutta l'oggetto **SearchCriteria** per identificare le filigrane specifiche che richiedono la modifica. Questo oggetto consente di individuare le filigrane in base alle proprietà desiderate.
      3. Una volta eseguita con successo la ricerca, riceverai una raccolta di filigrane pertinenti. Queste filigrane offrono un controllo granulare, consentendoti di aggiornare proprietà come dimensioni, posizionamento della pagina, contenuto del testo, combinazione di colori, dati di immagine e altro ancora.
      4. Una volta completati gli aggiornamenti della filigrana, rendere persistente il documento modificato. L'API facilita l'archiviazione utilizzando un percorso file locale o un oggetto flusso.
   
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

        // Aggiorna la filigrana di testo EXCEL

        // Fornisci l'istanza Watermarker per il file EXCEL
        const watermarker = new groupdocs.watermark.Watermarker("input.xslx");

        // Utilizza TextSearchCriteria per trovare filigrane di testo
        const searchCriteria = 
            new groupdocs.watermark.TextSearchCriteria("test", false);
        const watermarks = watermarker.search(searchCriteria);
        
        // Aggiorna la filigrana del testo
        for (const watermark of watermarks.getInnerList().toArray())
        {
            watermark.setText("passed");
        }

        // Goditi il ​​risultato
        watermarker.save("output.xslx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Padroneggiare la modifica della filigrana in PDF s con GroupDocs.Watermark"
  description: "Esplora le funzionalità API complete per regolare e gestire le filigrane in PDF s all'interno di Node.js via Java applicazioni."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Modifica filigrana"
  features:
    # feature loop
    - title: "Modifica facilmente le filigrane in PDF s"
      content: "GroupDocs.Watermark offre potenti strumenti in Node.js via Java per modificare senza problemi le filigrane esistenti nei documenti PDF. Regola posizione, trasparenza e altro con facilità."

    # feature loop
    - title: "Perfeziona i dettagli della filigrana per una maggiore precisione"
      content: "Assumi il controllo dei dettagli. La nostra API ti consente di ottimizzare l'aspetto delle filigrane, consentendo modifiche precise di dimensioni, opacità e colore nei tuoi PDF s."

    # feature loop
    - title: "Gestione semplificata delle filigrane"
      content: "La nostra API semplifica la gestione delle filigrane. Che si tratti di aggiornare o rimuovere, puoi gestire le filigrane in modo efficiente, mantenendo l'integrità del documento e soddisfacendo le tue esigenze di branding."
      
  code_samples:
    # code sample loop
    - title: "Java Esempio: Modifica filigrana PDF"
      content: |
        Questo esempio Java dimostra come modificare una filigrana esistente in un documento PDF, mostrando come regolarne le proprietà a livello di codice.
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Carica il documento PDF per l'elaborazione
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  Cerca filigrane specifiche che soddisfano i tuoi criteri
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria("test", false);
            const watermarks = watermarker.search(searchCriteria);
  
            //  Modifica le impostazioni della filigrana, come dimensione, colore e posizione
            for (const watermark of watermarks.getInnerList().toArray()) {
                watermark.getFormattedTextFragments().clear();
                watermark.getFormattedTextFragments().add("passed", 
                    new groupdocsWatermark.Font("Calibri", 19, groupdocsWatermark.FontStyle.Bold), 
                    groupdocsWatermark.Color.getRed(), groupdocsWatermark.Color.getAqua());
            }

            //  Salva il documento aggiornato su un sistema locale o trasmettilo in streaming direttamente
            watermarker.save("result.pdf");
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
    title: "Aggiorna le filigrane nei formati di file supportati"
    exclude: "EXCEL"
    description: "Aggiorna in modo efficiente le filigrane in PDF, Word, Excel e altro con GroupDocs.Watermark for Node.js via Java. I documenti con filigrana possono arricchire i tuoi processi aziendali."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/update//pdf/"
          description: "Formato documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/nodejs-java/update//word/"
          description: "MS Word e documenti Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/update//excel/"
          description: "MS Excel e fogli di calcolo Open Office"

        # format loop 4
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/update//powerpoint/"
          description: "MS PowerPoint e presentazioni Open Office"

        # format loop 5
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/update//docx/"
          description: "Documento XML aperto Microsoft Word"
          
        # format loop 6
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/update//pptx/"
          description: "PowerPoint Presentazione XML aperta"
          
        # format loop 7
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/update//xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"

        # format loop 8
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/update//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/update//xls/"
          description: "Cartella di lavoro Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/update//ppt/"
          description: "PowerPoint Presentazione 97-2003"

        # format loop 11
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/update//rtf/"
          description: "Formato RTF"

---