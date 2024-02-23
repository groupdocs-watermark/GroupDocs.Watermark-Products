
---
############################# Static ############################
layout: "autogen"
date: 2023-12-04T15:21:05
draft: false
path: "watermark/java/edit/text/xlsm/"
otherformats: PDF WORD EXCEL VISIO PRESENTATION SPREADSHEET WORKSHEET DOC DOCM DOCX DOT DOTM DOTX EXCEL ODT POT POTM POTX PPS PPSM PPSX PPT PPTM PPTX RTF SXC TXT VDW VDX VSD VSDM VSDX VSS VSSM VSSX VST VSTM VSTX VSX VTX WORD XLAM XLS XLSB XLSM XLSX XLT XLTM XLTX

############################# Head ############################
head_title: "{java_text.head.title}"
head_description: "{java_text.head.description}"

############################# Header ############################
title: "{java_text.header.title}"
description: "{java_text.header.description}"

############################# SubMenu ############################
submenu:
    enable: true

############################# About ############################
about:
    enable: true
    title: "{java_text.about.title}"
    content: |
        {java_text.about.content1}
        
        {java_text.about.content2}

############################# Steps ############################
steps:
    enable: true
    title_left: "{java_text.steps.title_left}"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/) {java_text.steps.content_left.description}

        *   {java_text.steps.content_left.step_1}
        *   {java_text.steps.content_left.step_2}
        *   {java_text.steps.content_left.step_3}
        *   {java_text.steps.content_left.step_4}
        *   {java_text.steps.content_left.step_5}
        
    title_right: "{java_text.steps.title_right}"
    content_right: |
        {java_text.steps.content_right.description}

        *   {java_text.steps.content_right.step_1}
        *   {java_text.steps.content_right.step_2}
        *   {java_text.steps.content_right.step_3}
        *   {java_text.steps.content_right.step_4} [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
        
    code: |
        ```cs
        // {java_text.example.coment1}
        // {java_text.example.coment2}
        Watermarker watermarker = new Watermarker("input.xlsm")
        
        // {java_text.example.coment3}
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        for (PossibleWatermark watermark : watermarks)
        {
            try
            {
                // {java_text.example.coment4}
                watermark.getFormattedTextFragments().clear();
                watermark.getFormattedTextFragments().add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
            }
            catch (Exception ex)
            {
                // {java_text.example.coment5}
                // {java_text.example.coment6}
                // {java_text.example.coment7}
            }
        }
            
        // {java_text.example.coment8}
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