---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:49
draft: false

lang: en
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"
    # supported_platforms loop
    - title: "Python"
      tag: "python-net"

############################# Head ############################
head_title: "Python Watermarking Library | Document Watermarks"
head_description: "Python protects business documents with text and image watermarks. File formats like PDF, Word, Excel, and PowerPoint are supported."

############################# Header ############################
title: "Access Python via .NET Watermarking Technology"
description: "Safeguard your data and prevent unauthorized copying with this Python solution. Easily add watermarks to business documents in various formats, including PDF, Word, Excel, PowerPoint, images, etc."
words:
  for: "for"

actions:
  main: "PyPi download for free"
  main_link: "https://pypi.org/project/groupdocs-watermark-net/"
  alt: "Licensing"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
  title: "Ready to get started?"
  description: "Try GroupDocs.Watermark features for free or request a license"

release:
  title: "Version {0} released"
  notes: "See what’s new"
  downloads: "Downloads"
  link: "https://releases.groupdocs.com/watermark/python-net/"

code:
  title: "Add Watermark to PDF using Python"
  more: "More examples"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
  install: "pip install groupdocs-watermark-net"
  content: |
    ```python {style=abap}

    import groupdocs.watermark as gw
    import groupdocs.watermark.watermarks as gww
    import groupdocs.watermark.options.pdf as gwop
    import groupdocs.watermark.common as gwc

    # Instantiate Watermarker passing PDF path
    pdf_lo = gwop.PdfLoadOptions()
    with gw.Watermarker("source.pdf", pdf_lo) as watermarker:
        options = gwop.PdfArtifactWatermarkOptions()

        # Customize watermark options
        text_watermark = 
            gww.TextWatermark("Approved", gww.Font("Arial", 8.0))
        text_watermark.horizontal_alignment = 
            gwc.HorizontalAlignment.RIGHT

        # Apply watermark to PDF document
        watermarker.add(text_watermark, options)

        # Save result document
        watermarker.save("result.pdf")

    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark at a glance"
  description: "Python Library for Watermarking"
  features:
    # feature loop
    - title: "Python Document Watermarking"
      content: "Secure your sensitive data with GroupDocs.Watermark for Python via .NET. Put text or images on various file formats as watermarks."

    # feature loop
    - title: "Customize Watermarks"
      content: "Many customization options are available in GroupDocs.Watermark for Python via .NET. Set up text styles (bold, italic, font) or image properties like  size or rotation to tune document watermarking."

    # feature loop
    - title: "Popular File Formats Support"
      content: "GroupDocs.Watermark for Python via .NET supports wide range of file formats, including PDF, MS Office docs like Word, Excel, PowerPoint, and images such as JPEG, PNG, GIF, BMP, Visio diagrams, emails, etc. Enhance document processing to meet business goals."

    # feature loop
    - title: "Watermark Search and Update"
      content: "Retrieve and update watermarks which are placed in documents. Modify text style, image content, or remove them entirely. GroupDocs.Watermark for Python via .NET offers a wide range of watermark processing capabilities."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform independence"
  description: "GroupDocs.Watermark for Python via .NET seamlessly integrates with various operating systems and package managers."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Supported file formats"
  description: |
    GroupDocs.Watermark for Python via .NET empowers you to process a diverse range of file formats. [Explore the full list](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office & OpenDocument formats
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### Images & Graphics
        * **Popular image formats:** BMP, JPG, JPEG, PNG
        * **Multi-page images:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### Other
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark for Python via .NET features"
  description: "Strengthen document security through programmatic watermarking. Process diverse file formats including PDF, DOCX, XLSX, PPTX, and image formats (PNG, JPG, etc.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Precise Watermarking Control"
      content: "Precisely manage watermarks by adding or removing them from specific sections, entire documents, or individual attachments and shapes within different file formats."

    # feature loop
    - icon: "watermark_style"
      title: "Customize Watermark Appearance"
      content: "Exert fine-grained control over watermark aesthetics by modifying attributes like color, font, opacity, rotation, and positioning within the document."

    # feature loop
    - icon: "hidden_print"
      title: "Print PDF Watermarking"
      content: "Add hidden watermarks into regular documents which become visible only during the printing process, enhancing document security discreetly."

    # feature loop
    - icon: "image_only"
      title: "Specific Image Watermarking"
      content: "Watermark specific images within a document using our solution. Embed watermarks in a designated section (e.g., page, slide) or across the entire document."

    # feature loop
    - icon: "image_frame"
      title: "Multi-Layer Image Watermarks"
      content: "Add watermarks precisely to specific frames within a multi-frame image format, achieving granular control over watermark placement."

    # feature loop
    - icon: "attachments"
      title: "Comprehensive Content Protection"
      content: "Extend protection to various document elements like attachments within Excel documents and image shapes within presentations, providing an additional layer of security."

    # feature loop
    - icon: "pdf_objects"
      title: "Advanced PDF Watermarking"
      content: "Watermark different areas of PDFs, including Bleed Box, Art Box, Crop Box, Trim Box, etc."

    # feature loop
    - icon: "doc_background"
      title: "Background Image Watermarking"
      content: "Manage watermarks within the background images of spreadsheets and presentations, offering additional customization options for visual security measures."

    # feature loop
    - icon: "unreadable_characters"
      title: "Text Watermark with Unreadable Characters"
      content: "Employ unreadable characters within text watermarks embedded in presentations, bolstering security by making unauthorized watermark extraction significantly more challenging."

    # feature loop
    - icon: "watermark_text_search"
      title: "Advanced Watermark Search"
      content: "Use comprehensive search features to locate watermarks in documents based on specific parameters or by combining various criteria."

    # feature loop
    - icon: "watermark_image_search"
      title: "Similar Image Watermark Detection"
      content: "Find similar watermark images within documents that visually resemble a source image."

    # feature loop
    - icon: "document_info"
      title: "Analyze Document Information"
      content: "Extract essential document data like page setup for further analysis."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "Explore code examples showcasing common GroupDocs.Watermark for Python via .NET functionalities."
  items:
    # code sample loop
    - title: "Watermark a Document with an Image"
      content: |
        Use GroupDocs.Watermark for Python via .NET to protect documents by adding image watermarks. [Learn more](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="How to protect file by image watermark.">}}
        ```python {style=abap}

        # Load source document to Watermarker
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Specify path to a watermark image
            watermark = groupdocs.watermark.watermarks.ImageWatermark("watermark.jpg")
            watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwgroupdocs.watermark.common.VerticalAlignment.CENTER

            # Protect the file and save it
            watermarker.add(watermark)
            watermarker.save("result.pdf")
       
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Search and Modify Existing Watermarks"
      content: |
        GroupDocs.Watermark for Python via .NET empowers you to manage document watermarks. Select watermarks and modify their properties. [Discover how](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Watermarks search & modification.">}}
        ```python {style=abap}

        # Load source document
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Search for watermarks to be updated
            search_criteria = groupdocs.watermark.search.searchcriteria.TextSearchCriteria("annotation", False)
            watermarks = watermarker.search(search_criteria)
            
            # Update desired properties
            for watermark in watermarks:
                watermark.text = "passed"

            # Save modified document to a specified path
            watermarker.save("result.pdf")


        ```
        {{< /landing/code >}}

---
