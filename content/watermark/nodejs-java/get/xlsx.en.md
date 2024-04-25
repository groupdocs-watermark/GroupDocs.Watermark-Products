
---
############################# Static ############################
layout: "format"
date:  2024-04-25T17:42:49
draft: false
lang: en
format: Xlsx
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Efficient XLSX Spreadsheets Watermark Handling"
head_description: "Efficiently handle watermarks in documents with GroupDocs.Watermark for Node.js via Java."

############################# Header ############################
title: "Streamlined Watermark Control in XLSX Spreadsheets" 
description: "Take control of watermarks efficiently using GroupDocs.Watermark for Node.js via Java streamlined approach."
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download NPM package"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Base GroupDocs.Watermark for Node.js via Java Information"
    link: "/watermark/nodejs-java/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java provides a streamlined solution for managing watermarks across Node.js via Java. Simplify the process of watermark handling across various file formats.

############################# Steps ############################
steps:
    enable: true
    title: "Get Watermarks from Xlsx Files Using GroupDocs.Watermark"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** offers a comprehensive solution for getting watermarks placed in popular business document formats. By integrating our library into your Node.js via Java applications, you can equip them with powerful watermark searching capabilities.
      
      1. To access the functionalities provided by GroupDocs.Watermark, instantiate the **Watermarker** class and provide the Xlsx file path. Also you can use file saved as byte stream. This action essentially loads the target document for comprehensive watermark analysis.
      2. To achieve targeted watermark identification, create the **SearchCriteria** object. You can specify an image for locating similar image watermarks. Alternatively, for textual watermarks, define the text content, font properties, color attributes, and other relevant parameters to refine the search criteria and achieve more precise results.
      3. Call the **Get** method (or a similar naming convention) of the **Watermarker** object to start the watermark getting process within the loaded document. This function returns a collection of objects representing potential watermarks, facilitating further processing based on your specific requirements.
      4. The result collection of watermarks allows you to control over the watermarks identified within the document. You can remove unwanted watermarks or dynamically modify their properties, such as adjusting their size, position, or text content, to suit your needs.
   
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

        // Get image watermarks placed in XLSX

        // Create Watermarker object with source path
        const watermarker = new groupdocs.watermark.Watermarker("input.xlsx");
        
        // Get watermarks by similar image hash
        const imageSearchCriteria = 
            new groupdocs.watermark.ImageDctHashSearchCriteria("watermark.jpg");
        imageSearchCriteria.setMaxDifference(0.9);
        const possibleWatermarks = watermarker.search(imageSearchCriteria);

        // Process watermarks as you wish
        console.log(`Found ${possibleWatermarks.getCount()} possible watermark(s).`);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Deep dive into adding Watermark"
  description: "API to render, display, convert documents, slides, diagrams, and many other document types in .NET applications"
  image: "/img/watermark/features_search.webp" # 500x500 px
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
    - title: "Get various file format watermarks"
      content: |
        This example shows us how to get watermarks from different documents 
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            const files = ["source.docx", "source.xlsx", "source.pptx", "source.vsdx"];
            for (const file of files) {
                //  Create search settings for required document types
                const settings = new groupdocsWatermark.WatermarkerSettings();
                settings.setSearchableObjects(new groupdocsWatermark.SearchableObjects());
                settings.getSearchableObjects().setWordProcessingSearchableObjects(
                    groupdocsWatermark.WordProcessingSearchableObjects.Hyperlinks | 
                    groupdocsWatermark.WordProcessingSearchableObjects.Text
                );
                settings.getSearchableObjects().setSpreadsheetSearchableObjects(
                    groupdocsWatermark.SpreadsheetSearchableObjects.HeadersFooters
                );
                settings.getSearchableObjects().setPresentationSearchableObjects(
                    groupdocsWatermark.PresentationSearchableObjects.SlidesBackgrounds |
                    groupdocsWatermark.PresentationSearchableObjects.Shapes
                );
                settings.getSearchableObjects().setDiagramSearchableObjects(groupdocsWatermark.DiagramSearchableObjects.None);
                settings.getSearchableObjects().setPdfSearchableObjects(groupdocsWatermark.PdfSearchableObjects.All);

                //  Create Watermarker for current file
                const watermarker = new groupdocsWatermark.Watermarker(file, settings);

                //  Get watermarks from the file
                const watermarks = watermarker.search();

                //  Process list of watermarks
                console.log(`In ${documentPath} found ${watermarks.getCount()} possible watermark(s).`);
                watermarker.close();
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
    title: "Streamline Watermark Control"
    exclude: "XLSX"
    description: "Streamline watermark control across different file formats with GroupDocs.Watermark for Node.js via Java."
    items: 
        # format loop 1
        - name: "Watermark PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/get//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark Word"
          format: "WORD"
          link: "/watermark/nodejs-java/get//word/"
          description: "MS Word and Open Office documents"
          
        # format loop 3
        - name: "Watermark Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/get//excel/"
          description: "MS Excel and Open Office spreadsheets"

        # format loop 4
        - name: "Watermark PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/get//powerpoint/"
          description: "MS PowerPoint and Open Office presentations"

        # format loop 5
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/get//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 6
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/get//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 7
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/get//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/get//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 9
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/get//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 10
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/get//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 11
        - name: "Watermark RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/get//rtf/"
          description: "Rich Text Format"

---