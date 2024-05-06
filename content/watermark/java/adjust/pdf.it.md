
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:35
draft: false
lang: it
format: Pdf
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Modifica le filigrane in PDF - GroupDocs.Watermark"
head_description: "Regola e rifinisci le filigrane su diversi tipi di documenti senza sforzo con GroupDocs.Watermark. Garantisci la credibilità dei documenti."

############################# Header ############################
title: "Regola le filigrane PDF: protezione versatile" 
description: "Proteggi i tuoi contenuti in vari formati con le nostre versatili funzioni di regolazione della filigrana. Adattati alle tue esigenze senza problemi."
subtitle: "GroupDocs.Watermark for Java Soluzione" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Pacchetto gratuito Maven"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java Soluzione"
    link: "/watermark/java/"
    link_title: "Scopri di più"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Modifica filigrane**: proteggi i tuoi contenuti in diversi formati di documento con le nostre versatili funzioni di regolazione della filigrana. Personalizza la tua strategia di filigrana per soddisfare con facilità i tuoi requisiti specifici.

############################# Steps ############################
steps:
    enable: true
    title: "Modifica le filigrane dei documenti Pdf utilizzando Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** consente agli sviluppatori di Java di modificare facilmente le filigrane in molti documenti utilizzando le loro applicazioni. Ecco una guida rapida:
      
      1. Innanzitutto, devi passare il file Pdf come parametro del costruttore della classe **Watermarker**. Fornire flusso di byte o file o un percorso del disco locale.
      2. In secondo luogo, individua le filigrane che devono essere modificate. Utilizza **SearchCriteria** per identificare le filigrane con le proprietà specifiche precedentemente aggiunte al documento.
      3. Dopo la ricerca, riceverai un elenco di filigrane rilevanti. Puoi quindi regolarne le proprietà, tra cui dimensioni, allineamento della pagina, testo, colore, contenuto dell'immagine e altro. Ciò offre un elevato grado di personalizzazione dei tuoi dati.
      4. Una volta terminata la regolazione delle filigrane, salva il documento aggiornato. È possibile utilizzare un percorso file locale o uno streaming per archiviare il risultato.
   
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
        // Regola la filigrana dell'immagine PDF

        // Crea un'istanza di Watermarker con PDF
        Watermarker watermarker = new Watermarker("input.pdf");
        
        // Inizializza SearchCriteria per abbinare un'immagine particolare
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);

        for (PossibleWatermark watermark : watermarks)
        {
            // Sostituisci l'immagine trovata
            watermark.setImageData(imageData);
        }

        // Salva il file modificato
        watermarker.save("output.pdf");
        
        ```
        
############################# More features ############################
more_features:
  enable: true
  title: "Gestione avanzata della filigrana PDF per le applicazioni Java"
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
    - title: "Sfruttamento delle funzionalità native dei documenti PDF"
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
    title: "Gestisci le filigrane nei formati più diffusi con GroupDocs.Watermark for Java"
    exclude: "PDF"
    description: "Proteggi i tuoi contenuti in vari formati con le nostre versatili funzioni di regolazione della filigrana. Adattati alle tue esigenze senza problemi."
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