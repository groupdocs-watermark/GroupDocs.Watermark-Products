
---
############################# Static ############################
layout: "autogen"
date: 2023-12-04T15:21:05
draft: false
path: "watermark/net/edit/image/presentation/"
otherformats: PDF WORD EXCEL VISIO PRESENTATION SPREADSHEET WORKSHEET DOC DOCM DOCX DOT DOTM DOTX EXCEL ODT POT POTM POTX PPS PPSM PPSX PPT PPTM PPTX RTF SXC TXT VDW VDX VSD VSDM VSDX VSS VSSM VSSX VST VSTM VSTX VSX VTX WORD XLAM XLS XLSB XLSM XLSX XLT XLTM XLTX

############################# Head ############################
head_title: "Edit Image Watermark in PRESENTATION in C#, ASP.NET, VB.NET"
head_description: ".NET library to edit a found image watermark in a PRESENTATION file in C#, ASP.NET, VB.NET & .NET Core applications using GroupDocs.Watermark APIs for .NET."

############################# Header ############################
title: "Edit Image Watermark in PRESENTATION in C# .NET"
description: "Find & modify a found image watermark in a PRESENTATION document within C#, ASP.NET, VB.NET & .NET Core applications. Add BMP, PNG, GIF & JPEG image watermarks to the documents. Also manage the watermark size, font type, rotation angle and position of the watermark on the document pages, as you may need."

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
    title_left: "Edit Image Watermark in PRESENTATION File in .NET"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/) makes it easy for .NET developers to edit image (BMP, PNG, GIF or JPEG) watermarks in their applications by implementing a few easy steps.

        *   Instantiate **Watermarker** with input PRESENTATION document.
        *   Initialize **SearchCriteria** to find the image watermarks.
        *   Replace the found watermark.
        *   Save the newly watermarked document.
        
    title_right: "System Requirements"
    content_right: |
        Before executing the code example below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Watermark for .NET from [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)
        
    code: |
        ```cs
        // Find & replace image watermark in a PRESENTATION in C#, ASP.NET, VB.NET & .NET Core applications
        // Instantiate Watermarker with input PRESENTATION document
        using (Watermarker watermarker = new Watermarker("input.presentation"))
        {
            // Initialize the SearchCriteria to match a particular image
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                try
                {
                    // Replace the found image
                    watermark.ImageData = imageData;
                }
                catch (Exception e)
                {
                    // Found entity may not support text editing
                    // Passed arguments can have inappropriate value
                    // Process such cases here
                }
            }
            // Save the updated document
            watermarker.Save("output.presentation");
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