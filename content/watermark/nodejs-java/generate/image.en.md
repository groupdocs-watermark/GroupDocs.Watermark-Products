
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:19
draft: false
lang: en
format: Image
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Dynamic Watermarking for Images protection"
head_description: "Secure your image copyrights with Node.js dynamic watermarking. Supports JPG, PNG, WEBP and more."

############################# Header ############################
title: "Dynamic Watermarking for Image Protection with Node.js" 
description: "Use our Node.js toolkit to generate dynamic, secure watermarks to your images, supporting formats like JPG, PNG, and WEBP. Ensure your image copyrights with advanced protection features."
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
       With GroupDocs.Watermark for Node.js via Java, applying watermarks to images is straightforward and customizable. This toolkit supports a wide range of image formats, including traditional raster images like JPG and PNG, as well as newer formats like WEBP. It allows developers to dynamically add watermarks that are not only secure but also blend naturally with the image content, providing robust protection against copyright infringement without detracting from the image's original appeal.

############################# Steps ############################
steps:
    enable: true
    title: "Secure Business Documents: Generate Watermarks for Image Formats"
    content: |
      Boost Your Document Security with **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/):** Inject our API to your applications and generate watermarks for many supported file formats.
      
      1. **Initiate Watermarking:** Start document processing with the **Watermarker** class providing our main features. Instantiate it by passing to the constructor the Image file which is supposed to be secured by generated watermarks.
      2. **Create main Watermark object:** Elevate your documents by sculpting bespoke **Watermark** objects. Beyond mere pages, they seamlessly integrate into native elements like attachments or headers, adding layers of security and professionalism.
      3. **Refine Watermark Attributes:** Fine-tune your watermarks with precision, adjusting dimensions, alignment, and color schemes. Every detail enhances document integrity, making your files unmistakably yours.
      4. **Implement with Precision:** Utilize the **Watermarker** method to apply your customized watermarks flawlessly. Whether singular or multiple, each watermark adds an extra layer of protection. For added security, consider storing your processed documents in a separate, secure location.
   
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

        // Generate text watermark for IMAGE

        // Pass source file to Watermarker instance
        const watermarker = new groupdocs.watermark.Watermarker("input.jpeg");
        
        // Generate text watermark and set its options
        const  watermark = new groupdocs.watermark.TextWatermark
            ("My Watermark", groupdocs.watermark.new Font("Arial", 36));

        // Obtain IMAGE result
        watermarker.add(watermark);
        watermarker.save("output.jpeg");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Advanced Watermarking Techniques"
  description: "Discover cutting-edge watermarking techniques with our robust API, designed to integrate seamlessly into .NET environments. Perfect for adding sophisticated and secure watermarks to a diverse array of document types including presentations, legal documents, and technical diagrams."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Sophisticated Watermark"
  features:
    # feature loop
    - title: "Dynamic Watermark Placement"
      content: "Our API offers dynamic placement options that adapt watermark positioning based on document content. Ideal for complex layouts in presentations and technical diagrams, this feature ensures that watermarks are always optimally placed without interfering with the readability of underlying information."

    # feature loop
    - title: "Enhanced Security with Invisible Watermarks"
      content: "Implement invisible watermarks that offer robust protection without altering the appearance of your documents. These watermarks are designed to be detected only through specific software tools, making them perfect for protecting sensitive information in legal and financial documents."

    # feature loop
    - title: "Automated Watermarking Workflows"
      content: "Streamline your document security processes with automated watermarking workflows. Configure rules based on document type, content sensitivity, and user access levels to apply watermarks automatically, ensuring consistent security protocols are maintained across all documents."
      
  code_samples:
    # code sample loop
    - title: "Generate watermark for PDF attachments"
      content: |
        This example shows how to generate watermarks in all PDF attachments
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Load PDF document
            const loadOptions = new groupdocsWatermark.PdfLoadOptions();
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf", loadOptions);
            const pdfContent = watermarker.getContent(groupdocsWatermark.PdfContent.class);

            //  Generate text watermark
            const watermark = new groupdocsWatermark.TextWatermark('WaterMark', new groupdocsWatermark.Font('Arial', 19));
  
            //  Add watermark to suitable attachments
            for (const attachment of pdfContent.getAttachments().getInnerList().toArray()) {
                const info = attachment.getDocumentInfo();
                if (info.getFileType() !== groupdocsWatermark.FileType.Unknown && !info.isEncrypted()) {
                    const attachedWatermarker = attachment.createWatermarker();
                    attachedWatermarker.add(watermark);
                    attachment.updateContent(attachedWatermarker);
                    attachedWatermarker.close();
                }
            }

            //  Save processed PDF
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
    title: "Implementing amazing Watermarks in Images via JavaScript"
    exclude: "IMAGE"
    description: "Protect your image copyrights effectively with our Node.js API. Dynamically add watermarks to JPG, PNG, and WEBP files, ensuring each image is marked for its rightful owner."
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