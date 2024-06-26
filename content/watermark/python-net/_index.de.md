---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:49
draft: false

lang: de
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"
    # supported_platforms loop
    - title: "Python"
      tag: "python-net"

############################# Head ############################
head_title: "Python Wasserzeichenbibliothek | Dokumentwasserzeichen"
head_description: "Python schützt Geschäftsdokumente mit Text- und Bildwasserzeichen. Dateiformate wie PDF, Word, Excel und PowerPoint werden unterstützt."

############################# Header ############################
title: "Greifen Sie auf die Wasserzeichentechnologie von Python via .NET zu"
description: "Schützen Sie Ihre Daten und verhindern Sie unbefugtes Kopieren mit dieser Python-Lösung. Fügen Sie ganz einfach Wasserzeichen zu Geschäftsdokumenten in verschiedenen Formaten hinzu, darunter PDF, Word, Excel, PowerPoint, Bilder usw."
words:
  for: "zum"

actions:
  main: "PyPi kostenlos herunterladen"
  main_link: "https://pypi.org/project/groupdocs-watermark-net/"
  alt: "Lizenzierung"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
  title: "Bereit loszulegen?"
  description: "Testen Sie GroupDocs.Watermark Funktionen kostenlos oder fordern Sie eine Lizenz an"

release:
  title: "Version {0} veröffentlicht"
  notes: "Schau dir an, was es Neues gibt"
  downloads: "herunterladbare"
  link: "https://releases.groupdocs.com/watermark/python-net/"

code:
  title: "Wasserzeichen zu PDF hinzufügen mit Python"
  more: "Mehr Beispiele"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
  install: "pip install groupdocs-watermark-net"
  content: |
    ```python {style=abap}

    import groupdocs.watermark as gw
    import groupdocs.watermark.watermarks as gww
    import groupdocs.watermark.options.pdf as gwop
    import groupdocs.watermark.common as gwc

    # Instanziieren Sie den Wassermarker, der den PDF -Pfad übergibt
    pdf_lo = gwop.PdfLoadOptions()
    with gw.Watermarker("source.pdf", pdf_lo) as watermarker:
        options = gwop.PdfArtifactWatermarkOptions()

        # Passen Sie die Wasserzeichenoptionen an
        text_watermark = 
            gww.TextWatermark("Approved", gww.Font("Arial", 8.0))
        text_watermark.horizontal_alignment = 
            gwc.HorizontalAlignment.RIGHT

        # Wasserzeichen auf PDF Dokument anwenden
        watermarker.add(text_watermark, options)

        # Ergebnisdokument speichern
        watermarker.save("result.pdf")

    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark auf einen Blick"
  description: "Python Bibliothek für Wasserzeichen"
  features:
    # feature loop
    - title: "Python Dokument-Wasserzeichen"
      content: "Sichern Sie Ihre sensiblen Daten mit GroupDocs.Watermark for Python via .NET. Fügen Sie Text oder Bilder als Wasserzeichen in verschiedene Dateiformate ein."

    # feature loop
    - title: "Passen Sie Wasserzeichen an"
      content: "In GroupDocs.Watermark for Python via .NET sind viele Anpassungsoptionen verfügbar. Richten Sie Textstile (Fett, Kursiv, Schriftart) oder Bildeigenschaften wie Größe oder Drehung ein, um das Wasserzeichen im Dokument zu optimieren."

    # feature loop
    - title: "Unterstützung beliebter Dateiformate"
      content: "GroupDocs.Watermark for Python via .NET unterstützt eine Vielzahl von Dateiformaten, darunter PDF, MS Office-Dokumente wie Word, Excel, PowerPoint und Bilder wie JPEG, PNG, GIF, BMP, Visio-Diagramme, E-Mails usw. Verbessern Sie die Dokumentenverarbeitung, um Ihren Anforderungen gerecht zu werden Ziele."

    # feature loop
    - title: "Suche und Aktualisierung von Wasserzeichen"
      content: "Rufen Sie Wasserzeichen ab, die in Dokumenten platziert sind, und aktualisieren Sie sie. Ändern Sie den Textstil und den Bildinhalt oder entfernen Sie sie vollständig. GroupDocs.Watermark for Python via .NET bietet eine breite Palette an Wasserzeichenverarbeitungsfunktionen."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformunabhängigkeit"
  description: "GroupDocs.Watermark for Python via .NET lässt sich nahtlos in verschiedene Betriebssysteme und Paketmanager integrieren."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Unterstützte Dateiformate"
  description: |
    GroupDocs.Watermark for Python via .NET ermöglicht Ihnen die Verarbeitung einer Vielzahl von Dateiformaten. [Erkunden Sie die vollständige Liste](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office & OpenDocument Formate
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### Bilder & Grafiken
        * **Beliebte Bildformate:** BMP, JPG, JPEG, PNG
        * **Mehrseitige Bilder:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### Andere
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark for Python via .NET-Funktionen"
  description: "Stärken Sie die Dokumentensicherheit durch programmatische Wasserzeichen. Verarbeiten Sie verschiedene Dateiformate, darunter PDF, DOCX, XLSX, PPTX und Bildformate (PNG, JPG usw.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Präzise Wasserzeichensteuerung"
      content: "Verwalten Sie Wasserzeichen präzise, ​​indem Sie sie zu bestimmten Abschnitten, ganzen Dokumenten oder einzelnen Anhängen und Formen in verschiedenen Dateiformaten hinzufügen oder entfernen."

    # feature loop
    - icon: "watermark_style"
      title: "Passen Sie das Erscheinungsbild des Wasserzeichens an"
      content: "Üben Sie eine differenzierte Kontrolle über die Ästhetik des Wasserzeichens aus, indem Sie Attribute wie Farbe, Schriftart, Deckkraft, Drehung und Positionierung innerhalb des Dokuments ändern."

    # feature loop
    - icon: "hidden_print"
      title: "PDF-Wasserzeichen drucken"
      content: "Fügen Sie versteckte Wasserzeichen in normale Dokumente ein, die erst während des Druckvorgangs sichtbar werden, und erhöhen Sie so diskret die Dokumentensicherheit."

    # feature loop
    - icon: "image_only"
      title: "Spezifisches Bildwasserzeichen"
      content: "Mit unserer Lösung können Sie bestimmte Bilder in einem Dokument mit Wasserzeichen versehen. Betten Sie Wasserzeichen in einem bestimmten Abschnitt (z. B. einer Seite, einer Folie) oder im gesamten Dokument ein."

    # feature loop
    - icon: "image_frame"
      title: "Mehrschichtige Bildwasserzeichen"
      content: "Fügen Sie Wasserzeichen präzise zu bestimmten Frames innerhalb eines Bildformats mit mehreren Frames hinzu und erreichen Sie so eine detaillierte Kontrolle über die Platzierung von Wasserzeichen."

    # feature loop
    - icon: "attachments"
      title: "Umfassender Inhaltsschutz"
      content: "Erweitern Sie den Schutz auf verschiedene Dokumentelemente wie Anhänge in Excel-Dokumenten und Bildformen in Präsentationen und bieten Sie so eine zusätzliche Sicherheitsebene."

    # feature loop
    - icon: "pdf_objects"
      title: "Erweiterte PDF-Wasserzeichen"
      content: "Versehen Sie verschiedene Bereiche von PDFs mit Wasserzeichen, einschließlich Anschnitt-Box, Art-Box, Zuschnitt-Box, Endformat-Box usw."

    # feature loop
    - icon: "doc_background"
      title: "Hintergrundbild-Wasserzeichen"
      content: "Verwalten Sie Wasserzeichen in den Hintergrundbildern von Tabellenkalkulationen und Präsentationen und bieten Sie so zusätzliche Anpassungsoptionen für visuelle Sicherheitsmaßnahmen."

    # feature loop
    - icon: "unreadable_characters"
      title: "Textwasserzeichen mit unleserlichen Zeichen"
      content: "Verwenden Sie unleserliche Zeichen in Textwasserzeichen, die in Präsentationen eingebettet sind, und erhöhen Sie so die Sicherheit, indem Sie die unbefugte Extraktion von Wasserzeichen erheblich erschweren."

    # feature loop
    - icon: "watermark_text_search"
      title: "Erweiterte Wasserzeichensuche"
      content: "Nutzen Sie umfassende Suchfunktionen, um Wasserzeichen in Dokumenten anhand bestimmter Parameter oder durch die Kombination verschiedener Kriterien zu finden."

    # feature loop
    - icon: "watermark_image_search"
      title: "Erkennung ähnlicher Bildwasserzeichen"
      content: "Suchen Sie in Dokumenten nach ähnlichen Wasserzeichenbildern, die optisch einem Quellbild ähneln."

    # feature loop
    - icon: "document_info"
      title: "Dokumentinformationen analysieren"
      content: "Extrahieren Sie wichtige Dokumentdaten wie die Seiteneinrichtung zur weiteren Analyse."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Codebeispiele"
  description: "Entdecken Sie Codebeispiele, die gängige GroupDocs.Watermark for Python via .NET-Funktionen veranschaulichen."
  items:
    # code sample loop
    - title: "Versehen Sie ein Dokument mit einem Bild mit einem Wasserzeichen"
      content: |
        Verwenden Sie GroupDocs.Watermark for Python via .NET, um Dokumente durch das Hinzufügen von Bildwasserzeichen zu schützen. [Weitere Informationen](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="So schützen Sie eine Datei mit einem Bildwasserzeichen.">}}
        ```python {style=abap}

        # Quelldokument in Watermarker laden
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Pfad zu einem Wasserzeichenbild angeben
            watermark = groupdocs.watermark.watermarks.ImageWatermark("watermark.jpg")
            watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwgroupdocs.watermark.common.VerticalAlignment.CENTER

            # Schützen Sie die Datei und speichern Sie sie
            watermarker.add(watermark)
            watermarker.save("result.pdf")
       
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Vorhandene Wasserzeichen suchen und ändern"
      content: |
        GroupDocs.Watermark for Python via .NET ermöglicht Ihnen die Verwaltung von Dokumentwasserzeichen. Wählen Sie Wasserzeichen aus und ändern Sie ihre Eigenschaften. [Entdecken Sie, wie](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Suche und Änderung von Wasserzeichen.">}}
        ```python {style=abap}

        # Quelldokument laden
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Suchen Sie nach Wasserzeichen, die aktualisiert werden sollen
            search_criteria = groupdocs.watermark.search.searchcriteria.TextSearchCriteria("annotation", False)
            watermarks = watermarker.search(search_criteria)
            
            # Gewünschte Eigenschaften aktualisieren
            for watermark in watermarks:
                watermark.text = "passed"

            # Speichern Sie das geänderte Dokument in einem angegebenen Pfad
            watermarker.save("result.pdf")


        ```
        {{< /landing/code >}}

---
