
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:06
draft: false
lang: en
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Edit Watermarks in Excel formats"
head_description: "Customize and secure your documents effortlessly with GroupDocs.Watermark for .NET. Enhance document integrity and edit Excel watermarks with ease."

############################# Header ############################
title: "Edit Your Excel Spreadsheets Watermarks: .NET Efficiency" 
description: "Elevate your document security with our customizable watermarking tool designed for .NET efficiency. Edit Excel watermarks effortlessly."
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
    title: "GroupDocs.Watermark for .NET Library"
    link: "/watermark/net/"
    link_title: "Learn more"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Edit Excel Watermarks With Our Tool:** Our GroupDocs.Watermark for .NET tools offer efficient strategies to enhance and protect your documents. With various features for .NET developers, managing watermarks becomes a breeze, ensuring document security and authenticity.

############################# Steps ############################
steps:
    enable: true
    title: "Edit watermarks in Excel documents using .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** empowers .NET developers to effortlessly edit watermarks within various Excel documents. Here's a simplified guide how to use our API in your application:
      
      1. Begin by passing your Excel file as a parameter to the **Watermarker** class constructor. You can provide the file either as a byte stream, a file stream, or a local disk path.
      2. Next, locate the specific watermarks that require editing. Utilize the **SearchCriteria** to identify watermarks with the corresponding properties previously added to the document.
      3. Following the search, you'll obtain a list of relevant watermarks. You can then customize their properties, such as size, page alignment, text, color, image content, and more. This grants you extensive control over your data.
      4. Once you've completed editing the watermarks, save the updated document. You can utilize a local file path or a stream to store the final result.
   
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
        // Edit EXCEL text watermark

        // Make Watermarker providing EXCEL file
        using (Watermarker watermarker = new Watermarker("input.xslx"))
        {
            // Construct the TextSearchCriteria and get text watermarks
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                 // Edit text watermark
                 watermark.FormattedTextFragments.Clear();
                 watermark.FormattedTextFragments.Add("passed", 
                    new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
            }

            // Save the document
            watermarker.Save("output.xslx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Learn more about watermarks modification"
  description: "Empower your .NET applications with our library and add, edit, remove, or search for watermarks within various file formats."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Edit Watermark"
  features:
    # feature loop
    - title: "Watermark Files for Your Business"
      content: "Use GroupDocs.Watermark for .NET to watermark files and documents. Add and manage watermarks without extra efforts implementing our API in your applications. Search, edit and remove previously added watermarks."

    # feature loop
    - title: "Fine-Tune Watermarks for Your Requirements"
      content: "Our API offers a comprehensive set of customization options. Effortlessly modify aspects like size, orientation, color scheme, font family, and more to create the ideal watermark."

    # feature loop
    - title: "Leverage Document-Specific Features"
      content: "Depending on the file format you're using, you can incorporate built-in functionalities. These may include document background, annotations, headers, or other elements to serve as watermark containers."
      
  code_samples:
    # code sample loop
    - title: "Excel watermark text edit"
      content: |
        This example shows how to edit text for particular watermarks in Excel Worksheets
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Load XLSX spreadsheet
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  Load spreadsheet content
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();

                //  Edit watermark inner text
                foreach (SpreadsheetShape shape in content.Worksheets[0].Shapes)
                {
                    if (shape.Text == "GroupDocs 2016")
                    {
                        shape.Text = "GroupDocs 2017";
                    }
                }

                //  Save output result
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
    title: "Customize Your Watermarks in Other Formats"
    exclude: "EXCEL"
    description: "Watermark a variety of document formats to your needs with GroupDocs.Watermark for .NET."
    items: 
        # format loop 1
        - name: "Watermark PDF"
          format: "PDF"
          link: "/watermark/net/edit//pdf/"
          description: "Adobe Portable Document Format"

        # format loop 2
        - name: "Watermark Word"
          format: "WORD"
          link: "/watermark/net/edit//word/"
          description: "MS Word and Open Office documents"
          
        # format loop 3
        - name: "Watermark Excel"
          format: "EXCEL"
          link: "/watermark/net/edit//excel/"
          description: "MS Excel and Open Office spreadsheets"

        # format loop 4
        - name: "Watermark PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/edit//powerpoint/"
          description: "MS PowerPoint and Open Office presentations"

        # format loop 5
        - name: "Watermark DOCX"
          format: "DOCX"
          link: "/watermark/net/edit//docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 6
        - name: "Watermark PPTX"
          format: "PPTX"
          link: "/watermark/net/edit//pptx/"
          description: "PowerPoint Open XML Presentation"
          
        # format loop 7
        - name: "Watermark XLSX"
          format: "XLSX"
          link: "/watermark/net/edit//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Watermark DOC"
          format: "DOC"
          link: "/watermark/net/edit//doc/"
          description: "Microsoft Word 97 - 2007 Document"

        # format loop 9
        - name: "Watermark XLS"
          format: "XLS"
          link: "/watermark/net/edit//xls/"
          description: "Microsoft Excel Workbook 97-2003"

        # format loop 10
        - name: "Watermark PPT"
          format: "PPT"
          link: "/watermark/net/edit//ppt/"
          description: "PowerPoint Presentation 97-2003"

        # format loop 11
        - name: "Watermark RTF"
          format: "RTF"
          link: "/watermark/net/edit//rtf/"
          description: "Rich Text Format"

---