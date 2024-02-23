<% configRef "..\\configs\\remove\\config_net_image.yml" %>
<% include "..\\data\\format_data.md" %>

---
############################# Static ############################
layout: "autogen"
date: <% date "utcnow" %>
draft: false
path: "watermark/<% lower (get "ProdCode") %>/<% lower (get "Operation") %>/<% (get "WatermarktypeLow") %>/<% lower (get "Fileformat") %>/"

############################# Head ############################
head_title: "<% "{net_image.head.title}" %>"
head_description: "<% "{net_image.head.description}" %>"

############################# Header ############################
title: "<% "{net_image.header.title}" %>"
description: "<% "{net_image.header.description}" %>"

############################# SubMenu ############################
submenu:
    enable: true

############################# About ############################
about:
    enable: true
    title: "<% "{net_image.about.title}" %>"
    content: |
        <% "{net_image.about.content1}" %>
        
        <% "{net_image.about.content2}" %>

############################# Steps ############################
steps:
    enable: true
    title_left: "<% "{net_image.steps.title_left}" %>"
    content_left: |
        [GroupDocs.Watermark](<% lower (get "ProductUrl") %>) <% "{net_image.steps.content_left.description}" %>

        *   <% "{net_image.steps.content_left.step_1}" %>
        *   <% "{net_image.steps.content_left.step_2}" %>
        *   <% "{net_image.steps.content_left.step_3}" %>
        *   <% "{net_image.steps.content_left.step_4}" %>
        
    title_right: "<% "{net_image.steps.title_right}" %>"
    content_right: |
        <% "{net_image.steps.content_right.description}" %>

        *   <% "{net_image.steps.content_right.step_1}" %>
        *   <% "{net_image.steps.content_right.step_2}" %>
        *   <% "{net_image.steps.content_right.step_3}" %>
        *   <% "{net_image.steps.content_right.step_4}" %> [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)
        
    code: |
        ```cs
        // <% "{net_image.example.coment1}" %>
        // <% "{net_image.example.coment2}" %>
        using (Watermarker watermarker = new Watermarker("input.<% (get "FileFormat") %>"))
        {
            // <% "{net_image.example.coment3}" %>
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria(logo.png);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            // <% "{net_image.example.coment4}" %>
            possibleWatermarks.Remove(possibleWatermarks[0]);

            // <% "{net_image.example.coment5}" %>
            watermarker.Save("output.<% (get "FileFormat") %>");
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