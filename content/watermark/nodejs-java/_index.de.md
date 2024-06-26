---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:49
draft: false

lang: de
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js Wasserzeichen-Bibliothek | Dokumentwasserzeichen"
head_description: "Die Lösung Node.js schützt Geschäftsdokumente mit Text- und Bildwasserzeichen. Beliebte Formate wie PDF, Word, Excel, PowerPoint werden unterstützt."

############################# Header ############################
title: "Zugriff auf die Wasserzeichen-Technologie in Node.js über Java Lösungen"
description: "Schützen Sie Ihr geistiges Eigentum und verhindern Sie unbefugtes Kopieren mit dieser Node.js Lösung. Es ermöglicht Benutzern das einfache Hinzufügen von Wasserzeichen zu Geschäftsdokumenten in verschiedenen Formaten, darunter PDF, Word, Excel, PowerPoint, Bilder usw."
words:
  for: "zum"

actions:
  main: "Verwenden Sie NPM zum kostenlosen Herunterladen"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.watermark"
  alt: "Lizenzierung"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
  title: "Bereit loszulegen?"
  description: "Testen Sie GroupDocs.Watermark Funktionen kostenlos oder fordern Sie eine Lizenz an"

release:
  title: "Version {0} veröffentlicht"
  notes: "Schau dir an, was es Neues gibt"
  downloads: "herunterladbare"
  link: "https://releases.groupdocs.com/watermark/nodejs-java/"

code:
  title: "Fügen Sie mit TypeScript ein Wasserzeichen zu PDF hinzu"
  more: "Mehr Beispiele"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.watermark"
  content: |
    ```javascript {style=abap}

    // Instanziieren Sie den Wassermarker, der den PDF -Pfad übergibt
    let loadOptions = new PdfLoadOptions();
    let watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Passen Sie die Wasserzeichenoptionen an
    let textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Wasserzeichen auf PDF Dokument anwenden
    watermarker.add(textWatermark);

    // Ergebnisdokument speichern
    watermarker.save("result.pdf");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark auf einen Blick"
  description: "Node.js TypeScript-Bibliothek für Wasserzeichen"
  features:
    # feature loop
    - title: "Wasserzeichen in der Datei Node.js"
      content: "Schützen Sie Ihre Geschäftsdokumente mit GroupDocs.Watermark for Node.js via Java. Fügen Sie Text, Bilder, Diagramme oder E-Mail-Anhänge als Wasserzeichen zu verschiedenen Dateiformaten hinzu."

    # feature loop
    - title: "Passen Sie Wasserzeichen an Ihre Bedürfnisse an"
      content: "GroupDocs.Watermark for Node.js via Java bietet umfangreiche Anpassungsoptionen für Wasserzeichen. Durch die Feinabstimmung von Textstilen (fett, kursiv, Schriftart) und Bildeigenschaften (Drehung usw.) können Sie die Verarbeitung von Dokumenten individuell anpassen."

    # feature loop
    - title: "Umfassende Formatunterstützung"
      content: "GroupDocs.Watermark for Node.js via Java lässt sich nahtlos in eine Vielzahl von Dateiformaten integrieren, darunter: PDF, MS Office wie Word, Excel, PowerPoint, Bilder wie JPEG, PNG, GIF, BMP, Visio, Visio, E-Mails usw. Ermöglichen Sie die Dokumentenverarbeitung, um Geschäftsziele zu erreichen."

    # feature loop
    - title: "Leistungsstarke Suche und Aktualisierung von Wasserzeichen"
      content: "Abrufen und aktualisieren Sie vorhandene Wasserzeichen in Dokumenten mit Wasserzeichen. Ändern Sie Text, Stil, Bildinhalt oder entfernen Sie sie vollständig. GroupDocs.Watermark for Node.js via Java bietet eine breite Palette der Verarbeitung von Wasserzeichen."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformunabhängigkeit"
  description: "GroupDocs.Watermark for Node.js via Java lässt sich problemlos in verschiedene Betriebssysteme und Paketmanager integrieren."
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
    GroupDocs.Watermark for Node.js via Java ermöglicht es Ihnen, eine Vielzahl von Dateiformaten zu verarbeiten. [Erkunden Sie die vollständige Liste](https://docs.groupdocs.com/watermark/java/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Node.js via Java: Funktionsumfang"
  description: "Sorgen Sie für eine robuste Dokumentensicherheit durch programmatisches Wasserzeichen. Unterstützt verschiedene Dateiformate, darunter: PDF, DOCX, XLSX, PPTX und Bildformate (PNG, JPG usw.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Präzise Steuerung von Wasserzeichen"
      content: "Bearbeiten Sie Wasserzeichen präzise, indem Sie sie bestimmten Abschnitten, ganzen Dokumenten oder einzelnen Anhängen und Formen in verschiedenen Dateiformaten hinzufügen oder daraus entfernen."

    # feature loop
    - icon: "watermark_style"
      title: "Anpassung des Aussehens von Wasserzeichen"
      content: "Übernehmen Sie eine präzise Kontrolle über die Ästhetik von Wasserzeichen, indem Sie Attribute wie Farbe, Schriftart, Deckkraft, Drehung und Positionierung innerhalb des Dokuments ändern."

    # feature loop
    - icon: "hidden_print"
      title: "PDF Wasserzeichen drucken"
      content: "Setzen Sie ein unsichtbares Wasserzeichen ein, das beim normalen Anzeigen von Dokumenten unsichtbar bleibt, aber erst während des Druckvorgangs sichtbar wird, wodurch die Dokumentensicherheit unauffällig erhöht wird."

    # feature loop
    - icon: "image_only"
      title: "Spezifisches Bild-Wasserzeichen"
      content: "Verwenden Sie unsere Lösung, um bestimmte Bilder in einem Dokument mit einem Wasserzeichen zu versehen. Wählen Sie, ob Sie Wasserzeichen in einen bestimmten Abschnitt (z. B. Seite, Folie) oder in das gesamte Dokument einbetten möchten."

    # feature loop
    - icon: "image_frame"
      title: "Wasserzeichen für Bilder mit mehreren Frames"
      content: "Wenden Sie Wasserzeichen selektiv auf bestimmte Frames in einem Bildformat mit mehreren Frames an und sorgen Sie so für eine detaillierte Kontrolle über die Platzierung von Wasserzeichen."

    # feature loop
    - icon: "attachments"
      title: "Umfassender Inhaltsschutz"
      content: "Erweitern Sie den Schutz auf verschiedene Dokumentelemente wie Anlagen in Excel Dokumenten und Bildformen in Präsentationen und bieten Sie so eine zusätzliche Sicherheitsebene."

    # feature loop
    - icon: "pdf_objects"
      title: "Erweitertes Wasserzeichen in PDF"
      content: "Markieren Sie verschiedene Bereiche von PDF s mit Wasserzeichen, einschließlich Bleed Box, Art Box, Crop Box, Trim Box usw."

    # feature loop
    - icon: "doc_background"
      title: "Wasserzeichen für das Hintergrundbild"
      content: "Verwalte Wasserzeichen in den Hintergrundbildern von Tabellen und Präsentationen und biete zusätzliche Anpassungsoptionen für visuelle Sicherheitsmaßnahmen."

    # feature loop
    - icon: "unreadable_characters"
      title: "Textwasserzeichen mit unlesbaren Zeichen"
      content: "Verwenden Sie unlesbare Zeichen in Textwasserzeichen, die in Präsentationen eingebettet sind, und erhöhen Sie so die Sicherheit, indem Sie die unbefugte Extraktion von Wasserzeichen erheblich erschweren."

    # feature loop
    - icon: "watermark_text_search"
      title: "Erweiterte Wasserzeichensuche"
      content: "Nutzen Sie umfassende Suchfunktionen, um Wasserzeichen in Dokumenten anhand bestimmter Parameter oder durch Kombination verschiedener Kriterien zu finden und so ein effizientes Abrufen und Verwalten zu ermöglichen."

    # feature loop
    - icon: "watermark_image_search"
      title: "Wasserzeichenerkennung mit ähnlichem Bild"
      content: "Finden Sie ähnliche Wasserzeichenbilder in Dokumenten, die optisch einem Quellbild ähneln."

    # feature loop
    - icon: "document_info"
      title: "Programmatische Extraktion von Dokumentinformationen"
      content: "Extrahieren Sie programmgesteuert wertvolle Metadaten, einschließlich Details zur Seiteneinrichtung und anderer Dokumentinformationen für unterstützte Dateiformate."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Codebeispiele"
  description: "Tauchen Sie ein in Codebeispiele, die allgemeine GroupDocs.Watermark for Node.js via Java Funktionen zeigen"
  items:
    # code sample loop
    - title: "Ein Dokument mit einem Bild mit einem Wasserzeichen versehen"
      content: |
        Nutzen Sie GroupDocs.Watermark for Node.js via Java, um die Dokumentensicherheit zu erhöhen, indem Sie Bildwasserzeichen hinzufügen. Weitere Informationen: [Bild-Wasserzeichen](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="So schützen Sie eine Datei mit einem Bildwasserzeichen.">}}
        ```javascript {style=abap}
        // Quelldokument in Watermarker laden
        let watermarker = new Watermarker("document.pdf");
        
        // Pfad zu einem Wasserzeichenbild angeben
        let watermark = new ImageWatermark("watermark.jpg");

        // Schützen Sie die Datei und speichern Sie sie
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Suchen und ändern Sie vorhandene Wasserzeichen"
      content: |
        GroupDocs.Watermark for Node.js via Java ermöglicht es Ihnen, Dokumentwasserzeichen zu verwalten. Wählen Sie Wasserzeichen aus und ändern Sie ihre Eigenschaften. Erfahre wie: [Wasserzeichen ändern](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Suche und Änderung von Wasserzeichen.">}}
        ```javascript {style=abap}   
        // Quelldokument laden
        let watermarker = new Watermarker("document.pdf");

        // Suchen Sie nach Wasserzeichen, die aktualisiert werden sollen
        let searchCriteria = new TextSearchCriteria("test", false);                               
        let watermarks = watermarker.search(searchCriteria); 

        // Gewünschte Eigenschaften aktualisieren
        watermarks.forEach((watermark)
        {  
            watermark.setText("New Text");
        }

        // Speichern Sie das geänderte Dokument in einem angegebenen Pfad
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
