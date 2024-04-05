---
############################# Static ############################
layout: "landing"
date: 2024-04-05T13:59:21
draft: false

lang: en
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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

############################# Head ############################
head_title: "Node.js Watermarking Library | document watermarks"
head_description: "Node.js solution protect business documents with text and image watermarks. Popular formats like PDF, Word, Excel, PowerPoint are supported."

############################# Header ############################
title: "Access to watermarking technology in Node.js via Java solutions"
description: "Protect your intellectual property and prevent unauthorized copying with this Node.js solution. It allows users to easily add watermarks to business documents in various formats, including PDF, Word, Excel, PowerPoint, images etc."
words:
  for: "for"

actions:
  main: "Use NPM to download for free"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.watermark"
  alt: "Licensing"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
  title: "Ready to get started?"
  description: "Try GroupDocs.Watermark features for free or request a license"

release:
  title: "Version {0} released"
  notes: "See what’s new"
  downloads: "Downloads"
  link: "https://releases.groupdocs.com/watermark/nodejs-java/"

code:
  title: "Add watermark to PDF with TypeScript"
  more: "More examples"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.watermarker"
  content: |
    ```javascript {style=abap}

    // Instantiate Watermarker passing PDF path
    let loadOptions = new PdfLoadOptions();
    let watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Customize watermark options
    let textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Apply watermark to PDF document
    watermarker.add(textWatermark);

    // Save result document
    watermarker.save("result.pdf");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark at a glance"
  description: "Node.js TypeScript library for watermarking"
  features:
    # feature loop
    - title: "Node.js File Watermarking"
      content: "Protect your business documents with GroupDocs.Watermark for Node.js via Java. Add text, images, diagrams, or email attachments as watermarks to various file formats."

    # feature loop
    - title: "Customize Watermarks for Your Needs"
      content: "GroupDocs.Watermark for Node.js via Java provides extensive customization options for watermarks. Fine-tune text styles (bold, italic, font) and image properties (rotation, etc.) allow to customize documents processing."

    # feature loop
    - title: "Comprehensive Format Support"
      content: "GroupDocs.Watermark for Node.js via Java seamlessly integrates with a wide range of file formats, including: PDF, MS Office like Word, Excel, PowerPoint, images such as JPEG, PNG, GIF, BMP, Visio diagrams, emails etc. Empower documents processing to achieve business goals."

    # feature loop
    - title: "Powerful Watermark Search and Update"
      content: "Get and update existing watermarks in watermarked documents. Modify text, style, image content, or remove them entirely. GroupDocs.Watermark for Node.js via Java provides wide range of the watermarks processing."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform independence"
  description: "GroupDocs.Watermark for Node.js via Java readily integrates with various operating systems and package managers."
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
    GroupDocs.Watermark for Node.js via Java empowers you to process a diverse range of file formats. [Explore the full list](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Node.js via Java: Feature Set"
  description: "Empower robust document security through programmatic watermarking. Supports diverse file formats including: PDF, DOCX, XLSX, PPTX, and image formats (PNG, JPG, etc.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Precise Watermarking Control"
      content: "Precisely manipulate watermarks by adding or removing them from specific sections, entire documents, or individual attachments and shapes within different file formats."

    # feature loop
    - icon: "watermark_style"
      title: "Customization of Watermark Appearance"
      content: "Exert fine-grained control over watermark aesthetics by modifying attributes like color, font, opacity, rotation, and positioning within the document."

    # feature loop
    - icon: "hidden_print"
      title: "Print PDF Watermarking"
      content: "Deploy a stealthy watermark that remains invisible during regular document viewing but becomes apparent only during the printing process, enhancing document security discreetly."

    # feature loop
    - icon: "image_only"
      title: "Specific Image Watermarking"
      content: "Watermark specific images within a document using our solution. Choose to embed watermarks in a designated section (e.g., page, slide) or across the entire document."

    # feature loop
    - icon: "image_frame"
      title: "Multi-Frame Images Watermarking"
      content: "Apply watermarks selectively to specific frames within a multi-frame image format, ensuring granular control over watermark placement."

    # feature loop
    - icon: "attachments"
      title: "Comprehensive Content Protection"
      content: "Extend protection to various document elements like attachments within Excel documents and image shapes within Presentations, providing an additional layer of security."

    # feature loop
    - icon: "pdf_objects"
      title: "Advanced Watermarking in PDF"
      content: "Watermark different areas of PDFs, including Bleed Box, Art Box, Crop Box, Trim Box etc."

    # feature loop
    - icon: "doc_background"
      title: "Background Image Watermarking"
      content: "Manage watermarks within the background images of Spreadsheets and Presentations, offering additional customization options for visual security measures."

    # feature loop
    - icon: "unreadable_characters"
      title: "Text Watermark with Unreadable Characters"
      content: "Employ unreadable characters within text watermarks embedded in Presentations, bolstering security by making unauthorized watermark extraction significantly more challenging."

    # feature loop
    - icon: "watermark_text_search"
      title: "Advanced Watermark Search"
      content: "Utilize comprehensive search capabilities to locate watermarks within documents based on specific parameters or by combining various criteria, enabling efficient retrieval and management."

    # feature loop
    - icon: "watermark_image_search"
      title: "Similar Image Watermark Detection"
      content: "Find similar watermark images within documents that visually resemble an source image."

    # feature loop
    - icon: "document_info"
      title: "Programmatic Document Information Extraction"
      content: "Extract valuable metadata programmatically, including page setup details and other document information for supported file formats."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "Dive into code examples showcasing common GroupDocs.Watermark for Node.js via Java functionalities"
  items:
    # code sample loop
    - title: "Watermark a Document with an Image"
      content: |
        Leverage GroupDocs.Watermark for Node.js via Java to enhance document security by adding image watermarks. Learn more: [Image watermarks](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="How to protect file by image watermark.">}}
        ```javascript {style=abap}
        // Load source document to Watermarker
        let watermarker = new Watermarker("document.pdf");
        
        // Specify path to a watermark image
        let watermark = new ImageWatermark("watermark.jpg");

        // Protect the file and save it
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Search and Modify Existing Watermarks"
      content: |
        GroupDocs.Watermark for Node.js via Java empowers you to manage document watermarks. Select watermarks, modify their properties. Discover how: [Modify watermarks](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Watermarks search & modification.">}}
        ```javascript {style=abap}   
        // Load source document
        let watermarker = new Watermarker("document.pdf");

        // Search for watermarks to be updated
        let searchCriteria = new TextSearchCriteria("test", false);                               
        let watermarks = watermarker.search(searchCriteria); 

        // Update desired properties
        watermarks.forEach((watermark)
        {  
            watermark.setText("New Text");
        }

        // Save modified document to a specified path
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
