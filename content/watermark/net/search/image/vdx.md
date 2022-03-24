---
############################# Static ############################
layout: "autogen"
draft: false
path: "watermark/net/search/image/vdx/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

############################# Head ############################
head_title: "Search Image Watermarks from VDX in C# ASP.NET VB.NET"
head_description: ".NET library to search image watermarks from VDX document using smart search features within C#, ASP.NET, VB.NET & .NET Core applications using GroupDocs.Watermark APIs for .NET."

############################# Header ############################
title: "Search Image Watermarks from VDX in C#"
description: "Use smart search to find all possible image watermarks from VDX file from within C#, ASP.NET, VB.NET & .NET Core applications. Define search criteria tp find all matching image watermarks from the whole or specific pages of the source document."

############################# SubMenu ############################
submenu:
    enable: true

############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET API"
    content: |
        GroupDocs.Watermark for .NET is a complete watermarks management solution for .NET applications. Developers can quickly perform watermarks manipulation operations like; add, edit, search and delete different types of watermarks from within documents of all popular file formats. It supports working with text and image watermarks in a variety of documents including PDF, Microsoft Word, Excel, PowerPoint, Visio, Email and image formats.
        
        GroupDocs.Watermark APIs are well supported on all major operating systems and platforms including .NET Framework, .NET Standard, .NET Core, Mono and Xamarin.

############################# Steps ############################
steps:
    enable: true
    title_left: "Search Watermarks from VDX in .NET"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/) makes it easy for .NET developers to intelligently search image watermarks from within their documents by implementing a few easy steps.

        *   Instantiate **Watermarker** with input VDX document.
        *   Initialize **ImageSearchCriteria** to perform watermark search.
        *   Set maximum allowed difference between images.
        *   Display the possible matching watermarks.
        
    title_right: "System Requirements"
    content_right: |
        Before executing the code example below, please make sure that you have the following prerequisites installled on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Watermark for .NET from [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)
        
    code: |
        ```cs
        // search possible IMAGE watermarks in VDX document using C#, ASP.NET, VB.NET & .NET Core.
        // Instantiate Watermarker with input VDX document
        using (Watermarker watermarker = new Watermarker(input.vdx))
          {
            // Initialize ImageSearchCriteria to start watermark search
            ImageSearchCriteria imageSearchCriteria = new ImageDctHashSearchCriteria(watermark.jpeg);

            // Set maximum allowed difference between sample image and the possible watermark
            imageSearchCriteria.MaxDifference = 0.9;
            PossibleWatermarkCollection possibleWatermarks = watermarker.Search(imageSearchCriteria);
            Console.WriteLine("Found {0} possible watermark(s).", possibleWatermarks.Count);
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