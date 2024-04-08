
---
############################# Static ############################
layout: "format"
date:  2024-04-08T14:33:43
draft: false
lang: en
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Search Watermark for Excel Spreadsheets"
head_description: "GroupDocs.Watermark for Java generates watermark for MS Excel files in applications based on Java, J2SE 7.0 (1.7) or above."

############################# Header ############################
title: "Search Watermark for MS Excel Spreadsheets via Java" 
description: "Text and image watermark generation for MS Excel files using Java J2SE applications. Watermarks your business documents with BMP, PNG, GIF, and JPEG images or text. Adjust watermark size, alignment, rotation angle, and position on the document pages."
subtitle: "GroupDocs.Watermark for Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Free Maven download"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java library"
    link: "/watermark/java/"
    link_title: "Learn more"
    picture: "about_viewer.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java is a comprehensive solution for managing watermarks using Java. With this tool, developers can easily perform operations such as generation, adjust, search, and clear watermarks from documents in popular file formats. It supports working with both text and image watermarks in a variety of documents, including PDF, Microsoft Word, Excel, PowerPoint, Visio, email, and image formats. GroupDocs.Watermark supports all major operating systems and Java versions including J2SE 7.0 (1.7), J2SE 8.0 (1.8) or above.

############################# Steps ############################
steps:
    enable: true
    title: "Search for text watermarks in Excel files using Java"
    content: |
      [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/) makes it easy to search for text watermarks in business documents with Java applications.
      
      1. Instantiate **Watermarker** by Excel document path
      2. Create and set up options of **TextSearchCriteria**
      3. Search for watermarks in the document
      4. Use list of found text watermarks
   
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

        // Search text watermarks in EXCEL document

        // Get Watermarker instance for EXCEL document
        Watermarker watermarker = new Watermarker("input.xslx");

        // Search watermarks by criteria
        ImageSearchCriteria imageSearchCriteria = new ImageDctHashSearchCriteria("watermark.jpeg");
        imageSearchCriteria.setMaxDifference(0.9);
        PossibleWatermarkCollection possibleWatermarks = watermarker.search(imageSearchCriteria);

        // Process watermarks
        System.out.println("Found " + possibleWatermarks.getCount() + " possible watermark(s).");
        
        ```            

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
    title: "Use images as watermarks via Java"
    exclude: "EXCEL"
    description: "Our Java solutions allows to protect various formats of business documents. Watermarked documents may enrich your business processes."
    items: 
        # format loop 1
        - name: "Watermark PDF"
          format: "PDF"
          link: "/watermark/java/search//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark Word"
          format: "WORD"
          link: "/watermark/java/search//word/"
          description: "MS Word and Open Office documents"
          
        # format loop 3
        - name: "Watermark Excel"
          format: "EXCEL"
          link: "/watermark/java/search//excel/"
          description: "MS Excel and Open Office spreadsheets"

        # format loop 4
        - name: "Watermark PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/search//powerpoint/"
          description: "MS PowerPoint and Open Office presentations"

        # format loop 5
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/java/search//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 6
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/java/search//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 7
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/java/search//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/java/search//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 9
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/java/search//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 10
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/java/search//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 11
        - name: "Watermark RTF"
          format: "RTF"
          link: "/watermark/java/search//rtf/"
          description: "Rich Text Format"

---