
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:10
draft: false
lang: en
format: Pdf
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Adjust Watermarks in PDF - GroupDocs.Watermark"
head_description: "Adjust and refine watermarks across different document types effortlessly with GroupDocs.Watermark. Ensure document credibility."

############################# Header ############################
title: "Adjust PDF Watermarks: Versatile Protection" 
description: "Protect your content across various formats with our versatile watermark adjustment features. Adapt to your needs seamlessly."
subtitle: "GroupDocs.Watermark for Java Solution" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Free Maven package"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java Solution"
    link: "/watermark/java/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Adjust Watermarks**: Protect your content across diverse document formats with our versatile watermark adjustment features. Tailor your watermarking strategy to meet your specific requirements with ease.

############################# Steps ############################
steps:
    enable: true
    title: "Adjust Pdf document watermarks using Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** allows Java developers to easily adjust watermarks in many documents using their applications. Here's a quick guide:
      
      1. Firstly, you need to pass Pdf file as parameter of the **Watermarker** class constructor. Provide byte or file stream or a local disk path.
      2. Secondly, locate the watermarks that need to be adjusted. Use **SearchCriteria** to identify watermarks with the specific properties previously added to the document.
      3. Following the search, you'll receive a list of relevant watermarks. You can then adjust their properties, including size, page alignment, text, color, image content, and more. This offers a high degree of customization for your data.
      4. Once you've finished adjusting the watermarks, save the updated document. You can use a local file path, or stream to store the result.
   
    code:
      platform: "net"
      copy_title: "Copy"
      install:
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-watermark</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/watermark/java/"
          
      content: |
        ```java {style=abap}
        // Adjust PDF image watermark

        // Instantiate Watermarker with PDF
        Watermarker watermarker = new Watermarker("input.pdf");
        
        // Initialize the SearchCriteria to match a particular image
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);

        for (PossibleWatermark watermark : watermarks)
        {
            // Replace image which was found
            watermark.setImageData(imageData);
        }

        // Save adjusted file
        watermarker.save("output.pdf");
        
        ```
        
############################# More features ############################
more_features:
  enable: true
  title: "Advanced PDF Watermark Management for Java Applications"
  description: "The GroupDocs.Watermark API empowers developers to seamlessly integrate watermarking functionality into their Java applications. It supports adding, editing, removing, and searching for watermarks across a wide range of document formats."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Watermark Adjustment"
  features:
    # feature loop
    - title: "Effortless Watermark Integration"
      content: "GroupDocs.Watermark simplifies the process of adding diverse watermarks to various business documents and files within Java applications. Developers can not only apply watermarks, but also update or remove existing ones programmatically."

    # feature loop
    - title: "Granular Watermark Customization"
      content: "The API provides extensive customization options for watermarks. Developers can easily adjust size, rotation, color, font, styles, and other properties to achieve the desired visual effect."

    # feature loop
    - title: "Leveraging PDF Native Document Features"
      content: "Depending on the target document format, developers can utilize native functionalities for watermark placement. These functionalities might include document page background, annotations, headers, or other objects as watermark containers."
      
  code_samples:
    # code sample loop
    - title: "Adjust image watermark in Spreadsheets"
      content: |
        This examples shows how to adjust the image of the particular shapes in an Excel Worksheet.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Load document as Spreadsheet
        SpreadsheetLoadOptions loadOptions = new SpreadsheetLoadOptions();
        Watermarker watermarker = new Watermarker("source.xlsx", loadOptions);

        //  Get new watermark bytes
        File file = new File("new_watermark.png");
        byte[] imageBytes = new byte[(int) file.length()];
        FileInputStream inputStream = new FileInputStream(file);
        inputStream.read(imageBytes);
        inputStream.close();

        //  Adjust content of particular watermark
        for (SpreadsheetShape shape : content.getWorksheets().get_Item(0).getShapes())
        {
            if (shape.getImage() != null)
            {
                shape.setImage(new SpreadsheetWatermarkableImage(imageBytes));
            }
        }

        //  Save result document
        watermarker.save("result.xlsx");
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
    - title: "Maven download"
      link: "https://releases.groupdocs.com/watermark/java/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/watermark/java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Manage Watermarks in popular formats with GroupDocs.Watermark for Java"
    exclude: "PDF"
    description: "Protect your content across various formats with our versatile watermark adjustment features. Adapt to your needs seamlessly."
    items: 
        # format loop 1
        - name: "Watermark PDF"
          format: "PDF"
          link: "/watermark/java/adjust//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark Word"
          format: "WORD"
          link: "/watermark/java/adjust//word/"
          description: "MS Word and Open Office documents"
          
        # format loop 3
        - name: "Watermark Excel"
          format: "EXCEL"
          link: "/watermark/java/adjust//excel/"
          description: "MS Excel and Open Office spreadsheets"

        # format loop 4
        - name: "Watermark PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/adjust//powerpoint/"
          description: "MS PowerPoint and Open Office presentations"

        # format loop 5
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/java/adjust//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 6
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/java/adjust//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 7
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/java/adjust//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/java/adjust//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 9
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/java/adjust//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 10
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/java/adjust//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 11
        - name: "Watermark RTF"
          format: "RTF"
          link: "/watermark/java/adjust//rtf/"
          description: "Rich Text Format"

---