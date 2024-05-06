---
############################# Static ############################
layout: "landing"
date: 2024-05-06T23:13:47
draft: false

lang: de
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

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

############################# Head ############################
head_title: "Java Wasserzeichen-Bibliothek | Wasserzeichen zu Dokumenten hinzufügen"
head_description: "Native Java Software zum Hinzufügen und Bearbeiten von Text- und Bildwasserzeichen in PDF, Word, Excel, Präsentationen, Visio Diagrammen, E-Mail- und Bilddateien."

############################# Header ############################
title: "Implementieren Sie einfach das Wasserzeichen von Dokumenten in Java Projekten"
description: "Erweitern Sie Ihre Java Anwendungen um die Möglichkeit, Dateien mithilfe der GroupDocs.Watermark -Bibliothek mit Wasserzeichen zu versehen. Unsere API bietet anpassbare Wasserzeichen für eine Vielzahl gängiger Dateiformate."
words:
  for: "zum"

actions:
  main: "Kostenloser Download von Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "Lizenzierung"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java/"
  title: "Bereit loszulegen?"
  description: "Testen Sie GroupDocs.Watermark Funktionen kostenlos oder fordern Sie eine Lizenz an"

release:
  title: "Version {0} veröffentlicht"
  notes: "Schau dir an, was es Neues gibt"
  downloads: "herunterladbare"

code:
  title: "Wasserzeichen PDF s über Java"
  more: "Mehr Beispiele"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-watermark</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Instanziieren Sie den Wassermarker, der den PDF -Pfad übergibt
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Passen Sie die Wasserzeichenoptionen an
    TextWatermark textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Wasserzeichen auf PDF Dokument anwenden
    watermarker.add(textWatermark);

    // Ergebnisdokument speichern
    watermarker.save("result.pdf");
    watermarker.close();
      
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark auf einen Blick"
  description: "Bibliothek zum Hinzufügen von Wasserzeichen mithilfe von Java Technologien"
  features:
    # feature loop
    - title: "Wasserzeichendateien über Java"
      content: "Schützen Sie Ihre Geschäftsdokumente mit GroupDocs.Watermark for Java. Fügen Sie Text, Bilder, Diagramme oder E-Mail-Anhänge als Wasserzeichen zu verschiedenen Dateiformaten hinzu."

    # feature loop
    - title: "Passen Sie Wasserzeichen an spezifische Bedürfnisse an"
      content: "GroupDocs.Watermark for Java bietet umfangreiche Anpassungsmöglichkeiten für Wasserzeichen. Passen Sie die Textstile (fett, kursiv, Schriftart) und die Bildeigenschaften (Drehung usw.) an, um den Wasserzeichenvorgang an Ihre spezifischen Ziele anzupassen."

    # feature loop
    - title: "Breite Formatunterstützung"
      content: "GroupDocs.Watermark for Java lässt sich nahtlos in eine Vielzahl von Dateiformaten integrieren, darunter: PDF, Microsoft Office (Word, Excel, PowerPoint), Bilder (JPEG, PNG, GIF, BMP), Visio Diagramme und E-Mails. Verbessern Sie die Dokumentensicherheit für verschiedene Dateitypen."

    # feature loop
    - title: "Mühelose Suche und Verwaltung von Wasserzeichen"
      content: "Verwalten Sie effizient vorhandene Wasserzeichen in Dokumenten. Suchen Sie nach bestimmten Wasserzeichen, ändern Sie deren Text, Stil oder Bilder oder entfernen Sie sie vollständig. GroupDocs.Watermark for Java vereinfacht den Wasserzeichen-Workflow."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformunabhängigkeit"
  description: "GroupDocs.Watermark for Java unterstützt verschiedene Betriebssysteme und Paketmanager."
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Unterstützte Dateiformate"
  description: |
    GroupDocs.Watermark for Java ermöglicht die Verarbeitung einer Vielzahl von Dateiformaten. [Vollständige Liste ansehen](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Java: Funktionen"
  description: "Schützen Sie Ihre Dateien, indem Sie Wasserzeichen hinzufügen. Unterstützt verschiedene Formate, darunter PDF, Office-Dokumente und Bilder."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Wasserzeichen für Dateien"
      content: "Fügen Sie für verschiedene unterstützte Dateiformate Wasserzeichen zu bestimmten Abschnitten oder ganzen Dokumenten hinzu oder entfernen Sie sie."

    # feature loop
    - icon: "watermark_style"
      title: "Anpassung des Wasserzeichens"
      content: "Passen Sie das Aussehen Ihres Wasserzeichens mit Optionen wie Farbe, Schriftart, Drehung und mehr an."

    # feature loop
    - icon: "hidden_print"
      title: "Verstecktes Druckwasserzeichen für PDF"
      content: "Fügen Sie ein Wasserzeichen hinzu, das nur beim Drucken eines PDF -Dokuments erscheint."

    # feature loop
    - icon: "image_only"
      title: "Selektives Bild-Wasserzeichen"
      content: "Markieren Sie alle Bilder in einem bestimmten Abschnitt, einer Seite, einer Folie oder einem gesamten Dokument mit einem Wasserzeichen."

    # feature loop
    - icon: "image_frame"
      title: "Bestimmte Bildrahmen mit Wasserzeichen versehen"
      content: "Wenden Sie Wasserzeichen auf bestimmte Rahmen in einem Bild mit mehreren Frames an."

    # feature loop
    - icon: "attachments"
      title: "Wasserzeichenanhänge und Formen"
      content: "Fügen Sie Wasserzeichen zu allen Anhängen in Excel Dokumenten oder allen Bildformen in Presentations hinzu."

    # feature loop
    - icon: "pdf_objects"
      title: "Wasserzeichenausrichtung in PDF"
      content: "Richten Sie Wasserzeichen an verschiedenen Bereichen eines PDF -Dokuments aus, einschließlich Bleed Box, Art Box, Crop Box und Trim Box."

    # feature loop
    - icon: "doc_background"
      title: "Wasserzeichen von Background Images"
      content: "Fügen Sie ein Hintergrundbildwasserzeichen zu Tabellen oder Präsentationen hinzu oder entfernen Sie es."

    # feature loop
    - icon: "unreadable_characters"
      title: "Schutz mit unlesbaren Zeichen"
      content: "Schützen Sie Präsentationen mit Textwasserzeichen mit unlesbaren Zeichen."

    # feature loop
    - icon: "watermark_text_search"
      title: "Suche nach Wasserzeichen"
      content: "Ruft eine Liste der Wasserzeichen ab, die in der Datei dargestellt werden, wobei verschiedene Parameter, einschließlich regulärer Ausdrücke, verwendet werden."

    # feature loop
    - icon: "watermark_image_search"
      title: "Finden Sie ähnliche Bild-Wasserzeichen"
      content: "Suchen Sie Bildwasserzeichen, die wie ein bestimmtes Bild aussehen."

    # feature loop
    - icon: "document_info"
      title: "Dokumentinformationen extrahieren"
      content: "Rufen Sie verschiedene Dokumentdaten ab, z. B. die Seiteneinrichtung für unterstützte Dateiformate."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Codebeispiele"
  description: "Erkunden Sie Codebeispiele, die typische GroupDocs.Watermark for Java Funktionen veranschaulichen"
  items:
    # code sample loop
    - title: "Ein Dokument mit einem Bild mit einem Wasserzeichen versehen"
      content: |
        Verwenden Sie GroupDocs.Watermark for Java, um die Dokumentensicherheit zu erhöhen, indem Sie Bildwasserzeichen hinzufügen. Weitere Informationen: [Bild-Wasserzeichen](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="So schützen Sie eine Datei mit einem Bildwasserzeichen.">}}
        ```csharp {style=abap}
        // Quelldokument in Watermarker laden
        Watermarker watermarker = new Watermarker("document.pdf");
        
        // Pfad zu einem Wasserzeichenbild angeben
        ImageWatermark watermark = new ImageWatermark("watermark.jpg");

        // Schützen Sie die Datei und speichern Sie sie
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Wasserzeichen ändern"
      content: |
        GroupDocs.Watermark for Java ermöglicht es Ihnen, vorhandene Wasserzeichen in Dokumenten zu verwalten. Suchen Sie nach bestimmten Wasserzeichen und [ändern Sie deren Eigenschaften](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Suche und Änderung von Wasserzeichen.">}}
        ```csharp {style=abap}   
        // Quelldokument laden
        Watermarker watermarker = new Watermarker("document.pdf");

        // Suchen Sie nach Wasserzeichen, die aktualisiert werden sollen
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);                               
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);                             

        // Gewünschte Eigenschaften aktualisieren
        for (PossibleWatermark watermark : watermarks)                                                           
        {  
            watermark.setText("New Text");
        }

        // Speichern Sie das geänderte Dokument in einem angegebenen Pfad
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
