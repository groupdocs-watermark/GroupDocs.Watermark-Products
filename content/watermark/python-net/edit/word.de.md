
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: de
format: Word
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Wasserzeichen in Word-Dateien bearbeiten"
head_description: "Optimieren Sie die Wasserzeichen-Einstellungen und verbessern Sie den Dokumentenschutz mit GroupDocs.Watermark for Python via .NET für Word."

############################# Header ############################
title: "Wasserzeichen in Word-Dateien einfach aktualisieren mit Python" 
description: "Schützen Sie Ihre Marke und Dokumente mit GroupDocs.Watermark for Python via .NET. Ändern Sie Wasserzeichen in Word-Dateien schnell."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Jetzt kostenlos auf PyPi herunterladen"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "Erfahre mehr"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Sichern Sie Ihre Word-Dokumente:** Verwenden Sie GroupDocs.Watermark for Python via .NET, um Wasserzeichen einfach zu aktualisieren und zu verwalten, die Ihren Dokumentenanforderungen und Ihrer Markenrichtlinie entsprechen.

############################# Steps ############################
steps:
    enable: true
    title: "Wasserzeichen in Word-Dokumenten mit Python ändern"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** unterstützt Python-Entwickler beim Aktualisieren von Wasserzeichen in verschiedenen Word-Dateien. So können Sie es in Ihrem Projekt verwenden:
      
      1. Zunächst öffnen Sie Ihre Word-Datei, indem Sie sie an den **Watermarker**-Konstruktor übergeben. Sie können einen Dateipfad, einen Byte-Stream oder einen Datei-Stream verwenden.
      2. Dann suchen Sie die Wasserzeichen, die Sie ändern möchten, mithilfe von **SearchCriteria**, mit dem Sie nach Wasserzeichen-Text oder -Eigenschaften suchen können.
      3. Sobald Sie fündig geworden sind, können Sie Details wie Text, Schriftart, Größe, Position, Farbe und mehr ändern. So haben Sie die volle Kontrolle über das Erscheinungsbild des Wasserzeichens.
      4. Nachdem Sie die Änderungen vorgenommen haben, speichern Sie das Dokument. Sie können das Ergebnis in einen Stream oder einen Dateipfad schreiben.
   
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
        # Aktualisieren Sie den Wasserzeichen-Text in WORD
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Erstellen Sie einen Watermarker mit einer WORD-Datei
        with gw.Watermarker("input.docx") as watermarker:

            # Richten Sie TextSearchCriteria ein, um Wasserzeichen-Text zu finden
            search_criteria = gwss.TextSearchCriteria("test", False)

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # Ändern Sie den Wasserzeichen-Text
                        watermark.text = "passed"
                    except Exception as e:
                        pass
            
            watermarker.save("output.docx")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Entdecken Sie weitere Möglichkeiten zur Aktualisierung von Wasserzeichen"
  description: "Mit unserer Bibliothek können Python-Apps Wasserzeichen in vielen Dateitypen hinzufügen, finden, bearbeiten oder löschen."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Wasserzeichenbearbeitung"
  features:
    # feature loop
    - title: "Wasserzeichen in Ihren Dateien verwalten"
      content: "Verwenden Sie GroupDocs.Watermark for Python via .NET, um Wasserzeichen in Ihren Dokumenten hinzuzufügen und zu verwalten. Suchen, aktualisieren oder entfernen Sie Wasserzeichen nach Bedarf mithilfe einer einfachen API."

    # feature loop
    - title: "Wasserzeichen an Ihre Bedürfnisse anpassen"
      content: "Passen Sie Wasserzeichen-Einstellungen wie Schriftart, Größe, Ausrichtung und Farbe mit unserer flexiblen API an, um genau das Ergebnis zu erhalten, das Sie wünschen."

    # feature loop
    - title: "Nutzen Sie format-spezifische Funktionen"
      content: "Je nach Dateiformat können Sie native Funktionen wie Kopfzeilen, Fußzeilen, Anmerkungen oder Hintergründe als Wasserzeichenbereiche verwenden."
      
  code_samples:
    # code sample loop
    - title: "Textwasserzeichen in Excel bearbeiten"
      content: |
        Dieser Code zeigt, wie man den Wasserzeichen-Text in Excel-Tabellenblättern ändert.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # Öffnen Sie die XLSX-Datei
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # Lesen Sie die Tabellendaten
        with gw.Watermarker("source.xlsx") as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,3]

            # Ändern Sie den Wasserzeichen-Text
            watermarks = watermarker.search(search_criteria)
            for watermark in watermarks:
                try:
                    watermark.formatted_text_fragments.clear()
                    watermark.formatted_text_fragments.add(
                       "passed", 
                        gww.Font("Calibri", 19.0, gww.FontStyle.bold), 
                        gww.Color.red, 
                        gww.Color.aqua
                    )
                except Exception as e:
                    pass
        
            # Speichern Sie das Ergebnis
            watermarker.save("output.xlsx")
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
    title: "Wasserzeichen in anderen Dateiformaten"
    exclude: "WORD"
    description: "GroupDocs.Watermark for Python via .NET hilft Ihnen, mehrere Dateitypen mit flexiblen Werkzeugen für Wasserzeichen zu schützen."
    items: 
        # format loop 1
        - name: "Wasserzeichen PDF"
          format: "PDF"
          link: "/watermark/python-net/edit//pdf/"
          description: "Adobe Portable Dokumentformat"

        # format loop 2
        - name: "Wasserzeichen Word"
          format: "WORD"
          link: "/watermark/python-net/edit//word/"
          description: "MS Word und Open Office-Dokumente"
          
        # format loop 3
        - name: "Wasserzeichen Excel"
          format: "EXCEL"
          link: "/watermark/python-net/edit//excel/"
          description: "MS Excel und Open Office-Tabellen"

        # format loop 4
        - name: "Wasserzeichen PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/edit//powerpoint/"
          description: "MS PowerPoint und Open Office-Präsentationen"

        # format loop 5
        - name: "Wasserzeichen DOCX"
          format: "DOCX"
          link: "/watermark/python-net/edit//docx/"
          description: "Microsoft Word XML-Dokument öffnen"
          
        # format loop 6
        - name: "Wasserzeichen PPTX"
          format: "PPTX"
          link: "/watermark/python-net/edit//pptx/"
          description: "PowerPoint XML-Präsentation öffnen"
          
        # format loop 7
        - name: "Wasserzeichen XLSX"
          format: "XLSX"
          link: "/watermark/python-net/edit//xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"

        # format loop 8
        - name: "Wasserzeichen DOC"
          format: "DOC"
          link: "/watermark/python-net/edit//doc/"
          description: "Microsoft Word 97 - 2007-Dokument"

        # format loop 9
        - name: "Wasserzeichen XLS"
          format: "XLS"
          link: "/watermark/python-net/edit//xls/"
          description: "Microsoft Excel Arbeitsmappe 97-2003"

        # format loop 10
        - name: "Wasserzeichen PPT"
          format: "PPT"
          link: "/watermark/python-net/edit//ppt/"
          description: "PowerPoint Präsentation 97-2003"

        # format loop 11
        - name: "Wasserzeichen RTF"
          format: "RTF"
          link: "/watermark/python-net/edit//rtf/"
          description: "Rich-Text-Format"

---