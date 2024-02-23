
---
############################# Static ############################
layout: "autogen"
date: 2023-12-01T17:51:41
draft: false
path: "watermark/net/add/image/vss/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

############################# Head ############################
head_title: "{net_image.head.title}"
head_description: "{net_image.head.description}"

############################# Header ############################
title: "{net_image.header.title}"
description: "{net_image.header.description}"

############################# SubMenu ############################
submenu:
    enable: true

############################# About ############################
about:
    enable: true
    title: "{net_image.about.title}"
    content: |
        {net_image.about.content1}
        
        {net_image.about.content2}

############################# Steps ############################
steps:
    enable: true
    title_left: "{net_image.steps.title_left}"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/) {net_image.steps.content_left.description}

        *   {net_image.steps.content_left.step_1}
        *   {net_image.steps.content_left.step_2}
        *   {net_image.steps.content_left.step_3}
        *   {net_image.steps.content_left.step_4}
        
    title_right: "{net_image.steps.title_right}"
    content_right: |
        {net_image.steps.content_right.description}

        *   {net_image.steps.content_right.step_1}
        *   {net_image.steps.content_right.step_2}
        *   {net_image.steps.content_right.step_3}
        *   {net_image.steps.content_right.step_4} [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)
        
    code: |
        ```cs
        // {net_image.example.coment1}
        // {net_image.example.coment2}
        using (Watermarker watermarker = new Watermarker("input.vss")
          {
            // {net_image.example.coment3}
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                // {net_image.example.coment4}
                watermark.Width = 140;
                watermark.Height = 140;
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;

                // {net_image.example.coment5}
                watermarker.Add(watermark);
                watermarker.Save("output.vss");
            }
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