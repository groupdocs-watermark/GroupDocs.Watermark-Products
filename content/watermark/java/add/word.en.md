
---
############################# Static ############################
layout: "format"
date:  2024-04-26T10:23:25
draft: false
lang: en
format: Word
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Compose Tailored Watermarks for Word with Java"
head_description: "Integrate custom watermarks in Word documents using Java. Enhance security and add a professional touch."

############################# Header ############################
title: "Create Custom Watermarks in Word Documents" 
description: "Secure your Word files with Java by embedding tailored text or image watermarks. This resource is ideal for those needing to enhance document security and visual appeal with minimal effort."
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
       GroupDocs.Watermark for Java enables precise and flexible watermark creation in Word documents. This tool empowers Java developers to add customized watermarks that can include text, images, or logos, tailored to your specific branding needs. It supports all major Word document formats and provides comprehensive features for editing and removing watermarks, as well as searching through documents to verify watermark integrity. Compatible with all Java-supported operating systems, this API is perfect for businesses looking to reinforce their document security protocols.

############################# Steps ############################
steps:
    enable: true
    title: "Add Watermark to Word Document via Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** makes it easy for Java developers to add watermarks of various types to popular business file formats. Add our library to your application and watermark documents in a few easy steps as listed below.
      
      1. The main class of our API is **Watermarker**. You need to instantiate it before document processing. Do not forget to pass the Word file to the constructor as a path or a stream object.
      2. The next step is constructing a **Watermark** object of the desired type. It can be placed not only on a specific document page but also in native document parts like attachments or headers.
      3. Set watermark properties such as height and width, page alignment (top, left, central, etc.), font family and color, and many others.
      4. Call the **Watermarker** method to add a new watermark. You can add as many watermarks as you need. It is recommended to save the processed document to another location.
   
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

        // Add text watermark to WORD

        // Pass file to be watermarked to Watermarker
        Watermarker watermarker = new Watermarker("input.docx");
        
        // Create text watermark and set up properties
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        watermark.setForegroundColor(Color.getRed());

        // Save watermarked file
        watermarker.add(watermark);
        watermarker.save("output.docx");
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Enhance Your Watermarks Easily"
  description: "Harness the power of GroupDocs.Watermark to generate, compose, and add watermarks across multiple document formats. This API not only enhances document security but also protects your intellectual property by embedding customizable watermarks that are both versatile and robust."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Add Watermark"
  features:
    # feature loop
    - title: "Versatile Watermark Options."
      content: "Explore a wide range of watermarking options with GroupDocs.Watermark. From adjusting opacity and rotation to scaling size proportionally, our API lets you customize watermarks precisely to your needs, ensuring that they blend seamlessly with your documents while maintaining content integrity."

    # feature loop
    - title: "Advanced Watermark Styling."
      content: "GroupDocs.Watermark allows you to style your watermarks with various fonts, colors, and shadows, making them distinctive and harder to remove. Enhance the aesthetic appeal of your protected documents and images with stylish watermarks that reflect your brand's identity and professionalism."

    # feature loop
    - title: "Watermark Tiling & Positioning"
      content: "With GroupDocs.Watermark, implement tiling effects to cover your entire document, ensuring complete protection. Position watermarks exactly where you need them—center, corner, or custom locations. Our flexible positioning options help safeguard your documents against unauthorized use and duplication."
      
  code_samples:
    # code sample loop
    - title: "PDF annotation watermark"
      content: |
        This example shows how to add watermark annotation to a PDF document
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Load document as PDF
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Create watermark based on PDF annotation
        PdfAnnotationWatermarkOptions options = new PdfAnnotationWatermarkOptions();
        TextWatermark textWatermark = new TextWatermark("Annotation watermark", new Font("Arial", 8));

        //  Set up watermark options
        textWatermark.setHorizontalAlignment(HorizontalAlignment.Left);
        textWatermark.setVerticalAlignment(VerticalAlignment.Top);

        //  Add text watermark to result document
        watermarker.add(textWatermark, options);
        watermarker.save("result.pdf");

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
    title: "Personalize Your MS Word Files with Java Watermarks generation."
    exclude: "WORD"
    description: "GroupDocs.Watermark for Java allows developers to easily insert tailored text or image watermarks into Word documents. These enhancements not only boost document security but also enrich business communications with a professional touch."
    items: 
        # format loop 1
        - name: "Watermark PDF"
          format: "PDF"
          link: "/watermark/java/add//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark Word"
          format: "WORD"
          link: "/watermark/java/add//word/"
          description: "MS Word and Open Office documents"
          
        # format loop 3
        - name: "Watermark Excel"
          format: "EXCEL"
          link: "/watermark/java/add//excel/"
          description: "MS Excel and Open Office spreadsheets"

        # format loop 4
        - name: "Watermark Image"
          format: "IMAGE"
          link: "/watermark/java/add//image/"
          description: "Popular image formats"

        # format loop 5
        - name: "Watermark Photo"
          format: "PHOTO"
          link: "/watermark/java/add//photo/"
          description: "Photo formats"

        # format loop 6
        - name: "Watermark PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/add//powerpoint/"
          description: "MS PowerPoint and Open Office presentations"

        # format loop 7
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/java/add//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 8
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/java/add//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 9
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/java/add//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 10
        - name: "Watermark JPEG"
          format: "JPEG"
          link: "/watermark/java/add//jpeg/"
          description: "JPEG Image"

        # format loop 11
        - name: "Watermark PNG"
          format: "PNG"
          link: "/watermark/java/add//png/"
          description: "Portable Network Graphic"

        # format loop 12
        - name: "Watermark TIFF"
          format: "TIFF"
          link: "/watermark/java/add//tiff/"
          description: "Tag Image File Format"

        # format loop 13
        - name: "Watermark WEBP"
          format: "WEBP"
          link: "/watermark/java/add//webp/"
          description: "WEB Picture"

        # format loop 14
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/java/add//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 15
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/java/add//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 16
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/java/add//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 17
        - name: "Watermark RTF"
          format: "RTF"
          link: "/watermark/java/add//rtf/"
          description: "Rich Text Format"

---