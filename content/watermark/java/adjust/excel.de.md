
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:05
draft: false
lang: de
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Excel Wasserzeichen-Tool anpassen — GroupDocs.Watermark"
head_description: "Passen Sie Wasserzeichen mühelos an, aktualisieren und verwalten Sie sie mit GroupDocs.Watermark. Passen Sie Ihre Dokumente mühelos an."

############################# Header ############################
title: "Tool zum Anpassen von SpreadSheets-Wasserzeichen: Leistungsstark und einfach" 
description: "Verbessern Sie Ihre Dokumente mit unserem intuitiven Tool zur Bearbeitung von Wasserzeichen. Vereinfachen Sie mühelos Ihren Arbeitsablauf."
subtitle: "GroupDocs.Watermark for Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlos Maven herunterladen"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java API"
    link: "/watermark/java/"
    link_title: "Erfahre mehr"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Tool zur Anpassung von Wasserzeichen**: Unser Wasserzeichen-Tool bietet eine benutzerfreundliche Lösung zur Verbesserung und zum Schutz Ihrer Dokumente. Mit den intuitiven Bearbeitungsfunktionen wird die Verwaltung von Wasserzeichen zum Kinderspiel und gewährleistet so die Sicherheit und Authentizität von Dokumenten.

############################# Steps ############################
steps:
    enable: true
    title: "Wasserzeichen in Excel-Dokumenten mit Java anpassen"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** macht es Java-Entwicklern einfach, Textwasserzeichen in ihren Anwendungen anzupassen, indem sie ein paar einfache Schritte implementieren:
      
      1. Laden Sie Ihre Excel-Datei in das Hauptobjekt unserer API namens **Watermarker**. Sie können die Datei zur weiteren Verarbeitung als Stream oder als Pfad auf einer lokalen Festplatte bereitstellen.
      2. Der nächste Schritt besteht darin, Wasserzeichen zu finden, die angepasst werden müssen. **SearchCriteria** hilft dabei, Wasserzeichen mit den richtigen Eigenschaften zu identifizieren, die zuvor einem Dokument hinzugefügt wurden.
      3. Erhalten Sie eine Liste geeigneter Wasserzeichen als Ergebnis der Prozedur **Search**. Passen Sie die Eigenschaften gefundener Wasserzeichen wie Größe, Seitenausrichtung, Text, Farbe, Bildinhalt usw. an. Es gibt viele Möglichkeiten, Ihre Daten anzupassen.
      4. Nach Abschluss des Wasserzeichen-Anpassungsprozesses müssen Sie das aktualisierte Dokument speichern. Verwenden Sie den lokalen Dateipfad, die Datei oder den Bytestream, um das Ergebnis zu speichern.
   
    code:
      platform: "net"
      copy_title: "Kopieren"
      install:
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-watermark</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "zum Kopieren anklicken"
        copy_done: "kopiert"
      links:
        #  loop
        - title: "Mehr Beispiele"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
        #  loop
        - title: "Dokumentation"
          link: "https://docs.groupdocs.com/watermark/java/"
          
      content: |
        ```java {style=abap}

        // Passen Sie das Textwasserzeichen EXCEL an

        // Instanziieren Sie Watermarker mit dem Eingabedokument EXCEL
        Watermarker watermarker = new Watermarker("input.xslx");

        // Initialisieren Sie TextSearchCriteria und suchen Sie nach Textwasserzeichen
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        
        // Passen Sie die Eigenschaften des Textwasserzeichens an
        for (PossibleWatermark watermark : watermarks)
        {
            watermark.getFormattedTextFragments().clear();
            watermark.getFormattedTextFragments().
                add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
        }

        // Speichern Sie das aktualisierte Dokument
        watermarker.save("output.xslx");
        
        ```            
        
############################# More features ############################
more_features:
  enable: true
  title: "Erfahre mehr über die Anpassung von EXCEL Wasserzeichen"
  description: "Unsere API ermöglicht es Java Anwendungen, Wasserzeichen in gängigen Dokumentformaten hinzuzufügen, zu bearbeiten, zu entfernen und nach ihnen zu suchen."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Wasserzeichen anpassen"
  features:
    # feature loop
    - title: "Versehen Sie Ihre Dokumente mühelos mit einem Wasserzeichen"
      content: "GroupDocs.Watermark vereinfacht das Wasserzeichen für Java Entwickler. Fügen Sie verschiedenen Geschäftsdokumenten und Dateien verschiedene Wasserzeichen hinzu. Sie können nicht nur Wasserzeichen anbringen, sondern auch vorhandene aktualisieren oder entfernen."

    # feature loop
    - title: "Passen Sie Wasserzeichen an Ihre Bedürfnisse an"
      content: "Unsere API bietet umfangreiche Anpassungsmöglichkeiten. Passen Sie Größe, Drehung, Farbe, Schriftart, Stile und mehr einfach an, um das perfekte Wasserzeichen zu erzielen."

    # feature loop
    - title: "EXCEL Native Document-Funktionen verwenden"
      content: "Abhängig vom jeweiligen Dokumentformat können Sie native Funktionen nutzen. Dazu können der Hintergrund der Dokumentseite, Anmerkungen, Kopfzeilen oder andere Objekte als Behälter für Wasserzeichen gehören."
      
  code_samples:
    # code sample loop
    - title: "PDF Textwasserzeichen anpassen"
      content: |
        Dieses Beispiel zeigt, wie der Text der jeweiligen Artefakte angepasst wird.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  PDF Dokument laden
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Dokumentinhalt abrufen
        PdfContent pdfContent = watermarker.getContent(PdfContent.class);

        //  Passen Sie bestimmten Wasserzeichentext an
        for (PdfArtifact artifact : pdfContent.getPages().get_Item(0).getArtifacts())
        {
            if (artifact.getText().contains("Test"))
            {
                artifact.setText("Passed");
            }
        }

        //  Speichern Sie das Dokument
        watermarker.save("result.pdf");
        watermarker.close();
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Bereit loszulegen?"
  description: "Testen Sie GroupDocs.Watermark Funktionen kostenlos oder fordern Sie eine Lizenz an"
  items:
    #  loop
    - title: "Maven herunterladen"
      link: "https://releases.groupdocs.com/watermark/java/"
      color: "red"
        #  loop
    - title: "Lizenzierung"
      link: "https://purchase.groupdocs.com/pricing/watermark/java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Passen Sie das Wasserzeichen über GroupDocs.Watermark for Java für andere Formate an"
    exclude: "EXCEL"
    description: "Passen Sie Wasserzeichen in einer Vielzahl von Dokumentformaten mühelos an. Verbessern Sie mühelos die Sicherheit und Authentizität von Dokumenten."
    items: 
        # format loop 1
        - name: "Wasserzeichen PDF"
          format: "PDF"
          link: "/watermark/java/adjust//pdf/"
          description: "Adobe Portable Dokumentformat"

        # format loop 2
        - name: "Wasserzeichen Word"
          format: "WORD"
          link: "/watermark/java/adjust//word/"
          description: "MS Word und Open Office-Dokumente"
          
        # format loop 3
        - name: "Wasserzeichen Excel"
          format: "EXCEL"
          link: "/watermark/java/adjust//excel/"
          description: "MS Excel und Open Office-Tabellen"

        # format loop 4
        - name: "Wasserzeichen PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/adjust//powerpoint/"
          description: "MS PowerPoint und Open Office-Präsentationen"

        # format loop 5
        - name: "Wasserzeichen DOCX"
          format: "DOCX"
          link: "/watermark/java/adjust//docx/"
          description: "Microsoft Word XML-Dokument öffnen"
          
        # format loop 6
        - name: "Wasserzeichen PPTX"
          format: "PPTX"
          link: "/watermark/java/adjust//pptx/"
          description: "PowerPoint XML-Präsentation öffnen"
          
        # format loop 7
        - name: "Wasserzeichen XLSX"
          format: "XLSX"
          link: "/watermark/java/adjust//xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"

        # format loop 8
        - name: "Wasserzeichen DOC"
          format: "DOC"
          link: "/watermark/java/adjust//doc/"
          description: "Microsoft Word 97 - 2007-Dokument"

        # format loop 9
        - name: "Wasserzeichen XLS"
          format: "XLS"
          link: "/watermark/java/adjust//xls/"
          description: "Microsoft Excel Arbeitsmappe 97-2003"

        # format loop 10
        - name: "Wasserzeichen PPT"
          format: "PPT"
          link: "/watermark/java/adjust//ppt/"
          description: "PowerPoint Präsentation 97-2003"

        # format loop 11
        - name: "Wasserzeichen RTF"
          format: "RTF"
          link: "/watermark/java/adjust//rtf/"
          description: "Rich-Text-Format"

---