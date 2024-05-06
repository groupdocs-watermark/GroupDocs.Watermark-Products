
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:37
draft: false
lang: it
format: Jpg
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Filigrana C# per JPG immagini"
head_description: "Integra la filigrana nei file JPG usando .NET C#, proteggendo efficacemente le tue immagini digitali."

############################# Header ############################
title: "Proteggi JPG immagini con .NET C#" 
description: "Applica .NET C# per creare filigrane robuste per JPG immagini, ideali per proteggere il copyright e prevenire l'uso non autorizzato."
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
       GroupDocs.Watermark for .NET fornisce agli sviluppatori .NET C# un framework avanzato per aggiungere filigrane a JPG immagini. Questa API consente l'incorporamento preciso di testo, loghi e filigrane grafiche personalizzabili in opacità, posizione e dimensioni, perfette per i media digitali e la fotografia professionale. Migliora la sicurezza delle tue immagini senza sacrificare la qualità, con funzionalità progettate per incorporare filigrane che scoraggiano la pirateria mantenendo l'integrità della grafica originale. Adatto per un'ampia gamma di applicazioni, dalla protezione fotografica personale all'uso commerciale nella pubblicità e nei media, GroupDocs.Watermark garantisce che le tue risorse visive siano contrassegnate in modo univoco e protette legalmente.

############################# Steps ############################
steps:
    enable: true
    title: "Genera facilmente filigrane per documenti Jpg"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/):** Libreria avanzata di filigrana per applicazioni .NET. Potenzia la tua soluzione e proteggi i documenti con filigrane appena in tempo.
      
      1. **Classe principale: Watermarker.** La classe principale della nostra API è **Watermarker**. È necessario crearne un'istanza prima dell'elaborazione del documento. Non dimenticare di passare il file Jpg al costruttore come percorso o oggetto stream.
      2. **Creazione della filigrana.** Il passaggio successivo è la costruzione di un oggetto Filigrana del tipo desiderato. Può essere posizionato non solo su una pagina specifica del documento ma anche in parti native del documento come immagini o intestazioni.
      3. **Ottimizzazione dell'aspetto.** Imposta le proprietà della filigrana come altezza e larghezza, allineamenti in alto, a sinistra, al centro, caratteri e colori, ecc.
      4. **Applicazione e salvataggio.** Utilizza il metodo **Watermarker** per aggiungere una nuova filigrana. Sentiti libero di aggiungere tutte le filigrane di cui hai bisogno. È possibile salvare il documento con filigrana in qualsiasi posizione.
   
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
        // Genera filigrana immagine nel file JPG

        // Fornisci il percorso del file di origine al costruttore Watermarker
        using (Watermarker watermarker = new Watermarker("input.jpg"))
        {
            // Genera un'istanza di filigrana immagine con il file immagine
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // Salva il risultato JPG con filigrana
            watermarker.Save("output.jpg");
        }
        
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "Migliora il tuo gioco di filigrana"
  description: "Sblocca funzionalità avanzate di watermarking con la nostra API GroupDocs.Watermark per .NET. Questo potente strumento consente una personalizzazione precisa e l'applicazione di filigrane su vari tipi di documenti per garantire la massima sicurezza e rispetto del copyright con interruzioni visive minime."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Soluzioni complete per la filigrana"
  features:
    # feature loop
    - title: "Sofisticate opzioni di piastrellatura"
      content: "Estendi le tue filigrane su interi documenti senza problemi con le nostre opzioni di piastrellatura. Questa funzione consente alle filigrane di coprire l'intera area del documento, impedendone la rimozione e garantendo una protezione completa del documento senza compromettere il design o la leggibilità."

    # feature loop
    - title: "Personalizzazione dei colori vivaci"
      content: "Aggiungi un tocco di colore alle tue filigrane! La nostra API consente la personalizzazione completa dei colori, consentendoti di applicare filigrane che si adattano perfettamente al marchio aziendale o allo stile del documento. Migliora l'appeal visivo mantenendo al contempo solide funzionalità di sicurezza."

    # feature loop
    - title: "Impostazioni di sicurezza avanzate"
      content: "Porta la sicurezza dei documenti a un livello superiore con le impostazioni avanzate della filigrana. Configura filigrane a più livelli, che incorporano elementi visibili e invisibili, per proteggerti da copie non autorizzate e garantire che solo i destinatari previsti possano accedere alle informazioni critiche."
      
  code_samples:
    # code sample loop
    - title: "Genera filigrana PowerPoint"
      content: |
        Questo esempio mostra come aggiungere una filigrana alle immagini di sfondo PPTX
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Carica la presentazione PPTX
            var loadOptions = new PresentationLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pptx", loadOptions))
            {
                //  Impostare le proprietà della filigrana
                TextWatermark watermark = new TextWatermark("Protected image", new Font("Arial", 8));
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermark.RotateAngle = 45;
                watermark.SizingType = SizingType.ScaleToParentDimensions;
                watermark.ScaleFactor = 1;

                //  Sfondo di diapositive con filigrana
                PresentationContent content = watermarker.GetContent<PresentationContent>();
                foreach (PresentationSlide slide in content.Slides)
                {
                    if (slide.ImageFillFormat.BackgroundImage != null)
                    {
                        slide.ImageFillFormat.BackgroundImage.Add(watermark);
                    }
                }

                //  Salva la presentazione elaborata
                watermarker.save("result.pptx");
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
    title: "Implementa le filigrane in JPG con C#"
    exclude: "JPG"
    description: "Sfrutta .NET C# per incorporare filigrane invisibili o visibili nei file JPG, essenziali per contenuti digitali sicuri e riconoscibili."
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