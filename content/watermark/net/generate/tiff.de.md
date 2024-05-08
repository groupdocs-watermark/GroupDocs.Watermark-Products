
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:23
draft: false
lang: de
format: Tiff
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Generieren Sie TIFF Wasserzeichen mit C#"
head_description: "Erstellen und fügen Sie mit .NET C# präzise Wasserzeichen zu TIFF Bildern hinzu, um Ihre digitalen Inhalte zu schützen."

############################# Header ############################
title: "Erstellen Sie Wasserzeichen für TIFF mit C#" 
description: "Generieren Sie robuste, benutzerdefinierte Wasserzeichen in TIFF Dateien mit .NET C#, unverzichtbar für den Schutz und die Verwaltung digitaler und archivierter Bilder."
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlos unter Nuget herunterladen"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "Erfahre mehr"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET bietet ein umfassendes .NET C#-Toolkit zum Generieren, Verfassen und Hinzufügen von Wasserzeichen zu TIFF Dateien. Diese Lösung ist auf die besonderen Anforderungen digitaler Archive und professioneller Fotografie zugeschnitten, bei denen die Aufrechterhaltung der Bildqualität und der Urheberrechtsschutz von größter Bedeutung sind. Benutzer können die Opazität, den Maßstab und die Position von Wasserzeichen anpassen, um sicherzustellen, dass sie nahtlos integriert werden, ohne das Bild zu beeinträchtigen. Die Möglichkeit, textuelle oder grafische Wasserzeichen zu erzeugen, in Verbindung mit fortschrittlichen Funktionen wie Wasserzeichen-Layering und bedingter Formatierung macht GroupDocs.Watermark zu einem unverzichtbaren Tool für alle, die ihre visuellen Ressourcen schützen müssen. Diese API ist vollständig kompatibel mit den neuesten .NET Umgebungen und verbessert Ihre Fähigkeit, TIFF Bilder effektiv zu verwalten und zu sichern.

############################# Steps ############################
steps:
    enable: true
    title: "Generieren Sie mühelos Wasserzeichen für Tiff-Dokumente"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/):** Erweiterte Wasserzeichenbibliothek für .NET-Anwendungen. Stärken Sie Ihre Lösung und sichern Sie Dokumente rechtzeitig mit Wasserzeichen.
      
      1. **Kernklasse: Watermarker.** Die Hauptklasse unserer API ist **Watermarker**. Sie müssen es vor der Dokumentverarbeitung instanziieren. Vergessen Sie nicht, die Datei Tiff als Pfad oder Stream-Objekt an den Konstruktor zu übergeben.
      2. **Erstellen Sie Ihr Wasserzeichen.** Der nächste Schritt besteht darin, ein Wasserzeichenobjekt des gewünschten Typs zu erstellen. Es kann nicht nur auf einer bestimmten Dokumentseite, sondern auch in nativen Dokumentteilen wie Bildern oder Kopfzeilen platziert werden.
      3. **Optimierung der Darstellung.** Legen Sie Wasserzeicheneigenschaften wie Höhe und Breite, Ausrichtung oben, links, mittig, Schriftarten und Farben usw. fest.
      4. **Anwenden und Speichern.** Verwenden Sie die Methode **Watermarker**, um ein neues Wasserzeichen hinzuzufügen. Sie können beliebig viele Wasserzeichen hinzufügen. Sie können das mit Wasserzeichen versehene Dokument an einem beliebigen Ort speichern.
   
    code:
      platform: "net"
      copy_title: "Kopieren"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "zum Kopieren anklicken"
        copy_done: "kopiert"
      links:
        #  loop
        - title: "Mehr Beispiele"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "Dokumentation"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // Bildwasserzeichen in der Datei TIFF generieren

        // Geben Sie den Pfad der Quelldatei zum Konstruktor Watermarker an
        using (Watermarker watermarker = new Watermarker("input.tiff"))
        {
            // Generieren Sie eine Bildwasserzeicheninstanz mit einer Bilddatei
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // Mit Wasserzeichen versehenes TIFF-Ergebnis speichern
            watermarker.Save("output.tiff");
        }
        
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "Verbessern Sie Ihr Wasserzeichen-Spiel"
  description: "Erschließen Sie erweiterte Wasserzeichenfunktionen mit unserer GroupDocs.Watermark API für .NET. Dieses leistungsstarke Tool ermöglicht die präzise Anpassung und Anbringung von Wasserzeichen für verschiedene Dokumenttypen, um maximale Sicherheit und Einhaltung der Urheberrechte bei minimaler visueller Beeinträchtigung zu gewährleisten."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Umfassende Wasserzeichenlösungen"
  features:
    # feature loop
    - title: "Raffinierte Optionen für die Verlegung von Fliesen"
      content: "Erweitern Sie Ihre Wasserzeichen mit unseren Kacheloptionen nahtlos auf ganze Dokumente. Mit dieser Funktion können Wasserzeichen den gesamten Dokumentbereich abdecken, sodass das Entfernen verhindert wird und ein vollständiger Schutz der Dokumente gewährleistet ist, ohne dass das Design oder die Lesbarkeit beeinträchtigt werden."

    # feature loop
    - title: "Lebendige Farbanpassung"
      content: "Verleihen Sie Ihren Wasserzeichen einen Farbtupfer! Unsere API ermöglicht die vollständige Farbanpassung, sodass Sie Wasserzeichen anbringen können, die perfekt zu Ihrem Unternehmensmarke oder Dokumentstil passen. Verbessern Sie die visuelle Attraktivität und behalten Sie gleichzeitig robuste Sicherheitsfunktionen bei."

    # feature loop
    - title: "Verbesserte Sicherheitseinstellungen"
      content: "Bringen Sie die Dokumentensicherheit mit erweiterten Wasserzeicheneinstellungen auf die nächste Stufe. Konfigurieren Sie mehrschichtige Wasserzeichen, die sowohl sichtbare als auch unsichtbare Elemente enthalten, um sich vor unbefugtem Kopieren zu schützen und sicherzustellen, dass nur die vorgesehenen Empfänger auf wichtige Informationen zugreifen können."
      
  code_samples:
    # code sample loop
    - title: "PowerPoint Wasserzeichen generieren"
      content: |
        Dieses Beispiel zeigt, wie Sie den PPTX Hintergrundbildern ein Wasserzeichen hinzufügen
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  PPTX Präsentation laden
            var loadOptions = new PresentationLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pptx", loadOptions))
            {
                //  Wasserzeicheneigenschaften einrichten
                TextWatermark watermark = new TextWatermark("Protected image", new Font("Arial", 8));
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermark.RotateAngle = 45;
                watermark.SizingType = SizingType.ScaleToParentDimensions;
                watermark.ScaleFactor = 1;

                //  Hintergrund der Wasserzeichen-Folien
                PresentationContent content = watermarker.GetContent<PresentationContent>();
                foreach (PresentationSlide slide in content.Slides)
                {
                    if (slide.ImageFillFormat.BackgroundImage != null)
                    {
                        slide.ImageFillFormat.BackgroundImage.Add(watermark);
                    }
                }

                //  Bearbeitete Präsentation speichern
                watermarker.save("result.pptx");
            }

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Bereit loszulegen?"
  description: "Testen Sie GroupDocs.Watermark Funktionen kostenlos oder fordern Sie eine Lizenz an"
  items:
    #  loop
    - title: "Nuget herunterladen"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "Lizenzierung"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Verbesserung der TIFF -Sicherheit mit C#-Wasserzeichen"
    exclude: "TIFF"
    description: "Verwenden Sie .NET C#, um benutzerdefinierte Wasserzeichen zu generieren und in TIFF Dateien zu integrieren, um Ihren Bildern eine Ebene der Sicherheit und Copyright-Kontrolle zu verleihen."
    items: 
        # format loop 1
        - name: "Wasserzeichen PDF"
          format: "PDF"
          link: "/watermark/net/generate//pdf/"
          description: "Adobe Portable Dokumentformat"

        # format loop 2
        - name: "Wasserzeichen Word"
          format: "WORD"
          link: "/watermark/net/generate//word/"
          description: "MS Word und Open Office-Dokumente"
          
        # format loop 3
        - name: "Wasserzeichen Excel"
          format: "EXCEL"
          link: "/watermark/net/generate//excel/"
          description: "MS Excel und Open Office-Tabellen"

        # format loop 4
        - name: "Wasserzeichen-Bild"
          format: "IMAGE"
          link: "/watermark/net/generate//image/"
          description: "Beliebte Bildformate"

        # format loop 5
        - name: "Wasserzeichen-Foto"
          format: "PHOTO"
          link: "/watermark/net/generate//photo/"
          description: "Foto-Formate"

        # format loop 6
        - name: "Wasserzeichen PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/generate//powerpoint/"
          description: "MS PowerPoint und Open Office-Präsentationen"

        # format loop 7
        - name: "Wasserzeichen DOCX"
          format: "DOCX"
          link: "/watermark/net/generate//docx/"
          description: "Microsoft Word XML-Dokument öffnen"
          
        # format loop 8
        - name: "Wasserzeichen PPTX"
          format: "PPTX"
          link: "/watermark/net/generate//pptx/"
          description: "PowerPoint XML-Präsentation öffnen"
          
        # format loop 9
        - name: "Wasserzeichen XLSX"
          format: "XLSX"
          link: "/watermark/net/generate//xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"

        # format loop 10
        - name: "Wasserzeichen JPEG"
          format: "JPEG"
          link: "/watermark/net/generate//jpeg/"
          description: "JPEG Bild"

        # format loop 11
        - name: "Wasserzeichen PNG"
          format: "PNG"
          link: "/watermark/net/generate//png/"
          description: "Portable Netzwerkgrafik"

        # format loop 12
        - name: "Wasserzeichen TIFF"
          format: "TIFF"
          link: "/watermark/net/generate//tiff/"
          description: "Tag-Bilddateiformat"

        # format loop 13
        - name: "Wasserzeichen WEBP"
          format: "WEBP"
          link: "/watermark/net/generate//webp/"
          description: "WEB-Bild"

        # format loop 14
        - name: "Wasserzeichen DOC"
          format: "DOC"
          link: "/watermark/net/generate//doc/"
          description: "Microsoft Word 97 - 2007-Dokument"

        # format loop 15
        - name: "Wasserzeichen XLS"
          format: "XLS"
          link: "/watermark/net/generate//xls/"
          description: "Microsoft Excel Arbeitsmappe 97-2003"

        # format loop 16
        - name: "Wasserzeichen PPT"
          format: "PPT"
          link: "/watermark/net/generate//ppt/"
          description: "PowerPoint Präsentation 97-2003"

        # format loop 17
        - name: "Wasserzeichen RTF"
          format: "RTF"
          link: "/watermark/net/generate//rtf/"
          description: "Rich-Text-Format"

---