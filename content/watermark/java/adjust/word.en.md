
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:57
draft: false
lang: en
format: Word
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Adjust Word Watermarks Effortlessly - GroupDocs.Watermark"
head_description: "Seamlessly adjust watermarks across multiple document formats using GroupDocs.Watermark. Enhance your document security."

############################# Header ############################
title: "Adjust Word Watermarks: Effortlessly Secure" 
description: "Secure your documents effortlessly with our powerful watermark modification capabilities. Protect your content with confidence."
subtitle: "GroupDocs.Watermark for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download at Maven for free"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java"
    link: "/watermark/java/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Modify Watermarks**: GroupDocs.Watermark empowers users to modify watermarks across various document formats seamlessly. With precise control and versatile options, customize your documents with confidence.

############################# Steps ############################
steps:
    enable: true
    title: "Adjust watermarks in Word documents with Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** makes it easy for Java developers to adjust text watermarks in their applications by implementing a few easy steps:
      
      1. Load your Word file to the main object of our API called **Watermarker**. You can provide file for the further processing as stream or as a path on a local disk.
      2. Next step is locating watermarks which must be adjusted. **SearchCriteria** helps as to identify watermarks with right properties which were previously added to a document.
      3. Get list of suitable watermarks as a result of the **Search** procedure. Adjust found watermarks properties such as size, page alignment, text, color, image content, etc. There are a lot of ways to customize your data.
      4. After completion of watermarks adjustment process you need to save updated document. Use local file path, file or byte stream to store result.
   
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

        // Adjust WORD text watermark

        // Instantiate Watermarker with input WORD document
        Watermarker watermarker = new Watermarker("input.docx");

        // Initialize the TextSearchCriteria and find text watermarks
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        
        // Adjust text watermark properties
        for (PossibleWatermark watermark : watermarks)
        {
            watermark.getFormattedTextFragments().clear();
            watermark.getFormattedTextFragments().
                add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
        }

        // Save the updated document
        watermarker.save("output.docx");
        
        ```            
        
############################# More features ############################
more_features:
  enable: true
  title: "Deep dive into WORD Watermark adjustment"
  description: "Our API empowers Java applications to add, edit, remove, and search for watermarks across popular document formats."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Adjust Watermark"
  features:
    # feature loop
    - title: "Effortlessly Watermark Your Documents"
      content: "GroupDocs.Watermark simplifies watermarking for Java developers. Add diverse watermarks to various business documents and files. Not only can you apply watermarks, but you can also update or remove existing ones."

    # feature loop
    - title: "Customize Watermarks to Your Needs"
      content: "Our API provides extensive customization options. Easily adjust size, rotation, color, font, styles, and more to achieve the perfect watermark."

    # feature loop
    - title: "Use WORD Native Document Features"
      content: "Depending on the specific document format, you can utilize native functionalities. These might include document page background, annotations, headers, or other objects as watermark containers."
      
  code_samples:
    # code sample loop
    - title: "PDF adjust text watermark"
      content: |
        This example shows how to adjust the text of the particular artifacts.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Load PDF document
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Get document content
        PdfContent pdfContent = watermarker.getContent(PdfContent.class);

        //  Adjust particular watermark text
        for (PdfArtifact artifact : pdfContent.getPages().get_Item(0).getArtifacts())
        {
            if (artifact.getText().contains("Test"))
            {
                artifact.setText("Passed");
            }
        }

        //  Save the document
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
    title: "Adjust Watermarks using GroupDocs.Watermark for Java for popular formats"
    exclude: "WORD"
    description: "GroupDocs.Watermark supports seamless modification of watermarks in various formats. Tailor your watermarking strategy to meet your specific needs."
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