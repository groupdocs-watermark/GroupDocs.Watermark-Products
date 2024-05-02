
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:27:05
draft: false
lang: de
format: Png
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "PNG mit .NET C#-Wasserzeichen sichern"
head_description: "Betten Sie Wasserzeichen mit .NET C# in PNG Dateien ein, perfekt für Bildrechte und Sicherheit."

############################# Header ############################
title: "C#-Wasserzeichen für PNG Dateien" 
description: "Verwenden Sie .NET C#, um erweiterte Wasserzeichen auf PNG Bilder anzuwenden und so künstlerische und digitale Inhalte effektiv zu schützen."
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
       GroupDocs.Watermark for .NET bietet ein spezielles .NET C#-Toolkit zum Einbetten von Wasserzeichen in PNG Dateien, das sich an Künstler, Designer und Inhaltsersteller richtet, die ihre visuellen Ressourcen schützen müssen. Diese API ermöglicht das nahtlose Hinzufügen transparenter und undurchsichtiger Wasserzeichen, die kompliziert positioniert und skaliert werden können, um die Integrität des Originalbilds zu wahren und gleichzeitig den rechtlichen Schutz zu gewährleisten. Zu den Funktionen gehören benutzerdefinierte Text- und Bildwasserzeichen, eine präzise Steuerung der Opazität von Wasserzeichen und die Möglichkeit, mehrschichtige Wasserzeichen hinzuzufügen, um die Sicherheit zu erhöhen. Ob für den persönlichen Gebrauch oder für professionelle Portfolios, GroupDocs.Watermark stellt sicher, dass Ihre PNG Bilder vor unberechtigter Reproduktion und Verwendung geschützt sind und in .NET Umgebungen vollständig unterstützt werden.

############################# Steps ############################
steps:
    enable: true
    title: "Mühelos Wasserzeichen für Png Dokumente generieren"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/) :** Erweiterte Wasserzeichen-Bibliothek für .NET Anwendungen. Machen Sie Ihre Lösung noch leistungsfähiger und sichern Sie Dokumente rechtzeitig mit Wasserzeichen.
      
      1. **Core Class: Watermarker.** Die Hauptklasse unserer API ist **Watermarker**. Sie müssen es vor der Dokumentenverarbeitung instanziieren. Vergessen Sie nicht, die Datei Png als Pfad- oder Stream-Objekt an den Konstruktor zu übergeben.
      2. **Erstellen Sie Ihr Wasserzeichen.** Der nächste Schritt besteht darin, ein Wasserzeichen-Objekt des gewünschten Typs zu erstellen. Es kann nicht nur auf einer bestimmten Dokumentseite platziert werden, sondern auch in systemeigenen Dokumentteilen wie Bildern oder Kopfzeilen.
      3. **Feinabstimmung des Aussehen.** Stellen Sie Wasserzeicheneigenschaften wie Höhe und Breite, obere, linke, mittige Ausrichtung, Schriftarten und Farben usw. ein.
      4. **Anwenden und Speichern.** Verwenden Sie die Methode **Watermarker**, um ein neues Wasserzeichen hinzuzufügen. Fühlen Sie sich frei, so viele Wasserzeichen hinzuzufügen, wie Sie benötigen. Sie können das Dokument mit Wasserzeichen an einem beliebigen Ort speichern.
   
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
        // Bild-Wasserzeichen in PNG -Datei generieren

        // Geben Sie den Quelldateipfad für den Watermarker-Konstruktor an
        using (Watermarker watermarker = new Watermarker("input.png"))
        {
            // Generieren Sie eine Bildwasserzeicheninstanz mit einer Bilddatei
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // Ergebnis mit Wasserzeichen PNG speichern
            watermarker.Save("output.png");
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
    title: "Implementierung von Wasserzeichen in PNG mit C#"
    exclude: "PNG"
    description: "Stellen Sie .NET C# bereit, um diskrete oder fett gedruckte Wasserzeichen in PNG Bildern zu erstellen und dabei sowohl ästhetische Flexibilität als auch robusten Urheberrechtsschutz zu gewährleisten."
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