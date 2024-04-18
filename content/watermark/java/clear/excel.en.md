
---
############################# Static ############################
layout: "format"
date:  2024-04-18T15:29:25
draft: false
lang: en
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Clear Watermark for Excel Spreadsheets"
head_description: "GroupDocs.Watermark for Java generates watermark for MS Excel files in applications based on Java, J2SE 7.0 (1.7) or above."

############################# Header ############################
title: "Clear Watermark for MS Excel Spreadsheets via Java" 
description: "Text and image watermark generation for MS Excel files using Java J2SE applications. Watermarks your business documents with BMP, PNG, GIF, and JPEG images or text. Adjust watermark size, alignment, rotation angle, and position on the document pages."
subtitle: "GroupDocs.Watermark for Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Free Maven download"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java library"
    link: "/watermark/java/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java is a comprehensive solution for managing watermarks using Java. With this tool, developers can easily perform operations such as generation, adjust, search, and clear watermarks from documents in popular file formats. It supports working with both text and image watermarks in a variety of documents, including PDF, Microsoft Word, Excel, PowerPoint, Visio, email, and image formats. GroupDocs.Watermark supports all major operating systems and Java versions including J2SE 7.0 (1.7), J2SE 8.0 (1.8) or above.

############################# Steps ############################
steps:
    enable: true
    title: "Clear Excel documents of watermarks using Java"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/)** makes it easy to clear business documents of previously added watermarks. Empower your Java application by installing our library and do it in a few simple steps:
      
      1. First of all instantiate the main class called **Watermarker** with Excel document. Our API supports passing a document to be processed as stream or a local path.
      2. Use **SearchCriteria** to limit set of watermarks to be processed. It is possible to use an image as search parameter as well as text or formating features. Then more specific search parameters you provide, then more precise result you obtain.
      3. Process list of the document watermarks that you have obtained as a search result. Clear the document.
      4. After clearing the document save result as a local file or a byte stream.
   
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

        // Clear text watermark in EXCEL document

        // Instantiate Watermarker with EXCEL document
        Watermarker watermarker = new Watermarker("input.xslx");
        
        // Clear specific watermark
        PossibleWatermarkCollection possibleWatermarks = watermarker.search();
        possibleWatermarks.removeAt(0);

        // Save processed file
        watermarker.save("output.xslx");
        
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
      content: "GroupDocs.Watermark makes it easy for Java developers to add various types of watermarks in popular business documents and files."

    # feature loop
    - title: "Customize watermarks for your goals."
      content: "Our solution supports many watermark features. You can easily adjust size, rotation, color, font, font styles and other options to make watermark looks perfect."

    # feature loop
    - title: "Use native document objects"
      content: "Accordingly do particular document format it is possible to use native document features. Native PDF annotations or MS Word page watermark may be used for watermarking."
      
  code_samples:
    # code sample loop
    - title: "PDF clear text watermark"
      content: |
        This example shows how to find and remove all annotations containing text with a particular formatting from a PDF document.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Load PDF document
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Get document content
        PdfContent pdfContent = watermarker.getContent(PdfContent.class);

        //  Clear text watermarks with particular font
        for (PdfPage page : pdfContent.getPages()){
            for (int i = page.getAnnotations().getCount() - 1; i >= 0; i--){
                for (FormattedTextFragment fragment : page.getAnnotations().get_Item(i).getFormattedTextFragments()){
                    if (fragment.getFont().getFamilyName() == "Verdana"){
                        page.getAnnotations().removeAt(i);
                        break;
                    }
                }
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
    title: "Use images as watermarks via Java"
    exclude: "EXCEL"
    description: "Our Java solutions allows to protect various formats of business documents. Watermarked documents may enrich your business processes."
    items: 
        # format loop 1
        - name: "Watermark PDF"
          format: "PDF"
          link: "/watermark/java/clear//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark Word"
          format: "WORD"
          link: "/watermark/java/clear//word/"
          description: "MS Word and Open Office documents"
          
        # format loop 3
        - name: "Watermark Excel"
          format: "EXCEL"
          link: "/watermark/java/clear//excel/"
          description: "MS Excel and Open Office spreadsheets"

        # format loop 4
        - name: "Watermark PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/clear//powerpoint/"
          description: "MS PowerPoint and Open Office presentations"

        # format loop 5
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/java/clear//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 6
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/java/clear//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 7
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/java/clear//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/java/clear//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 9
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/java/clear//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 10
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/java/clear//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 11
        - name: "Watermark RTF"
          format: "RTF"
          link: "/watermark/java/clear//rtf/"
          description: "Rich Text Format"

---