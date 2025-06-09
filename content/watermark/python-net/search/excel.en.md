
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:16
draft: false
lang: en
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Detect Unseen Watermarks in Excel Spreadsheets"
head_description: "Reveal hidden marks in spreadsheet files with GroupDocs.Watermark quickly and accurately."

############################# Header ############################
title: "Instantly Identify Watermarks in Excel Spreadsheets" 
description: "Locate and manage watermarks seamlessly using GroupDocs.Watermark for Python via .NET."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download PyPi Now – It's Free"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Overview of GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET delivers a full-featured watermark toolkit for Python developers. Generate, modify, find, and remove watermark content from documents like Excel, Word, PDF, and more with minimal effort.

############################# Steps ############################
steps:
    enable: true
    title: "How to Detect Watermarks in Excel Files via Python"
    content: |
      With **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/python-net/)**, identifying embedded watermarks in your business documents is simplified. Bring its capabilities into your Python workflows for seamless detection.
      
      1. Begin by loading the Excel document into an instance of the **Watermarker** class. Accepts input as a path, stream, or byte array.
      2. Narrow your search using the **SearchCriteria** object. To find image-based marks, use a sample image. For textual ones, specify characteristics such as content, style, or color.
      3. Invoke the **Search** method from the **Watermarker** object to extract watermark data. A collection of watermark instances will be returned for inspection.
      4. After retrieval, you can manage the results: remove undesired marks, or update details such as dimensions or message content.
   
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
        # Detect text watermark in EXCEL format
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Initialize Watermarker with EXCEL file
        with gw.Watermarker("input.xslx") as watermarker:

            # Execute watermark search
            search_criteria = gwss.TextSearchCriteria("test", False)
            possible_watermarks = watermarker.search(search_criteria)

            # Process the list of detected watermarks
            print("\nFound {0} possible watermark(s).".format(len(possible_watermarks)))
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Powerful Watermark Detection with GroupDocs.Watermark"
  description: "Use GroupDocs.Watermark in your Python projects to efficiently scan and locate watermark elements in diverse document types."
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "Detecting Watermarks"
  features:
    # feature loop
    - title: "Advanced Detection with Smart Filters"
      content: "Easily identify watermarks in a wide array of document formats. GroupDocs.Watermark supports filtering by visual and textual traits including shape, transparency, and more."

    # feature loop
    - title: "Flexible Criteria for Search"
      content: "Define personalized watermark search parameters with GroupDocs.Watermark. This precision enables targeted retrieval of hidden or customized watermark data."

    # feature loop
    - title: "Access and Organize Detected Watermarks"
      content: "Simplify document auditing by fetching all embedded watermarks. Our tools enable efficient extraction, display, and management of found items."
      
  code_samples:
    # code sample loop
    - title: "Code Example: Detect Watermarks"
      content: |
        See how to use GroupDocs.Watermark to search documents for embedded watermark content using flexible detection rules.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # Open the target document from disk or stream
        load_options = gwos.SpreadsheetLoadOptions()
        with gw.Watermarker("source.xlsx", load_options) as watermarker:

            # Define the specific watermark properties to be used in the search
            criteria = gwss.TextFormattingSearchCriteria()
            criteria.foreground_color_range = gwss.ColorRange()
            criteria.foreground_color_range.min_hue = -5.0
            criteria.foreground_color_range.max_hue = 10.0
            criteria.foreground_color_range.min_brightness = 0.01
            criteria.foreground_color_range.max_brightness = 0.99
            criteria.background_color_range = gwss.ColorRange()
            criteria.background_color_range.is_empty = True
            criteria.font_name = "Arial"
            criteria.min_font_size = 19.0
            criteria.max_font_size = 42.0
            criteria.font_bold = True

            # Perform the search and collect matches
            possible_watermarks = watermarker.search(criteria)

            # Work with the found results for further action
            print("Found {0} possible watermark(s).".format(len(possible_watermarks)))
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
    title: "Multi-Format Watermark Search"
    exclude: "EXCEL"
    description: "Locate watermark content across all file types supported by GroupDocs.Watermark."
    items: 
        # format loop 1
        - name: "Watermark PDF"
          format: "PDF"
          link: "/watermark/python-net/search//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark Word"
          format: "WORD"
          link: "/watermark/python-net/search//word/"
          description: "MS Word and Open Office documents"
          
        # format loop 3
        - name: "Watermark Excel"
          format: "EXCEL"
          link: "/watermark/python-net/search//excel/"
          description: "MS Excel and Open Office spreadsheets"

        # format loop 4
        - name: "Watermark PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/search//powerpoint/"
          description: "MS PowerPoint and Open Office presentations"

        # format loop 5
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/python-net/search//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 6
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/python-net/search//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 7
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/python-net/search//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/python-net/search//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 9
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/python-net/search//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 10
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/python-net/search//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 11
        - name: "Watermark RTF"
          format: "RTF"
          link: "/watermark/python-net/search//rtf/"
          description: "Rich Text Format"

---