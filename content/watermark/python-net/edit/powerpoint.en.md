
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: en
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Edit Watermarks in Powerpoint files"
head_description: "Use GroupDocs.Watermark for Python via .NET to quickly change watermark content in Powerpoint presentations and keep your documents secure."

############################# Header ############################
title: "Precise Powerpoint Watermark Editing in Python" 
description: "Get full control over watermark layout and visibility in your presentations using GroupDocs.Watermark for Python via .NET."
subtitle: "GroupDocs.Watermark for Python via .NET Library" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Free download from PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET API"
    link: "/watermark/python-net/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Control Watermark Layout in Powerpoint Files:** With GroupDocs.Watermark for Python via .NET, you can place watermarks exactly where needed and secure your presentations easily.

############################# Steps ############################
steps:
    enable: true
    title: "Modify watermarks in Powerpoint documents with Python"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** helps Python developers easily update watermarks in various Powerpoint files. Here's how you can use it in your project:
      
      1. First, open your Powerpoint file by passing it to the **Watermarker** constructor. You can use a file path, byte stream, or file stream.
      2. Then, find the watermarks you want to change using **SearchCriteria**, which lets you search for watermark text or properties.
      3. Once found, you can change details like text, font, size, position, color, and more. This gives you full control over how the watermark looks.
      4. After making changes, save the document. You can write the result to a stream or a file path.
   
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
        # Update watermark text in POWERPOINT
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Create a Watermarker using a POWERPOINT file
        with gw.Watermarker("input.pptx") as watermarker:

            # Set up TextSearchCriteria to find watermark text
            search_criteria = gwss.TextSearchCriteria("test", False)

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # Modify watermark text
                        watermark.text = "passed"
                    except Exception as e:
                        pass
            
            watermarker.save("output.pptx")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Discover more ways to update watermarks"
  description: "With our library, Python apps can add, find, edit, or delete watermarks in many file types."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Watermark Editing"
  features:
    # feature loop
    - title: "Watermark Your Files with Ease"
      content: "Use GroupDocs.Watermark for Python via .NET to add and manage watermarks in your documents. Search, update, or remove watermarks as needed using a simple API."

    # feature loop
    - title: "Customize Watermarks to Fit Your Needs"
      content: "Adjust watermark settings like font, size, orientation, and color using our flexible API to get exactly the result you want."

    # feature loop
    - title: "Use Format-Specific Features"
      content: "Depending on the file format, you can use native features like headers, footers, annotations, or backgrounds as watermark areas."
      
  code_samples:
    # code sample loop
    - title: "Edit Text Watermark in Excel"
      content: |
        This code shows how to change watermark text in Excel spreadsheets.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # Open XLSX file
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # Read spreadsheet data
        with gw.Watermarker("source.xlsx") as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,3]

            # Change watermark text
            watermarks = watermarker.search(search_criteria)
            for watermark in watermarks:
                try:
                    watermark.formatted_text_fragments.clear()
                    watermark.formatted_text_fragments.add(
                       "passed", 
                        gww.Font("Calibri", 19.0, gww.FontStyle.bold), 
                        gww.Color.red, 
                        gww.Color.aqua
                    )
                except Exception as e:
                    pass
        
            # Save the result
            watermarker.save("output.xlsx")
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
    title: "Edit Watermarks in Other File Types"
    exclude: "POWERPOINT"
    description: "Use GroupDocs.Watermark for Python via .NET to work with watermarks in different document formats."
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