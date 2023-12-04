<% configRef "..\\configs\\edit\\config_net_image.yml" %>
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
<% set "OtherFormats" (dict "otherformats_edit.image") %>

---
############################# Static ############################
layout: "autogen"
date: <% date "utcnow" %>
draft: false
path: "watermark/<% lower (get "ProductCode") %>/<% lower (get "Operation") %>/<% (get "WatermarktypeLow") %>/<% lower (get "Fileformat") %>/"
otherformats: <% get "OtherFormats" %>

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
        using (Watermarker watermarker = new Watermarker("input.<% (get "FileformatLow") %>"))
        {
            // <% "{net_image.example.coment3}" %>
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                try
                {
                    // <% "{net_image.example.coment4}" %>
                    watermark.ImageData = imageData;
                }
                catch (Exception e)
                {
                    // <% "{net_image.example.coment5}" %>
                    // <% "{net_image.example.coment6}" %>
                    // <% "{net_image.example.coment7}" %>
                }
            }
            // <% "{net_image.example.coment8}" %>
            watermarker.Save("output.<% (get "FileformatLow") %>");
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