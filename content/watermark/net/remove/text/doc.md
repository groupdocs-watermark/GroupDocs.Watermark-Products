---
############################# Static ############################
layout: "autogen"
draft: false
path: "watermark/net/remove/text/doc/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

############################# Head ############################
head_title: "Remove Watermark from DOC in C#, ASP.NET, VB.NET"
head_description: ".NET library to find and remove watermark from DOC document using smart search within C#, ASP.NET, VB.NET & .NET Core applications using GroupDocs.Watermark APIs for .NET."

############################# Header ############################
title: "Remove Watermark from DOC in C# .NET"
description: "Use smart search to find & remove watermark from a DOC document with text formatting from within C#, ASP.NET, VB.NET & .NET Core applications. Define a search criterion to search & delete the watermarks based on a specific font name, color, size and other matching properties."

############################# SubMenu ############################
submenu:
    enable: true

############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET API"
    content: |
        GroupDocs.Watermark for .NET is a complete watermark management solution for .NET applications. Developers can quickly perform watermark manipulation operations like; add, edit, search and delete different types of watermarks from within documents of all popular file formats. It supports working with text and image watermarks in a variety of documents including PDF, Microsoft Word, Excel, PowerPoint, Visio, Email and image formats.
        
        GroupDocs.Watermark APIs are well supported on all major operating systems and platforms including .NET Framework, .NET Standard, .NET Core, Mono and Xamarin.

############################# Steps ############################
steps:
    enable: true
    title_left: "Delete Watermark from DOC File in .NET"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/) makes it easy for .NET developers to search and remove watermarks with text formatting from their applications by implementing a few easy steps.

        *   Instantiate **Watermarker** with input DOC document.
        *   Initialize **TextFormattingSearchCriteria** to find the text watermarks.
        *   Initialize the defined search criteria to find & remove watermarks.
        *   Save the modified document.
        
    title_right: "System Requirements"
    content_right: |
        Before executing the code example below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Watermark for .NET from [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)
        
    code: |
        ```cs
        // Search & remove watermark with text formatting from a DOC document in C#, ASP.NET, VB.NET & .NET Core applications
        // Instantiate Watermarker with input DOC document
        using (Watermarker watermarker = new Watermarker(input.doc))
          {
            // Initialize the TextFormattingSearchCriteria to define the watermarks to search for
            TextFormattingSearchCriteria criteria = new TextFormattingSearchCriteria();
            criteria.ForegroundColorRange = new ColorRange();
            criteria.ForegroundColorRange.MinHue = -5;
            criteria.ForegroundColorRange.MaxHue = 10;
            criteria.ForegroundColorRange.MinBrightness = 0.01f;
            criteria.ForegroundColorRange.MaxBrightness = 0.99f;
            criteria.BackgroundColorRange = new ColorRange();
            criteria.BackgroundColorRange.IsEmpty = true;
            criteria.FontName = "Arial";
            criteria.MinFontSize = 19;
            criteria.MaxFontSize = 42;
            criteria.FontBold = true;

            PossibleWatermarkCollection watermarks = watermarker.Search(criteria);
            watermarks.Clear();

            // Save the modified document
            watermarker.Save(output.doc);
          }
        ```        

demos:
    enable: true
        

about_formats:
    enable: true


more_formats:
    enable: true


back_to_top:
    enable: true
---