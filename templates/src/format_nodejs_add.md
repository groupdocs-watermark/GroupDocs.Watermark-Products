<% configRef "..\\configs\\add\\config_nodejs_format.yml" %>
<% include "..\\data\\format_data.md" %>

---
############################# Static ############################
layout: "format"
date:  <% date "utcnow" %>
draft: false
lang: <% lower ( get "lang") %>
format: <% get "FileformatCap" %>
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "<% (dict "{product}.{fileformat}.head.title") %>"
head_description: "<% (dict "{product}.{fileformat}.head.description") %>"

############################# Header ############################
title: "<% (dict "{product}.{fileformat}.header.title") %>" 
description: "<% (dict "{product}.{fileformat}.header.description") %>"
subtitle: "<% (dict "{product}.{fileformat}.header.subtitle") %>" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "<% (dict "{product}.{fileformat}.header.action_title") %>"
      link: "<% get "ReleaseDownloads" %>"
      
############################# About ############################
about:
    enable: true
    title: "<% (dict "{product}.{fileformat}.about.title") %>"
    link: "/watermark/<% get "ProdCode" %>/"
    link_title: "<% "{common-content.texts.learn_more}" %>"
    picture: "about_viewer.svg" # 480 X 400
    content: |
       <% (dict "{product}.{fileformat}.about.content") %>

############################# Steps ############################
steps:
    enable: true
    title: "<% (dict "{product}.{fileformat}.steps.title") %>"
    content: |
      <% (dict "{product}.{fileformat}.steps.content.title") %>
      
      1. <% (dict "{product}.{fileformat}.steps.content.step_1") %>
      2. <% (dict "{product}.{fileformat}.steps.content.step_2") %>
      3. <% (dict "{product}.{fileformat}.steps.content.step_3") %>
      4. <% (dict "{product}.{fileformat}.steps.content.step_4") %>
   
    code:
      platform: "net"
      copy_title: "<% "{common-content.format-code.copy_title}" %>"
      install:
        command: "npm i @groupdocs/groupdocs.watermark"
        copy_tip: "<% "{common-content.format-code.copy_tip}" %>"
        copy_done: "<% "{common-content.format-code.copy_done}" %>"
      links:
        #  loop
        - title: "<% "{common-content.format-code.links.title_1}" %>"
          link: "<% get "MoreLink" %>"
        #  loop
        - title: "<% "{common-content.format-code.links.title_2}" %>"
          link: "<% get "DocsUrl" %>"
          
      content: |
        ```javascript {style=abap}

        // <% (dict "{product}.{fileformat}.steps.code.comments.comment_1") %>

        // <% (dict "{product}.{fileformat}.steps.code.comments.comment_2") %>
        const watermarker = new groupdocs.watermark.Watermarker("input.<% get "fileformat" %>");
        
        // <% (dict "{product}.{fileformat}.steps.code.comments.comment_3") %>
        const watermark = new groupdocs.watermark.ImageWatermark("watermark.png");
        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
        watermark.setVerticalAlignment(VerticalAlignment.Center);

        // <% (dict "{product}.{fileformat}.steps.code.comments.comment_4") %>
        watermarker.add(watermark);
        watermarker.save("output.<% get "fileformat" %>");
        
        ```            

############################# Actions ############################

actions:
  enable: true
  title: "<% "{common-content.format-actions.title}" %>"
  description: "<% "{common-content.format-actions.description}" %>"
  items:
    #  loop
    - title: "<% "{common-content.format-actions.comment_1}" %>"
      link: "<% get "ReleaseDownloads" %>"
      color: "red"
        #  loop
    - title: "<% "{common-content.format-actions.comment_2}" %>"
      link: "<% get "PricesUrl" %>"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "<% (dict "{product}.{fileformat}.formats.title") %>"
    exclude: "<% get "FileFormatUp" %>"
    description: "<% (dict "{product}.{fileformat}.formats.description") %>"
<% include "..\\data\\format_others.md" %>

---