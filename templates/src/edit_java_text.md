<% configRef "..\\configs\\edit\\config_java_text.yml" %>
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
<% set "OtherFormats" (dict "otherformats_edit.text") %>

---
############################# Static ############################
layout: "autogen"
date: <% date "utcnow" %>
draft: false
path: "watermark/<% lower (get "ProductCode") %>/<% lower (get "Operation") %>/<% (get "WatermarktypeLow") %>/<% lower (get "Fileformat") %>/"
otherformats: <% get "OtherFormats" %>

############################# Head ############################
head_title: "<% "{java_text.head.title}" %>"
head_description: "<% "{java_text.head.description}" %>"

############################# Header ############################
title: "<% "{java_text.header.title}" %>"
description: "<% "{java_text.header.description}" %>"

############################# SubMenu ############################
submenu:
    enable: true

############################# About ############################
about:
    enable: true
    title: "<% "{java_text.about.title}" %>"
    content: |
        <% "{java_text.about.content1}" %>
        
        <% "{java_text.about.content2}" %>

############################# Steps ############################
steps:
    enable: true
    title_left: "<% "{java_text.steps.title_left}" %>"
    content_left: |
        [GroupDocs.Watermark](<% lower (get "ProductUrl") %>) <% "{java_text.steps.content_left.description}" %>

        *   <% "{java_text.steps.content_left.step_1}" %>
        *   <% "{java_text.steps.content_left.step_2}" %>
        *   <% "{java_text.steps.content_left.step_3}" %>
        *   <% "{java_text.steps.content_left.step_4}" %>
        *   <% "{java_text.steps.content_left.step_5}" %>
        
    title_right: "<% "{java_text.steps.title_right}" %>"
    content_right: |
        <% "{java_text.steps.content_right.description}" %>

        *   <% "{java_text.steps.content_right.step_1}" %>
        *   <% "{java_text.steps.content_right.step_2}" %>
        *   <% "{java_text.steps.content_right.step_3}" %>
        *   <% "{java_text.steps.content_right.step_4}" %> [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
        
    code: |
        ```cs
        // <% "{java_text.example.coment1}" %>
        // <% "{java_text.example.coment2}" %>
        Watermarker watermarker = new Watermarker("input.<% (get "FileformatLow") %>")
        
        // <% "{java_text.example.coment3}" %>
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        for (PossibleWatermark watermark : watermarks)
        {
            try
            {
                // <% "{java_text.example.coment4}" %>
                watermark.getFormattedTextFragments().clear();
                watermark.getFormattedTextFragments().add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
            }
            catch (Exception ex)
            {
                // <% "{java_text.example.coment5}" %>
                // <% "{java_text.example.coment6}" %>
                // <% "{java_text.example.coment7}" %>
            }
        }
            
        // <% "{java_text.example.coment8}" %>
        watermarker.save("output.<% (get "FileformatLow") %>");

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