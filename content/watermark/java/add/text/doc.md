---
############################# Static ############################
layout: "autogen"
draft: false
path: "watermark/java/add/text/doc/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

############################# Head ############################
head_title: "Add Text Watermark to DOC in Java"
head_description: "Java library to add text watermark to DOC file in Java & J2SE applications using GroupDocs.Watermark API for Java"

############################# Header ############################
title: "Add Text Watermark to DOC in Java"
description: "Add text watermarks to DOC files in Java & J2SE applications. The watermark size, font type, rotation angle, and position can be managed with ease."

############################# SubMenu ############################
submenu:
    enable: true

############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java API"
    content: |
        GroupDocs.Watermark for Java is a comprehensive solution for managing watermarks in Java applications. It enables developers to easily perform various watermark manipulation operations such as adding, editing, searching, and deleting different types of watermarks in documents of various popular file formats. It supports working with text and image watermarks in a variety of documents, including PDF, Microsoft Word, Excel, PowerPoint, Visio, Email, and image formats.
        
        GroupDocs.Watermark API supports all major operating systems and Java versions including J2SE 7.0 (1.7), J2SE 8.0 (1.8), and Java 10.

############################# Steps ############################
steps:
    enable: true
    title_left: "Add Text Watermark to DOC File in Java"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/) makes it easy for Java developers to add text watermarks in their applications by implementing a few easy steps.

        *   Instantiate **Watermarker** with input DOC document.
        *   Initialize **TextWatermarker** with watermark text, font size and style.
        *   Set watermark properties (alignment, color etc).
        *   Add watermark to the watermarker and generate output document.
        
    title_right: "System Requirements"
    content_right: |
        Before executing the code example below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: NetBeans, IntelliJ IDEA, Eclipse
        *   Frameworks: Java 7 (1.7) and above
        *   Download the latest version of GroupDocs.Watermark for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
        
    code: |
        ```cs
        // Add text watermark to DOC in Java
        // Instantiate Watermarker with input DOC document
        (Watermarker watermarker = new Watermarker(input.doc))
        
        // Instantiate TextWatermarker with watermark text, font size and style
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
            
        // Set watermark properties
        watermark.setForegroundColor(Color.getRed());
        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
        watermark.setVerticalAlignment(VerticalAlignment.Center);

        // Add watermark and save watermarked image
        watermarker.add(watermark);
        watermarker.save(output.doc);
        
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