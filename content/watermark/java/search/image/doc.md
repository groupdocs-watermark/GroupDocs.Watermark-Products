---
############################# Static ############################
layout: "autogen"
draft: false
path: "watermark/java/search/image/doc/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

############################# Head ############################
head_title: "Search Image Watermarks from DOC in Java"
head_description: "Java library to search image watermarks from DOC document using smart search features within Java & J2SE applications using GroupDocs.Watermark APIs for Java."

############################# Header ############################
title: "Search Image Watermarks from DOC in Java"
description: "Utilize a smart search function to locate all image watermarks in DOC files within Java & J2SE applications. Establish search criteria to identify matching image watermarks on any or specific pages of the source document."

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
    title_left: "Search Watermarks from DOC in Java"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/) makes it easy for Java developers to intelligently search image watermarks from within their documents by implementing a few easy steps.

        *   Instantiate **Watermarker** with input DOC document.
        *   Initialize **ImageSearchCriteria** to perform a watermark search.
        *   Set maximum allowed difference between images.
        *   Display the possible matching watermarks.
        
    title_right: "System Requirements"
    content_right: |
        Before executing the code example below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: NetBeans, IntelliJ IDEA, Eclipse
        *   Frameworks: Java 7 (1.7) and above
        *   Download the latest version of GroupDocs.Watermark for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
        
    code: |
        ```cs
        // search for possible image watermarks in a DOC document using Java.
        // Instantiate Watermarker with input DOC document
        Watermarker watermarker = new Watermarker(input.doc);
        
        // Initialize ImageSearchCriteria to start watermark search
        ImageSearchCriteria imageSearchCriteria = new ImageDctHashSearchCriteria(watermark.jpeg);

        // Set the maximum allowed difference between the sample image and the possible watermark
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