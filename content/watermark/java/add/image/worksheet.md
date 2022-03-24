---
############################# Static ############################
layout: "autogen"
draft: false
path: "watermark/java/add/image/worksheet/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

############################# Head ############################
head_title: "Add Image Watermark to WORKSHEET in Java"
head_description: "Java library to add image watermark to WORKSHEET file in Java & J2SE applications using GroupDocs.Watermark APIs for Java."

############################# Header ############################
title: "Add Image Watermark to WORKSHEET in Java"
description: "Adding image watermark to WORKSHEET file in Java & J2SE applications. Add BMP, PNG, GIF & JPEG image watermarks to the documents. Also manage the watermark size, alignment, rotation angle and position of the watermark on the document pages, as you may need."

############################# SubMenu ############################
submenu:
    enable: true

############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java API"
    content: |
        GroupDocs.Watermark for Java is a complete watermarks management solution for Java applications. Developers can quickly perform watermarks manipulation operations like; add, edit, search and delete different types of watermarks from within documents of all popular file formats. It supports working with text and image watermarks in a variety of documents including PDF, Microsoft Word, Excel, PowerPoint, Visio, Email and image formats.
        
        GroupDocs.Watermark APIs are well supported on all major operating systems and Java versions including J2SE 7.0 (1.7), J2SE 8.0 (1.8) and Java 10.

############################# Steps ############################
steps:
    enable: true
    title_left: "Add Image Watermark to WORKSHEET File in Java"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/) makes it easy for Java developers to add image (BMP, PNG, GIF or JPEG) watermarks in their applications by implementing a few easy steps.

        *   Instantiate **Watermarker** with input WORKSHEET document.
        *   Use image watermark path as constructor parameter of **ImageWatermark** class.
        *   Set watermark properties (size, alignment, color etc).
        *   Add watermark to the watermarker and generate output document.
        
    title_right: "System Requirements"
    content_right: |
        Before executing the code example below, please make sure that you have the following prerequisites installled on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: NetBeans, IntelliJ IDEA, Eclipse
        *   Frameworks: Java 7 (1.7) and above
        *   Download the latest version of GroupDocs.Watermark for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
        
    code: |
        ```cs
        // Add image watermark to WORKSHEET in Java applications
        // Instantiate Watermarker with input WORKSHEET document
        Watermarker watermarker = new Watermarker(input.worksheet)
        
        // Use image watermark path as constructor parameter of ImageWatermark class
        ImageWatermark watermark = new ImageWatermark(watermark.png)
        
        // Set watermark properties (width, height, alignment)
        watermark.Width = 140;
        watermark.Height = 140;
        watermark.HorizontalAlignment = HorizontalAlignment.Center;
        watermark.VerticalAlignment = VerticalAlignment.Center;

        //Add watermark to the watermarker and generate output document
        watermarker.add(watermark);
        watermarker.save(output.worksheet);

        watermark.close();
        watermarker.close();
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