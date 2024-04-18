
---
############################# Static ############################
layout: "format"
date:  2024-04-18T15:29:26
draft: false
lang: en
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Delete Watermark for Presentations"
head_description: "GroupDocs.Watermark for Node.js via Java allows to generate Word Document watermarks in Node.js via Java, J2SE 7.0 (1.7) or above applications."

############################# Header ############################
title: "Delete Watermark for Document of MS Word formats with Node.js via Java" 
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
    title: "Powerpoint Watermarks Deletion using Node.js via Java"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/nodejs-java/)** furnishes Node.js via Java developers with a comprehensive API for the programmatic deletion of specific watermarks embedded within various Powerpoint documents. This guide delves into the technical process:
      
      1. Initiate the workflow by instantiating the **Watermarker** class and providing your Powerpoint file as a constructor argument. The file can be supplied as a byte stream, a file stream, or a path reference to a local disk location.
      2. To achieve precise watermark targeting, leverage the capabilities of the **SearchCriteria** object. This object facilitates the construction of intricate filters based on properties previously embedded within the document. You can utilize an image as a search parameter alongside text or formatting attributes to enable a highly granular selection process.
      3. Following the execution of the search, you'll receive a collection of identified watermarks. These watermarks may be deleted easily.
      4. Upon successful watermark deletion, persist the modified document. The API provides storage flexibility, allowing you to utilize either a local file path or a stream object for final output.
   
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

        // Delete text watermark in POWERPOINT document

        // Instantiate Watermarker with POWERPOINT document
        const watermarker = new groupdocs.watermark.Watermarker("input.pptx");
        
        // Clear text watermarks suit search conditions
        const criteria = new groupdocs.watermark.TextFormattingSearchCriteria();
        criteria.setFontBold(true);
        const watermarks = watermarker.search(criteria);
        watermarks.clear();

        // Save processed file
        watermarker.save("output.pptx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Deep dive into adding Watermark"
  description: "API to render, display, convert documents, slides, diagrams, and many other document types in .NET applications"
  image: "/img/watermark/features_remove.webp" # 500x500 px
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
    - title: "Delete PDF hyper-link watermarks"
      content: |
        This example shows how to delete all watermarks with proper hyper-link from a PDF
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Load PDF in Watermarker
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  Search for watermarks with hyper-link
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria('someurl.com');
            const watermarks = watermarker.search(searchCriteria);
  
            //  Delete selected watermarks
            for (let i = watermarks.getCount() - 1; i >= 0; i--) {
                if (watermarks.get_Item(i) instanceof groupdocsWatermark.HyperlinkPossibleWatermark) {
                    console.log(watermarks.get_Item(i).getText());
                    watermarks.removeAt(i);
                }
            }

            //  Save changes in the document
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
    title: "MS Word documents watermarking via JavaScript"
    exclude: "POWERPOINT"
    description: "Protect MS Word business documents with image or text watermarks. Involve GroupDocs.Watermark for Node.js via Java API to your business processes."
    items: 
        # format loop 1
        - name: "Watermark PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/delete//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark Word"
          format: "WORD"
          link: "/watermark/nodejs-java/delete//word/"
          description: "MS Word and Open Office documents"
          
        # format loop 3
        - name: "Watermark Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/delete//excel/"
          description: "MS Excel and Open Office spreadsheets"

        # format loop 4
        - name: "Watermark PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/delete//powerpoint/"
          description: "MS PowerPoint and Open Office presentations"

        # format loop 5
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/delete//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 6
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/delete//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 7
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/delete//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/delete//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 9
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/delete//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 10
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/delete//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 11
        - name: "Watermark RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/delete//rtf/"
          description: "Rich Text Format"

---