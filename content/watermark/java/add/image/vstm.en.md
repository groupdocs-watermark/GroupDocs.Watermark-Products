
---
############################# Static ############################
layout: "format"
date:  2024-03-07T13:11:48
draft: false
lang: en
format: Vstm
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java GroupDocs.Watermark - Watermark Files VSTM with images"
head_description: "Java library to add image watermark to VSTM file in Java, J2SE 7.0 (1.7) or above applications using GroupDocs.Watermark for Java."

############################# Header ############################
title: "Add Image Watermark to VSTM in Java" 
description: "Adding image watermark to VSTM files for Java J2SE applications. Add BMP, PNG, GIF, and JPEG images as watermarks to your documents. You can also manage the watermark's size, alignment, rotation angle, and position on the document pages as per your requirements."
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
       GroupDocs.Watermark for Java is a comprehensive solution for managing watermarks using Java. With this tool, developers can easily perform operations such as adding, editing, searching, and deleting different types of watermarks from documents in popular file formats. It supports working with both text and image watermarks in a variety of documents, including PDF, Microsoft Word, Excel, PowerPoint, Visio, email, and image formats. GroupDocs.Watermark supports all major operating systems and Java versions including J2SE 7.0 (1.7), J2SE 8.0 (1.8) or above.

############################# Steps ############################
steps:
    enable: true
    title: "How to add image watermark in VSTM documents using Java"
    content: |
      [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/) makes it easy for Java developers to add image (BMP, PNG, GIF or JPEG) watermarks in their applications by implementing a few easy steps.
      
      1. Instantiate **Watermarker** with input VSTM document
      2. Use the image watermark path as the constructor parameter of the **ImageWatermark** class
      3. Set watermark properties (size, alignment, color etc)
      4. Get output document
   
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

        // Add image watermark in your document

        // Create a Watermarker object specifying a source file
        try (Comparer comparer = new Comparer("source.vstm") 
        {
            // Set up watermark options
        	comparer.add("target1.vstm");
            comparer.add("target2.vstm");

            // Get result file protected by watermark
            final Path resultPath = comparer.compare("result.vstm"); 

            System.out.println("\nDocuments compared successfully.");
        }
        
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
    exclude: "VSTM"
    description: "Our Java solutions allows to protect various formats of business documents. Watermarked documents may enrich your business processes."
    items: 
        # format loop 1
        - name: "Watermark PDFs"
          format: "PDF"
          link: "/watermark/java/add/image/pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/java/add/image/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop 3
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/java/add/image/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/java/add/image/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 5
        - name: "Watermark JPEG"
          format: "JPEG"
          link: "/watermark/java/add/image/jpeg/"
          description: "JPEG Image"

        # format loop 6
        - name: "Watermark PNG"
          format: "PNG"
          link: "/watermark/java/add/image/png/"
          description: "Portable Network Graphic"

        # format loop 7
        - name: "Watermark GIF"
          format: "GIF"
          link: "/watermark/java/add/image/gif/"
          description: "Graphical Interchange Format File"

        # format loop 8
        - name: "Watermark BMP"
          format: "BMP"
          link: "/watermark/java/add/image/bmp/"
          description: "Bitmap File Format"

        # format loop 9
        - name: "Watermark TIFF"
          format: "TIFF"
          link: "/watermark/java/add/image/tiff/"
          description: "Tag Image File Format"

        # format loop 10
        - name: "Watermark WEBP"
          format: "WEBP"
          link: "/watermark/java/add/image/webp/"
          description: "WEB Picture"

        # format loop 11
        - name: "Watermark JP2"
          format: "JP2"
          link: "/watermark/java/add/image/jp2/"
          description: "JPEG2000 Core Image File"

        # format loop 12
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/java/add/image/doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 13
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/java/add/image/xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 14
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/java/add/image/ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 15
        - name: "Watermark ODT"
          format: "ODT"
          link: "/watermark/java/add/image/odt/"
          description: "Open Document Text"

        # format loop 16
        - name: "Watermark DOTM"
          format: "DOTM"
          link: "/watermark/java/add/image/dotm/"
          description: "Word Open XML Macro-Enabled Document "

        # format loop 17
        - name: "Watermark XLTM"
          format: "XLTM"
          link: "/watermark/java/add/image/xltm/"
          description: "OOXML Macro Enabled Workbook Template"

        # format loop 18
        - name: "Watermark PPTM"
          format: "PPTM"
          link: "/watermark/java/add/image/pptm/"
          description: "OOXML Macro Enabled Presentation"

        # format loop 19
        - name: "Watermark VSDX"
          format: "VSDX"
          link: "/watermark/java/add/image/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop 20
        - name: "Watermark VSD"
          format: "VSD"
          link: "/watermark/java/add/image/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop 21
        - name: "Watermark VSTM"
          format: "VSTM"
          link: "/watermark/java/add/image/vstm/"
          description: "Visio Macro-Enabled Drawing Template"



---