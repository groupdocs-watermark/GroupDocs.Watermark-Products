
---
############################# Static ############################
layout: "autogen"
date: 2023-12-04T15:21:06
draft: false
path: "watermark/net/edit/text/odt/"
otherformats: PDF WORD EXCEL VISIO PRESENTATION SPREADSHEET WORKSHEET DOC DOCM DOCX DOT DOTM DOTX EXCEL ODT POT POTM POTX PPS PPSM PPSX PPT PPTM PPTX RTF SXC TXT VDW VDX VSD VSDM VSDX VSS VSSM VSSX VST VSTM VSTX VSX VTX WORD XLAM XLS XLSB XLSM XLSX XLT XLTM XLTX

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
        using (Watermarker watermarker = new Watermarker("input.odt"))
        {
            // {net_text.example.coment3}
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                try
                {
                     // {net_text.example.coment4}
                     watermark.FormattedTextFragments.Clear();
                     watermark.FormattedTextFragments.Add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
                }
                catch (Exception e)
                {
                    // {net_text.example.coment5}
                    // {net_text.example.coment6}
                    // {net_text.example.coment7}
                }
            }
            
            // {net_text.example.coment8}
            watermarker.Save("output.odt");
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