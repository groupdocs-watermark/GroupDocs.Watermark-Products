
---
############################# Static ############################
layout: "autogen"
date: 2023-12-05T14:00:15
draft: false
path: "watermark/java/remove/text/presentation/"
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
        Watermarker watermarker = new Watermarker("input.presentation")
        
        PossibleWatermarkCollection possibleWatermarks = watermarker.search();

        // {java_text.example.coment3}
        possibleWatermarks.removeAt(0);

        // {java_text.example.coment4}
        possibleWatermarks.remove(possibleWatermarks.get_Item(0));

        // {java_text.example.coment5}
        watermarker.save("output.doc");

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