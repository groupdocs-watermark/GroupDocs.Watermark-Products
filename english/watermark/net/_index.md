---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET API to Add Search Remove Watermarks to Word Excel PDF Images"
head_description: "C# .NET API to add, search and remove image & text-based watermarks from documents: PDF, Word, Excel, presentations, Visio, email and image file formats."

############################# Header ############################
title: ".NET API for Watermark Manipulation"
description: "‎Build .NET Applications to Operate Text & Image Based Watermarks with Smart Search & Strong Security Features.‎"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Watermark for .NET"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-watermark-net.png"
        product: "GroupDocs.Watermark"
        platform: ".NET"

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
            - link: "https://purchase.groupdocs.com/pricing/watermark/net"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/watermark"
        link_learn: "https://docs.groupdocs.com/watermark/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Watermark for .NET enables you to build ready-to-market business applications in C#, ASP.NET and other .NET related technologies, which let your end-users, add new watermarks, search and remove existing watermarks in supported file formats. Using GroupDocs.Watermark for .NET, you can programmatically apply digital watermarks to multitude of file formats and discourage unauthorized use of intellectual property and securely label documents of sensitive nature by employing various built-in security measures offered by this API.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Following is an overview of GroupDocs.Watermark for .NET:
      
        right:
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
          Supported [document formats and watermark type](https://docs.groupdocs.com/watermark/net/supported-document-formats/) for each format is listed below:

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT‎
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
          GroupDocs.Watermark for .NET supports following Operating Systems, Frameworks & Package Managers:‎
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operating Systems"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux

            # table loop
            - icon: "fas fa-code"
              title: "Supported Frameworks"
              content: |
                * .NET Framework 2.0 or higher
                * Mono Framework 1.2 or higher
                * .NET Standard 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Package Manager"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Development Environments"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Watermark for .NET Features"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Add or Remove Watermarks from a Particular Section or whole Document of Various File Formats"

      # feature loop
      - icon: "fas fa-eye"
        content: "Attach Watermark to all Images in a Particular Section, Page, Slide, or Document"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Assign Watermark to only Particular Frames of a Multi-Framed Image"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Allocate Hidden Watermark to PDF that only Appears when Printing Document"

      # feature loop
      - icon: "fas fa-code"
        content: "Set Watermark to all Attachments in an Excel Document & all Image Shapes in Slides"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Place Watermark or Remove it from the Background Images of Spreadsheet or Slides"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Employ Watermark to Supported Files in all Attachments of an Email or PDF Document"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Apply or Remove Watermark as XObjects, Artifacts & Annotations in PDF Documents‎"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Eliminate Watermark Containing Text with Particular Formatting"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Look for Image Watermarks that Resemble a Particular Image"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Identify Text Watermark Even if there are Unreadable Characters between Letters"

      # feature loop
      - icon: "fas fa-columns"
        content: "Search Watermarks Based on Specific Parameters or by Combining Multiple Criteria"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Specify Font Formatting to Look for Matching Text Watermark"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Programmatically Extract Page Setup & Other Information for Supported Formats"

      # feature loop
      - icon: "fas fa-print"
        content: "Add Watermark to Images inside any Header & Footer in Supported Document Formats"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Add Watermark to Image Shapes in a Word Document & Lock Watermarks to Restrict Editing"

      # feature loop
      - icon: "fas fa-lock"
        content: "Protect Text Watermark using Unreadable Characters in Presentations"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Rasterize Particular Page or Whole PDF Document to Protect Added Watermarks"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Change Text Formatting While Replacing Existing Text Watermark"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Align Watermark to Bleed Box, Art Box, Crop Box, or Trim Box in PDF Document"

      # feature loop
      - icon: "fas fa-heading"
        content: "Edit Shape Properties in Microsoft Visio Documents"

    more_feature:
      # more_feature_loop
      - title: "Adding Watermarks"
        content: |
          GroupDocs.Watermark for .NET supports multiple types of watermarks. Adding watermarks of any type is only a matter of few lines of code. Following example demonstrates, applying an image watermark to Word document using C#:

          ```cs
          // Load the document
          using (FileStream stream = File.Open("document.docx", FileMode.Open, FileAccess.ReadWrite))
          {
            using (Watermarker watermarker = new(Watermarker(stream))
            {
                    // Use path to the image as constructor's parameter
                    using (ImageWatermark watermark = new ImageWatermark("logo.png"))
                      {
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermarker.Add(watermark);
                }
                // Save the resultant document
                watermarker.Save("document_watermarked.docx");
                }
          }
          ```
      # more_feature_loop
      - title: "Apply Watermark to Files of Different Formats in a Go"
        content: "GroupDocs.Watermark API allows you to apply watermark or delete watermark of all files in a specific folder in one go. The files can even be of different format and yet the watermark will be applied to all of them accurately.‎"

      # more_feature_loop
      - title: "Foolproof Security for Watermark"
        content: "With only one line of code you can make it very difficult for any tool to remove your watermark from PDF files. This is achieved by converting all pages of a PDF document to raster images while keeping the original quality intact."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Watermark offers document viewing APIs for other popular development environments"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Watermark for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-watermark-java.png"
          product: "GroupDocs.Watermark"
          platform: "Java"
          link: "/watermark/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---