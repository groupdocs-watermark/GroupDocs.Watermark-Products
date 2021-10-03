---
############################# Static ############################
layout: "autogen"
draft: false
path: "watermark/net/remove/image/ppt/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

############################# Head ############################
head_title: "Remove Image Watermark from PPT in C# .NET"
head_description: ".NET library to find and remove image watermark from PPT document using smart search within C#, ASP.NET, VB.NET & .NET Core applications using GroupDocs.Watermark APIs for .NET."

############################# Header ############################
title: "Remove Image Watermark from PPT in C#"
description: "Use smart search to find & remove image watermark from a PPT document from within C#, ASP.NET, VB.NET & .NET Core applications. Define a search criterion to search & delete the specified watermarks from the document."

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
    title_left: "Delete Watermark from PPT File in .NET"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/) makes it easy for .NET developers to search and remove watermarks with text formatting from their applications by implementing a few easy steps.

        *   Instantiate **Watermarker** with input PPT document.
        *   Initialize **SearchCriteria** to find the image watermarks.
        *   Remove defined watermark from the document.
        *   Save the modified document.
        
    title_right: "System Requirements"
    content_right: |
        Before executing the code example below, please make sure that you have the following prerequisites installled on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Watermark for .NET from [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)
        
    code: |
        ```cs
        // Search & remove image watermark with from a PPT document in C#, ASP.NET, VB.NET & .NET Core applications
        // Instantiate Watermarker with input PPT document
        using (Watermarker watermarker = new Watermarker(input.ppt))
          {
            // Initialize the SearchCriteria to match a particular image
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria(logo.png);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            // Remove specified watermark from the document
            possibleWatermarks.Remove(possibleWatermarks[0]);

            // Save the modified document
            watermarker.Save(output.ppt);
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