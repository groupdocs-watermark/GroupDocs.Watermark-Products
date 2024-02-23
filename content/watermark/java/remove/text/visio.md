---
############################# Static ############################
layout: "autogen"
draft: false
path: "watermark/java/remove/text/visio/"
otherformats: PDF WORD EXCEL IMAGE DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

############################# Head ############################
head_title: "Remove Watermark from VISIO in Java"
head_description: "Java library to find and remove watermark from VISIO document using smart search within Java applications using GroupDocs.Watermark APIs for Java."

############################# Header ############################
title: "Remove Watermark from VISIO in Java"
description: "Use smart search to find & remove watermark from a VISIO document with text formatting from within Java & J2SE applications. Define a search criterion to search & delete the watermarks based on a specific font name, color, size and other matching properties."

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
    title_left: "Delete Watermark from VISIO File in Java"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/) makes it easy for Java developers to search and remove watermarks with text formatting from their applications by implementing a few easy steps.

        *   Instantiate **Watermarker** with input VISIO document.
        *   Initialize the defined search criteria to find & remove watermarks.
        *   Save the modified document.
        
    title_right: "System Requirements"
    content_right: |
        Before executing the code example below, please make sure that you have the following prerequisites installled on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: NetBeans, IntelliJ IDEA, Eclipse
        *   Frameworks: Java 7 (1.7) and above
        *   Download the latest version of GroupDocs.Watermark for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
        
    code: |
        ```cs
        // Search & remove watermark from a VISIO document in Java applications
        // Instantiate Watermarker with input VISIO document
        Watermarker watermarker = new Watermarker(input.visio))

        PossibleWatermarkCollection possibleWatermarks = watermarker.search();

        // Remove possible watermark at the specified index from the document
        possibleWatermarks.removeAt(0);

        // Remove specified possible watermark from the document
        possibleWatermarks.remove(possibleWatermarks.get_Item(0));

        // Save the modified document
        watermarker.save(output.visio);

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