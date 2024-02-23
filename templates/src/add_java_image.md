<% configRef "..\\configs\\add\\config_java_image.yml" %>
<% include "..\\data\\format_data.md" %>

---
############################# Static ############################
layout: "autogen"
date: <% date "utcnow" %>
draft: false
path: "watermark/<% lower (get "ProdCode") %>/<% lower (get "Operation") %>/<% (get "WatermarktypeLow") %>/<% lower (get "Fileformat") %>/"

############################# Head ############################
head_title: "<% "{java_image.head.title}" %>"
head_description: "<% "{java_image.head.description}" %>"

############################# Header ############################
title: "<% "{java_image.header.title}" %>"
description: "<% "{java_image.header.description}" %>"

############################# SubMenu ############################
submenu:
    enable: true

############################# About ############################
about:
    enable: true
    title: "<% "{java_image.about.title}" %>"
    content: |
        <% "{java_image.about.content1}" %>
        
        <% "{java_image.about.content2}" %>

############################# Steps ############################
steps:
    enable: true
    title_left: "<% "{java_image.steps.title_left}" %>"
    content_left: |
        [GroupDocs.Watermark](<% lower (get "ProductUrl") %>) <% "{java_image.steps.content_left.description}" %>

        *   <% "{java_image.steps.content_left.step_1}" %>
        *   <% "{java_image.steps.content_left.step_2}" %>
        *   <% "{java_image.steps.content_left.step_3}" %>
        *   <% "{java_image.steps.content_left.step_4}" %>
        
    title_right: "<% "{java_image.steps.title_right}" %>"
    content_right: |
        <% "{java_image.steps.content_right.description}" %>

        *   <% "{java_image.steps.content_right.step_1}" %>
        *   <% "{java_image.steps.content_right.step_2}" %>
        *   <% "{java_image.steps.content_right.step_3}" %>
        *   <% "{java_image.steps.content_right.step_4}" %> [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
        
    code: |
        ```cs
        // <% "{java_image.example.coment1}" %>
        // <% "{java_image.example.coment2}" %>
        Watermarker watermarker = new Watermarker("input.<% (get "FileFormat") %>")
        
        // <% "{java_image.example.coment3}" %>
        ImageWatermark watermark = new ImageWatermark("watermark.png")
        
        // <% "{java_image.example.coment4}" %>
        watermark.Width = 140;
        watermark.Height = 140;
        watermark.HorizontalAlignment = HorizontalAlignment.Center;
        watermark.VerticalAlignment = VerticalAlignment.Center;

        // <% "{example.coment5}" %>
        watermarker.add(watermark);
        watermarker.save("output.<% (get "FileFormat") %>");

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