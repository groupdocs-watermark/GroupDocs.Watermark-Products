---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET-API zum Hinzufügen von Suchen und Entfernen von Wasserzeichen zu Word-Excel-PDF-Bildern"
head_description: "C# .NET API zum Hinzufügen, Suchen und Entfernen von bild- und textbasierten Wasserzeichen aus Dokumenten: PDF, Word, Excel, Präsentationen, Visio, E-Mail und Bilddateiformate."

############################# Header ############################
title: ".NET-API für die Wasserzeichenbearbeitung"
description: "Erstellen Sie .NET-Anwendungen, um text- und bildbasierte Wasserzeichen mit intelligenter Suche und starken Sicherheitsmerkmalen zu betreiben."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Watermark for .NET"
        image: "/border/groupdocs-watermark-net.svg"
        product: "GroupDocs.Watermark"
        platform: ".NET"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Überblick"

            # button loop
            - link: "#features"
              text: "Merkmale"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/watermark"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/watermark/net"
              text: "Preisgestaltung"

    right:
        link_download: "https://downloads.groupdocs.com/watermark"
        link_learn: "https://docs.groupdocs.com/watermark/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Überblick ############################
overview:
    enable: true
    content: |
      GroupDocs.Watermark für .NET ermöglicht es Ihnen, marktreife Geschäftsanwendungen C#, ASP.NET und anderen .NET-bezogenen Technologien zu erstellen, mit denen Ihre Endbenutzer neue Wasserzeichen hinzufügen und vorhandene Wasserzeichen in unterstützten Dateiformaten suchen und entfernen können . Mit GroupDocs.Watermark für .NET können Sie digitale Wasserzeichen programmgesteuert auf eine Vielzahl von Dateiformaten anwenden und die unbefugte Nutzung von geistigem Eigentum verhindern und vertrauliche Dokumente sicher kennzeichnen, indem Sie verschiedene integrierte Sicherheitsmaßnahmen anwenden, die von dieser API angeboten werden.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Nachfolgend finden Sie eine Übersicht über GroupDocs.Watermark für .NET:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Überblick"
          content: |
            * Wasserzeichen hinzufügen und entfernen
            * Wasserzeichen suchen & ersetzen
            * Suche nach Formatierung
            * Suche nach Bildvergleich
            * Arbeiten Sie mit Kopf- und Fußzeilen
            * Arbeiten Sie mit Hintergrundbildern
            * Mit Anhängen arbeiten
            * Seiten rastern
            * Wenden Sie Bearbeitungsbeschränkungen an
      
      ## TAB TWO ##
      tab_two:
        description: |
          Unterstützte [Dokumentformate und Wasserzeichentyp](https://docs.groupdocs.com/watermark/net/supported-document-formats/) für jedes Format sind unten aufgeführt:

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
                * **Visio:** VSD, VDX, VSS, VSSX, VSX, VST, VSTX, VTX, VSDX, VDW, VSTM, VSSM, VSDM

            # table loop
            - title: "Wasserzeichen hinzufügen"
              content: |
                * **PDF**: XObject, Artefakt, Anmerkung
                * **Wort**: Form
                * **Excel**: Form, Kopf- und Fußzeile
                * **PowerPoint**: Form
                * **Visio**: Form
                * **Rasterbild**: Text, Bild
                * **Mehrseitiges TIFF**: Text, Bild
                * **Animiertes Gif**: Text, Bild

        right:
          enable: true
          table:
            # table loop
            - title: "PDF- und Bilddokumente"
              content: |
                * **Portables Dokumentenformat**: PDF
                * **Open Document**: ODT
                * **Email**: EML, MSG, EMLX, OFT
                * **Images**: PNG, BMP, GIF, JPG, JPEG, JP2, TIF, TIFF, WebP

            # table loop
            - title: "Wasserzeichen entfernen"
              content: |
                * **PDF**: XObject, Artefakt, Anmerkung, normaler Text
                * **Wort**: Form, normaler Text
                * **Excel**: Form, Kopf- und Fußzeile, Hintergrundbild, Text und Formeln in Zellen
                * **PowerPoint**: Form
                * **Visio**: Form, Diagrammkommentare
                * **E-Mail**: Angehängte und eingebettete Bilder, Betreff- und Textfragmente

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Watermark for .NET unterstützt das Folgen Betriebssysteme, Frameworks & Paket-Manager:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Betriebssysteme"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux

            # table loop
            - icon: "fas fa-code"
              title: "Unterstützte Frameworks"
              content: |
                * .NET Framework 2.0 oder höher
                * Mono Framework 1.2 oder höher
                * .NET-Standard 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Paket-Manager"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Entwicklungsumgebungen"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Merkmale ############################
features:
    enable: true
    title: "GroupDocs.Watermark for .NET Merkmale"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Hinzufügen oder Entfernen von Wasserzeichen aus einem bestimmten Abschnitt oder einem ganzen Dokument in verschiedenen Dateiformaten"

      # feature loop
      - icon: "fas fa-eye"
        content: "Fügen Sie allen Bildern in einem bestimmten Abschnitt, einer Seite, einer Folie oder einem Dokument ein Wasserzeichen hinzu"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Weisen Sie Wasserzeichen nur bestimmten Frames eines Bildes mit mehreren Frames zu"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "PDF verstecktes Wasserzeichen zuweisen, das nur beim Drucken des Dokuments erscheint"

      # feature loop
      - icon: "fas fa-code"
        content: "Legen Sie Wasserzeichen für alle Anhänge in einem Excel-Dokument und alle Bildformen in Folien fest"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Platzieren Sie Wasserzeichen oder entfernen Sie es aus den Hintergrundbildern von Tabellenkalkulationen oder Folien"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Verwenden Sie Wasserzeichen für unterstützte Dateien in allen Anhängen einer E-Mail oder eines PDF-Dokuments"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Anwenden oder Entfernen von Wasserzeichen als XObjects, Artefakte und Anmerkungen in PDF-Dokumenten"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Beseitigen Sie Wasserzeichen, die Text mit einer bestimmten Formatierung enthalten"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Suchen Sie nach Bildwasserzeichen, die einem bestimmten Bild ähneln"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Identifizieren Sie Textwasserzeichen, selbst wenn zwischen Buchstaben unlesbare Zeichen stehen"

      # feature loop
      - icon: "fas fa-columns"
        content: "Suchen Sie Wasserzeichen basierend auf bestimmten Parametern oder durch Kombination mehrerer Kriterien"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Geben Sie die Schriftartformatierung an, um nach passendem Textwasserzeichen zu suchen"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Seiteneinrichtung und andere Informationen für unterstützte Formate programmgesteuert extrahieren"

      # feature loop
      - icon: "fas fa-print"
        content: "Fügen Sie Wasserzeichen zu Bildern in jeder Kopf- und Fußzeile in unterstützten Dokumentformaten hinzu"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Fügen Sie Wasserzeichen zu Bildformen in einem Word-Dokument hinzu und sperren Sie Wasserzeichen, um die Bearbeitung einzuschränken"

      # feature loop
      - icon: "fas fa-lock"
        content: "Schützen Sie Textwasserzeichen mit unlesbaren Zeichen in Präsentationen"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Rastern Sie eine bestimmte Seite oder ein ganzes PDF-Dokument, um hinzugefügte Wasserzeichen zu schützen"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Ändern Sie die Textformatierung, während Sie das vorhandene Textwasserzeichen ersetzen"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Richten Sie das Wasserzeichen im PDF-Dokument am Anschnitt-, Art-, Zuschneide- oder Beschnittrahmen aus"

      # feature loop
      - icon: "fas fa-heading"
        content: "Formeigenschaften in Microsoft Visio-Dokumenten bearbeiten"

    more_feature:
      # more_feature_loop
      - title: "Wasserzeichen hinzufügens"
        content: |
          GroupDocs.Watermark für .NET unterstützt mehrere Arten von Wasserzeichen. Das Hinzufügen von Wasserzeichen jeglicher Art ist nur eine Frage weniger Codezeilen. Das folgende Beispiel zeigt das Anwenden eines Bildwasserzeichens auf ein Word-Dokument mit C#:

          ```cs
          // Legen Sie das Dokument ein
          using (FileStream stream = File.Open("document.docx", FileMode.Open, FileAccess.ReadWrite))
          {
            using (Watermarker watermarker = new(Watermarker(stream))
            {
                // Verwenden Sie den Pfad zum Bild als Parameter des Konstruktors
                using (ImageWatermark watermark = new ImageWatermark("logo.png"))
                {
                  watermark.HorizontalAlignment = HorizontalAlignment.Center;
                  watermark.VerticalAlignment = VerticalAlignment.Center;
                  watermarker.Add(watermark);
                }
                // Speichern Sie das resultierende Dokument
                watermarker.Save("document_watermarked.docx");
                }
          }
          ```
      # more_feature_loop
      - title: "Wasserzeichen anwenden to Files of Different Formats in a Go"
        content: "Mit der GroupDocs.Watermark-API können Sie Wasserzeichen auf alle Dateien in einem bestimmten Ordner auf einmal anwenden oder Wasserzeichen löschen. Die Dateien können sogar unterschiedliche Formate haben und dennoch wird das Wasserzeichen auf alle genau angewendet."

      # more_feature_loop
      - title: "Kinderleichte Sicherheit für Wasserzeichen"
        content: "Mit nur einer Codezeile können Sie es jedem Tool sehr schwer machen, Ihr Wasserzeichen aus PDF-Dateien zu entfernen. Dies wird erreicht, indem alle Seiten eines PDF-Dokuments in Rasterbilder konvertiert werden, während die ursprüngliche Qualität erhalten bleibt."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Watermark bietet APIs zum Anzeigen von Dokumenten für andere beliebte Entwicklungsumgebungen"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Watermark for Java"
          image: "/border/groupdocs-watermark-java.svg"
          product: "GroupDocs.Watermark"
          platform: "Java"
          link: "/watermark/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---