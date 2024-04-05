
---
############################# Static ############################
layout: "format"
date:  2024-04-05T13:59:14
draft: false
lang: en
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Edit Watermark for Excel Spreadsheets"
head_description: "GroupDocs.Watermark for .NET generates watermark for MS Excel files in applications based on .NET, J2SE 7.0 (1.7) or above."

############################# Header ############################
title: "Edit Watermark for MS Excel Spreadsheets via .NET" 
description: "Text and image watermark generation for MS Excel files using .NET J2SE applications. Watermarks your business documents with BMP, PNG, GIF, and JPEG images or text. Adjust watermark size, alignment, rotation angle, and position on the document pages."
subtitle: "GroupDocs.Watermark for .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Free Nuget download"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET library"
    link: "/watermark/net/"
    link_title: "Learn more"
    picture: "about_viewer.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET is a comprehensive solution for managing watermarks using .NET. With this tool, developers can easily perform operations such as generation, adjust, search, and clear watermarks from documents in popular file formats. It supports working with both text and image watermarks in a variety of documents, including PDF, Microsoft Word, Excel, PowerPoint, Visio, email, and image formats. GroupDocs.Watermark supports all major operating systems and .NET versions including J2SE 7.0 (1.7), J2SE 8.0 (1.8) or above.

############################# Steps ############################
steps:
    enable: true
    title: "Edit Excel document text watermarks using .NET"
    content: |
      [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/) allows developers to edit text watermarks in .NET applications swiftly and easily
      
      1. Provide **Watermarker** object with Excel document
      2. Search for text watermarks in the document using **TextSearchCriteria**
      3. Edit particular watermark options like size, alignment, color
      4. Enjoy output result
   
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
        // Edit EXCEL text watermark

        // Make Watermarker providing EXCEL file
        using (Watermarker watermarker = new Watermarker("input.xslx"))
        {
            // Construct the TextSearchCriteria and get text watermarks
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                 // Edit text watermark
                 watermark.FormattedTextFragments.Clear();
                 watermark.FormattedTextFragments.Add("passed", 
                    new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
            }

            // Save the document
            watermarker.Save("output.xslx");
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
    title: "Use images as watermarks via C#"
    exclude: "EXCEL"
    description: "Our .NET solutions allows to protect various formats of business documents. Watermarked documents may enrich your business processes."
    items: 
        # format loop 1
        - name: "Watermark PDFs"
          format: "PDF"
          link: "/watermark/net/edit//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/net/edit//docx/"
          description: "Microsoft Word Open XML Document"

        # format loop 3
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/net/edit//pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/net/edit//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 5
        - name: "Watermark JPEG"
          format: "JPEG"
          link: "/watermark/net/edit//jpeg/"
          description: "JPEG Image"

        # format loop 6
        - name: "Watermark PNG"
          format: "PNG"
          link: "/watermark/net/edit//png/"
          description: "Portable Network Graphic"

        # format loop 7
        - name: "Watermark GIF"
          format: "GIF"
          link: "/watermark/net/edit//gif/"
          description: "Graphical Interchange Format File"

        # format loop 8
        - name: "Watermark BMP"
          format: "BMP"
          link: "/watermark/net/edit//bmp/"
          description: "Bitmap File Format"

        # format loop 9
        - name: "Watermark TIFF"
          format: "TIFF"
          link: "/watermark/net/edit//tiff/"
          description: "Tag Image File Format"

        # format loop 10
        - name: "Watermark WEBP"
          format: "WEBP"
          link: "/watermark/net/edit//webp/"
          description: "WEB Picture"

        # format loop 11
        - name: "Watermark JP2"
          format: "JP2"
          link: "/watermark/net/edit//jp2/"
          description: "JPEG2000 Core Image File"

        # format loop 12
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/net/edit//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 13
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/net/edit//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 14
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/net/edit//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 15
        - name: "Watermark ODT"
          format: "ODT"
          link: "/watermark/net/edit//odt/"
          description: "Open Document Text"

        # format loop 16
        - name: "Watermark DOTM"
          format: "DOTM"
          link: "/watermark/net/edit//dotm/"
          description: "Word Open XML Macro-Enabled Document "

        # format loop 17
        - name: "Watermark XLTM"
          format: "XLTM"
          link: "/watermark/net/edit//xltm/"
          description: "OOXML Macro Enabled Workbook Template"

        # format loop 18
        - name: "Watermark PPTM"
          format: "PPTM"
          link: "/watermark/net/edit//pptm/"
          description: "OOXML Macro Enabled Presentation"

        # format loop 19
        - name: "Watermark VSDX"
          format: "VSDX"
          link: "/watermark/net/edit//vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop 20
        - name: "Watermark VSD"
          format: "VSD"
          link: "/watermark/net/edit//vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop 21
        - name: "Watermark VSTM"
          format: "VSTM"
          link: "/watermark/net/edit//vstm/"
          description: "Visio Macro-Enabled Drawing Template"



---