
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:26
draft: false
lang: en
format: Jpg
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Add Watermarks to JPG with Node.js"
head_description: "Use Node.js to seamlessly integrate watermarks into JPG images, enhancing copyright security."

############################# Header ############################
title: "Create Watermarks for JPG Files via Node.js" 
description: "Implement Node.js to generate custom watermarks in JPG files, protecting your images from misuse and copyright breaches."
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download at NPM for free"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java enables Node.js developers to efficiently compose and apply watermarks on JPG images. This API facilitates the insertion of watermarks that are tailored to the content's needs, whether for personal use or professional display. Developers can customize watermark features including opacity, size, and placement to ensure they are effective yet unobtrusive. Ideal for securing photographic content, digital artwork, and other media assets against unauthorized reproduction, GroupDocs.Watermark provides robust protection capabilities within a Node.js environment, ensuring that your intellectual property is both safe and visually intact.

############################# Steps ############################
steps:
    enable: true
    title: "Protect Business Documents: Generate Jpg Watermarks"
    content: |
      Strengthen Document Security with **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/):** - A Powerful Watermark Generation Solution for Node.js via Java.
      
      1. **Streamline Secure Watermarking in Your Node.js via Java Applications:** The **Watermarker** class acts as the core component of the GroupDocs.Watermark API. This library simplifies watermarks generation various document formats, including Jpg. To get started, create a Watermarker instance before processing your document. Provide the Jpg file path or a stream object to the constructor during initialization.
      2. **Generate Watermarks for Enhanced Protection:** Empower watermarks that perfectly align with your security needs. Construct a **Watermark** object specifying the desired type. Unlike traditional page placement, you can embed watermarks within native document elements like headers or attachments, fortifying document security and adding a professional touch.
      3. **Fine-Tune Watermark Appearance for Optimal Impact:** Control the visual aspects of your watermarks. Customize properties such as height, width, alignment (top, left, center, etc.), font families, and colors to achieve a visually effective and consistent outcome that reinforces document legitimacy.
      4. **Watermark Application and Secure Storage**: Incorporate your watermarks using the **Watermarker** method. The library allows you to add multiple watermarks if necessary for enhanced protection. It's recommended to save the modified Jpg document to a separate, secure location to preserve the original file and safeguard your watermarked documents.
   
    code:
      platform: "net"
      copy_title: "Copy"
      install:
        command: "npm i @groupdocs/groupdocs.watermark"
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/watermark/nodejs-java/"
          
      content: |
        ```javascript {style=abap}

        // Generate image watermark for JPG

        // Instantiate Watermarker passing source file
        const watermarker = new groupdocs.watermark.Watermarker("input.jpg");
        
        // Generate watermark by providing image file
        const watermark = new groupdocs.watermark.ImageWatermark("watermark.png");

        // Get JPG result
        watermarker.add(watermark);
        watermarker.save("output.jpg");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Refined Watermark Integration"
  description: "Our GroupDocs.Watermark API for .NET developers offers refined solutions for integrating watermarks seamlessly into any document. This tool is designed to create sophisticated, unobtrusive watermarks that ensure copyright protection while maintaining document aesthetics."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Precision Watermark Integration"
  features:
    # feature loop
    - title: "Gradient Watermark Effects"
      content: "Implement gradient watermarks that blend smoothly across your documents. This feature allows for linear or radial gradients, adding a modern look to security features that enhances both protection and visual engagement without overpowering the content."

    # feature loop
    - title: "Pattern Watermarks for Extra Security"
      content: "Use pattern-based watermarking to add an extra layer of security. Our API supports various patterns that can be intricately designed and repeated across the document, making the watermark more resistant to tampering and removal."

    # feature loop
    - title: "Document-Specific Watermarking"
      content: "Tailor watermarks uniquely for different document types. Whether it's legal contracts, business plans, or scientific reports, customize watermarks to suit the document’s purpose and reader accessibility, ensuring optimal integration and security."
      
  code_samples:
    # code sample loop
    - title: "Generate PDF image watermark"
      content: |
        Generate image watermarks for all images presented inside a PDF document
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Load document as PDF
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  Create watermark based on PDF annotation
            const imageWatermark = new groupdocsWatermark.ImageWatermark("watermark.jpg");
            imageWatermark.setHorizontalAlignment(groupdocsWatermark.HorizontalAlignment.Center);
            imageWatermark.setVerticalAlignment(groupdocsWatermark.VerticalAlignment.Center);
            imageWatermark.setRotateAngle(-45);
            imageWatermark.setSizingType(groupdocsWatermark.SizingType.ScaleToParentDimensions);
            imageWatermark.setScaleFactor(1);
  
            //  Set up watermark options
            const images = watermarker.getImages();
            for (let i = 0; i < images.getCount(); i++) {
                if (images.get_Item(i).getWidth() > 100 && images.get_Item(i).getHeight() > 100) {
                    images.get_Item(i).add(imageWatermark);
                }
            }

            //  Add text watermark to result document
            watermarker.save("result.pdf");
            watermarker.close();

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Watermark features for free or request a license"
  items:
    #  loop
    - title: "NPM download"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Secure JPG Images with Node.js Watermarks"
    exclude: "JPG"
    description: "Utilize Node.js to embed watermarks that safeguard your JPG images, maintaining their original quality while ensuring copyright protection."
    items: 
        # format loop 1
        - name: "Watermark PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/generate//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark Word"
          format: "WORD"
          link: "/watermark/nodejs-java/generate//word/"
          description: "MS Word and Open Office documents"
          
        # format loop 3
        - name: "Watermark Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/generate//excel/"
          description: "MS Excel and Open Office spreadsheets"

        # format loop 4
        - name: "Watermark Image"
          format: "IMAGE"
          link: "/watermark/nodejs-java/generate//image/"
          description: "Popular image formats"

        # format loop 5
        - name: "Watermark Photo"
          format: "PHOTO"
          link: "/watermark/nodejs-java/generate//photo/"
          description: "Photo formats"

        # format loop 6
        - name: "Watermark PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/generate//powerpoint/"
          description: "MS PowerPoint and Open Office presentations"

        # format loop 7
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/generate//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 8
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/generate//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 9
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/generate//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 10
        - name: "Watermark JPEG"
          format: "JPEG"
          link: "/watermark/nodejs-java/generate//jpeg/"
          description: "JPEG Image"

        # format loop 11
        - name: "Watermark PNG"
          format: "PNG"
          link: "/watermark/nodejs-java/generate//png/"
          description: "Portable Network Graphic"

        # format loop 12
        - name: "Watermark TIFF"
          format: "TIFF"
          link: "/watermark/nodejs-java/generate//tiff/"
          description: "Tag Image File Format"

        # format loop 13
        - name: "Watermark WEBP"
          format: "WEBP"
          link: "/watermark/nodejs-java/generate//webp/"
          description: "WEB Picture"

        # format loop 14
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/generate//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 15
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/generate//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 16
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/generate//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 17
        - name: "Watermark RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/generate//rtf/"
          description: "Rich Text Format"

---