
---
############################# Static ############################
layout: "format"
date:  2024-04-04T13:37:50
draft: false
lang: en
format: Word
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Remove Word Document Watermark"
head_description: "GroupDocs.Watermark for .NET allows to generate Word Document watermarks in .NET, J2SE 7.0 (1.7) or above applications."

############################# Header ############################
title: "Remove Watermark for Document of MS Word formats with .NET" 
description: "Text and image watermark generation for MS Excel files using .NET J2SE applications. Watermarks your business documents with BMP, PNG, GIF, and JPEG images or text. Adjust watermark size, alignment, rotation angle, and position on the document pages."
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download at Nuget for free"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "Learn more"
    picture: "about_viewer.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET is designed for generation various Word watermarks using .NET. Our solution may enrich .NET apps by performing generation, adjusting, search, and clearing various watermarks in Word documents. GroupDocs.Watermark available for many operating systems and .NET J2SE 7.0 (1.7), J2SE 8.0 (1.8) or above.

############################# Steps ############################
steps:
    enable: true
    title: "MS Word Document Watermarking via .NET"
    content: |
      [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/) helps .NET developers to generate watermarks in .NET applications with a few easy steps.
      
      1. Create **Watermarker** instance passing document path
      2. Provide path to watermark image at the constructor of the **ImageWatermark** class
      3. Adjust watermark properties
      4. Save watermarked document
   
    code:
      platform: "net"
      copy_title: "Copy"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // Remove text watermark from WORD document

        // Provide Watermarker instance for document WORD source document
        using (Watermarker watermarker = new Watermarker("input.docx"))
        {
            // Remove selected watermarks from the document
            TextFormattingSearchCriteria criteria = new TextFormattingSearchCriteria();
            criteria.ForegroundColorRange = new ColorRange();
            criteria.FontBold = true;
            PossibleWatermarkCollection watermarks = watermarker.Search(criteria);
            watermarks.Clear();

            // Save file to provided path
            watermarker.Save("output.docx");
        }
        
        ```            

############################# Actions ############################

actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Watermark features for free or request a license"
  items:
    #  loop
    - title: "Nuget download"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "MS Word documents watermarking via C#"
    exclude: "WORD"
    description: "Protect MS Word business documents with image or text watermarks. Involve GroupDocs.Watermark for .NET API to your business processes."
    items: 
        # format loop 1
        - name: "Watermark PDFs"
          format: "PDF"
          link: "/watermark/net/remove//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/net/remove//docx/"
          description: "Microsoft Word Open XML Document"

        # format loop 3
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/net/remove//pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/net/remove//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 5
        - name: "Watermark JPEG"
          format: "JPEG"
          link: "/watermark/net/remove//jpeg/"
          description: "JPEG Image"

        # format loop 6
        - name: "Watermark PNG"
          format: "PNG"
          link: "/watermark/net/remove//png/"
          description: "Portable Network Graphic"

        # format loop 7
        - name: "Watermark GIF"
          format: "GIF"
          link: "/watermark/net/remove//gif/"
          description: "Graphical Interchange Format File"

        # format loop 8
        - name: "Watermark BMP"
          format: "BMP"
          link: "/watermark/net/remove//bmp/"
          description: "Bitmap File Format"

        # format loop 9
        - name: "Watermark TIFF"
          format: "TIFF"
          link: "/watermark/net/remove//tiff/"
          description: "Tag Image File Format"

        # format loop 10
        - name: "Watermark WEBP"
          format: "WEBP"
          link: "/watermark/net/remove//webp/"
          description: "WEB Picture"

        # format loop 11
        - name: "Watermark JP2"
          format: "JP2"
          link: "/watermark/net/remove//jp2/"
          description: "JPEG2000 Core Image File"

        # format loop 12
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/net/remove//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 13
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/net/remove//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 14
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/net/remove//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 15
        - name: "Watermark ODT"
          format: "ODT"
          link: "/watermark/net/remove//odt/"
          description: "Open Document Text"

        # format loop 16
        - name: "Watermark DOTM"
          format: "DOTM"
          link: "/watermark/net/remove//dotm/"
          description: "Word Open XML Macro-Enabled Document "

        # format loop 17
        - name: "Watermark XLTM"
          format: "XLTM"
          link: "/watermark/net/remove//xltm/"
          description: "OOXML Macro Enabled Workbook Template"

        # format loop 18
        - name: "Watermark PPTM"
          format: "PPTM"
          link: "/watermark/net/remove//pptm/"
          description: "OOXML Macro Enabled Presentation"

        # format loop 19
        - name: "Watermark VSDX"
          format: "VSDX"
          link: "/watermark/net/remove//vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop 20
        - name: "Watermark VSD"
          format: "VSD"
          link: "/watermark/net/remove//vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop 21
        - name: "Watermark VSTM"
          format: "VSTM"
          link: "/watermark/net/remove//vstm/"
          description: "Visio Macro-Enabled Drawing Template"



---