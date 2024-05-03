
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
head_title: "Node.js via Java API for Powerpoint Watermark Removal"
head_description: "Enhance presentation clarity by seamlessly removing watermarks from Powerpoint slides with our Node.js via Java API."

############################# Header ############################
title: "Node.js via Java Powerpoint Watermark Control" 
description: "Use the GroupDocs.Watermark for Node.js via Java API to effectively clear watermarks from Powerpoint presentations, ensuring unobstructed and professional slide visuals."
subtitle: "GroupDocs.Watermark for Node.js via Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Free NPM download"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java library"
    link: "/watermark/nodejs-java/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       The GroupDocs.Watermark for Node.js via Java library enables developers to easily remove and manage watermarks in Powerpoint files. This robust tool supports precise control over text and image watermarks, allowing for the maintenance of high-quality presentations in business and educational environments.

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

        // Delete text watermark in Powerpoint document

        // Instantiate Watermarker with Powerpoint document
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
  title: "Node.js via Java API for Efficient Watermark Removal"
  description: "Leverage our Node.js via Java API to seamlessly remove or clear watermarks from a variety of document formats including PDFs and Office files. Designed for developers, this API integrates effortlessly with your Node.js via Java applications, ensuring clean and clear documents."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "Remove Watermark"
  features:
    # feature loop
    - title: "Node.js via Java Watermark Removal"
      content: "Use our Node.js via Java API to remove watermarks with precision and ease. Perfect for applications requiring unmarked documents for presentation or further processing."

    # feature loop
    - title: "Batch Watermark removal processing"
      content: "Efficiently handle multiple documents with our bulk watermark removal feature. Save time and server resources by processing large batches of files simultaneously in your Node.js via Java applications."

    # feature loop
    - title: "Edit out and Delete Watermarks Flexibly"
      content: "Our API allows for flexible editing and deletion of watermark elements, catering to various business needs and document types. Adapt your documents to maintain a professional appearance while ensuring content integrity."
      
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
    title: "Optimizing Powerpoint Slides with Node.js via Java"
    exclude: "POWERPOINT"
    description: "Discover how the GroupDocs.Watermark for Node.js via Java API can streamline the process of removing watermarks from Powerpoint slides, facilitating clearer and more impactful presentations."
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