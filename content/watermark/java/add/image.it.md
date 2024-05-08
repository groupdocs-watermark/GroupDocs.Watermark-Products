
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:17
draft: false
lang: it
format: Image
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Genera filigrane efficaci per le immagini con Java"
head_description: "Usa Java per creare filigrane sofisticate per le immagini. Proteggi i tuoi documenti e fai valere il copyright in modo efficace."

############################# Header ############################
title: "Filigrana delle immagini senza soluzione di continuità in Java" 
description: "Implementa filigrane dinamiche nei tuoi file di immagine usando Java. Questo strumento consente regolazioni precise del posizionamento, della scalabilità e della trasparenza per migliorare la sicurezza e il riconoscimento del marchio."
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
       GroupDocs.Watermark for Java GroupDocs.Watermark for Java consente agli sviluppatori di generare e gestire in modo efficace le filigrane sui file di immagine. Grazie al supporto per un'ampia gamma di formati di immagine, gli utenti possono implementare filigrane di testo e grafiche completamente personalizzabili in posizione, scala e trasparenza. Questa funzionalità è fondamentale per le applicazioni nei media digitali, nella pubblicità e nella distribuzione di contenuti online, dove l'integrità del marchio e del copyright sono fondamentali. Inoltre, GroupDocs.Watermark include funzionalità per cercare e rimuovere filigrane esistenti, fornendo uno strumento versatile per la gestione e la sicurezza delle immagini.

############################# Steps ############################
steps:
    enable: true
    title: "Aggiungi filigrana al documento Image tramite Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** consente agli sviluppatori di Java di aggiungere facilmente filigrane di vario tipo ai formati di file aziendali più diffusi. Aggiungi la nostra libreria alla tua applicazione e aggiungi la filigrana ai documenti in pochi semplici passaggi, come elencato di seguito.
      
      1. La classe principale della nostra API è **Watermarker**. È necessario crearne un'istanza prima dell'elaborazione del documento. Non dimenticare di passare il file Image al costruttore come percorso o oggetto stream.
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

        // Aggiungi filigrana di testo a IMAGE

        // Passa il file da filigranare a Watermarker
        Watermarker watermarker = new Watermarker("input.jpeg");
        
        // Crea una filigrana di testo e imposta le proprietà
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        watermark.setForegroundColor(Color.getRed());

        // Salva il file con filigrana
        watermarker.add(watermark);
        watermarker.save("output.jpeg");
        
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
    title: "Semplifica le immagini di sicurezza con la filigrana in Java"
    exclude: "IMAGE"
    description: "Il nostro toolkit Java consente la generazione di filigrane personalizzate per qualsiasi formato di immagine, migliorando la sicurezza e il marchio. Le filigrane personalizzate assicurano che le immagini siano riconosciute e protette su vari supporti."
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