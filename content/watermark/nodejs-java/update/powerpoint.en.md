
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:08
draft: false
lang: en
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Update Watermarks in POWERPOINT Effortlessly"
head_description: "Efficiently update watermarks in POWERPOINT document formats using GroupDocs.Watermark for Node.js via Java. Polish your business processes."

############################# Header ############################
title: "Effortlessly Update POWERPOINT Document Watermarks" 
description: "Experience hassle-free watermark removal with GroupDocs.Watermark for Node.js via Java. Safeguard your business papers with diverse watermarks. Customize watermark dimensions, alignment, angle of rotation, and placement, and more."
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Get from NPM for free"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java API"
    link: "/watermark/nodejs-java/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java provides a user-friendly solution for managing POWERPOINT watermarks using Node.js via Java. With this tool, developers can efficiently update watermarks in various documents and file formats, including PDF, Microsoft Word, Excel, PowerPoint, Visio, and email formats. GroupDocs.Watermark supports all major operating systems and Node.js via Java versions.

############################# Steps ############################
steps:
    enable: true
    title: "Update Watermarks in POWERPOINT via Node.js via Java"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** equips Node.js via Java developers with a robust API for programmatically updating watermarks within various POWERPOINT documents. This guide outlines the process:
      
      1. Start the process by supplying your POWERPOINT file as an argument to the **Watermarker** class constructor. Depending no your demands the file can be provided as either a stream or a reference to a local disk location.
      2. Subsequently, leverage the **SearchCriteria** object to identify the specific watermarks requiring modification. This object enables the pinpointing of watermarks based on the desired properties.
      3. Upon successful execution of the search, you'll receive a collection of relevant watermarks. These watermarks offer granular control, allowing you to update properties such as dimensions, page positioning, text content, color scheme, image data, and more.
      4. Following the completion of watermark updates, persist the modified document. The API facilitates storage using either a local file path or a stream object.
   
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

        // Update POWERPOINT text watermark

        // Provide Watermarker instance for POWERPOINT file
        const watermarker = new groupdocs.watermark.Watermarker("input.pptx");

        // Use TextSearchCriteria to find text watermarks
        const searchCriteria = 
            new groupdocs.watermark.TextSearchCriteria("test", false);
        const watermarks = watermarker.search(searchCriteria);
        
        // Update text watermark
        for (const watermark of watermarks.getInnerList().toArray())
        {
            watermark.setText("passed");
        }

        // Enjoy the result
        watermarker.save("output.pptx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Mastering Watermark Editing in PDFs with GroupDocs.Watermark"
  description: "Explore comprehensive API features for adjusting and managing watermarks in PDFs within Node.js via Java applications."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Edit Watermark"
  features:
    # feature loop
    - title: "Effortlessly Edit Watermarks in PDFs"
      content: "GroupDocs.Watermark offers robust tools in Node.js via Java to seamlessly edit existing watermarks in PDF documents. Adjust position, transparency, and more with ease."

    # feature loop
    - title: "Refine Watermark Details for Precision"
      content: "Take control over the details. Our API allows you to fine-tune the appearance of watermarks, enabling precise modifications of size, opacity, and color in your PDFs."

    # feature loop
    - title: "Streamlined Watermark Management"
      content: "Our API simplifies watermark management. Whether updating or removing, you can manage watermarks efficiently, maintaining document integrity while catering to your branding needs."
      
  code_samples:
    # code sample loop
    - title: "Java Example: Edit PDF Watermark"
      content: |
        This Java example demonstrates how to edit an existing watermark in a PDF document, showcasing how to adjust its properties programmatically.
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Load the PDF document for processing
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  Search for specific watermarks that meet your criteria
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria("test", false);
            const watermarks = watermarker.search(searchCriteria);
  
            //  Edit the watermark's settings, such as size, color, and position
            for (const watermark of watermarks.getInnerList().toArray()) {
                watermark.getFormattedTextFragments().clear();
                watermark.getFormattedTextFragments().add("passed", 
                    new groupdocsWatermark.Font("Calibri", 19, groupdocsWatermark.FontStyle.Bold), 
                    groupdocsWatermark.Color.getRed(), groupdocsWatermark.Color.getAqua());
            }

            //  Save the updated document to a local system or stream it directly
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
    title: "Update Watermarks in Other File Formats"
    exclude: "POWERPOINT"
    description: "Efficiently update watermarks in PDF, Word, Excel, etc. using GroupDocs.Watermark for Node.js via Java. We support all popular business formats."
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