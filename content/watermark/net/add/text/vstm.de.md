
---
############################# Static ############################
layout: "autogen"
date: 2023-12-01T17:51:41
draft: false
path: "watermark/net/add/text/vstm/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

############################# Head ############################
head_title: "{net_text.head.title}"
head_description: "{net_text.head.description}"

############################# Header ############################
title: "{net_text.header.title}"
description: "{net_text.header.description}"

############################# SubMenu ############################
submenu:
    enable: true

############################# About ############################
about:
    enable: true
    title: "{net_text.about.title}"
    content: |
        {net_text.about.content1}
        
        {net_text.about.content2}

############################# Steps ############################
steps:
    enable: true
    title_left: "{net_text.steps.title_left}"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/) {net_text.steps.content_left.description}

        *   {net_text.steps.content_left.step_1}
        *   {net_text.steps.content_left.step_2}
        *   {net_text.steps.content_left.step_3}
        *   {net_text.steps.content_left.step_4}
        *   {net_text.steps.content_left.step_5}
        
    title_right: "{net_text.steps.title_right}"
    content_right: |
        {net_text.steps.content_right.description}

        *   {net_text.steps.content_right.step_1}
        *   {net_text.steps.content_right.step_2}
        *   {net_text.steps.content_right.step_3}
        *   {net_text.steps.content_right.step_4} [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)
        
    code: |
        ```cs
        // {net_text.example.coment1}
        // {net_text.example.coment2}
        using (Watermarker watermarker = new Watermarker("input.vstm"))
          {
            // {net_text.example.coment3}
            Font font = new Font("Arial", 19, FontStyle.Bold | FontStyle.Italic);
            
            // {net_text.example.coment4}
            TextWatermark watermark = new TextWatermark("my watermark", font);

            // {net_text.example.coment5}
            watermark.ForegroundColor = Color.Red;
            watermark.BackgroundColor = Color.Blue;
            watermark.TextAlignment = TextAlignment.Right;
            watermark.Opacity = 0.5;

            // {net_text.example.coment6}
            watermarker.Add(watermark);
            watermarker.Save("output.vstm");
          }
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