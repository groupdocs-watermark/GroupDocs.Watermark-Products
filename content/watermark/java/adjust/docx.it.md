
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:27:03
draft: false
lang: it
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Modifica le filigrane nei documenti DOCX - GroupDocs.Watermark"
head_description: "Modifica le filigrane in modo efficiente in diversi formati di documento utilizzando GroupDocs.Watermark. Migliora l'autenticità dei documenti."

############################# Header ############################
title: "Regola le filigrane DOCX: personalizzazione senza interruzioni" 
description: "Personalizza senza problemi i tuoi documenti con il nostro efficiente strumento di modifica delle filigrane. Migliora l'immagine del tuo marchio senza sforzo."
subtitle: "GroupDocs.Watermark for Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download gratuito di Maven"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java API"
    link: "/watermark/java/"
    link_title: "Scopri di più"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Modifica filigrane**: personalizza senza problemi i tuoi documenti con i nostri potenti strumenti di modifica. Che si tratti di regolare il posizionamento o di modificare il contenuto, ottieni gli effetti di filigrana desiderati senza sforzo.

############################# Steps ############################
steps:
    enable: true
    title: "Modifica le filigrane dei documenti Docx usando Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** consente agli sviluppatori Java di modificare facilmente le filigrane in molti documenti utilizzando le loro applicazioni. Ecco una guida rapida:
      
      1. **Watermarker**. Fornisci un byte o un flusso di file o un percorso del disco locale.
      2. **SearchCriteria** per identificare le filigrane con le proprietà specifiche aggiunte in precedenza al documento.
      3. Dopo la ricerca, riceverai un elenco di filigrane pertinenti. Puoi quindi modificarne le proprietà, tra cui dimensioni, allineamento della pagina, testo, colore, contenuto dell'immagine e altro ancora. Ciò offre un elevato grado di personalizzazione dei dati.
      4. Una volta terminata la regolazione delle filigrane, salva il documento aggiornato. Puoi utilizzare un percorso di file locale o uno stream per memorizzare il risultato.
   
    code:
      platform: "net"
      copy_title: "Copia"
      install:
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-watermark</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "clicca per copiare"
        copy_done: "copiato"
      links:
        #  loop
        - title: "Altri esempi"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
        #  loop
        - title: "Documentazione"
          link: "https://docs.groupdocs.com/watermark/java/"
          
      content: |
        ```java {style=abap}
        // Regola la filigrana dell'immagine DOCX

        // Crea un'istanza di Watermarker con DOCX
        Watermarker watermarker = new Watermarker("input.docx");
        
        // Inizializza i criteri di ricerca in modo che corrispondano a una particolare immagine
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);

        for (PossibleWatermark watermark : watermarks)
        {
            // Sostituisci l'immagine trovata
            watermark.setImageData(imageData);
        }

        // Salva il file modificato
        watermarker.save("output.docx");
        
        ```
        
############################# More features ############################
more_features:
  enable: true
  title: "Gestione avanzata della filigrana DOCX per le applicazioni Java"
  description: "L'API GroupDocs.Watermark consente agli sviluppatori di integrare senza problemi la funzionalità di watermarking nelle loro applicazioni Java. Supporta l'aggiunta, la modifica, la rimozione e la ricerca di filigrane in un'ampia gamma di formati di documenti."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Regolazione della filigrana"
  features:
    # feature loop
    - title: "Semplice integrazione con filigrana"
      content: "GroupDocs.Watermark semplifica il processo di aggiunta di filigrane diverse a vari documenti e file aziendali all'interno di Java applicazioni. Gli sviluppatori possono non solo applicare filigrane, ma anche aggiornare o rimuovere quelle esistenti a livello di programmazione."

    # feature loop
    - title: "Personalizzazione granulare della filigrana"
      content: "L'API offre ampie opzioni di personalizzazione per le filigrane. Gli sviluppatori possono facilmente regolare dimensioni, rotazione, colore, carattere, stili e altre proprietà per ottenere l'effetto visivo desiderato."

    # feature loop
    - title: "Sfruttamento delle funzionalità native dei documenti DOCX"
      content: "A seconda del formato del documento di destinazione, gli sviluppatori possono utilizzare funzionalità native per il posizionamento della filigrana. Queste funzionalità potrebbero includere lo sfondo della pagina del documento, le annotazioni, le intestazioni o altri oggetti come contenitori di filigrane."
      
  code_samples:
    # code sample loop
    - title: "Regola la filigrana dell'immagine nei fogli di calcolo"
      content: |
        Questo esempio mostra come regolare l'immagine delle forme particolari in un foglio di lavoro Excel.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Carica documento come foglio di calcolo
        SpreadsheetLoadOptions loadOptions = new SpreadsheetLoadOptions();
        Watermarker watermarker = new Watermarker("source.xlsx", loadOptions);

        //  Ottieni nuovi byte di filigrana
        File file = new File("new_watermark.png");
        byte[] imageBytes = new byte[(int) file.length()];
        FileInputStream inputStream = new FileInputStream(file);
        inputStream.read(imageBytes);
        inputStream.close();

        //  Regola il contenuto di una particolare filigrana
        for (SpreadsheetShape shape : content.getWorksheets().get_Item(0).getShapes())
        {
            if (shape.getImage() != null)
            {
                shape.setImage(new SpreadsheetWatermarkableImage(imageBytes));
            }
        }

        //  Salva il documento dei risultati
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
    - title: "Maven scarica"
      link: "https://releases.groupdocs.com/watermark/java/"
      color: "red"
        #  loop
    - title: "Licenze"
      link: "https://purchase.groupdocs.com/pricing/watermark/java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Modifica le filigrane in molti formati usando GroupDocs.Watermark for Java"
    exclude: "DOCX"
    description: "Modifica facilmente le filigrane in più formati di documento. Personalizza i tuoi documenti con facilità garantendo protezione e autenticità."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/java/adjust//pdf/"
          description: "Formato documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/java/adjust//word/"
          description: "MS Word e documenti Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/java/adjust//excel/"
          description: "MS Excel e fogli di calcolo Open Office"

        # format loop 4
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/adjust//powerpoint/"
          description: "MS PowerPoint e presentazioni Open Office"

        # format loop 5
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/java/adjust//docx/"
          description: "Documento XML aperto Microsoft Word"
          
        # format loop 6
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/java/adjust//pptx/"
          description: "PowerPoint Presentazione XML aperta"
          
        # format loop 7
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/java/adjust//xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"

        # format loop 8
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/java/adjust//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/java/adjust//xls/"
          description: "Cartella di lavoro Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/java/adjust//ppt/"
          description: "PowerPoint Presentazione 97-2003"

        # format loop 11
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/java/adjust//rtf/"
          description: "Formato RTF"

---