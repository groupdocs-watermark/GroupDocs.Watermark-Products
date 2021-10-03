---
############################# Static ############################
layout: "autogen"
draft: false
path: "watermark/java/search/image/xlt/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

############################# Head ############################
head_title: "Search Image Watermarks from XLT in Java"
head_description: "Java library to search image watermarks from XLT document using smart search features within Java & J2SE applications using GroupDocs.Watermark APIs for Java."

############################# Header ############################
title: "Search Image Watermarks from XLT in Java"
description: "Use smart search to find all possible image watermarks from XLT file from within Java & J2SE applications. Define search criteria to find all matching image watermarks from the whole or specific pages of the source document."

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
    title_left: "Search Watermarks from XLT in Java"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/) makes it easy for Java developers to intelligently search image watermarks from within their documents by implementing a few easy steps.

        *   Instantiate **Watermarker** with input XLT document.
        *   Initialize **ImageSearchCriteria** to perform watermark search.
        *   Set maximum allowed difference between images.
        *   Display the possible matching watermarks.
        
    title_right: "System Requirements"
    content_right: |
        Before executing the code example below, please make sure that you have the following prerequisites installled on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: NetBeans, IntelliJ IDEA, Eclipse
        *   Frameworks: Java 7 (1.7) and above
        *   Download the latest version of GroupDocs.Watermark for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
        
    code: |
        ```cs
        // search possible IMAGE watermarks in XLT document using Java.
        // Instantiate Watermarker with input XLT document
        Watermarker watermarker = new Watermarker(input.xlt);
        
        // Initialize ImageSearchCriteria to start watermark search
        ImageSearchCriteria imageSearchCriteria = new ImageDctHashSearchCriteria(watermark.jpeg);

        // Set maximum allowed difference between sample image and the possible watermark
        imageSearchCriteria.setMaxDifference(0.9);
        PossibleWatermarkCollection possibleWatermarks = watermarker.search(imageSearchCriteria);
        System.out.println("Found " + possibleWatermarks.getCount() + " possible watermark(s).");

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