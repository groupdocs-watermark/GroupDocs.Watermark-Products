
---
############################# Static ############################
layout: "format"
date:  2024-04-03T18:16:19
draft: false
lang: en
format: Ppt
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Add PPT Document Watermark"
head_description: "GroupDocs.Watermark for Node.js via Java allows to generate Word Document watermarks in Node.js via Java, J2SE 7.0 (1.7) or above applications."

############################# Header ############################
title: "Add Watermark for Document of MS Word formats with Node.js via Java" 
description: "Text and image watermark generation for MS Excel files using Node.js via Java J2SE applications. Watermarks your business documents with BMP, PNG, GIF, and JPEG images or text. Adjust watermark size, alignment, rotation angle, and position on the document pages."
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download at NPM for free"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "Learn more"
    picture: "about_viewer.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java is designed for generation various Word watermarks using Node.js via Java. Our solution may enrich Node.js via Java apps by performing generation, adjusting, search, and clearing various watermarks in Word documents. GroupDocs.Watermark available for many operating systems and Node.js via Java J2SE 7.0 (1.7), J2SE 8.0 (1.8) or above.

############################# Steps ############################
steps:
    enable: true
    title: "MS Word Document Watermarking via Node.js via Java"
    content: |
      [GroupDocs.Watermark](https://products.groupdocs.com/watermark/nodejs-java/) helps Node.js via Java developers to generate watermarks in Node.js via Java applications with a few easy steps.
      
      1. Create **Watermarker** instance passing document path
      2. Provide path to watermark image at the constructor of the **ImageWatermark** class
      3. Adjust watermark properties
      4. Save watermarked document
   
    code:
      platform: "net"
      copy_title: "Copy"
      install:
        command: "npm i @groupdocs/groupdocs.watermark"
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/watermark/nodejs-java/"
          
      content: |
        ```javascript {style=abap}

        // Add image watermark to PPT

        // Instantiate Watermarker passing source file
        const watermarker = new groupdocs.watermark.Watermarker("input.ppt");
        
        // Construct watermark by providing image file
        const watermark = new groupdocs.watermark.ImageWatermark("watermark.png");

        // Get PPT result
        watermarker.add(watermark);
        watermarker.save("output.ppt");
        
        ```            

############################# Actions ############################

actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Watermark features for free or request a license"
  items:
    #  loop
    - title: "NPM download"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "MS Word documents watermarking via JavaScript"
    exclude: "PPT"
    description: "Protect MS Word business documents with image or text watermarks. Involve GroupDocs.Watermark for Node.js via Java API to your business processes."
    items: 
        # format loop 1
        - name: "Watermark PDFs"
          format: "PDF"
          link: "/watermark/nodejs-java/add//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/add//docx/"
          description: "Microsoft Word Open XML Document"

        # format loop 3
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/add//pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/add//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 5
        - name: "Watermark JPEG"
          format: "JPEG"
          link: "/watermark/nodejs-java/add//jpeg/"
          description: "JPEG Image"

        # format loop 6
        - name: "Watermark PNG"
          format: "PNG"
          link: "/watermark/nodejs-java/add//png/"
          description: "Portable Network Graphic"

        # format loop 7
        - name: "Watermark GIF"
          format: "GIF"
          link: "/watermark/nodejs-java/add//gif/"
          description: "Graphical Interchange Format File"

        # format loop 8
        - name: "Watermark BMP"
          format: "BMP"
          link: "/watermark/nodejs-java/add//bmp/"
          description: "Bitmap File Format"

        # format loop 9
        - name: "Watermark TIFF"
          format: "TIFF"
          link: "/watermark/nodejs-java/add//tiff/"
          description: "Tag Image File Format"

        # format loop 10
        - name: "Watermark WEBP"
          format: "WEBP"
          link: "/watermark/nodejs-java/add//webp/"
          description: "WEB Picture"

        # format loop 11
        - name: "Watermark JP2"
          format: "JP2"
          link: "/watermark/nodejs-java/add//jp2/"
          description: "JPEG2000 Core Image File"

        # format loop 12
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/add//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 13
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/add//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 14
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/add//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 15
        - name: "Watermark ODT"
          format: "ODT"
          link: "/watermark/nodejs-java/add//odt/"
          description: "Open Document Text"

        # format loop 16
        - name: "Watermark DOTM"
          format: "DOTM"
          link: "/watermark/nodejs-java/add//dotm/"
          description: "Word Open XML Macro-Enabled Document "

        # format loop 17
        - name: "Watermark XLTM"
          format: "XLTM"
          link: "/watermark/nodejs-java/add//xltm/"
          description: "OOXML Macro Enabled Workbook Template"

        # format loop 18
        - name: "Watermark PPTM"
          format: "PPTM"
          link: "/watermark/nodejs-java/add//pptm/"
          description: "OOXML Macro Enabled Presentation"

        # format loop 19
        - name: "Watermark VSDX"
          format: "VSDX"
          link: "/watermark/nodejs-java/add//vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop 20
        - name: "Watermark VSD"
          format: "VSD"
          link: "/watermark/nodejs-java/add//vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop 21
        - name: "Watermark VSTM"
          format: "VSTM"
          link: "/watermark/nodejs-java/add//vstm/"
          description: "Visio Macro-Enabled Drawing Template"



---