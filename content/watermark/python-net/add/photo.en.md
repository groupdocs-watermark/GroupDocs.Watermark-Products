
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: en
format: Photo
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Easily Watermark Your Photos"
head_description: "Add watermarks to your photos in Python to protect your work and copyright."

############################# Header ############################
title: "Fast Photo Watermarking with Python" 
description: "Use our Python library to quickly add watermarks to your photos. Protect your copyright and brand without losing image quality."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download PyPi for free"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET is great for photographers who want to protect their work. Add text or image watermarks to photos in formats like JPEG, PNG, and RAW. Adjust transparency, size, and position so your watermark fits perfectly and your photo still looks good.

############################# Steps ############################
steps:
    enable: true
    title: "Easily Add Watermarks: Python Watermarking for Photo"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** is a library that makes it easy to add watermarks to many business file types. Follow these steps to quickly add watermarks to your documents in Python:
      
      1. **Get Started with Watermarking:** Begin by creating an instance of the **Watermarker** class. Pass your Photo file (as a path or stream) to the constructor to open it for watermarking.
      2. **Create Your Watermark:** Make a **Watermark** object with your desired text and settings. You can add watermarks to any page or even to document elements like headers or attachments.
      3. **Customize the Watermark:** Adjust the watermark’s size, position, font, color, and alignment to fit your needs. This helps your watermark look just right in your document.
      4. **Apply and Save:** Use the **Watermarker** method to add your watermark(s) to the document. Save the result, ideally to a new file for safety.
   
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
        # Add a text watermark to a PHOTO file
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # Select the file you want to watermark
        with gw.Watermarker("input.png") as watermarker:

            # Create a text watermark object
            font = gww.Font("Arial", 36.0)
            watermark = gww.TextWatermark("top secret", font)
            watermark.foreground_color = gww.Color.red
            watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
            watermark.opacity = 0.4

            watermarker.add(watermark)

            # Save the updated PHOTO file
            watermarker.save("output.png")
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Explore More Watermarking Features"
  description: "Use our Python API to add, view, convert, and manage watermarks in documents, slides, diagrams, and more. GroupDocs.Watermark for Python via .NET helps you protect your files and add copyright information easily."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Add Watermark"
  features:
    # feature loop
    - title: "Add Watermarks Easily"
      content: "GroupDocs.Watermark lets Python developers quickly add text, image, or dynamic watermarks to business documents. Keep your files secure and branded with minimal effort."

    # feature loop
    - title: "Fully Customizable Watermarks"
      content: "Change watermark size, rotation, transparency, color, and font with GroupDocs.Watermark. Make your watermark fit your document perfectly and keep important content visible."

    # feature loop
    - title: "Use Document Features for Watermarking"
      content: "Take advantage of built-in document features like PDF annotations, Word backgrounds, or Excel headers to add watermarks. GroupDocs.Watermark works with document structures for effective, non-intrusive watermarking."
      
  code_samples:
    # code sample loop
    - title: "Add an Image Watermark to DOCX"
      content: |
        This example shows how to apply image effects to shape watermarks.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.wordprocessing as gwow

        # Open a Word document
        load_options = gwow.WordProcessingLoadOptions()
        with gw.Watermarker("source.docx", load_options) as watermarker:

            # Set watermark options
            with gww.ImageWatermark("logo.png") as watermark:

                effects = gwow.WordProcessingImageEffects()
                effects.brightness = 0.7
                effects.contrast = 0.6
                effects.chroma_key = gww.Color.red

                options = gwow.WordProcessingWatermarkSectionOptions()
                options.Effects = effects;

                # Create the watermark
                watermarker.add(watermark, options)

                # Save the document with the watermark
                watermarker.save("result.docx")
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
    title: "Protect Your Photos with Watermarks in Python"
    exclude: "PHOTO"
    description: "Add custom watermarks to your photos using our Python API. Keep your images safe and looking professional."
    items: 
        # format loop 1
        - name: "Watermark PDF"
          format: "PDF"
          link: "/watermark/python-net/add//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark Word"
          format: "WORD"
          link: "/watermark/python-net/add//word/"
          description: "MS Word and Open Office documents"
          
        # format loop 3
        - name: "Watermark Excel"
          format: "EXCEL"
          link: "/watermark/python-net/add//excel/"
          description: "MS Excel and Open Office spreadsheets"

        # format loop 4
        - name: "Watermark Image"
          format: "IMAGE"
          link: "/watermark/python-net/add//image/"
          description: "Popular image formats"

        # format loop 5
        - name: "Watermark Photo"
          format: "PHOTO"
          link: "/watermark/python-net/add//photo/"
          description: "Photo formats"

        # format loop 6
        - name: "Watermark PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/add//powerpoint/"
          description: "MS PowerPoint and Open Office presentations"

        # format loop 7
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/python-net/add//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 8
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/python-net/add//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 9
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/python-net/add//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 10
        - name: "Watermark JPEG"
          format: "JPEG"
          link: "/watermark/python-net/add//jpeg/"
          description: "JPEG Image"

        # format loop 11
        - name: "Watermark PNG"
          format: "PNG"
          link: "/watermark/python-net/add//png/"
          description: "Portable Network Graphic"

        # format loop 12
        - name: "Watermark TIFF"
          format: "TIFF"
          link: "/watermark/python-net/add//tiff/"
          description: "Tag Image File Format"

        # format loop 13
        - name: "Watermark WEBP"
          format: "WEBP"
          link: "/watermark/python-net/add//webp/"
          description: "WEB Picture"

        # format loop 14
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/python-net/add//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 15
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/python-net/add//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 16
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/python-net/add//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 17
        - name: "Watermark RTF"
          format: "RTF"
          link: "/watermark/python-net/add//rtf/"
          description: "Rich Text Format"

---