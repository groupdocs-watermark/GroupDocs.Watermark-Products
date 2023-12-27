---
############################# Static ############################
layout: "autogen"
draft: false
path: "watermark/java/edit/image/doc/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

############################# Head ############################
head_title: "Edit Image Watermark in DOC in Java"
head_description: "Java library to edit a found image watermark in a DOC file in Java & J2SE applications using GroupDocs.Watermark APIs for Java."

############################# Header ############################
title: "Edit Image Watermark in DOC in Java"
description: "Search for and edit image watermarks in DOC documents in Java and J2SE applications. You can also add watermarks to the documents in BMP, PNG, GIF, and JPEG formats. You have the flexibility to control the size, font, rotation angle, and position of the watermark on the document pages as per your requirements."

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
    title_left: "Edit Image Watermarks in DOC File in Java"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/) makes it easy for Java developers to edit image (BMP, PNG, GIF or JPEG) watermarks in their applications by implementing a few easy steps.

        *   Instantiate **Watermarker** with input DOC document.
        *   Initialize **SearchCriteria** to find the image watermarks.
        *   Replace the found watermark.
        *   Save the newly watermarked document.
        
    title_right: "System Requirements"
    content_right: |
        Before executing the code example below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: NetBeans, IntelliJ IDEA, Eclipse
        *   Frameworks: Java 7 (1.7) and above
        *   Download the latest version of GroupDocs.Watermark for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
        
    code: |
        ```cs
        // Find & replace image watermark in a DOC in Java applications
        // Instantiate Watermarker with input DOC document
        Watermarker watermarker = new Watermarker(input.doc)
        
        // Initialize the SearchCriteria to match a particular image
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria(logo.png);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        for (PossibleWatermark watermark : watermarks)
            {
                try
                {
                    // Replace the found image
                    watermark.setImageData(imageData);
                }
                
                catch (Exception e)
                {
                    // Found entity may not support text editing
                    // Passed arguments can have inappropriate value
                    // Process such cases here
                }
            }
            
            // Save the watermarked document
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