<% configRef "..\\configs\\remove\\config_net_text.yml" %>
<% include "..\\data\\format_data.md" %>

---
############################# Static ############################
layout: "autogen"
date: <% date "utcnow" %>
draft: false
path: "watermark/<% lower (get "ProdCode") %>/<% lower (get "Operation") %>/<% (get "WatermarktypeLow") %>/<% lower (get "Fileformat") %>/"

############################# Head ############################
head_title: "<% "{net_text.head.title}" %>"
head_description: "<% "{net_text.head.description}" %>"

############################# Header ############################
title: "<% "{net_text.header.title}" %>"
description: "<% "{net_text.header.description}" %>"

############################# SubMenu ############################
submenu:
    enable: true

############################# About ############################
about:
    enable: true
    title: "<% "{net_text.about.title}" %>"
    content: |
        <% "{net_text.about.content1}" %>
        
        <% "{net_text.about.content2}" %>

############################# Steps ############################
steps:
    enable: true
    title_left: "<% "{net_text.steps.title_left}" %>"
    content_left: |
        [GroupDocs.Watermark](<% lower (get "ProductUrl") %>) <% "{net_text.steps.content_left.description}" %>

        *   <% "{net_text.steps.content_left.step_1}" %>
        *   <% "{net_text.steps.content_left.step_2}" %>
        *   <% "{net_text.steps.content_left.step_3}" %>
        *   <% "{net_text.steps.content_left.step_4}" %>
        
    title_right: "<% "{net_text.steps.title_right}" %>"
    content_right: |
        <% "{net_text.steps.content_right.description}" %>

        *   <% "{net_text.steps.content_right.step_1}" %>
        *   <% "{net_text.steps.content_right.step_2}" %>
        *   <% "{net_text.steps.content_right.step_3}" %>
        *   <% "{net_text.steps.content_right.step_4}" %> [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)
        
    code: |
        ```cs
        // <% "{net_text.example.coment1}" %>
        // <% "{net_text.example.coment2}" %>
        using (Watermarker watermarker = new Watermarker("input.<% (get "FileFormat") %>"))
        {
            // <% "{net_text.example.coment3}" %>
            TextFormattingSearchCriteria criteria = new TextFormattingSearchCriteria();
            criteria.ForegroundColorRange = new ColorRange();
            criteria.ForegroundColorRange.MinHue = -5;
            criteria.ForegroundColorRange.MaxHue = 10;
            criteria.ForegroundColorRange.MinBrightness = 0.01f;
            criteria.ForegroundColorRange.MaxBrightness = 0.99f;
            criteria.BackgroundColorRange = new ColorRange();
            criteria.BackgroundColorRange.IsEmpty = true;
            criteria.FontName = "Arial";
            criteria.MinFontSize = 19;
            criteria.MaxFontSize = 42;
            criteria.FontBold = true;

            PossibleWatermarkCollection watermarks = watermarker.Search(criteria);
            watermarks.Clear();

            // <% "{net_text.example.coment4}" %>
            watermarker.Save("output.doc");
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