
---
############################# Static ############################
layout: "format"
date:  2024-04-18T15:29:29
draft: false
lang: en
format: Rtf
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Update RTF Document Watermark"
head_description: "GroupDocs.Watermark for Node.js via Java allows to generate Word Document watermarks in Node.js via Java, J2SE 7.0 (1.7) or above applications."

############################# Header ############################
title: "Update Watermark for Document of MS Word formats with Node.js via Java" 
description: "Text and image watermark generation for MS Excel files using Node.js via Java J2SE applications. Watermarks your business documents with BMP, PNG, GIF, and JPEG images or text. Adjust watermark size, alignment, rotation angle, and position on the document pages."
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
       GroupDocs.Watermark for Node.js via Java is designed for generation various Word watermarks using Node.js via Java. Our solution may enrich Node.js via Java apps by performing generation, adjusting, search, and clearing various watermarks in Word documents. GroupDocs.Watermark available for many operating systems and Node.js via Java J2SE 7.0 (1.7), J2SE 8.0 (1.8) or above.

############################# Steps ############################
steps:
    enable: true
    title: "Dynamic Watermark Edit for Rtf in Node.js via Java"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** offers Node.js via Java developers a powerful API for editing watermarks across diverse Rtf documents. Here's a comprehensive guide to streamline your workflow:
      
      1. **Start the Process:** Begin by providing your Rtf file as an argument to the **Watermarker** class constructor. Depending on your requirements, the file can be sourced either as a stream or from a local disk location.
      2. **Pinpoint Watermarks:** Use the **SearchCriteria** object to identify the watermarks in need of modification. This versatile tool enables targeted watermark selection based on specific properties.
      3. **Refine with Precision:** Upon successful execution of the search, gain access to a collection of relevant watermarks. Enjoy granular control over each element, with the ability to update dimensions, page positioning, text content, color, image data, and more.
      4. **Seamless Persistence:** Once watermark updates are complete, securely store the modified document. The API offers flexible storage options, allowing you to save to a local file path or as a stream object.
   
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

        // Update image RTF watermark

        // Compose Watermarker for RTF file
        const watermarker = new groupdocs.watermark.Watermarker("input.rtf");

        // Use SearchCriteria to find a particular image
        const searchCriteria = 
            new groupdocs.watermark.ImageDctHashSearchCriteria("logo.png");
        const watermarks = watermarker.search(searchCriteria);
        
        // Update image content
        for (const watermark of watermarks.getInnerList().toArray())
        {
            watermark.setImageData(imageData);
        }

        // Save updated file
        watermarker.save("output.rtf");
        
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
      content: "GroupDocs.Watermark makes it easy for Node.js via Java developers to add various types of watermarks in popular business documents and files."

    # feature loop
    - title: "Customize watermarks for your goals."
      content: "Our solution supports many watermark features. You can easily adjust size, rotation, color, font, font styles and other options to make watermark looks perfect."

    # feature loop
    - title: "Use native document objects"
      content: "Accordingly do particular document format it is possible to use native document features. Native PDF annotations or MS Word page watermark may be used for watermarking."
      
  code_samples:
    # code sample loop
    - title: "Update Presentation watermark content"
      content: |
        This example shows how to update text content of Presentation watermarks
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Load a presentation for processing
            const watermarker = new groupdocsWatermark.Watermarker("source.pptx");

            //  Get list of appropriate watermarks using search
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria("denied", false);
            const watermarks = watermarker.search(searchCriteria);
  
            //  Update watermark text
            for (const watermark of watermarks.getInnerList().toArray()) {
                watermark.setText("accepted");
            }

            //  Save updated presentation to local disk or stream
            watermarker.save("result.pptx");
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
    title: "MS Word documents watermarking via JavaScript"
    exclude: "RTF"
    description: "Protect MS Word business documents with image or text watermarks. Involve GroupDocs.Watermark for Node.js via Java API to your business processes."
    items: 
        # format loop 1
        - name: "Watermark PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/update//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark Word"
          format: "WORD"
          link: "/watermark/nodejs-java/update//word/"
          description: "MS Word and Open Office documents"
          
        # format loop 3
        - name: "Watermark Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/update//excel/"
          description: "MS Excel and Open Office spreadsheets"

        # format loop 4
        - name: "Watermark PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/update//powerpoint/"
          description: "MS PowerPoint and Open Office presentations"

        # format loop 5
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/update//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 6
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/update//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 7
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/update//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/update//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 9
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/update//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 10
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/update//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 11
        - name: "Watermark RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/update//rtf/"
          description: "Rich Text Format"

---