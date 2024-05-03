
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:04
draft: false
lang: it
format: Photo
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Filigrana fotografica rapida semplificata in Java"
head_description: "Semplifica la protezione delle tue foto con la filigrana. Veloce e affidabile."

############################# Header ############################
title: "Strumenti efficienti Java per la filigrana fotografica" 
description: "Aggiungi filigrane alle tue foto in modo rapido ed efficiente utilizzando la nostra API Java. Perfetto per proteggere le immagini digitali e migliorare la visibilità del marchio con il minimo sforzo."
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
       GroupDocs.Watermark for Java è ottimizzato per una filigrana rapida ed efficace dei file fotografici. Questo strumento consente una rapida integrazione di filigrane di testo e immagini in un'ampia gamma di formati fotografici, tra cui JPEG, PNG e BMP. Personalizza le tue filigrane con ampie opzioni di stile, trasparenza e posizionamento per assicurarti che si fondano perfettamente senza compromettere la qualità della foto. Adatto per operazioni ad alto volume, supporta l'elaborazione in batch per applicare filigrane a più foto contemporaneamente, rendendolo ideale per aziende e creatori di contenuti digitali che hanno bisogno di proteggere e marchiare le proprie risorse visive in modo efficiente

############################# Steps ############################
steps:
    enable: true
    title: "Aggiungi filigrana al documento Photo tramite Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** consente agli sviluppatori di Java di aggiungere facilmente filigrane di vario tipo ai formati di file aziendali più diffusi. Aggiungi la nostra libreria alla tua applicazione e aggiungi la filigrana ai documenti in pochi semplici passaggi, come elencato di seguito.
      
      1. La classe principale della nostra API è **Watermarker**. È necessario crearne un'istanza prima dell'elaborazione del documento. Non dimenticare di passare il file Photo al costruttore come percorso o oggetto stream.
      2. Il passaggio successivo è costruire un oggetto **Watermark** del tipo desiderato. Può essere posizionato non solo su una pagina specifica del documento ma anche in parti native del documento come allegati o intestazioni.
      3. Imposta le proprietà della filigrana come altezza e larghezza, allineamento della pagina (in alto, a sinistra, al centro, ecc.), famiglia e colore dei caratteri e molto altro.
      4. Chiama il metodo **Watermarker** per aggiungere una nuova filigrana. Puoi aggiungere tutte le filigrane di cui hai bisogno. Si consiglia di salvare il documento elaborato in un'altra posizione.
   
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

        // Aggiungi filigrana di testo a PHOTO

        // Passa il file da filigranare a Watermarker
        Watermarker watermarker = new Watermarker("input.png");
        
        // Crea una filigrana di testo e imposta le proprietà
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        watermark.setForegroundColor(Color.getRed());

        // Salva il file con filigrana
        watermarker.add(watermark);
        watermarker.save("output.png");
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Migliora facilmente le tue filigrane"
  description: "Sfrutta la potenza di GroupDocs.Watermark per generare, comporre e aggiungere filigrane in più formati di documento. Questa API non solo migliora la sicurezza dei documenti, ma protegge anche la tua proprietà intellettuale incorporando filigrane personalizzabili che sono sia versatili che robuste."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Aggiungi filigrana"
  features:
    # feature loop
    - title: "Versatili opzioni di filigrana."
      content: "Esplora una vasta gamma di opzioni di filigrana con GroupDocs.Watermark. Dalla regolazione dell'opacità e della rotazione al ridimensionamento proporzionale delle dimensioni, la nostra API ti consente di personalizzare le filigrane con precisione in base alle tue esigenze, assicurando che si integrino perfettamente con i tuoi documenti e mantenendo l'integrità dei contenuti."

    # feature loop
    - title: "Stile avanzato della filigrana."
      content: "GroupDocs.Watermark ti consente di modellare le tue filigrane con vari tipi di carattere, colori e ombre, rendendole distintive e più difficili da rimuovere. Migliora l'aspetto estetico dei tuoi documenti e immagini protetti con filigrane eleganti che riflettono l'identità e la professionalità del tuo marchio."

    # feature loop
    - title: "Piastrellatura e posizionamento della filigrana"
      content: "Con GroupDocs.Watermark, implementa effetti di piastrellatura per coprire l'intero documento, garantendo una protezione completa. Posiziona le filigrane esattamente dove ti servono: al centro, negli angoli o in posizioni personalizzate. Le nostre opzioni di posizionamento flessibili aiutano a proteggere i tuoi documenti da usi e duplicazioni non autorizzati."
      
  code_samples:
    # code sample loop
    - title: "filigrana di annotazione PDF"
      content: |
        Questo esempio mostra come aggiungere un'annotazione con filigrana a un documento PDF
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Carica documento come PDF
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Crea una filigrana in base all'annotazione PDF
        PdfAnnotationWatermarkOptions options = new PdfAnnotationWatermarkOptions();
        TextWatermark textWatermark = new TextWatermark("Annotation watermark", new Font("Arial", 8));

        //  Impostare le opzioni per la filigrana
        textWatermark.setHorizontalAlignment(HorizontalAlignment.Left);
        textWatermark.setVerticalAlignment(VerticalAlignment.Top);

        //  Aggiungi filigrana di testo al documento dei risultati
        watermarker.add(textWatermark, options);
        watermarker.save("result.pdf");

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
    title: "Integrazione rapida della filigrana per le foto tramite Java"
    exclude: "PHOTO"
    description: "Sfrutta la nostra API Java per applicare rapidamente filigrane alle foto, migliorando la sicurezza e l'identità del marchio. I processi automatizzati consentono un'applicazione di massa, garantendo risultati coerenti e professionali."
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