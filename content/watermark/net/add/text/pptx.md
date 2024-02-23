---
############################# Static ############################
layout: "autogen"
draft: false
path: "watermark/net/add/text/pptx/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

############################# Head ############################
head_title: "Add Text Watermark to PPTX in C#, ASP.NET, VB.NET"
head_description: ".NET library to add text watermark to PPTX file in C#, ASP.NET, VB.NET & .NET Core applications using GroupDocs.Watermark APIs for .NET."

############################# Header ############################
title: "Add Text Watermark to PPTX in C# .NET"
description: "Adding text watermark to PPTX file in C#, ASP.NET, VB.NET & .NET Core applications. Manage the watermark size, font type, rotation angle and position of the watermark on the document pages, as you may need."

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
    title_left: "Add Text Watermark to PPTX File in .NET"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/) makes it easy for .NET developers to add text watermarks in their applications by implementing a few easy steps.

        *   Instantiate **Watermarker** with input PPTX document.
        *   Initialize the **Font** to be used for watermark.
        *   Create the **TextWatermark** object.
        *   Set watermark properties (alignment, color etc).
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
        // Add text watermark to PPTX in C#, ASP.NET, VB.NET & .NET Core applications
        // Instantiate Watermarker with input PPTX document
        using (Watermarker watermarker = new Watermarker(input.pptx))
          {
            // Initialize the Font to be used for watermark
            Font font = new Font("Arial", 19, FontStyle.Bold | FontStyle.Italic);
            
            // Create the TextWatermark object
            TextWatermark watermark = new TextWatermark("my watermark", font);

            // Set watermark properties
            watermark.ForegroundColor = Color.Red;
            watermark.BackgroundColor = Color.Blue;
            watermark.TextAlignment = TextAlignment.Right;
            watermark.Opacity = 0.5;

            // Add watermark and save watermarked image
            watermarker.Add(watermark);
            watermarker.Save(output.pptx);
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