---
############################# Static ############################
layout: "landing"
date: 2024-02-26T19:06:43
draft: false

lang: en
product: "Watermark"
product_tag: "watermark"
platform: "Net"
platform_tag: "net"

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
head_title: "C# .NET Document Watermark Software | add watermark library | remove watermark software | watermark office documents"
head_description: "C# .NET Library to add, search and remove image & text-based watermarks to documents: PDF, Word, Excel, presentations, Visio diagrams, email and image file formats."

############################# Header ############################
title: "Watermark documents easily in your C# .NET applications"
description: "Empower your C# solutions with a flexible document watermarking API that provides adding customizable watermarks to all popular document formats."
words:
  for: "for"

actions:
  main: "Free NuGet Download"
  main_link: "https://www.nuget.org/packages/GroupDocs.Watermark"
  alt: "Licensing"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/net/"
  title: "Ready to get started?"
  description: "Try GroupDocs.Watermark features for free or request a license"

release:
  title: "Version {0} released"
  notes: "See what’s new"
  downloads: "Downloads"

code:
  title: "Watermark PDF files in C#"
  more: "More examples"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
  install: "dotnet add package GroupDocs.Watermark"
  content: |
    ```csharp {style=abap}   
    // Instantiate Watermarker passing PDF path
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    using (Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions))
    {
        // Customize watermark options
        TextWatermark textWatermark = 
            new TextWatermark("Approved", new Font("Arial", 8));
        
        // Apply watermark to PDF document
        watermarker.Add(textWatermark);

        // Save result document
        watermarker.Save("result.pdf");
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark at a glance"
  description: "API to put watermarks on documents via .NET"
  features:
    # feature loop
    - title: "C# files watermark"
      content: "Add watermarks to your business files using GroupDocs.Watermark. Use text, images, diagrams or email attachments."

    # feature loop
    - title: "Customize watermarks to your goals"
      content: "GroupDocs.Watermark for .NET software allows to customize watermarks in various ways. Text styles like bold, italic, font types along with image properties like rotation etc. enrich watermarking process."

    # feature loop
    - title: "All popular file formats are supported"
      content: "Many file and document formats are supported by GroupDocs.Watermark solution. PDF, Microsoft Office Word, Excel, PowerPoint, images like JPEG, PNG, GIF, BMP, Visio diagrams, emails etc. could be protected with our watermarks."

    # feature loop
    - title: "Search and update watermarks"
      content: "Watermarks which are already presented in a document may be found and processed again. Modify text, style, images or remove revealed watermarks without extra efforts."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform independence"
  description: "GroupDocs.Watermark for .NET supports operating systems, frameworks and package managers listed below"
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Supported file formats"
  description: |
    GroupDocs.Watermark for .NET provides processing of the following [file formats](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark features"
  description: "Protect PDF, Office, Images and other formats by watermark"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Documents watermarking"
      content: "Add or Remove Watermarks from a Particular Section or whole Document of Various File Formats."

    # feature loop
    - icon: "watermark_style"
      title: "Style your watermark"
      content: "Customize various watermark properties like color, font, rotation etc."

    # feature loop
    - icon: "hidden_print"
      title: "PDF hidden printing watermark"
      content: "Allocate Hidden Watermark to PDF that only Appears when Printing Document."

    # feature loop
    - icon: "image_only"
      title: "Watermark only images in documents"
      content: "Watermark all Images in a Particular Section, Page, Slide, or Document."

    # feature loop
    - icon: "image_frame"
      title: "Process selected image frames"
      content: "Assign Watermark to only Particular Frames of a Multi-Framed Image."

    # feature loop
    - icon: "attachments"
      title: "Attachments & shapes"
      content: "Set Watermark to all Attachments in an Excel Document & all Image Shapes in Slides."

    # feature loop
    - icon: "pdf_objects"
      title: "PDF objects"
      content: "Align Watermark to Bleed Box, Art Box, Crop Box, or Trim Box in PDF Document."

    # feature loop
    - icon: "doc_background"
      title: "Documents background"
      content: "Place Watermark or Remove it from the Background Images of Spreadsheet or Slides."

    # feature loop
    - icon: "unreadable_characters"
      title: "Unreadable Characters Protection"
      content: "Protect Text Watermark using Unreadable Characters in Presentations."

    # feature loop
    - icon: "watermark_text_search"
      title: "Search Watermarks in Documents"
      content: "Search Watermarks Based on Specific Parameters or by Combining Multiple Criteria."

    # feature loop
    - icon: "watermark_image_search"
      title: "Search similar image watermarks"
      content: "Look for Image Watermarks that Resemble a Particular Image."

    # feature loop
    - icon: "document_info"
      title: "Get document information"
      content: "Programmatically Extract Page Setup & Other Information for Supported Formats."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "Some use cases of typical GroupDocs.Watermark for .NET operations"
  items:
    # code sample loop
    - title: "Watermark by adding an image to a document."
      content: |
        To protect any document you can use [image watermarks](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/):
        {{< landing/code title="How to protect file by image watermark.">}}
        ```csharp {style=abap}
        // Load source document to Watermarker
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Specify path to a watermark image
            using (ImageWatermark watermark = new ImageWatermark("watermark.jpg"))
            {
                // Protect the file and save it
                watermarker.Add(watermark);

                watermarker.Save("result.pdf");
            }
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Search and modify existing watermarks."
      content: |
        GroupDocs.Watermark is able to [modify watermarks](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/) that are already presented in a document. Search for desired items and update their properties.
        {{< landing/code title="Watermarks search & modification.">}}
        ```csharp {style=abap}   
        // Load source document
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Search for watermarks to be updated
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                // Update desired properties
                watermark.Text = "New Text";
            }

            // Save modified document to a specified path
            watermarker.Save("document.pdf");
        }
        ```
        {{< /landing/code >}}

---
