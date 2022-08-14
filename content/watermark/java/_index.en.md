---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java API to Add Search Remove Watermarks to PDF Word Excel Images"
head_description: "Java document watermarking API – Generate, search & remove watermarks from documents: PDF, Word, Excel, presentations, Visio, email and image file formats."

############################# Header ############################
title: "Java API to Manipulate Watermarks"
description: "Develop Java Applications to Perform Image & Text Watermarking Operations with Smart Search & Robust Security."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Watermark for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-watermark-java.png"
        product: "GroupDocs.Watermark"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overview"

            # button loop
            - link: "#features"
              text: "Features"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/watermark"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/watermark/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/watermark"
        link_learn: "https://docs.groupdocs.com/watermark/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Watermark for Java allows you to make business applications that enable your end-users to apply new watermarks, search and delete existing watermarks in files of supported formats. You can programmatically assign digital watermarks to lots of file formats and utilize its powerful smart search abilities. GroupDocs.Watermark for Java provides various built-in security measures that can be employed to avoid misuse of digital documents that contain sensitive information or intellectual property content.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          Following is an overview of GroupDocs.Watermark for Java:

        rright:
          enable: true
          icon: "fab fa-html5"
          title: "Overview"
          content: |
            * Add & Remove Watermark
            * Search & Replace Watermark
            * Search by Formatting
            * Search by Image Comparison
            * Work with Headers & Footers
            * Work with Background Images
            * Work with Attachments
            * Rasterize Pages
            * Apply Editing Restrictions
      
      ## TAB TWO ##
      tab_two:
        description: |
          Supported [document formats and watermark type](https://docs.groupdocs.com/watermark/java/supported-document-formats/) for each format is listed below:

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
                * **Visio:** VSD, VDX, VSS, VSSX, VSX, VST, VSTX, VTX, VSDX, VDW, VSTM, VSSM, VSDM

            # table loop
            - title: "Adding Watermark"
              content: |
                * **PDF**: XObject, Artifact, Annotation
                * **Word**: Shape
                * **Excel**: Shape, Header & Footer
                * **PowerPoint**: Shape
                * **Visio**: Shape
                * **Raster Image**: Text, Image
                * **Multi-page Tiff**: Text, Image
                * **Animated Gif**: Text, Image

        right:
          enable: true
          table:
            # table loop
            - title: "PDF and Image documents"
              content: |
                * **Portable Document Format**: PDF
                * **Open Document**: ODT
                * **Email**: EML, MSG, EMLX, OFT
                * **Images**: PNG, BMP, GIF, JPG, JPEG, JP2, TIF, TIFF, WebP

            # table loop
            - title: "Removing Watermark"
              content: |
                * **PDF**: XObject, Artifact, Annotation, Regular Text
                * **Word**: Shape, Regular Text
                * **Excel**: Shape, Header & Footer, Background Image, Text and formulas in cells
                * **PowerPoint**: Shape
                * **Visio**: Shape, Diagram Comments
                * **Email**: Attached and embedded images, Subject and body text fragments

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Watermark for Java supports following Operating Systems, Frameworks & Package Managers:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operating Systems"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Supported Frameworks"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Development Environments"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Build Automation Tool"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Watermark for Java Features"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Pull all Documents of Various Formats from a Folder and Apply or Remove Watermarks"

      # feature loop
      - icon: "fas fa-eye"
        content: "Employ or Delete Watermark from a Particular Section or Complete Document"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Apply Watermark to all Images in a Particular Section, Page, Slide, or Document"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Attach Watermark to Selected Frames of a Multi-Framed Image"

      # feature loop
      - icon: "fas fa-code"
        content: "Apply Hidden Watermark to PDF to Appear when Printing Document"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Employ Watermark to Attachments in an Excel Document & all Image Shapes in Slides"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Place Watermark or Delete it from the Background Images of Slides or Excel Sheet"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Set Watermark to Supported Files in Attachments of an Email or PDF File"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Add or Delete Watermark as XObject, Artifacts & Annotations in PDF Filese"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Delete Watermark matching Text with Particular Formatting"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Find Image Watermarks resembling a Particular Image"

      # feature loop
      - icon: "fas fa-columns"
        content: "Identify Text Watermark even if there are Unreadable Characters between Letters"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Look for Watermarks based on Specific Parameters or by Assigning Multiple Criteria"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Specify Font Formatting to locate Matching Text Watermark"

      # feature loop
      - icon: "fas fa-print"
        content: "Get Page, Slide, Cell Dimensions for Absolute Size & Positioning of Watermark"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Apply Watermark to Images inside any Header & Footer in Supported Document Formats"

      # feature loop
      - icon: "fas fa-lock"
        content: "Add Watermark to Image Shapes in a Word Document & Restrict Editing of Watermarks"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Secure Text Watermark in Presentations using Unreadable Characters"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Protect PDF Document Watermarks by Rasterizing Single Page or Whole Document"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Modify Text Formatting when Replacing Current Text Watermark"

      # feature loop
      - icon: "fas fa-heading"
        content: "Align Watermark to Bleed Box, Art Box, Crop Box, or Trim Box in PDF File"

    more_feature:
      # more_feature_loop
      - title: "Employ Watermarks"
        content: |
          GroupDocs.Watermark for Java allows you to work with numerous kinds of watermarks. It is only a matter of few lines of code to add watermark of any type. Following example shares, how you can add an image watermark in a Word document using Java:
          
          ```java
          Document doc = Document.load(Common.mapSourceFilePath("D://test.docx"));
          Font font = new Font("Times New Roman", 12);
          TextWatermark watermark = new TextWatermark("Test watermark", font);

          // Set sizing type
          watermark.setSizingType(SizingType.ScaleToParentDimensions);

          // Set watermark scale
          watermark.setScaleFactor(0.5);

          doc.addWatermark(watermark);
          doc.save(Common.mapOutputFilePath("D://test.docx"));
          doc.close();
          ```
      # more_feature_loop
      - title: "Add Watermark to Files of Different Formats in a Go"
        content: "With GroupDocs.Watermark for Java API you can add or remove watermark of all documents present in a particular folder in batch mode. It does not matter, if the documents are of different format, GroupDocs.Watermark for Java will apply watermark to all the files accurately."

      # more_feature_loop
      - title: "Assign Foolproof Security to your Watermarks"
        content: "With minimal code you can assign foolproof security to your watermarks and make it extremely difficult for any 3rd party tool to modify or remove your assigned watermark from PDF file. It is so because GroupDocs.Watermark for Java allows you to convert all pages of a PDF file into Rasterized images. This approach makes your digital watermarks secure while keeping their quality near to original."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Watermark offers document viewing APIs for other popular development environments"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Watermark for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-watermark-net.png"
          product: "GroupDocs.Watermark"
          platform: ".NET"
          link: "/watermark/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---