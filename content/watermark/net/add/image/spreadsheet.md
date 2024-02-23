---
############################# Static ############################
layout: "autogen"
draft: false
path: "watermark/net/add/image/spreadsheet/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

############################# Head ############################
head_title: "Add Image Watermark to SPREADSHEET in C#, ASP.NET, VB.NET"
head_description: ".NET library to add image watermark to SPREADSHEET file in C#, ASP.NET, VB.NET & .NET Core applications using GroupDocs.Watermark APIs for .NET."

############################# Header ############################
title: "Add Image Watermark to SPREADSHEET in C# .NET"
description: "Adding image watermark to SPREADSHEET file in C#, ASP.NET, VB.NET & .NET Core applications. Add BMP, PNG, GIF & JPEG image watermarks to the documents. Also manage the watermark size, alignment, rotation angle and position of the watermark on the document pages, as you may need."

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
    title_left: "Add Image Watermark to SPREADSHEET File in .NET"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/) makes it easy for .NET developers to add image (BMP, PNG, GIF or JPEG) watermarks in their applications by implementing a few easy steps.

        *   Instantiate **Watermarker** with input SPREADSHEET document.
        *   Use image watermark path as constructor parameter of **ImageWatermark** class.
        *   Set watermark properties (size, alignment, color etc).
        *   Add watermark to the watermarker and generate output document.
        
    title_right: "System Requirements"
    content_right: |
        Before executing the code example below, please make sure that you have the following prerequisites installled on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Watermark for .NET from [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)
        
    code: |
        ```cs
        // Add image watermark to SPREADSHEET in C#, ASP.NET, VB.NET & .NET Core applications
        // Instantiate Watermarker with input SPREADSHEET document
        using (Watermarker watermarker = new Watermarker(input.spreadsheet))
          {
            // Use image watermark path as constructor parameter of ImageWatermark class
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                // Set watermark properties (width, height, alignment)
                watermark.Width = 140;
                watermark.Height = 140;
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;

                //Add watermark to the watermarker and generate output document
                watermarker.Add(watermark);
                watermarker.Save(output.spreadsheet);
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