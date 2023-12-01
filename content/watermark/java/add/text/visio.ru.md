
---
############################# Static ############################
layout: "autogen"
date: 2023-12-01T17:51:40
draft: false
path: "watermark/java/add/text/visio/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

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
        (Watermarker watermarker = new Watermarker("input.visio"))
        
        // {java_text.example.coment3}
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
            
        // {java_text.example.coment4}
        watermark.setForegroundColor(Color.getRed());
        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
        watermark.setVerticalAlignment(VerticalAlignment.Center);

        // {java_text.example.coment5}
        watermarker.add(watermark);
        watermarker.save("output.visio");
        
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