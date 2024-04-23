
---
############################# Static ############################
layout: "format"
date:  2024-04-23T17:30:42
draft: false
lang: en
format: Word
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C# .NET API for Word Watermark Removal"
head_description: "Efficiently clear, delete, or edit out watermarks from Word documents using our C# .NET API for flawless document presentation."

############################# Header ############################
title: "C# .NET Word Watermark Remover" 
description: "Use the GroupDocs.Watermark C# .NET API to remove watermarks from Word documents, perfect for maintaining the integrity and cleanliness of legal and corporate documents."
subtitle: "GroupDocs.Watermark for .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Free Nuget download"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET library"
    link: "/watermark/net/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       With the GroupDocs.Watermark for .NET C# .NET library, developers can easily manage and remove watermarks in Microsoft Word files. This tool supports a wide range of watermark operations, including the detection, modification, and removal of both text and image watermarks, ensuring documents are free of unwanted marks while preserving layout and formatting.

############################# Steps ############################
steps:
    enable: true
    title: "Remove Watermarks from Word Documents Using .NET"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/)** simplifies the task of removing watermarks from business documents. Empower your .NET application by integrating our library and follow these simple steps:
      
      1. Begin by instantiating the main class, **Watermarker**, with the Word document. Our API supports processing documents provided as either a stream or a local path.
      2. Utilize **SearchCriteria** to narrow down the set of watermarks to be processed. You can use various parameters such as images, text, or formatting features. The more specific the search parameters you provide, the more precise the results you obtain.
      3. Process the list of document watermarks obtained as a search result and remove them from the document.
      4. After removing the watermarks, save the resulting document as a local file or a byte stream.
   
    code:
      platform: "net"
      copy_title: "Copy"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // Remove text watermark from WORD document

        // Provide Watermarker instance for document WORD source document
        using (Watermarker watermarker = new Watermarker("input.docx"))
        {
            // Remove selected watermarks from the document
            TextFormattingSearchCriteria criteria = new TextFormattingSearchCriteria();
            criteria.ForegroundColorRange = new ColorRange();
            criteria.FontBold = true;
            PossibleWatermarkCollection watermarks = watermarker.Search(criteria);
            watermarks.Clear();

            // Save file to provided path
            watermarker.Save("output.docx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Streamline Watermark Removal with C# .NET API"
  description: "Discover the powerful watermark removal capabilities of our C# .NET API, designed to seamlessly integrate with your .NET applications. Remove or clear watermarks from PDFs, images, and office documents efficiently while preserving the original file quality."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "Remove Watermark"
  features:
    # feature loop
    - title: "Precise Watermark Clearance"
      content: "Our .NET API provides precise tools to cleanly remove watermarks from any document. Tailored for developers, this feature ensures that removing watermarks does not compromise document quality or layout."

    # feature loop
    - title: "Automate Bulk Watermark Removal"
      content: "Automate the process of removing watermarks from large document sets with our .NET API. Ideal for businesses that handle large volumes of documents, improving both efficiency and document security."

    # feature loop
    - title: "Advanced Watermark Editing Features"
      content: "Leverage advanced features to selectively edit out or modify watermarks. Our API supports detailed adjustments to ensure your documents maintain a professional appearance while securing sensitive information."
      
  code_samples:
    # code sample loop
    - title: "Remove spreadsheets text watermark"
      content: |
        How to remove text watermarks with special formatting in Excel docs.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Load Excel workbook
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  Get content and find appropriate watermark
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();
                foreach (SpreadsheetWorksheet section in content.Worksheets)
                {
                    for (int i = section.Shapes.Count - 1; i >= 0; i--)
                    {
                        foreach (FormattedTextFragment fragment in section.Shapes[i].FormattedTextFragments)
                        {
                            if (fragment.ForegroundColor.Equals(Color.Red) && fragment.Font.FamilyName == "Arial")
                            {
                                //  Remove text watermark
                                section.Shapes.RemoveAt(i);
                                break;
                            }
                        }
                    }
                }

                //  Save processed XLSX
                watermarker.save("result.xlsx");
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
    - title: "Nuget download"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Managing Word Watermarks with .NET"
    exclude: "WORD"
    description: "Explore powerful features for watermark management in Word documents using our C# .NET API, designed to enhance document security and presentation without compromising on quality."
    items: 
        # format loop 1
        - name: "Watermark PDF"
          format: "PDF"
          link: "/watermark/net/remove//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark Word"
          format: "WORD"
          link: "/watermark/net/remove//word/"
          description: "MS Word and Open Office documents"
          
        # format loop 3
        - name: "Watermark Excel"
          format: "EXCEL"
          link: "/watermark/net/remove//excel/"
          description: "MS Excel and Open Office spreadsheets"

        # format loop 4
        - name: "Watermark PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/remove//powerpoint/"
          description: "MS PowerPoint and Open Office presentations"

        # format loop 5
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/net/remove//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 6
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/net/remove//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 7
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/net/remove//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/net/remove//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 9
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/net/remove//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 10
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/net/remove//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 11
        - name: "Watermark RTF"
          format: "RTF"
          link: "/watermark/net/remove//rtf/"
          description: "Rich Text Format"

---