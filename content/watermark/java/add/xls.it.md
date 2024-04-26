
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:39:00
draft: false
lang: it
format: Xls
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Filigrana XLS Fogli di calcolo con Java"
head_description: "Usa Java per applicare filigrane personalizzate ai file XLS, proteggendo i documenti Excel e OpenOffice."

############################# Header ############################
title: "Filigrana basata su Java per Excel" 
description: "Implementa filigrane nei file XLS usando Java per migliorare la sicurezza dei documenti per Excel e i fogli OpenOffice, perfetti per dati finanziari e riservati."
subtitle: "GroupDocs.Watermark for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica a Maven gratuitamente"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java"
    link: "/watermark/java/"
    link_title: "Scopri di più"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java offre agli Java sviluppatori la capacità di integrare la filigrana nei file XLS, supportando i formati Excel e OpenOffice. Questa API consente di incorporare filigrane visibili e discrete, assicurando che le informazioni sensibili siano protette senza alterare l'usabilità del documento. Le funzionalità principali includono la possibilità di personalizzare il testo, l'immagine e il posizionamento della filigrana, che possono essere applicati in modo condizionale in base al contenuto del documento o alle autorizzazioni dell'utente. Ciò lo rende ideale per applicazioni in ambienti che richiedono rigorose misure di protezione dei dati, come i settori bancario, legale e accademico. Con il supporto per Java 8 e versioni successive, GroupDocs.Watermark è in grado di gestire complesse esigenze di watermarking su diversi sistemi operativi.

############################# Steps ############################
steps:
    enable: true
    title: "Tecniche avanzate: aggiunta di filigrane ai documenti Xls tramite Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)**
      
      1. **Watermarker**. Questo passaggio fondamentale pone le basi per migliorare i documenti Xls con filigrane. Fornisci il file Xls al costruttore, come percorso o oggetto stream.
      2. **Watermark** su misura secondo le tue specifiche. Queste entità versatili offrono un posizionamento preciso non solo su pagine designate del documento, ma anche all'interno di elementi nativi come allegati o intestazioni.
      3. Perfeziona il processo di filigrana ottimizzando proprietà come dimensioni, allineamento, stili dei caratteri e colori. Questo livello di personalizzazione consente di creare filigrane che si adattano perfettamente all'estetica del documento.
      4. **Watermarker** per applicare le filigrane appena create sui tuoi documenti. Goditi la flessibilità di aggiungere più filigrane in base alle tue esigenze. Per conservare i documenti, valuta la possibilità di salvarli in un luogo sicuro.
   
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
        // Aggiungi filigrana dell'immagine a XLS

        // Passa il file da filigranare a Watermarker
        Watermarker watermarker = new Watermarker("input.xls");
        
        // Fornisci il percorso all'immagine con la filigrana
        ImageWatermark watermark = new ImageWatermark("watermark.png");

        // Salva risultato
        watermarker.add(watermark);
        watermarker.save("output.xls");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Masterizzazione delle filigrane dei documenti"
  description: "Migliora la gestione dei tuoi documenti con la nostra sofisticata API di watermarking, creata su misura per .NET sviluppatori. Questo strumento offre soluzioni complete per l'applicazione, la personalizzazione e la gestione delle filigrane in un'ampia gamma di formati di documenti, garantendo sia un aspetto estetico che una maggiore sicurezza."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Filigrana avanzata dei documenti"
  features:
    # feature loop
    - title: "Rotazione flessibile della filigrana"
      content: "Adatta le tue filigrane per adattarle a qualsiasi orientamento del documento con le nostre impostazioni di rotazione flessibili. Che il documento sia verticale o orizzontale, regola facilmente l'angolazione della filigrana per mantenere un aspetto uniforme che si integri perfettamente con il layout del documento."

    # feature loop
    - title: "Perfetto controllo della trasparenza"
      content: "Controlla la trasparenza delle tue filigrane con precisione, consentendo marcature sottili ma sicure che non coprano il contenuto del documento. Questa funzionalità è ideale per mantenere l'estetica originale dei documenti aggiungendo al contempo un livello di sicurezza."

    # feature loop
    - title: "Effetti d'ombra per enfatizzare"
      content: "Migliora la visibilità delle tue filigrane o integrale sottilmente nei tuoi documenti con effetti ombra personalizzabili. Questa funzione consente di creare ombre di sfocatura, diffusione e colore diversi, rendendo la filigrana più distintiva o discreta, a seconda delle necessità."
      
  code_samples:
    # code sample loop
    - title: "MS Word filigrana bloccata"
      content: |
        Questo esempio mostra come bloccare la filigrana in DOCX tutte le pagine
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Carica documento come MS Word doc
        WordProcessingLoadOptions loadOptions = new WordProcessingLoadOptions();
        Watermarker watermarker = new Watermarker("source.docx", loadOptions);

        //  Crea una filigrana
        TextWatermark watermark = new TextWatermark("Watermark text", new Font("Arial", 19));
        watermark.setForegroundColor(Color.getRed());

        //  Ottimizza le opzioni native Word
        WordProcessingWatermarkPagesOptions options = new WordProcessingWatermarkPagesOptions();
        options.setLocked(true);
        options.setLockType(WordProcessingLockType.AllowOnlyFormFields);

        //  Aggiungi filigrana alle pagine del documento dei risultati
        watermarker.add(textWatermark, options);
        watermarker.save("result.docx");
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
    title: "Migliorare la sicurezza dei documenti Excel con Java"
    exclude: "XLS"
    description: "Proteggi i tuoi documenti Excel e OpenOffice con filigrane personalizzabili implementate con Java, garantendo l'integrità dei dati e la protezione del copyright."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/java/add//pdf/"
          description: "Formato documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/java/add//word/"
          description: "MS Word e documenti Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/java/add//excel/"
          description: "MS Excel e fogli di calcolo Open Office"

        # format loop 4
        - name: "Immagine con filigrana"
          format: "IMAGE"
          link: "/watermark/java/add//image/"
          description: "Formati di immagine più diffusi"

        # format loop 5
        - name: "Foto con filigrana"
          format: "PHOTO"
          link: "/watermark/java/add//photo/"
          description: "Formati fotografici"

        # format loop 6
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/add//powerpoint/"
          description: "MS PowerPoint e presentazioni Open Office"

        # format loop 7
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/java/add//docx/"
          description: "Documento XML aperto Microsoft Word"
          
        # format loop 8
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/java/add//pptx/"
          description: "PowerPoint Presentazione XML aperta"
          
        # format loop 9
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/java/add//xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"

        # format loop 10
        - name: "Filigrana JPEG"
          format: "JPEG"
          link: "/watermark/java/add//jpeg/"
          description: "JPEG Immagine"

        # format loop 11
        - name: "Filigrana PNG"
          format: "PNG"
          link: "/watermark/java/add//png/"
          description: "Portable Grafica di rete"

        # format loop 12
        - name: "Filigrana TIFF"
          format: "TIFF"
          link: "/watermark/java/add//tiff/"
          description: "Formato del file di immagine per tag"

        # format loop 13
        - name: "Filigrana WEBP"
          format: "WEBP"
          link: "/watermark/java/add//webp/"
          description: "Immagine WEB"

        # format loop 14
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/java/add//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 15
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/java/add//xls/"
          description: "Cartella di lavoro Microsoft Excel 97-2003"

        # format loop 16
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/java/add//ppt/"
          description: "PowerPoint Presentazione 97-2003"

        # format loop 17
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/java/add//rtf/"
          description: "Formato RTF"

---