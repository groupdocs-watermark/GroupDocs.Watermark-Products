
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:23
draft: false
lang: en
format: Jpg
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C# Watermarking for JPG Images"
head_description: "Integrate watermarking into JPG files using .NET C#, safeguarding your digital images effectively."

############################# Header ############################
title: "Secure JPG Images with .NET C#" 
description: "Apply .NET C# to create robust watermarks for JPG images, ideal for copyright protection and preventing unauthorized use."
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download at Nuget for free"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET provides .NET C# developers with an advanced framework for adding watermarks to JPG images. This API allows for the precise embedding of text, logos, and graphic watermarks that are customizable in opacity, position, and size, perfect for digital media and professional photography. Enhance your images' security without sacrificing quality, with features designed to embed watermarks that deter piracy while maintaining the integrity of the original artwork. Suitable for a wide range of applications from personal photo protection to commercial use in advertising and media, GroupDocs.Watermark ensures that your visual assets are uniquely marked and legally protected.

############################# Steps ############################
steps:
    enable: true
    title: "Effortlessly Generate Watermarks for Jpg Documents"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/):** Advanced Watermarking library for .NET applications. Empower your solution and secure documents with watermarks just in time.
      
      1. **Core Class: Watermarker.** The main class of our API is **Watermarker**. You need to instantiate it before document processing. Do not forget to pass the Jpg file to the constructor as a path or a stream object.
      2. **Crafting Your Watermark.** The next step is constructing a Watermark object of the desired type. It can be placed not only on a specific document page but also in native document parts like images or headers.
      3. **Fine-Tuning Appearance.** Set watermark properties such as height and width, top, left, central alignments, fonts and colors, etc.
      4. **Applying and Saving.** Use the **Watermarker** method to add a new watermark. Feel free to add as many watermarks as you need. You may save the watermarked document to any location.
   
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
        // Generate image watermark in JPG file

        // Provide source file path to Watermarker constructor
        using (Watermarker watermarker = new Watermarker("input.jpg"))
        {
            // Generate image watermark instance with image file
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // Save watermarked JPG result
            watermarker.Save("output.jpg");
        }
        
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "Elevate Your Watermarking Game"
  description: "Unlock advanced watermarking capabilities with our GroupDocs.Watermark API for .NET. This powerful tool allows for precise customization and application of watermarks across various document types to ensure maximum security and copyright adherence with minimal visual disruption."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Comprehensive Watermarking Solutions"
  features:
    # feature loop
    - title: "Sophisticated Tiling Options"
      content: "Extend your watermarks across entire documents seamlessly with our tiling options. This feature allows watermarks to cover the full document area, preventing removal and ensuring complete document protection without compromising on design or readability."

    # feature loop
    - title: "Vibrant Color Customization"
      content: "Add a splash of color to your watermarks! Our API enables full spectrum color customization, allowing you to apply watermarks that perfectly match your corporate branding or document style. Enhance visual appeal while maintaining robust security features."

    # feature loop
    - title: "Enhanced Security Settings"
      content: "Take document security to the next level with advanced watermark settings. Configure multi-layer watermarks, incorporating both visible and invisible elements, to protect against unauthorized copying and ensure only intended recipients can access critical information."
      
  code_samples:
    # code sample loop
    - title: "Generate PowerPoint watermark"
      content: |
        This example shows how to add watermark to the PPTX background images
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Load PPTX presentation
            var loadOptions = new PresentationLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pptx", loadOptions))
            {
                //  Set up watermark properties
                TextWatermark watermark = new TextWatermark("Protected image", new Font("Arial", 8));
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermark.RotateAngle = 45;
                watermark.SizingType = SizingType.ScaleToParentDimensions;
                watermark.ScaleFactor = 1;

                //  Watermark slides background
                PresentationContent content = watermarker.GetContent<PresentationContent>();
                foreach (PresentationSlide slide in content.Slides)
                {
                    if (slide.ImageFillFormat.BackgroundImage != null)
                    {
                        slide.ImageFillFormat.BackgroundImage.Add(watermark);
                    }
                }

                //  Save processed presentation
                watermarker.save("result.pptx");
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
    title: "Implement Watermarks in JPG with C#"
    exclude: "JPG"
    description: "Leverage .NET C# for embedding invisible or visible watermarks in JPG files, essential for secure and recognizable digital content."
    items: 
        # format loop 1
        - name: "Watermark PDF"
          format: "PDF"
          link: "/watermark/net/generate//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark Word"
          format: "WORD"
          link: "/watermark/net/generate//word/"
          description: "MS Word and Open Office documents"
          
        # format loop 3
        - name: "Watermark Excel"
          format: "EXCEL"
          link: "/watermark/net/generate//excel/"
          description: "MS Excel and Open Office spreadsheets"

        # format loop 4
        - name: "Watermark Image"
          format: "IMAGE"
          link: "/watermark/net/generate//image/"
          description: "Popular image formats"

        # format loop 5
        - name: "Watermark Photo"
          format: "PHOTO"
          link: "/watermark/net/generate//photo/"
          description: "Photo formats"

        # format loop 6
        - name: "Watermark PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/generate//powerpoint/"
          description: "MS PowerPoint and Open Office presentations"

        # format loop 7
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/net/generate//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 8
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/net/generate//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 9
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/net/generate//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 10
        - name: "Watermark JPEG"
          format: "JPEG"
          link: "/watermark/net/generate//jpeg/"
          description: "JPEG Image"

        # format loop 11
        - name: "Watermark PNG"
          format: "PNG"
          link: "/watermark/net/generate//png/"
          description: "Portable Network Graphic"

        # format loop 12
        - name: "Watermark TIFF"
          format: "TIFF"
          link: "/watermark/net/generate//tiff/"
          description: "Tag Image File Format"

        # format loop 13
        - name: "Watermark WEBP"
          format: "WEBP"
          link: "/watermark/net/generate//webp/"
          description: "WEB Picture"

        # format loop 14
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/net/generate//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 15
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/net/generate//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 16
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/net/generate//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 17
        - name: "Watermark RTF"
          format: "RTF"
          link: "/watermark/net/generate//rtf/"
          description: "Rich Text Format"

---