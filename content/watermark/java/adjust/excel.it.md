
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:05
draft: false
lang: it
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Strumento Regola filigrana Excel - GroupDocs.Watermark"
head_description: "Regola, aggiorna e gestisci le filigrane senza problemi con GroupDocs.Watermark. Personalizza i tuoi documenti con facilità."

############################# Header ############################
title: "Strumento Regola le filigrane dei fogli di calcolo: estremamente semplice" 
description: "Migliora i tuoi documenti con il nostro intuitivo strumento di modifica delle filigrane. Semplifica il tuo flusso di lavoro senza sforzo."
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
       **Strumento di regolazione della filigrana**: il nostro strumento di filigrana offre una soluzione intuitiva per migliorare e proteggere i tuoi documenti. Grazie a funzionalità di modifica intuitive, la gestione delle filigrane diventa semplice, garantendo la sicurezza e l'autenticità dei documenti.

############################# Steps ############################
steps:
    enable: true
    title: "Modifica le filigrane nei documenti Excel con Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** semplifica agli sviluppatori di Java la regolazione delle filigrane di testo nelle loro applicazioni implementando alcuni semplici passaggi:
      
      1. Carica il tuo file Excel nell'oggetto principale della nostra API chiamato **Watermarker**. È possibile fornire il file per l'ulteriore elaborazione come flusso o come percorso su un disco locale.
      2. Il passo successivo è individuare le filigrane che devono essere modificate. **SearchCriteria** aiuta a identificare le filigrane con le proprietà giuste che sono state precedentemente aggiunte a un documento.
      3. Ottieni l'elenco delle filigrane adatte come risultato della procedura **Search**. Regola le proprietà delle filigrane trovate come dimensioni, allineamento della pagina, testo, colore, contenuto dell'immagine, ecc. Esistono molti modi per personalizzare i tuoi dati.
      4. Dopo il completamento del processo di regolazione delle filigrane è necessario salvare il documento aggiornato. Utilizza il percorso file locale, il file o il flusso di byte per memorizzare il risultato.
   
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

        // Regola la filigrana del testo EXCEL

        // Crea un'istanza di Watermarker con il documento di input EXCEL
        Watermarker watermarker = new Watermarker("input.xslx");

        // Inizializza TextSearchCriteria e trova filigrane di testo
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        
        // Regola le proprietà della filigrana del testo
        for (PossibleWatermark watermark : watermarks)
        {
            watermark.getFormattedTextFragments().clear();
            watermark.getFormattedTextFragments().
                add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
        }

        // Salva il documento aggiornato
        watermarker.save("output.xslx");
        
        ```            
        
############################# More features ############################
more_features:
  enable: true
  title: "Approfondisci la regolazione della filigrana EXCEL"
  description: "La nostra API consente alle Java applicazioni di aggiungere, modificare, rimuovere e cercare filigrane nei formati di documento più diffusi."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Regola filigrana"
  features:
    # feature loop
    - title: "Filigrana facilmente i tuoi documenti"
      content: "GroupDocs.Watermark semplifica la filigrana per Java sviluppatori. Aggiungi filigrane diverse a vari documenti e file aziendali. Non solo puoi applicare filigrane, ma puoi anche aggiornare o rimuovere quelle esistenti."

    # feature loop
    - title: "Personalizza le filigrane in base alle tue esigenze"
      content: "La nostra API offre ampie opzioni di personalizzazione. Regola facilmente dimensioni, rotazione, colore, carattere, stili e altro per ottenere la filigrana perfetta."

    # feature loop
    - title: "Usa le funzionalità native del documento EXCEL"
      content: "A seconda del formato specifico del documento, è possibile utilizzare funzionalità native. Questi possono includere lo sfondo della pagina del documento, le annotazioni, le intestazioni o altri oggetti come contenitori di filigrane."
      
  code_samples:
    # code sample loop
    - title: "PDF modifica la filigrana del testo"
      content: |
        Questo esempio mostra come regolare il testo di particolari artefatti.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Carica documento PDF
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Ottieni il contenuto del documento
        PdfContent pdfContent = watermarker.getContent(PdfContent.class);

        //  Regola un particolare testo della filigrana
        for (PdfArtifact artifact : pdfContent.getPages().get_Item(0).getArtifacts())
        {
            if (artifact.getText().contains("Test"))
            {
                artifact.setText("Passed");
            }
        }

        //  Salva il documento
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
    title: "Regola la filigrana tramite GroupDocs.Watermark for Java per altri formati"
    exclude: "EXCEL"
    description: "Personalizza con facilità le filigrane in un'ampia gamma di formati di documenti. Migliora la sicurezza e l'autenticità dei documenti senza sforzo."
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