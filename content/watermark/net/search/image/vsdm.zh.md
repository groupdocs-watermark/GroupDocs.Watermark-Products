
---
############################# Static ############################
layout: "autogen"
date: 2023-12-05T16:03:06
draft: false
path: "watermark/net/search/image/vsdm/"
otherformats: PDF WORD EXCEL VISIO PRESENTATION SPREADSHEET WORKSHEET DOC DOCM DOCX DOT DOTM DOTX EXCEL ODT POT POTM POTX PPS PPSM PPSX PPT PPTM PPTX RTF SXC TXT VDW VDX VSD VSDM VSDX VSS VSSM VSSX VST VSTM VSTX VSX VTX WORD XLAM XLS XLSB XLSM XLSX XLT XLTM XLTX

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
        using (Watermarker watermarker = new Watermarker("input.vsdm"))
        {
            // {net_image.example.coment3}
            ImageSearchCriteria imageSearchCriteria = new ImageDctHashSearchCriteria("watermark.jpeg");

            // {net_image.example.coment4}
            imageSearchCriteria.MaxDifference = 0.9;
            PossibleWatermarkCollection possibleWatermarks = watermarker.Search(imageSearchCriteria);
            Console.WriteLine("Found {0} possible watermark(s).", possibleWatermarks.Count);
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