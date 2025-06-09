
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: it
format: Photo
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Watermark le Tue Foto Facilmente"
head_description: "Aggiungi watermark alle tue foto in Python per proteggere il tuo lavoro e i diritti d'autore."

############################# Header ############################
title: "Watermark Foto Velocemente con Python" 
description: "Utilizza la nostra libreria Python per aggiungere rapidamente watermark alle tue foto. Proteggi i tuoi diritti d'autore e marchio senza perdere qualità dell'immagine."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica PyPi gratuitamente"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "Scopri di più"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET è ottima per i fotografi che vogliono proteggere il loro lavoro. Aggiungi watermark di testo o immagine a foto in formati come JPEG, PNG e RAW. Regola la trasparenza, la dimensione e la posizione affinché il tuo watermark si adatti perfettamente e la tua foto sembri ancora bella.

############################# Steps ############################
steps:
    enable: true
    title: "Aggiungi Watermark: Watermarking con Python per Photo"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** è una libreria che semplifica l'aggiunta di watermark a molti tipi di file aziendali. Segui questi passaggi per aggiungere rapidamente watermark ai tuoi documenti in Python:
      
      1. **Inizio con il Watermarking:** Inizia creando un'istanza della classe **Watermarker**. Passa il tuo file Photo (come percorso o stream) al costruttore per aprirlo per il watermarking.
      2. **Crea il Tuo Watermark:** Crea un oggetto **Watermark** con il testo e le impostazioni desiderate. Puoi aggiungere watermark a qualsiasi pagina o persino a elementi del documento come intestazioni o allegati.
      3. **Personalizza il Watermark:** Regola la dimensione, la posizione, il font, il colore e l'allineamento del watermark per adattarlo alle tue esigenze. Questo aiuta il tuo watermark a integrarsi correttamente nel documento.
      4. **Applica e Salva:** Utilizza il metodo **Watermarker** per aggiungere il(o i) watermark al documento. Salva il risultato, possibilmente in un nuovo file per maggiore sicurezza.
   
    code:
      platform: "python-net"
      copy_title: "Copia"
      install:
        command: |
        command: "pip install groupdocs-watermark-net"
        copy_tip: "clicca per copiare"
        copy_done: "copiato"
      links:
        #  loop
        - title: "Altri esempi"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
        #  loop
        - title: "Documentazione"
          link: "https://docs.groupdocs.com/watermark/python-net/"
          
      content: |
        ```python {style=abap}
        # Aggiungi un watermark di testo a un file PHOTO
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # Seleziona il file che vuoi watermarkare
        with gw.Watermarker("input.png") as watermarker:

            # Crea un oggetto watermark di testo
            font = gww.Font("Arial", 36.0)
            watermark = gww.TextWatermark("top secret", font)
            watermark.foreground_color = gww.Color.red
            watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
            watermark.opacity = 0.4

            watermarker.add(watermark)

            # Salva il file PHOTO aggiornato
            watermarker.save("output.png")
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Esplora Altre Funzionalità di Watermarking"
  description: "Utilizza la nostra API Python per aggiungere, visualizzare, convertire e gestire watermark in documenti, diapositive, diagrammi e altro. GroupDocs.Watermark for Python via .NET ti aiuta a proteggere i tuoi file e ad aggiungere informazioni di copyright in modo semplice."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Aggiungi Watermark"
  features:
    # feature loop
    - title: "Aggiungi Watermark con Facilità"
      content: "GroupDocs.Watermark consente agli sviluppatori Python di aggiungere rapidamente watermark di testo, immagine o dinamici a documenti aziendali. Tieni i tuoi file sicuri e con branding con il minimo sforzo."

    # feature loop
    - title: "Watermark Completamente Personalizzabili"
      content: "Cambia la dimensione, rotazione, trasparenza, colore e font del watermark con GroupDocs.Watermark. Fai in modo che il tuo watermark si adatti perfettamente al documento e mantenga il contenuto importante visibile."

    # feature loop
    - title: "Usa Caratteristiche del Documento per il Watermarking"
      content: "Sfrutta le caratteristiche integrate del documento come annotazioni PDF, sfondi di Word o intestazioni di Excel per aggiungere watermark. GroupDocs.Watermark funziona con le strutture documentali per un watermarking efficace e non intrusivo."
      
  code_samples:
    # code sample loop
    - title: "Aggiungi un Watermark Immagine a DOCX"
      content: |
        Questo esempio mostra come applicare effetti di immagine ai watermark di forma.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.wordprocessing as gwow

        # Apri un documento Word
        load_options = gwow.WordProcessingLoadOptions()
        with gw.Watermarker("source.docx", load_options) as watermarker:

            # Imposta le opzioni del watermark
            with gww.ImageWatermark("logo.png") as watermark:

                effects = gwow.WordProcessingImageEffects()
                effects.brightness = 0.7
                effects.contrast = 0.6
                effects.chroma_key = gww.Color.red

                options = gwow.WordProcessingWatermarkSectionOptions()
                options.Effects = effects;

                # Crea il watermark
                watermarker.add(watermark, options)

                # Salva il documento con il watermark
                watermarker.save("result.docx")
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Pronto per iniziare?"
  description: "Prova le funzioni GroupDocs.Watermark gratuitamente o richiedi una licenza"
  items:
    #  loop
    - title: "PyPi scarica"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      color: "red"
        #  loop
    - title: "Licenze"
      link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Proteggi le Tue Foto con Watermark in Python"
    exclude: "PHOTO"
    description: "Aggiungi watermark personalizzati alle tue foto utilizzando la nostra API Python. Mantieni le tue immagini sicure e professionali."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/python-net/add//pdf/"
          description: "Formato documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/python-net/add//word/"
          description: "MS Word e documenti Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/python-net/add//excel/"
          description: "MS Excel e fogli di calcolo Open Office"

        # format loop 4
        - name: "Immagine con filigrana"
          format: "IMAGE"
          link: "/watermark/python-net/add//image/"
          description: "Formati di immagine più diffusi"

        # format loop 5
        - name: "Foto con filigrana"
          format: "PHOTO"
          link: "/watermark/python-net/add//photo/"
          description: "Formati fotografici"

        # format loop 6
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/add//powerpoint/"
          description: "MS PowerPoint e presentazioni Open Office"

        # format loop 7
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/python-net/add//docx/"
          description: "Documento XML aperto Microsoft Word"
          
        # format loop 8
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/python-net/add//pptx/"
          description: "PowerPoint Presentazione XML aperta"
          
        # format loop 9
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/python-net/add//xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"

        # format loop 10
        - name: "Filigrana JPEG"
          format: "JPEG"
          link: "/watermark/python-net/add//jpeg/"
          description: "JPEG Immagine"

        # format loop 11
        - name: "Filigrana PNG"
          format: "PNG"
          link: "/watermark/python-net/add//png/"
          description: "Portable Grafica di rete"

        # format loop 12
        - name: "Filigrana TIFF"
          format: "TIFF"
          link: "/watermark/python-net/add//tiff/"
          description: "Formato del file di immagine per tag"

        # format loop 13
        - name: "Filigrana WEBP"
          format: "WEBP"
          link: "/watermark/python-net/add//webp/"
          description: "Immagine WEB"

        # format loop 14
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/python-net/add//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 15
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/python-net/add//xls/"
          description: "Cartella di lavoro Microsoft Excel 97-2003"

        # format loop 16
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/python-net/add//ppt/"
          description: "PowerPoint Presentazione 97-2003"

        # format loop 17
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/python-net/add//rtf/"
          description: "Formato RTF"

---