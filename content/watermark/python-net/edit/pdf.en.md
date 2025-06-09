
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:29
draft: false
lang: en
format: Pdf
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Precise Watermark Editing in Pdf Using GroupDocs.Watermark"
head_description: "Use GroupDocs.Watermark for Python via .NET to modify watermark content in Pdf documents efficiently."

############################# Header ############################
title: "Edit Pdf Watermarks Smoothly with Python Tools" 
description: "Customize watermarks in PDFs and beyond with the GroupDocs.Watermark for Python via .NET development toolkit."
subtitle: "GroupDocs.Watermark for Python via .NET Tools" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Try it free from PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET Tools"
    link: "/watermark/python-net/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Update Watermarks in PDF Documents:** Leverage the GroupDocs.Watermark for Python via .NET framework to adjust watermarks while maintaining professional formatting.

############################# Steps ############################
steps:
    enable: true
    title: "Use the Python API to Modify Watermarks in Pdf Documents"
    content: |
      With **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)**, Python developers can easily modify watermark content in various Pdf documents. Here's a quick walkthrough:
      
      1. Begin by loading the Pdf document using the **Watermarker** class, accepting file paths, memory streams, or byte arrays as input.
      2. Construct a **SearchCriteria** object to search for existing watermark elements in your document, whether textual or graphical.
      3. Once identified, the tool provides a collection of matched watermark instances you can update—adjust parameters such as color, alignment, font, or even embedded image data.
      4. Finalize the process by saving your revised document to disk or any supported output stream using the built-in save methods.
   
    code:
      platform: "python-net"
      copy_title: "Copy"
      install:
        command: |
        command: "pip install groupdocs-watermark-net"
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/watermark/python-net/"
          
      content: |
        ```python {style=abap}
        # Update image watermark in PDF file
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Create Watermarker instance with input file
        with gw.Watermarker("input.pdf") as watermarker:

            # Use SearchCriteria to locate image-based watermarks
            search_criteria = gwss.ImageDctHashSearchCriteria("logo.png")

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # Apply changes to image watermark
                        watermark.ImageData = imageData
                    except Exception as e:
                        pass

            # Export updated PDF file
            watermarker.save("output.pdf")
        ```     

############################# More features ############################
more_features:
  enable: true
  title: "Boost Productivity with Advanced Watermarking Tools"
  description: "Accelerate document branding and protection in Python with our dynamic watermarking API. Insert, detect, modify, or delete watermark layers with minimal effort."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Advanced Watermark Editing Workflow"
  features:
    # feature loop
    - title: "Integrated Watermark Control"
      content: "Bring full watermark lifecycle control to your Python applications using GroupDocs.Watermark for Python via .NET. Avoid repetitive tasks by automating watermark setup, updates, and removal."

    # feature loop
    - title: "Precision Tuning of Watermark Attributes"
      content: "Take full control over watermark aesthetics—resize, recolor, rotate, or reposition them to meet any visual requirement with our flexible API surface."

    # feature loop
    - title: "Leverage Native Format Features"
      content: "Adapt to any file format by embedding watermarks into headers, footers, annotations, or backgrounds. Our API respects native structures for optimal integration."
      
  code_samples:
    # code sample loop
    - title: "Modifying Watermark in a PDF File"
      content: |
        Demonstrates how to change watermark properties in a PDF document.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # Open PDF file
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.pdf as gwop

        # Read watermark content
        load_options = gwop.PdfLoadOptions()
        with gw.Watermarker("source.pdf", load_options) as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,5,8]

            # Apply watermark update
            watermarks = watermarker.search(search_criteria)
            for watermark in watermarks:
                try:
                    watermark.formatted_text_fragments.clear()
                    watermark.formatted_text_fragments.add(
                        "New text", 
                        gww.Font("Calibri", 5.0, gww.FontStyle.bold), 
                        gww.Color.white, 
                        gww.Color.aqua
                    )
                except Exception as e:
                    pass
        
            # Save edited result
            watermarker.save("output.pdf")
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Watermark features for free or request a license"
  items:
    #  loop
    - title: "PyPi download"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Watermark Adjustment in Various Formats"
    exclude: "PDF"
    description: "Enjoy wide-format support for watermarking using GroupDocs.Watermark for Python via .NET’s reliable API."
    items: 
        # format loop 1
        - name: "Watermark PDF"
          format: "PDF"
          link: "/watermark/python-net/edit//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark Word"
          format: "WORD"
          link: "/watermark/python-net/edit//word/"
          description: "MS Word and Open Office documents"
          
        # format loop 3
        - name: "Watermark Excel"
          format: "EXCEL"
          link: "/watermark/python-net/edit//excel/"
          description: "MS Excel and Open Office spreadsheets"

        # format loop 4
        - name: "Watermark PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/edit//powerpoint/"
          description: "MS PowerPoint and Open Office presentations"

        # format loop 5
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/python-net/edit//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 6
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/python-net/edit//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 7
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/python-net/edit//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/python-net/edit//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 9
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/python-net/edit//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 10
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/python-net/edit//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 11
        - name: "Watermark RTF"
          format: "RTF"
          link: "/watermark/python-net/edit//rtf/"
          description: "Rich Text Format"

---