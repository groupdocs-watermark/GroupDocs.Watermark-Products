---
############################# Static ############################
layout: "autogen"
draft: false
path: "watermark/java/add/image/doc/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

############################# Head ############################
head_title: "Add Image Watermark to DOC in Java"
head_description: "Java library to add image watermark to DOC file in Java & J2SE applications using GroupDocs.Watermark APIs for Java."

############################# Header ############################
title: "Add Image Watermark to DOC in Java"
description: "Adding image watermark to DOC files in Java & J2SE applications. Add BMP, PNG, GIF, and JPEG images as watermarks to your documents. You can also manage the watermark's size, alignment, rotation angle, and position on the document pages as per your requirements."

############################# SubMenu ############################
submenu:
    enable: true

############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java API"
    content: |
        GroupDocs.Watermark for Java is a comprehensive solution for managing watermarks in Java applications. With this tool, developers can easily perform operations such as adding, editing, searching, and deleting different types of watermarks from documents in popular file formats. It supports working with both text and image watermarks in a variety of documents, including PDF, Microsoft Word, Excel, PowerPoint, Visio, email, and image formats.
        
        GroupDocs.Watermark API supports all major operating systems and Java versions including J2SE 7.0 (1.7), J2SE 8.0 (1.8), and Java 10.

############################# Steps ############################
steps:
    enable: true
    title_left: "Add Image Watermark to DOC File in Java"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/) makes it easy for Java developers to add image (BMP, PNG, GIF or JPEG) watermarks in their applications by implementing a few easy steps.

        *   Instantiate **Watermarker** with input DOC document.
        *   Use the image watermark path as the constructor parameter of the **ImageWatermark** class.
        *   Set watermark properties (size, alignment, color etc).
        *   Add watermark to the watermarker object and generate the output document.
        
    title_right: "System Requirements"
    content_right: |
        Before executing the code example below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: NetBeans, IntelliJ IDEA, Eclipse
        *   Frameworks: Java 7 (1.7) and above
        *   Download the latest version of GroupDocs.Watermark for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
        
    code: |
        ```cs
        // Add image watermark to DOC in Java applications
        // Instantiate Watermarker with input DOC document
        Watermarker watermarker = new Watermarker(input.doc)
        
        // Use image watermark path as constructor parameter of ImageWatermark class
        ImageWatermark watermark = new ImageWatermark(watermark.png)
        
        // Set watermark properties (width, height, alignment)
        watermark.Width = 140;
        watermark.Height = 140;
        watermark.HorizontalAlignment = HorizontalAlignment.Center;
        watermark.VerticalAlignment = VerticalAlignment.Center;

        //Add watermark to the watermarker object and generate an output document
        watermarker.add(watermark);
        watermarker.save(output.doc);

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