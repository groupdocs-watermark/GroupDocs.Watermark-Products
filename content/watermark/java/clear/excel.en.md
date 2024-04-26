
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:57
draft: false
lang: en
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Remove Watermarks from Excel with Java API"
head_description: "Easily clear, delete, or edit out watermarks from Excel files using the GroupDocs.Watermark for Java API. Enhance document integrity and presentation."

############################# Header ############################
title: "Java Excel Watermark Management" 
description: "Utilize the GroupDocs.Watermark for Java to remove or edit watermarks in Excel spreadsheets efficiently and with precision."
subtitle: "GroupDocs.Watermark for Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Free download at Maven"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java library"
    link: "/watermark/java/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       With the GroupDocs.Watermark for Java library, developers can manage watermarks in Excel files seamlessly. This tool supports operations like removing, adjusting, and searching for both text and image watermarks. Ideal for applications requiring clean visual presentation of data without compromising the document's security or layout.

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

        // Clear text watermark in Excel document

        // Instantiate Watermarker with Excel document
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
  title: "Efficient Watermark Removal via Java API"
  description: "Explore our Java API's robust capabilities to remove or clear watermarks from various document types, including PDFs and Office files. Perfect for developers looking to maintain clean visuals and protect document integrity."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "Clear Watermark"
  features:
    # feature loop
    - title: "Remove Watermarks with Precision"
      content: "Utilize our Java API to precisely target and delete watermarks without disrupting the original document layout. Ideal for sensitive or official documents where clarity and accuracy are paramount."

    # feature loop
    - title: "Batch Watermark Deletion"
      content: "Enhance your document processing efficiency by removing watermarks from multiple files simultaneously. Our API supports batch operations, saving time and resources for large-scale tasks."

    # feature loop
    - title: "Edit Out Watermark Elements"
      content: "Our advanced editing tools allow you to selectively edit out watermark components, providing flexibility in managing document presentations while ensuring content security."
      
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
    title: "Managing Excel Watermarks in Java"
    exclude: "EXCEL"
    description: "Learn how the Excel API simplifies watermark removal from Excel documents, maintaining file integrity and clarity."
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