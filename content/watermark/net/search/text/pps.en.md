
---
############################# Static ############################
layout: "autogen"
date: 2023-12-05T16:03:06
draft: false
path: "watermark/net/search/text/pps/"
otherformats: PDF WORD EXCEL VISIO PRESENTATION SPREADSHEET WORKSHEET DOC DOCM DOCX DOT DOTM DOTX EXCEL ODT POT POTM POTX PPS PPSM PPSX PPT PPTM PPTX RTF SXC TXT VDW VDX VSD VSDM VSDX VSS VSSM VSSX VST VSTM VSTX VSX VTX WORD XLAM XLS XLSB XLSM XLSX XLT XLTM XLTX

############################# Head ############################
head_title: "Search Watermarks from PPS in C#, ASP.NET, VB.NET"
head_description: ".NET library to search watermarks from PPS document using smart search features within C#, ASP.NET, VB.NET & .NET Core applications using GroupDocs.Watermark APIs for .NET."

############################# Header ############################
title: "Search Watermarks from PPS in C#, ASP.NET, VB.NET"
description: "Use smart search to find all possible watermarks from PPS file from within C#, ASP.NET, VB.NET & .NET Core applications. Define search criteria based on text, regular expressions (RegEx), images, hyperlinks, characters and different search objects to find watermarks from the whole or specific pages of the source document."

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
    title_left: "Search Watermarks from PPS in .NET"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/) makes it easy for .NET developers to intelligently search watermarks from within their applications by implementing a few easy steps.

        *   Instantiate **Watermarker** with input PPS document.
        *   Initialize **PossibleWatermarkCollection** to perform watermark search.
        *   Defined search criteria to find possible watermarks.
        *   {net_text.steps.content_left.step_4}
        
    title_right: "System Requirements"
    content_right: |
        Before executing the code example below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Watermark for .NET from [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)
        
    code: |
        ```cs
        // Search possible watermarks in DOC document using C#, ASP.NET, VB.NET & .NET Core.
        // Instantiate Watermarker with input PPS document
        using (Watermarker watermarker = new Watermarker("input.pps"))
        {
            // Initialize PossibleWatermarkCollection to start watermark search
            PossibleWatermarkCollection possibleWatermarks = watermarker.Search();
            foreach (PossibleWatermark possibleWatermark in possibleWatermarks)
            {
                if (possibleWatermark.ImageData != null)
                {
                    Console.WriteLine(possibleWatermark.ImageData.Length);
                }

                // Defined search criteria to find possible watermarks
                Console.WriteLine(possibleWatermark.Text);
                Console.WriteLine(possibleWatermark.X);
                Console.WriteLine(possibleWatermark.Y);
                Console.WriteLine(possibleWatermark.RotateAngle);
                Console.WriteLine(possibleWatermark.Width);
                Console.WriteLine(possibleWatermark.Height);
            }
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