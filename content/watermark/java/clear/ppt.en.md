
---
############################# Static ############################
layout: "format"
date:  2024-04-18T15:29:27
draft: false
lang: en
format: Ppt
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Clear PPT Document Watermark"
head_description: "GroupDocs.Watermark for Java allows to generate Word Document watermarks in Java, J2SE 7.0 (1.7) or above applications."

############################# Header ############################
title: "Clear Watermark for Document of MS Word formats with Java" 
description: "Text and image watermark generation for MS Excel files using Java J2SE applications. Watermarks your business documents with BMP, PNG, GIF, and JPEG images or text. Adjust watermark size, alignment, rotation angle, and position on the document pages."
subtitle: "GroupDocs.Watermark for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download at Maven for free"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java"
    link: "/watermark/java/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java is designed for generation various Word watermarks using Java. Our solution may enrich Java apps by performing generation, adjusting, search, and clearing various watermarks in Word documents. GroupDocs.Watermark available for many operating systems and Java J2SE 7.0 (1.7), J2SE 8.0 (1.8) or above.

############################# Steps ############################
steps:
    enable: true
    title: "Clear Watermarks from Ppt Documents using Java"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/)** simplifies the process of clearing watermarks from your business documents within Java applications. Integrate our library and follow these steps:
      
      1. Begin by initializing the **Watermarker** class with your Ppt document. The API accepts the document either as a stream or a local file path for processing.
      2. Leverage the **SearchCriteria** object to refine the set of watermarks for clearing. You can utilize an image as a search parameter alongside text or formatting attributes. The more specific your search criteria, the more precise the results will be.
      3. Following the search, you'll receive a list of identified watermarks. Proceed by clearing these watermarks from the document.
      4. Once the watermarks are cleared, save the final document using a local file path or a stream object.
   
    code:
      platform: "net"
      copy_title: "Copy"
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
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/watermark/java/"
          
      content: |
        ```java {style=abap}
        // Clear image watermark PPT document

        // Pass PPT document path to Watermarker constructor
        Watermarker watermarker = new Watermarker("input.ppt");
        
        // Clear the document by deleting a watermark
        PossibleWatermarkCollection possibleWatermarks = watermarker.search();
        possibleWatermarks.removeAt(0);

        // Save cleared file
        watermarker.save("output.ppt");
        
        ```        
        
############################# More features ############################
more_features:
  enable: true
  title: "Deep dive into adding Watermark"
  description: "API to render, display, convert documents, slides, diagrams, and many other document types in .NET applications"
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "Add Watermark"
  features:
    # feature loop
    - title: "Watermark your documents easily."
      content: "GroupDocs.Watermark makes it easy for Java developers to add various types of watermarks in popular business documents and files."

    # feature loop
    - title: "Customize watermarks for your goals."
      content: "Our solution supports many watermark features. You can easily adjust size, rotation, color, font, font styles and other options to make watermark looks perfect."

    # feature loop
    - title: "Use native document objects"
      content: "Accordingly do particular document format it is possible to use native document features. Native PDF annotations or MS Word page watermark may be used for watermarking."
      
  code_samples:
    # code sample loop
    - title: "Clear DOCX of shape watermark"
      content: |
        This example shows how to clear Word document of a particular shape.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Load Word document
        WordProcessingLoadOptions loadOptions = new WordProcessingLoadOptions();
        Watermarker watermarker = new Watermarker("source.docx", loadOptions);

        WordProcessingContent content = watermarker.getContent(WordProcessingContent.class);

        //  Remove shape by index
        content.getSections().get_Item(0).getShapes().removeAt(0);

        //  Remove shape by reference
        content.getSections().get_Item(0).getShapes().
            remove(content.getSections().get_Item(0).getShapes().get_Item(0));

        //  Save the DOCX
        watermarker.save("result.docx");
        watermarker.close();
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Watermark features for free or request a license"
  items:
    #  loop
    - title: "Maven download"
      link: "https://releases.groupdocs.com/watermark/java/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/watermark/java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "MS Word documents watermarking via Java"
    exclude: "PPT"
    description: "Protect MS Word business documents with image or text watermarks. Involve GroupDocs.Watermark for Java API to your business processes."
    items: 
        # format loop 1
        - name: "Watermark PDF"
          format: "PDF"
          link: "/watermark/java/clear//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark Word"
          format: "WORD"
          link: "/watermark/java/clear//word/"
          description: "MS Word and Open Office documents"
          
        # format loop 3
        - name: "Watermark Excel"
          format: "EXCEL"
          link: "/watermark/java/clear//excel/"
          description: "MS Excel and Open Office spreadsheets"

        # format loop 4
        - name: "Watermark PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/clear//powerpoint/"
          description: "MS PowerPoint and Open Office presentations"

        # format loop 5
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/java/clear//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 6
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/java/clear//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 7
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/java/clear//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/java/clear//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 9
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/java/clear//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 10
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/java/clear//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 11
        - name: "Watermark RTF"
          format: "RTF"
          link: "/watermark/java/clear//rtf/"
          description: "Rich Text Format"

---