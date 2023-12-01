<% configRef "..\\configs\\add\\config_java_image.yml" %>
<% set "Operation" (capitalize (get "operation")) %>
<% set "Watermarktype" (capitalize (get "watermarktype")) %>
<% set "WatermarktypeLow" (lower (get "watermarktype")) %>
<% set "Fileformat" (capitalize (get "fileformat")) %>
<% set "FileformatLow" (lower (get "fileformat")) %>
<% set "FileformatUpper" (upper (get "fileformat")) %>
<% set "ProductName" (dict "products.{product}.name") %>
<% set "ProductFullName" (dict "products.{product}.fullName") %>
<% set "ProductCode" (dict "products.{product}.code") %>
<% set "ProductUrl" (dict "products.{product}.url") %>
<% set "ProgLang" (dict "products.{product}.progLang") %>
<% set "SrcFileExt" (dict "products.{product}.srcFileExt") %>
<% set "DevEnv" (dict "products.{product}.devEnv") %>
<% set "Runtime" (dict "products.{product}.runtime") %>
<% set "RepoName" (dict "products.{product}.repoName") %>
<% set "RepoUrl" (dict "products.{product}.repoUrl") %>
<% set "OtherFormats" (dict "otherformats_add.image") %>

---
############################# Static ############################
layout: "autogen"
date: <% date "utcnow" %>
draft: false
path: "watermark/<% lower (get "ProductCode") %>/<% lower (get "Operation") %>/<% (get "WatermarktypeLow") %>/<% lower (get "Fileformat") %>/"
otherformats: <% get "OtherFormats" %>

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
        Watermarker watermarker = new Watermarker("input.<% (get "FileformatLow") %>")
        
        // <% "{java_image.example.coment3}" %>
        ImageWatermark watermark = new ImageWatermark("watermark.png")
        
        // <% "{java_image.example.coment4}" %>
        watermark.Width = 140;
        watermark.Height = 140;
        watermark.HorizontalAlignment = HorizontalAlignment.Center;
        watermark.VerticalAlignment = VerticalAlignment.Center;

        // <% "{example.coment5}" %>
        watermarker.add(watermark);
        watermarker.save("output.<% (get "FileformatLow") %>");

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