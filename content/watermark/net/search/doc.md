---
############################# Static ############################
layout: "autogen"
draft: false
path: "watermark/net/search/doc/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

############################# Head ############################
head_title: "Search Watermarks from DOC in C#, ASP.NET, VB.NET"
head_description: ".NET library to search watermarks from DOC document using smart search features within C#, ASP.NET, VB.NET & .NET Core applications using GroupDocs.Watermark APIs for .NET."

############################# Header ############################
title: "Search Watermarks from DOC in C# .NET"
description: "Use smart search to find all possible watermarks from DOC file from within C#, ASP.NET, VB.NET & .NET Core applications. Define search criteria based on text, regular expressions (RegEx), images, hyperlinks, characters and different search objects to find watermarks from the whole or specific pages of the source document."

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
    title_left: "Search Watermarks from DOC in .NET"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/) makes it easy for .NET developers to intelligently search watermarks from within their applications by implementing a few easy steps.

        *   Instantiate **Watermarker** with input DOC document.
        *   Initialize **PossibleWatermarkCollection** to perform a watermark search.
        *   Defined search criteria to find possible watermarks.
        
    title_right: "System Requirements"
    content_right: |
        Before executing the code example below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Watermark for .NET from [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)
        
    code: |
        ```cs
        // search possible watermarks in DOC document using C#, ASP.NET, VB.NET & .NET Core.
        // Instantiate Watermarker with input DOC document
        using (Watermarker watermarker = new Watermarker(input.doc))
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