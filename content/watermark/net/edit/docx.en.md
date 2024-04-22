
---
############################# Static ############################
layout: "format"
date:  2024-04-22T14:58:29
draft: false
lang: en
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Edit Watermarks Across Docx Files"
head_description: "Edit watermarks across Docx files with GroupDocs.Watermark for .NET Applications. Enhance document authenticity effortlessly."

############################# Header ############################
title: "Edit Docx Watermarks Across Files: .NET Versatility" 
description: "Customize your documents with confidence using GroupDocs.Watermark for .NET Applications. Edit watermarks across various file formats effortlessly."
subtitle: "GroupDocs.Watermark for .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Free Nuget download"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Edit Watermarks Across Docx Files:** Seamlessly edit watermarks across various file formats with GroupDocs.Watermark for .NET Applications. Customize your documents with confidence and efficiency.

############################# Steps ############################
steps:
    enable: true
    title: "Programmatically Edit Watermarks in Docx Documents with the .NET API"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** furnishes .NET developers with a robust API for programmatically manipulating watermarks within diverse Docx documents. This guide outlines the process:
      
      1. Initiate the workflow by supplying your Docx file as an argument to the **Watermarker** class constructor. The file can be provided as either a byte stream, a file stream, or a reference to a local disk location.
      2. Subsequently, leverage the **SearchCriteria** object to pinpoint the specific watermarks requiring modification. This object enables the identification of watermarks previously embedded within the document.
      3. Upon successful execution of the search, you'll receive a collection of relevant watermarks. These watermarks offer granular control, allowing you to modify properties such as dimensions, page positioning, text content, color scheme, image data, and more.
      4. Following the completion of watermark edits, persist the modified document. The API facilitates storage using either a local file path or a stream object.
   
    code:
      platform: "net"
      copy_title: "Copy"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // Edit image watermark in DOCX doc

        // Initialize Watermarker by source file
        using (Watermarker watermarker = new Watermarker("input.docx"))
        {
            // Create SearchCriteria for image watermarks search
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                // Edit image watermark
                watermark.ImageData = imageData;
            }

            // Save result DOCX
            watermarker.Save("output.docx");
        }
        
        ```     

############################# More features ############################
more_features:
  enable: true
  title: "Deep dive into adding Watermark"
  description: "API to render, display, convert documents, slides, diagrams, and many other document types in .NET applications"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Add Watermark"
  features:
    # feature loop
    - title: "Watermark your documents easily."
      content: "GroupDocs.Watermark makes it easy for .NET developers to add various types of watermarks in popular business documents and files."

    # feature loop
    - title: "Customize watermarks for your goals."
      content: "Our solution supports many watermark features. You can easily adjust size, rotation, color, font, font styles and other options to make watermark looks perfect."

    # feature loop
    - title: "Use native document objects"
      content: "Accordingly do particular document format it is possible to use native document features. Native PDF annotations or MS Word page watermark may be used for watermarking."
      
  code_samples:
    # code sample loop
    - title: "PDF image watermark edit"
      content: |
        This example shows how to edit content of image watermark
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Load document as PDF
            var loadOptions = new PdfLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pdf", loadOptions))
            {
                //  Load content
                PdfContent pdfContent = watermarker.GetContent<PdfContent>();

                //  Edit image watermark
                foreach (PdfArtifact artifact in pdfContent.Pages[0].Artifacts)
                {
                    if (artifact.Image != null)
                    {
                        artifact.Image = new PdfWatermarkableImage(File.ReadAllBytes("test.png"));
                    }
                }

                //  Enjoy output result
                watermarker.save("result.pdf");
            }

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Watermark features for free or request a license"
  items:
    #  loop
    - title: "Nuget download"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Edit Watermarks Across Files"
    exclude: "DOCX"
    description: "Seamlessly edit watermarks across multiple file formats with applications powered by GroupDocs.Watermark for .NET."
    items: 
        # format loop 1
        - name: "Watermark PDF"
          format: "PDF"
          link: "/watermark/net/edit//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark Word"
          format: "WORD"
          link: "/watermark/net/edit//word/"
          description: "MS Word and Open Office documents"
          
        # format loop 3
        - name: "Watermark Excel"
          format: "EXCEL"
          link: "/watermark/net/edit//excel/"
          description: "MS Excel and Open Office spreadsheets"

        # format loop 4
        - name: "Watermark PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/edit//powerpoint/"
          description: "MS PowerPoint and Open Office presentations"

        # format loop 5
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/net/edit//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 6
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/net/edit//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 7
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/net/edit//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/net/edit//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 9
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/net/edit//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 10
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/net/edit//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 11
        - name: "Watermark RTF"
          format: "RTF"
          link: "/watermark/net/edit//rtf/"
          description: "Rich Text Format"

---