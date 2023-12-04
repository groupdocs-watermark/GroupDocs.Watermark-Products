
---
############################# Static ############################
layout: "autogen"
date: 2023-12-04T15:21:04
draft: false
path: "watermark/java/edit/text/excel/"
otherformats: PDF WORD EXCEL VISIO PRESENTATION SPREADSHEET WORKSHEET DOC DOCM DOCX DOT DOTM DOTX EXCEL ODT POT POTM POTX PPS PPSM PPSX PPT PPTM PPTX RTF SXC TXT VDW VDX VSD VSDM VSDX VSS VSSM VSSX VST VSTM VSTX VSX VTX WORD XLAM XLS XLSB XLSM XLSX XLT XLTM XLTX

############################# Head ############################
head_title: "Edit Text Watermark in EXCEL in Java"
head_description: "Java library to edit a found text watermark in a EXCEL file in Java applications using GroupDocs.Watermark API for Java."

############################# Header ############################
title: "Edit Text Watermark in EXCEL in Java"
description: "Search & modify a found text watermark in a EXCEL document with formatting within Java & J2SE applications. Manage the watermark size, font type, rotation angle and position of the watermark on the document pages, as you may need."

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
    title_left: "Edit Text Watermark in EXCEL File in Java"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/) makes it easy for Java developers to edit text watermarks in their applications by implementing a few easy steps.

        *   Instantiate **Watermarker** with input EXCEL document.
        *   Initialize **TextSearchCriteria** to search the text watermarks.
        *   Edit text of the found watermarks.
        *   Set watermark properties (font style, color etc).
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
        // Find & update text watermark with formatting in a EXCEL in Java applications
        // Instantiate Watermarker with input EXCEL document
        Watermarker watermarker = new Watermarker("input.excel")
        
        // Initialize the TextSearchCriteria to find the text watermarks
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        for (PossibleWatermark watermark : watermarks)
        {
            try
            {
                // Edit text and set watermark properties
                watermark.getFormattedTextFragments().clear();
                watermark.getFormattedTextFragments().add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
            }
            catch (Exception ex)
            {
                // Found entity may not support text editing
                // Passed arguments can have inappropriate value
                // Process such cases here
            }
        }
            
        // Save the updated document
        watermarker.save("output.excel");

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