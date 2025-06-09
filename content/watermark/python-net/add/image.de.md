
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: de
format: Image
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Wasserzeichen für Bilder mit Python"
head_description: "Erfahren Sie, wie Sie Wasserzeichen zu Bildern in Python hinzufügen. Schützen Sie Ihre Bilder, ohne die Qualität zu verlieren."

############################# Header ############################
title: "Schnelles Bild-Wasserzeichnen mit Python" 
description: "Unser Python-Tool ermöglicht es Ihnen, schnell Wasserzeichen zu Bildern hinzuzufügen. Unterstützt viele Formate, von Fotos bis digitale Kunst."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Laden Sie PyPi kostenlos herunter"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "Erfahre mehr"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET hilft Ihnen, Wasserzeichen zu Bildern in Python hinzuzufügen. Es unterstützt JPEG, PNG, BMP, TIFF und mehr. Sie können die Opazität, Größe und Position des Wasserzeichens anpassen, um Ihre Bedürfnisse zu erfüllen. Nutzen Sie es, um Ihre Bilder zu schützen oder Branding hinzuzufügen, während die Originalqualität erhalten bleibt.

############################# Steps ############################
steps:
    enable: true
    title: "Wasserzeichen hinzufügen: Python Wasserzeichen für Image"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** ist eine Bibliothek, die das Hinzufügen von Wasserzeichen zu vielen Geschäftsdokumenttypen erleichtert. Befolgen Sie diese Schritte, um schnell Wasserzeichen in Ihren Dokumenten in Python hinzuzufügen:
      
      1. **Erste Schritte mit Wasserzeichen:** Beginnen Sie, indem Sie eine Instanz der **Watermarker**-Klasse erstellen. Übergeben Sie Ihre Image-Datei (als Pfad oder Stream) an den Konstruktor, um sie für die Wasserzeichenbearbeitung zu öffnen.
      2. **Erstellen Sie Ihr Wasserzeichen:** Erstellen Sie ein **Watermark**-Objekt mit Ihrem gewünschten Text und den entsprechenden Einstellungen. Sie können Wasserzeichen auf beliebigen Seiten oder sogar auf Dokumentelementen wie Kopfzeilen oder Anhängen hinzufügen.
      3. **Passen Sie das Wasserzeichen an:** Passen Sie die Größe, Position, Schriftart, Farbe und Ausrichtung des Wasserzeichens an, um Ihren Anforderungen gerecht zu werden. Dies hilft, dass Ihr Wasserzeichen perfekt in Ihr Dokument passt.
      4. **Anwenden und Speichern:** Verwenden Sie die Methode **Watermarker**, um Ihr(e) Wasserzeichen zum Dokument hinzuzufügen. Speichern Sie das Ergebnis idealerweise in einer neuen Datei zur Sicherheit.
   
    code:
      platform: "python-net"
      copy_title: "Kopieren"
      install:
        command: |
        command: "pip install groupdocs-watermark-net"
        copy_tip: "zum Kopieren anklicken"
        copy_done: "kopiert"
      links:
        #  loop
        - title: "Mehr Beispiele"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
        #  loop
        - title: "Dokumentation"
          link: "https://docs.groupdocs.com/watermark/python-net/"
          
      content: |
        ```python {style=abap}
        # Fügen Sie ein Text-Wasserzeichen zu einer IMAGE-Datei hinzu
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # Wählen Sie die Datei aus, die Sie mit einem Wasserzeichen versehen möchten
        with gw.Watermarker("input.jpeg") as watermarker:

            # Erstellen Sie ein Text-Wasserzeichen-Objekt
            font = gww.Font("Arial", 36.0)
            watermark = gww.TextWatermark("top secret", font)
            watermark.foreground_color = gww.Color.red
            watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
            watermark.opacity = 0.4

            watermarker.add(watermark)

            # Speichern Sie die aktualisierte IMAGE-Datei
            watermarker.save("output.jpeg")
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Entdecken Sie Weitere Wasserzeichen-Funktionen"
  description: "Nutzen Sie unsere Python-API, um Wasserzeichen in Dokumenten, Folien, Diagrammen und mehr hinzuzufügen, anzuzeigen, zu konvertieren und zu verwalten. GroupDocs.Watermark for Python via .NET hilft Ihnen, Ihre Dateien zu schützen und Copyright-Informationen einfach hinzuzufügen."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Wasserzeichen hinzufügen"
  features:
    # feature loop
    - title: "Wasserzeichen einfach hinzufügen"
      content: "GroupDocs.Watermark ermöglicht es Python-Entwicklern, Text-, Bild- oder dynamische Wasserzeichen schnell zu Geschäftsdokumenten hinzuzufügen. Halten Sie Ihre Dateien sicher und gebrandet mit minimalem Aufwand."

    # feature loop
    - title: "Vollständig anpassbare Wasserzeichen"
      content: "Ändern Sie die Größe, Drehung, Transparenz, Farbe und Schriftart des Wasserzeichens mit GroupDocs.Watermark. Gestalten Sie Ihr Wasserzeichen so, dass es perfekt zu Ihrem Dokument passt, während wichtige Inhalte sichtbar bleiben."

    # feature loop
    - title: "Dokumentfunktionen für Wasserzeichen nutzen"
      content: "Nutzen Sie integrierte Dokumentfunktionen wie PDF-Anmerkungen, Word-Hintergründe oder Excel-Kopfzeilen, um Wasserzeichen hinzuzufügen. GroupDocs.Watermark arbeitet mit Dokumentstrukturen für effektives, nicht störendes Wasserzeichnen."
      
  code_samples:
    # code sample loop
    - title: "Fügen Sie ein Bild-Wasserzeichen zu DOCX hinzu"
      content: |
        Dieses Beispiel zeigt, wie man Bildeffekte auf Formwasserzeichen anwendet.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.wordprocessing as gwow

        # Öffnen Sie ein Word-Dokument
        load_options = gwow.WordProcessingLoadOptions()
        with gw.Watermarker("source.docx", load_options) as watermarker:

            # Stellen Sie die Wasserzeichenoptionen ein
            with gww.ImageWatermark("logo.png") as watermark:

                effects = gwow.WordProcessingImageEffects()
                effects.brightness = 0.7
                effects.contrast = 0.6
                effects.chroma_key = gww.Color.red

                options = gwow.WordProcessingWatermarkSectionOptions()
                options.Effects = effects;

                # Erstellen Sie das Wasserzeichen
                watermarker.add(watermark, options)

                # Speichern Sie das Dokument mit dem Wasserzeichen
                watermarker.save("result.docx")
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Bereit loszulegen?"
  description: "Testen Sie GroupDocs.Watermark Funktionen kostenlos oder fordern Sie eine Lizenz an"
  items:
    #  loop
    - title: "PyPi herunterladen"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      color: "red"
        #  loop
    - title: "Lizenzierung"
      link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Fügen Sie Wasserzeichen zu Bildern mit Python hinzu"
    exclude: "IMAGE"
    description: "Schützen Sie Ihre Bilder mit unserem Python-Toolkit. Fügen Sie schnell und einfach Wasserzeichen zu vielen Bildformaten hinzu."
    items: 
        # format loop 1
        - name: "Wasserzeichen PDF"
          format: "PDF"
          link: "/watermark/python-net/add//pdf/"
          description: "Adobe Portable Dokumentformat"

        # format loop 2
        - name: "Wasserzeichen Word"
          format: "WORD"
          link: "/watermark/python-net/add//word/"
          description: "MS Word und Open Office-Dokumente"
          
        # format loop 3
        - name: "Wasserzeichen Excel"
          format: "EXCEL"
          link: "/watermark/python-net/add//excel/"
          description: "MS Excel und Open Office-Tabellen"

        # format loop 4
        - name: "Wasserzeichen-Bild"
          format: "IMAGE"
          link: "/watermark/python-net/add//image/"
          description: "Beliebte Bildformate"

        # format loop 5
        - name: "Wasserzeichen-Foto"
          format: "PHOTO"
          link: "/watermark/python-net/add//photo/"
          description: "Foto-Formate"

        # format loop 6
        - name: "Wasserzeichen PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/add//powerpoint/"
          description: "MS PowerPoint und Open Office-Präsentationen"

        # format loop 7
        - name: "Wasserzeichen DOCX"
          format: "DOCX"
          link: "/watermark/python-net/add//docx/"
          description: "Microsoft Word XML-Dokument öffnen"
          
        # format loop 8
        - name: "Wasserzeichen PPTX"
          format: "PPTX"
          link: "/watermark/python-net/add//pptx/"
          description: "PowerPoint XML-Präsentation öffnen"
          
        # format loop 9
        - name: "Wasserzeichen XLSX"
          format: "XLSX"
          link: "/watermark/python-net/add//xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"

        # format loop 10
        - name: "Wasserzeichen JPEG"
          format: "JPEG"
          link: "/watermark/python-net/add//jpeg/"
          description: "JPEG Bild"

        # format loop 11
        - name: "Wasserzeichen PNG"
          format: "PNG"
          link: "/watermark/python-net/add//png/"
          description: "Portable Netzwerkgrafik"

        # format loop 12
        - name: "Wasserzeichen TIFF"
          format: "TIFF"
          link: "/watermark/python-net/add//tiff/"
          description: "Tag-Bilddateiformat"

        # format loop 13
        - name: "Wasserzeichen WEBP"
          format: "WEBP"
          link: "/watermark/python-net/add//webp/"
          description: "WEB-Bild"

        # format loop 14
        - name: "Wasserzeichen DOC"
          format: "DOC"
          link: "/watermark/python-net/add//doc/"
          description: "Microsoft Word 97 - 2007-Dokument"

        # format loop 15
        - name: "Wasserzeichen XLS"
          format: "XLS"
          link: "/watermark/python-net/add//xls/"
          description: "Microsoft Excel Arbeitsmappe 97-2003"

        # format loop 16
        - name: "Wasserzeichen PPT"
          format: "PPT"
          link: "/watermark/python-net/add//ppt/"
          description: "PowerPoint Präsentation 97-2003"

        # format loop 17
        - name: "Wasserzeichen RTF"
          format: "RTF"
          link: "/watermark/python-net/add//rtf/"
          description: "Rich-Text-Format"

---