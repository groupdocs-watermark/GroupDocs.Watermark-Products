
---
############################# Static ############################
layout: "autogen"
date: 2023-12-04T15:21:04
draft: false
path: "watermark/java/edit/image/xlsm/"
otherformats: PDF WORD EXCEL VISIO PRESENTATION SPREADSHEET WORKSHEET DOC DOCM DOCX DOT DOTM DOTX EXCEL ODT POT POTM POTX PPS PPSM PPSX PPT PPTM PPTX RTF SXC TXT VDW VDX VSD VSDM VSDX VSS VSSM VSSX VST VSTM VSTX VSX VTX WORD XLAM XLS XLSB XLSM XLSX XLT XLTM XLTX

############################# Head ############################
head_title: "Edit Image Watermark in XLSM using Java"
head_description: "Java library to edit a found image watermark in a XLSM file in Java & J2SE applications using GroupDocs.Watermark APIs for Java."

############################# Header ############################
title: "Edit Image Watermark in XLSM with Java"
description: "Find & modify a found image watermark in a XLSM document within Java & J2SE applications. Add BMP, PNG, GIF & JPEG image watermarks to the documents. Also manage the watermark size, font type, rotation angle and position of the watermark on the document pages, as you may need."

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
    title_left: "Edit Image Watermarks in XLSM File in Java"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/) makes it easy for Java developers to edit image (BMP, PNG, GIF or JPEG) watermarks in their applications by implementing a few easy steps.

        *   Instantiate **Watermarker** with input XLSM document.
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
        // Find & replace image watermark in a XLSM in Java applications
        // Instantiate Watermarker with input XLSM document
        Watermarker watermarker = new Watermarker("input.xlsm")
        
        // Initialize the SearchCriteria to match a particular image
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        for (PossibleWatermark watermark : watermarks)
            {
                try
                {
                    // Replace image which was found
                    watermark.setImageData(imageData);
                }
                
                catch (Exception ex)
                {
                    // Found entity may not support text editing
                    // Passed arguments can have inappropriate value
                    // Process such cases here
                }
            }
            
            // Save the updated document
            watermarker.save("output.xlsm");

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