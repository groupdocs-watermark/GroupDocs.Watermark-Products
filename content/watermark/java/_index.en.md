---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:28
draft: false

lang: en
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

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
head_title: "Java Watermark Library | add watermarks to documents"
head_description: "Native Java Software to add and manipulate text and image watermarks in PDF, Word, Excel, Presentations, Visio diagrams, email and images files."

############################# Header ############################
title: "Implement documents watermarking in Java projects easily"
description: "Enhance your Java applications with the ability to watermark files using the GroupDocs.Watermark library. Our API offers customizable watermarks for a wide range of popular file formats."
words:
  for: "for"

actions:
  main: "Free Download from Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "Licensing"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java/"
  title: "Ready to get started?"
  description: "Try GroupDocs.Watermark features for free or request a license"

release:
  title: "Version {0} released"
  notes: "See what’s new"
  downloads: "Downloads"

code:
  title: "Watermark PDFs via Java"
  more: "More examples"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-watermark</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Instantiate Watermarker passing PDF path
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Customize watermark options
    TextWatermark textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Apply watermark to PDF document
    watermarker.add(textWatermark);

    // Save result document
    watermarker.save("result.pdf");
    watermarker.close();
      
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark at a glance"
  description: "Library designed for adding watermarks using Java technologies"
  features:
    # feature loop
    - title: "Watermark Files via Java"
      content: "Protect your business documents using GroupDocs.Watermark for Java. Add text, images, diagrams, or email attachments as watermarks to various file formats."

    # feature loop
    - title: "Customize Watermarks for Specific Needs"
      content: "GroupDocs.Watermark for Java offers extensive customization options for watermarks. Adjust text styles (bold, italic, font) and image properties (rotation, etc.) to tailor the watermarking process to your specific goals."

    # feature loop
    - title: "Broad Format Support"
      content: "GroupDocs.Watermark for Java seamlessly integrates with a wide range of file formats, including: PDF, Microsoft Office (Word, Excel, PowerPoint), images (JPEG, PNG, GIF, BMP), Visio diagrams, and emails. Enhance document security across diverse file types."

    # feature loop
    - title: "Effortless Watermark Search and Management"
      content: "Efficiently manage existing watermarks within documents. Locate specific watermarks, modify their text, style, or images, or remove them entirely. GroupDocs.Watermark for Java simplifies the watermarking workflow."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform independence"
  description: "GroupDocs.Watermark for Java supports various operating systems and package managers."
  items:
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Supported file formats"
  description: |
    GroupDocs.Watermark for Java enables processing of a wide range of file formats. [See the complete list](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Java : Features"
  description: "Protect your files by adding watermarks. Supports various formats including PDF, Office documents, and images."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Files Watermarking"
      content: "Add or remove watermarks from specific sections or entire documents for various supported file formats."

    # feature loop
    - icon: "watermark_style"
      title: "Watermark Customization"
      content: "Customize your watermark's appearance with options like color, font, rotation, and more."

    # feature loop
    - icon: "hidden_print"
      title: "Hidden Printing Watermark for PDF"
      content: "Add a watermark that only appears when printing a PDF document."

    # feature loop
    - icon: "image_only"
      title: "Selective Image Watermarking"
      content: "Watermark all images within a specific section, page, slide, or entire document."

    # feature loop
    - icon: "image_frame"
      title: "Watermarking Specific Image Frames"
      content: "Apply watermarks to specific frames within a multi-framed image."

    # feature loop
    - icon: "attachments"
      title: "Watermarking Attachments and Shapes"
      content: "Add watermarks to all attachments in Excel documents or all image shapes in Presentations."

    # feature loop
    - icon: "pdf_objects"
      title: "Watermark Alignment in PDF"
      content: "Align watermarks to different areas of a PDF document, including Bleed Box, Art Box, Crop Box, and Trim Box."

    # feature loop
    - icon: "doc_background"
      title: "Watermark by Background Images"
      content: "Add or remove background image watermark to Spreadsheets or Presentations."

    # feature loop
    - icon: "unreadable_characters"
      title: "Protection with Unreadable Characters"
      content: "Protect Presentations using Text Watermark with Unreadable Characters."

    # feature loop
    - icon: "watermark_text_search"
      title: "Search for Watermarks"
      content: "Get list of watermarks presented in file, using various parameters including regular expressions."

    # feature loop
    - icon: "watermark_image_search"
      title: "Find Similar Image Watermarks"
      content: "Locate image watermarks that looks like a specific image."

    # feature loop
    - icon: "document_info"
      title: "Extract Document Information"
      content: "Get various document data like page setup for supported file formats."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "Explore code examples illustrating typical GroupDocs.Watermark for Java functionalities"
  items:
    # code sample loop
    - title: "Watermark a Document Using an Image"
      content: |
        Utilize GroupDocs.Watermark for Java to enhance document security by adding image watermarks. Learn more: [Image watermarks](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="How to protect file by image watermark.">}}
        ```csharp {style=abap}
        // Load source document to Watermarker
        Watermarker watermarker = new Watermarker("document.pdf");
        
        // Specify path to a watermark image
        ImageWatermark watermark = new ImageWatermark("watermark.jpg");

        // Protect the file and save it
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Modify Watermarks"
      content: |
        GroupDocs.Watermark for Java empowers you to manage existing watermarks within documents. Locate specific watermarks and [modify their properties](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Watermarks search & modification.">}}
        ```csharp {style=abap}   
        // Load source document
        Watermarker watermarker = new Watermarker("document.pdf");

        // Search for watermarks to be updated
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);                               
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);                             

        // Update desired properties
        for (PossibleWatermark watermark : watermarks)                                                           
        {  
            watermark.setText("New Text");
        }

        // Save modified document to a specified path
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
