
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:26:59
draft: false
lang: it
format: Image
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Filigrana delle immagini con .NET C#"
head_description: "Impara ad applicare filigrane senza interruzioni alle immagini usando .NET C#. Proteggi le tue risorse senza compromettere la qualità."

############################# Header ############################
title: "Filigrana personalizzata rapida per immagini con .NET" 
description: "Il nostro strumento C# .NET fornisce una soluzione rapida per incorporare filigrane nelle immagini. Il supporto per estesi formati di immagine garantisce una copertura completa dalle foto alle opere d'arte digitali."
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica a Nuget gratuitamente"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "Scopri di più"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET è progettato per automatizzare il processo di filigrana delle immagini, supportando un'ampia gamma di formati come JPEG, PNG, BMP e TIFF. Questa robusta API consente l'inserimento rapido di filigrane di testo e immagini regolabili in opacità, dimensioni e posizione, personalizzate in base alle esigenze specifiche. Che si tratti di proteggere i diritti d'autore o di migliorare il materiale di marketing, il nostro toolkit garantisce che le filigrane vengano applicate con alta fedeltà e con un impatto minimo sulla qualità dell'immagine originale.

############################# Steps ############################
steps:
    enable: true
    title: "Migliora i tuoi documenti: genera filigrane per Image usando .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** è una libreria che semplifica l'aggiunta di filigrane a vari formati di file aziendali per .NET sviluppatori. Integra la nostra libreria nella tua applicazione e aggiungi facilmente filigrane ai documenti seguendo questi passaggi:
      
      1. **Iniziare il tuo percorso con il watermarking:** Inizia conoscendo la classe **Watermarker**, la pietra angolare della nostra API. Per iniziare il processo, assicurati di crearne un'istanza prima dell'elaborazione del documento. Non trascurate l'importanza di fornire il file Image al costruttore, che si tratti di un percorso o di un oggetto stream.
      2. **Creazione di filigrane personalizzate:** Passa alla fase successiva creando un oggetto **Filigrana** personalizzato in base alle tue specifiche. Questo strumento versatile non si limita a pagine specifiche del documento; può anche essere integrato senza problemi in elementi nativi del documento come allegati o intestazioni.
      3. **Ottimizzazione degli attributi della filigrana:** Perfeziona la tua esperienza con la filigrana regolando proprietà come altezza, larghezza, allineamento della pagina, famiglia di caratteri e colore. Questo livello di personalizzazione garantisce che le filigrane si integrino perfettamente con i documenti.
      4. **Applicazione delle filigrane:** Utilizza il metodo **Watermarker** per applicare facilmente le filigrane personalizzate ai tuoi documenti. Che tu debba aggiungere una o più filigrane, questo processo offre flessibilità. Per una maggiore sicurezza, valuta la possibilità di salvare i documenti elaborati in una posizione separata.
   
    code:
      platform: "net"
      copy_title: "Copia"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "clicca per copiare"
        copy_done: "copiato"
      links:
        #  loop
        - title: "Altri esempi"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "Documentazione"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // Genera filigrana di testo nel file IMAGE

        // Fornisci il file da filigranare
        using (Watermarker watermarker = new Watermarker("input.jpeg"))
        {
            // Genera un'istanza di filigrana di testo
            Font font = new Font("Arial", 19, FontStyle.Bold | FontStyle.Italic);
            TextWatermark watermark = new TextWatermark("my watermark", font);
            watermark.ForegroundColor = Color.Red;
            watermark.BackgroundColor = Color.Blue;
            watermarker.Add(watermark);

            // Salva IMAGE risultati
            watermarker.Save("output.jpeg");
        }
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Approfondisci l'aggiunta di filigrane"
  description: "Sfrutta la nostra potente API per renderizzare, visualizzare, convertire e gestire documenti, diapositive, diagrammi e vari altri tipi di documenti all'interno di .NET applicazioni. GroupDocs.Watermark integra perfettamente le funzionalità di filigrana per migliorare la sicurezza dei documenti e la protezione del copyright."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Aggiungi filigrana"
  features:
    # feature loop
    - title: "Filigrana i tuoi documenti senza sforzo."
      content: "GroupDocs.Watermark consente a .NET sviluppatori di integrare facilmente la filigrana nelle loro applicazioni. Aggiungi facilmente testo, immagini o filigrane dinamiche ai documenti e ai file aziendali più diffusi, assicurando che i tuoi contenuti siano sicuri e con un marchio coerente su tutte le piattaforme."

    # feature loop
    - title: "Personalizza le filigrane per soddisfare le tue esigenze."
      content: "Personalizza le filigrane in base ai tuoi requisiti specifici con funzionalità complete supportate da GroupDocs.Watermark. Regola le dimensioni, la rotazione, la trasparenza, il colore e il carattere per garantire che la filigrana non solo abbia un aspetto perfetto, ma migliori anche la sicurezza dei documenti senza ostacolare le informazioni importanti."

    # feature loop
    - title: "Sfrutta le funzionalità dei documenti nativi per la filigrana"
      content: "Utilizza le funzionalità intrinseche dei formati di documento per creare filigrane sofisticate. Che si tratti di utilizzare annotazioni native PDF, sfondi MS Word o intestazioni e piè di pagina Excel, GroupDocs.Watermark si integra profondamente con le strutture dei documenti per applicare filigrane efficaci e minimamente invasive."
      
  code_samples:
    # code sample loop
    - title: "Genera filigrana dell'immagine per DOCX"
      content: |
        Questo esempio mostra come applicare effetti di immagine alle filigrane delle forme.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Carica documento Word
            var loadOptions = new WordProcessingLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.docx", loadOptions))
            {
                //  Impostare le opzioni per la filigrana
                using (ImageWatermark watermark = new ImageWatermark("logo.png"))
                {
                    WordProcessingImageEffects effects = new WordProcessingImageEffects();
                    effects.Brightness = 0.7;
                    effects.Contrast = 0.6;
                    effects.ChromaKey = Color.Red;
                    effects.BorderLineFormat.Enabled = true;
                    effects.BorderLineFormat.Weight = 1;

                    WordProcessingWatermarkSectionOptions options = new WordProcessingWatermarkSectionOptions();
                    options.Effects = effects;

                    //  Genera filigrana
                    watermarker.Add(watermark, options);
                }

                //  Salva documento aggiornato
                watermarker.save("result.docx");
            }

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Pronto per iniziare?"
  description: "Prova le funzioni GroupDocs.Watermark gratuitamente o richiedi una licenza"
  items:
    #  loop
    - title: "Nuget scarica"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "Licenze"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Implementa rapidamente le filigrane in tutti i formati di immagine tramite C#"
    exclude: "IMAGE"
    description: "Migliora la protezione delle tue immagini con il nostro toolkit C# .NET, in grado di gestire vari formati di immagine con velocità ed efficienza. Personalizza le tue filigrane per integrarle perfettamente con i tuoi contenuti visivi."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/net/generate//pdf/"
          description: "Formato documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/net/generate//word/"
          description: "MS Word e documenti Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/net/generate//excel/"
          description: "MS Excel e fogli di calcolo Open Office"

        # format loop 4
        - name: "Immagine con filigrana"
          format: "IMAGE"
          link: "/watermark/net/generate//image/"
          description: "Formati di immagine più diffusi"

        # format loop 5
        - name: "Foto con filigrana"
          format: "PHOTO"
          link: "/watermark/net/generate//photo/"
          description: "Formati fotografici"

        # format loop 6
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/generate//powerpoint/"
          description: "MS PowerPoint e presentazioni Open Office"

        # format loop 7
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/net/generate//docx/"
          description: "Documento XML aperto Microsoft Word"
          
        # format loop 8
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/net/generate//pptx/"
          description: "PowerPoint Presentazione XML aperta"
          
        # format loop 9
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/net/generate//xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"

        # format loop 10
        - name: "Filigrana JPEG"
          format: "JPEG"
          link: "/watermark/net/generate//jpeg/"
          description: "JPEG Immagine"

        # format loop 11
        - name: "Filigrana PNG"
          format: "PNG"
          link: "/watermark/net/generate//png/"
          description: "Portable Grafica di rete"

        # format loop 12
        - name: "Filigrana TIFF"
          format: "TIFF"
          link: "/watermark/net/generate//tiff/"
          description: "Formato del file di immagine per tag"

        # format loop 13
        - name: "Filigrana WEBP"
          format: "WEBP"
          link: "/watermark/net/generate//webp/"
          description: "Immagine WEB"

        # format loop 14
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/net/generate//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 15
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/net/generate//xls/"
          description: "Cartella di lavoro Microsoft Excel 97-2003"

        # format loop 16
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/net/generate//ppt/"
          description: "PowerPoint Presentazione 97-2003"

        # format loop 17
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/net/generate//rtf/"
          description: "Formato RTF"

---