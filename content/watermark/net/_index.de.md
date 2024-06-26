---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:48
draft: false

lang: de
product: "Watermark"
product_tag: "watermark"
platform: "Net"
platform_tag: "net"

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
head_title: "C# .NET Dokumentwasserzeichen-Software | Wasserzeichen hinzufügen"
head_description: "C# .NET Bibliothek zum Hinzufügen, Suchen und Entfernen von Wasserzeichen in Dokumenten: PDF, Word, Excel, Präsentationen, Visio Diagramme, E-Mail- und Bilddateiformate."

############################# Header ############################
title: "Dokumente einfach in Ihren C# .NET -Anwendungen mit Wasserzeichen versehen"
description: "Stärken Sie Ihre C#-Lösungen mit einer flexiblen API für Dokumentwasserzeichen, mit der Sie anpassbare Wasserzeichen zu allen gängigen Dokumentformaten hinzufügen können."
words:
  for: "zum"

actions:
  main: "Kostenlos NuGet Download"
  main_link: "https://www.nuget.org/packages/GroupDocs.Watermark"
  alt: "Lizenzierung"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/net/"
  title: "Bereit loszulegen?"
  description: "Testen Sie GroupDocs.Watermark Funktionen kostenlos oder fordern Sie eine Lizenz an"

release:
  title: "Version {0} veröffentlicht"
  notes: "Schau dir an, was es Neues gibt"
  downloads: "herunterladbare"

code:
  title: "Wasserzeichen PDF -Dateien in C#"
  more: "Mehr Beispiele"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
  install: "dotnet add package GroupDocs.Watermark"
  content: |
    ```csharp {style=abap}   
    // Instanziieren Sie den Wassermarker, der den PDF -Pfad übergibt
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    using (Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions))
    {
        // Passen Sie die Wasserzeichenoptionen an
        TextWatermark textWatermark = 
            new TextWatermark("Approved", new Font("Arial", 8));
        
        // Wasserzeichen auf PDF Dokument anwenden
        watermarker.Add(textWatermark);

        // Ergebnisdokument speichern
        watermarker.Save("result.pdf");
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark auf einen Blick"
  description: "API zum Einfügen von Wasserzeichen auf Dokumenten über .NET"
  features:
    # feature loop
    - title: "Wasserzeichen für C#-Dateien"
      content: "Fügen Sie Ihren Geschäftsdateien mit GroupDocs.Watermark Wasserzeichen hinzu. Verwenden Sie Text, Bilder, Diagramme oder E-Mail-Anhänge."

    # feature loop
    - title: "Passen Sie Wasserzeichen an Ihre Ziele an"
      content: "Die GroupDocs.Watermark for .NET -Software ermöglicht es, Wasserzeichen auf verschiedene Arten anzupassen. Textstile wie Fett, Kursiv, Schriftarten sowie Bildeigenschaften wie Drehung usw. bereichern den Wasserzeichenprozess."

    # feature loop
    - title: "Alle gängigen Dateiformate werden unterstützt"
      content: "Viele Datei- und Dokumentformate werden von der GroupDocs.Watermark -Lösung unterstützt. PDF, Microsoft Office Word, Excel, PowerPoint, Bilder wie JPEG, PNG, GIF, BMP, Visio, E-Mails usw. könnten mit unseren Wasserzeichen geschützt werden."

    # feature loop
    - title: "Suchen und aktualisieren Sie Wasserzeichen"
      content: "Wasserzeichen, die bereits in einem Dokument enthalten sind, können gefunden und erneut verarbeitet werden. Ändern Sie Text, Stil, Bilder oder entfernen Sie aufgedeckte Wasserzeichen ohne zusätzlichen Aufwand."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformunabhängigkeit"
  description: "GroupDocs.Watermark for .NET unterstützt die unten aufgeführten Betriebssysteme, Frameworks und Paketmanager"
  items:
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
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Unterstützte Dateiformate"
  description: |
    GroupDocs.Watermark for .NET ermöglicht die Verarbeitung der folgenden [Dateiformate](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark Funktionen"
  description: "Schützen Sie PDF, Office, Bilder und andere Formate durch Wasserzeichen"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Wasserzeichen für Dokumente"
      content: "Hinzufügen oder Entfernen von Wasserzeichen aus einem bestimmten Abschnitt oder einem ganzen Dokument in verschiedenen Dateiformaten."

    # feature loop
    - icon: "watermark_style"
      title: "Gestalten Sie Ihr Wasserzeichen"
      content: "Passen Sie verschiedene Wasserzeicheneigenschaften wie Farbe, Schriftart, Drehung usw. an."

    # feature loop
    - icon: "hidden_print"
      title: "PDF verstecktes Druckwasserzeichen"
      content: "Ordnen Sie PDF ein verstecktes Wasserzeichen zu, das nur beim Drucken des Dokuments erscheint."

    # feature loop
    - icon: "image_only"
      title: "Nur Bilder in Dokumenten mit Wasserzeichen versehen"
      content: "Markieren Sie alle Bilder in einem bestimmten Abschnitt, einer Seite, einer Folie oder einem Dokument mit einem Wasserzeichen."

    # feature loop
    - icon: "image_frame"
      title: "Ausgewählte Bildrahmen verarbeiten"
      content: "Weisen Sie ein Wasserzeichen nur bestimmten Frames eines Bilds mit mehreren Frames zu."

    # feature loop
    - icon: "attachments"
      title: "Anlagen und Formen"
      content: "Setzen Sie ein Wasserzeichen für alle Anlagen in einem Excel Dokument und alle Bildformen in Folien."

    # feature loop
    - icon: "pdf_objects"
      title: "PDF Objekte"
      content: "Richten Sie das Wasserzeichen im PDF Dokument am Anschnittrahmen, Grafikfeld, Zuschneidefeld oder Zuschneidefeld aus."

    # feature loop
    - icon: "doc_background"
      title: "Hintergrund der Dokumente"
      content: "Platzieren Sie ein Wasserzeichen oder entfernen Sie es aus den Hintergrundbildern der Tabelle oder der Folien."

    # feature loop
    - icon: "unreadable_characters"
      title: "Schutz vor unlesbaren Zeichen"
      content: "Schützen Sie Textwasserzeichen mit unlesbaren Zeichen in Präsentationen."

    # feature loop
    - icon: "watermark_text_search"
      title: "Suche nach Wasserzeichen in Dokumenten"
      content: "Suchen Sie nach Wasserzeichen anhand bestimmter Parameter oder durch Kombination mehrerer Kriterien."

    # feature loop
    - icon: "watermark_image_search"
      title: "Suche nach ähnlichen Bild-Wasserzeichen"
      content: "Suchen Sie nach Bildwasserzeichen, die einem bestimmten Bild ähneln."

    # feature loop
    - icon: "document_info"
      title: "Dokumentinformationen abrufen"
      content: "Extrahieren Sie programmgesteuert die Seiteneinrichtung und andere Informationen für unterstützte Formate."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Codebeispiele"
  description: "Einige Anwendungsfälle typischer GroupDocs.Watermark for .NET Operationen"
  items:
    # code sample loop
    - title: "Wasserzeichen, indem Sie ein Bild zu einem Dokument hinzufügen."
      content: |
        Um jedes Dokument zu schützen, können Sie [Bildwasserzeichen](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/) verwenden:
        {{< landing/code title="So schützen Sie eine Datei mit einem Bildwasserzeichen.">}}
        ```csharp {style=abap}
        // Quelldokument in Watermarker laden
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Pfad zu einem Wasserzeichenbild angeben
            using (ImageWatermark watermark = new ImageWatermark("watermark.jpg"))
            {
                // Schützen Sie die Datei und speichern Sie sie
                watermarker.Add(watermark);

                watermarker.Save("result.pdf");
            }
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Suchen und ändern Sie vorhandene Wasserzeichen."
      content: |
        GroupDocs.Watermark kann [Wasserzeichen ändern](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/), die bereits in einem Dokument enthalten sind. Suchen Sie nach den gewünschten Elementen und aktualisieren Sie deren Eigenschaften.
        {{< landing/code title="Suche und Änderung von Wasserzeichen.">}}
        ```csharp {style=abap}   
        // Quelldokument laden
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Suchen Sie nach Wasserzeichen, die aktualisiert werden sollen
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                // Gewünschte Eigenschaften aktualisieren
                watermark.Text = "New Text";
            }

            // Speichern Sie das geänderte Dokument in einem angegebenen Pfad
            watermarker.Save("document.pdf");
        }
        ```
        {{< /landing/code >}}

---
