---
############################# Static ############################
layout: "autogen"
draft: false
path: "watermark/java/remove/image/doc/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

############################# Head ############################
head_title: "Remove Image Watermark from DOC in Java"
head_description: "Java library to find and remove image watermark from DOC document using smart search within Java & J2SE applications using GroupDocs.Watermark APIs for Java."

############################# Header ############################
title: "Remove Image Watermark from DOC in Java"
description: "Use smart search to locate and delete image watermarks from a DOC document within Java and J2SE applications. Specify a search criterion that can be used to search and delete specific watermarks from a document."

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
    title_left: "Delete Watermark from DOC File in Java"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/) makes it easy for Java developers to search and remove watermarks with text formatting from their applications by implementing a few easy steps.

        *   Instantiate **Watermarker** with input DOC document.
        *   Initialize **PossibleWatermarkCollection** to find the image watermarks.
        *   Remove specified watermark(s) from the document.
        *   Save the modified document.
        
    title_right: "System Requirements"
    content_right: |
        Before executing the code example below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: NetBeans, IntelliJ IDEA, Eclipse
        *   Frameworks: Java 7 (1.7) and above
        *   Download the latest version of GroupDocs.Watermark for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
        
    code: |
        ```cs
        // Search & remove image watermark from a DOC document in Java applications
        // Instantiate Watermarker with input DOC document
        Watermarker watermarker = new Watermarker(input.doc)
        
        PossibleWatermarkCollection possibleWatermarks = watermarker.search();

        // Remove watermark from a specified index position from the document
        possibleWatermarks.removeAt(0);

        // Remove the specified possible watermark from the document
        possibleWatermarks.remove(possibleWatermarks.get_Item(0);

        // Save the modified document
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