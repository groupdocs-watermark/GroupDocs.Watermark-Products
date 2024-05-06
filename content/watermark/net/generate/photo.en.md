
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:28
draft: false
lang: en
format: Photo
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Watermark your Photos Quickly & Easily"
head_description: "Quickly secure and claim copyright on your photos with .NET C# watermarks. Start protecting your work today."

############################# Header ############################
title: "Fast and Easy Photo Watermarking with .NET" 
description: "Our powerful C# library allows for rapid watermarking of your photos, helping you secure copyright and enhance brand identity without compromising image quality."
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
       GroupDocs.Watermark for .NET offers a powerful solution for photographer's services looking to protect their copyright and brand identity. This API enables the quick addition of text or graphic watermarks to photos across a variety of formats including JPEG, PNG, and RAW. Customize your watermarks for transparency, size, and position to blend seamlessly with the photo, maintaining aesthetic quality while asserting your legal rights and deterring unauthorized use.

############################# Steps ############################
steps:
    enable: true
    title: "Enhance Your Documents: Generate Watermarks for Photo using .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** is a library that simplifies adding watermarks to various business file formats for .NET developers. Integrate our library into your application and effortlessly watermark documents using these following steps:
      
      1. **Initiating Your Watermarking Journey:** Start by acquainting yourself with the **Watermarker** class, the cornerstone of our API. To begin the process, ensure you instantiate it prior to document processing. Don't overlook the importance of providing the Photo file to the constructor, whether it's a path or a stream object.
      2. **Crafting Custom Watermarks:** Move on to the next phase by creating a **Watermark** object tailored to your specifications. This versatile tool isn't limited to specific document pages; it can also be seamlessly integrated into native document elements like attachments or headers.
      3. **Fine-tuning Watermark Attributes:** Refine your watermarking experience by adjusting properties such as height, width, page alignment, font family, and color. This level of customization ensures your watermarks blend seamlessly with your documents.
      4. **Applying Your Watermarks:** Utilize the **Watermarker** method to effortlessly apply your custom watermarks to your documents. Whether you need to add one or multiple watermarks, this process offers flexibility. For added security, consider saving your processed documents in a separate location.
   
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
        // Generate text watermark in PHOTO file

        // Provide file to be watermarked
        using (Watermarker watermarker = new Watermarker("input.png"))
        {
            // Generate text watermark instance
            Font font = new Font("Arial", 19, FontStyle.Bold | FontStyle.Italic);
            TextWatermark watermark = new TextWatermark("my watermark", font);
            watermark.ForegroundColor = Color.Red;
            watermark.BackgroundColor = Color.Blue;
            watermarker.Add(watermark);

            // Save PHOTO result
            watermarker.Save("output.png");
        }
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Deep dive into Adding Watermarks"
  description: "Leverage our powerful API to render, display, convert, and manage documents, slides, diagrams, and various other document types within .NET applications. GroupDocs.Watermark seamlessly integrates watermarking capabilities to enhance document security and copyright protection."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Add Watermark"
  features:
    # feature loop
    - title: "Watermark Your Documents Effortlessly"
      content: "GroupDocs.Watermark empowers .NET developers to easily integrate watermarking into their applications. Add text, image, or dynamic watermarks to popular business documents and files effortlessly, ensuring your content is secure and branded consistently across all platforms."

    # feature loop
    - title: "Tailor Watermarks to Meet Your Needs"
      content: "Customize watermarks to match your specific requirements with extensive features supported by GroupDocs.Watermark. Adjust size, rotation, transparency, color, and font to ensure your watermark not only looks perfect but also enhances document security without obstructing important information."

    # feature loop
    - title: "Harness Native Document Features for Watermarking"
      content: "Utilize the inherent features of document formats for sophisticated watermarking. Whether it’s using native PDF annotations, MS Word backgrounds, or Excel headers and footers, GroupDocs.Watermark integrates deeply with document structures to apply watermarks that are both effective and minimally invasive."
      
  code_samples:
    # code sample loop
    - title: "Generate image watermark for DOCX"
      content: |
        This example shows how to apply image effects to the shape watermarks.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Load Word document
            var loadOptions = new WordProcessingLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.docx", loadOptions))
            {
                //  Set up watermark options
                using (ImageWatermark watermark = new ImageWatermark("logo.png"))
                {
                    WordProcessingImageEffects effects = new WordProcessingImageEffects();
                    effects.Brightness = 0.7;
                    effects.Contrast = 0.6;
                    effects.ChromaKey = Color.Red;
                    effects.BorderLineFormat.Enabled = true;
                    effects.BorderLineFormat.Weight = 1;

                    WordProcessingWatermarkSectionOptions options = new WordProcessingWatermarkSectionOptions();
                    options.Effects = effects;

                    //  Generate watermark
                    watermarker.Add(watermark, options);
                }

                //  Save updated document
                watermarker.save("result.docx");
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
    title: "Safeguard Your Photos with Effective Watermarks C#"
    exclude: "PHOTO"
    description: "Secure and stylize your photographic content with customizable watermarks using our .NET C# API, designed to integrate seamlessly and preserve image quality."
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