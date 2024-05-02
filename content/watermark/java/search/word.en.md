
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:26:58
draft: false
lang: en
format: Word
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Power of Word Documents Watermark Search"
head_description: "Experience the unparalleled ability to search and manage watermarks across diverse document types with GroupDocs.Watermark for Java."

############################# Header ############################
title: "Discover Advanced Word Watermark Search" 
description: "Embark on a journey to explore the cutting-edge watermark search features offered by GroupDocs.Watermark for Java."
subtitle: "GroupDocs.Watermark for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Get from Maven"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Watermark for Java"
    link: "/watermark/java/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java provides a robust solution for managing watermarks using Java. Developers can effortlessly create, edit, search, and remove watermarks from documents in popular file formats. It supports both text and image watermarks across various document types, including PDF, Microsoft Word, Excel, PowerPoint, Visio, email, and image formats. GroupDocs.Watermark for Java seamlessly integrates with all major operating systems and Java versions.

############################# Steps ############################
steps:
    enable: true
    title: "Search for watermarks in Word files using Java"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/)** makes it easy to search for watermarks already placed in business documents. Download our package and involve it into your Java application to take advantage of its benefits.
      
      1. In order to use our library features you need to load Word file to the **Watermarker** class instance. It is possible to provide just a file path, file stream or a byte stream.
      2. To narrow list of possible watermarks use **SearchCriteria** object. Provide image as an example to get similar image watermark. If you want to search for textual watermark provide text, font, color and other options.
      3. To get watermarks placed in the document use method **Search** of the **Watermarker** object. You will be provided with collection of objects which may be processed as watermarks.
      4. Finally, you are free to do with result of search whatever you want. It is completely possible, to delete found watermarks or edit their properties. Change size or text, for example.
   
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

        // Search text watermarks in WORD document

        // Get Watermarker instance for WORD document
        Watermarker watermarker = new Watermarker("input.docx");

        // Search watermarks by criteria
        ImageSearchCriteria imageSearchCriteria = new ImageDctHashSearchCriteria("watermark.jpeg");
        imageSearchCriteria.setMaxDifference(0.9);
        PossibleWatermarkCollection possibleWatermarks = watermarker.search(imageSearchCriteria);

        // Process watermarks
        System.out.println("Found " + possibleWatermarks.getCount() + " possible watermark(s).");
        
        ```   
        
############################# More features ############################
more_features:
  enable: true
  title: "Harness Java for Advanced Watermark Search with GroupDocs.Watermark"
  description: "Utilize GroupDocs.Watermark Java API to perform sophisticated searches for watermarks in documents across diverse formats in the Java."
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "Advanced Watermark Search"
  features:
    # feature loop
    - title: "Java-Enhanced Watermark Search Techniques"
      content: "Empower your Java applications with advanced search techniques using GroupDocs.Watermark. Our API enables deep searches for embedded watermarks across various document types, offering precision and efficiency."

    # feature loop
    - title: "Identify Watermarks with Custom Java Queries"
      content: "Customize your Java queries to detect watermarks more effectively. Use GroupDocs.Watermark to sort and filter watermarks by properties like transparency, embedding method, and text or image content."

    # feature loop
    - title: "Efficient Management of Document Watermarks"
      content: "Streamline the management of watermarks in your Java applications. With GroupDocs.Watermark, quickly find, review, and analyze watermarks to ensure document integrity and compliance with branding guidelines."
      
  code_samples:
    # code sample loop
    - title: "Java Code Example: Intelligent Watermark Search"
      content: |
        Learn how to implement an intelligent watermark search using Java with GroupDocs.Watermark, demonstrating the API's ability to handle complex search operations and result management.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Set up the Java environment and load documents from various sources
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Define advanced search parameters to locate specific types of watermarks
        TextSearchCriteria textSearchCriteria = new TextSearchCriteria("Company Name");

        //  Execute the search and process the found watermarks for detailed review
        RotateAngleSearchCriteria rotateAngleSearchCriteria = new RotateAngleSearchCriteria(30, 60);
        SearchCriteria combinedSearchCriteria = imageSearchCriteria.or(textSearchCriteria)
                                                                   .and(rotateAngleSearchCriteria);

        //  Save or update the document based on the watermark search results
        PossibleWatermarkCollection possibleWatermarks = watermarker.search(combinedSearchCriteria);
        System.out.println("Found " + possibleWatermarks.getCount() + " possible watermark(s).");
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
    title: "Master Watermark Search Across Formats"
    exclude: "WORD"
    description: "Unlock the potential of GroupDocs.Watermark for Java to search and manipulate watermarks in different supported file formats."
    items: 
        # format loop 1
        - name: "Watermark PDF"
          format: "PDF"
          link: "/watermark/java/search//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark Word"
          format: "WORD"
          link: "/watermark/java/search//word/"
          description: "MS Word and Open Office documents"
          
        # format loop 3
        - name: "Watermark Excel"
          format: "EXCEL"
          link: "/watermark/java/search//excel/"
          description: "MS Excel and Open Office spreadsheets"

        # format loop 4
        - name: "Watermark PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/search//powerpoint/"
          description: "MS PowerPoint and Open Office presentations"

        # format loop 5
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/java/search//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 6
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/java/search//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 7
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/java/search//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/java/search//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 9
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/java/search//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 10
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/java/search//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 11
        - name: "Watermark RTF"
          format: "RTF"
          link: "/watermark/java/search//rtf/"
          description: "Rich Text Format"

---