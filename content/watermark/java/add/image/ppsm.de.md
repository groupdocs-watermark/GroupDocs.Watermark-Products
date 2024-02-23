
---
############################# Static ############################
layout: "autogen"
date: 2023-12-01T17:51:39
draft: false
path: "watermark/java/add/image/ppsm/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

############################# Head ############################
head_title: "{java_image.head.title}"
head_description: "{java_image.head.description}"

############################# Header ############################
title: "{java_image.header.title}"
description: "{java_image.header.description}"

############################# SubMenu ############################
submenu:
    enable: true

############################# About ############################
about:
    enable: true
    title: "{java_image.about.title}"
    content: |
        {java_image.about.content1}
        
        {java_image.about.content2}

############################# Steps ############################
steps:
    enable: true
    title_left: "{java_image.steps.title_left}"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/) {java_image.steps.content_left.description}

        *   {java_image.steps.content_left.step_1}
        *   {java_image.steps.content_left.step_2}
        *   {java_image.steps.content_left.step_3}
        *   {java_image.steps.content_left.step_4}
        
    title_right: "{java_image.steps.title_right}"
    content_right: |
        {java_image.steps.content_right.description}

        *   {java_image.steps.content_right.step_1}
        *   {java_image.steps.content_right.step_2}
        *   {java_image.steps.content_right.step_3}
        *   {java_image.steps.content_right.step_4} [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
        
    code: |
        ```cs
        // {java_image.example.coment1}
        // {java_image.example.coment2}
        Watermarker watermarker = new Watermarker("input.ppsm")
        
        // {java_image.example.coment3}
        ImageWatermark watermark = new ImageWatermark("watermark.png")
        
        // {java_image.example.coment4}
        watermark.Width = 140;
        watermark.Height = 140;
        watermark.HorizontalAlignment = HorizontalAlignment.Center;
        watermark.VerticalAlignment = VerticalAlignment.Center;

        // {example.coment5}
        watermarker.add(watermark);
        watermarker.save("output.ppsm");

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