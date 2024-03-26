<% configRef "..\\configs\\index\\index_java.yml" %>
<% include "..\\data\\platform_data.md" %>
---
############################# Static ############################
layout: "landing"
date: <% date "utcnow" %>
draft: false

lang: <% lower ( get "lang") %>
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "<% "{index-content-java.head_title}" %>"
head_description: "<% "{index-content-java.head_description}" %>"

############################# Header ############################
title: "<% "{index-content-java.title}" %>"
description: "<% "{index-content-java.description}" %>"
words:
  for: "<% "{index-content.words_for}" %>"

actions:
  main: "<% "{index-content-java.actions_main}" %>"
  main_link: "<% get "PackageUrl" %>"
  alt: "<% "{index-content.actions.alt}" %>"
  alt_link: "<% get "PricesUrl" %>"
  title: "<% "{index-content.actions.title}" %>"
  description: "<% "{index-content.actions.description}" %>"

release:
  title: "<% "{index-content.release_title}" %>"
  notes: "<% "{index-content.release_notes}" %>"
  downloads: "<% "{index-content.release_downloads}" %>"

code:
  title: "<% "{index-content-java.code_title}" %>"
  more: "<% "{index-content.code_more}" %>"
  more_link: "<% dict "products.java.more_link" %>"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-watermark</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // <% "{index-content.code_comment_1}" %>
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // <% "{index-content.code_comment_2}" %>
    TextWatermark textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // <% "{index-content.code_comment_3}" %>
    watermarker.add(textWatermark);

    // <% "{index-content.code_comment_4}" %>
    watermarker.save("result.pdf");
    watermarker.close();
      
    ```

############################# Overview ############################
overview:
  enable: true
  title: "<% "{index-content.overview_title}" %>"
  description: "<% "{index-content-java.overview_description}" %>"
  features:
    # feature loop
    - title: "<% "{index-content-java.overview_feature_1.title}" %>"
      content: "<% "{index-content-java.overview_feature_1.description}" %>"

    # feature loop
    - title: "<% "{index-content-java.overview_feature_2.title}" %>"
      content: "<% "{index-content-java.overview_feature_2.description}" %>"

    # feature loop
    - title: "<% "{index-content-java.overview_feature_3.title}" %>"
      content: "<% "{index-content-java.overview_feature_3.description}" %>"

    # feature loop
    - title: "<% "{index-content-java.overview_feature_4.title}" %>"
      content: "<% "{index-content-java.overview_feature_4.description}" %>"

############################# Platforms ############################
platforms:
  enable: true
  title: "<% "{index-content.platforms.title}" %>"
  description: "<% "{index-content-java.platforms_description}" %>"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "<% "{index-content.formats_title}" %>"
  description: |
    <% "{index-content-java.formats_description}" %>
  groups:
    # group loop
    - color: "green"
      content: |
        ### <% "{index-content.formats_groups.title_1}" %>
        * **<% "{index-content.formats_groups.format_portable}" %>:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### <% "{index-content.formats_groups.title_2}" %>
        * **<% "{index-content.formats_groups.format_popular_images}" %>:** BMP, JPG, JPEG, PNG
        * **<% "{index-content.formats_groups.format_multi_images}" %>:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### <% "{index-content.formats_groups.title_3}" %>
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "<% "{index-content-java.features.title}" %>"
  description: "<% "{index-content-java.features.description}" %>"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "<% "{index-content-java.features.feature_1.title}" %>"
      content: "<% "{index-content-java.features.feature_1.content}" %>"

    # feature loop
    - icon: "watermark_style"
      title: "<% "{index-content-java.features.feature_2.title}" %>"
      content: "<% "{index-content-java.features.feature_2.content}" %>"

    # feature loop
    - icon: "hidden_print"
      title: "<% "{index-content-java.features.feature_3.title}" %>"
      content: "<% "{index-content-java.features.feature_3.content}" %>"

    # feature loop
    - icon: "image_only"
      title: "<% "{index-content-java.features.feature_4.title}" %>"
      content: "<% "{index-content-java.features.feature_4.content}" %>"

    # feature loop
    - icon: "image_frame"
      title: "<% "{index-content-java.features.feature_5.title}" %>"
      content: "<% "{index-content-java.features.feature_5.content}" %>"

    # feature loop
    - icon: "attachments"
      title: "<% "{index-content-java.features.feature_6.title}" %>"
      content: "<% "{index-content-java.features.feature_6.content}" %>"

    # feature loop
    - icon: "pdf_objects"
      title: "<% "{index-content-java.features.feature_7.title}" %>"
      content: "<% "{index-content-java.features.feature_7.content}" %>"

    # feature loop
    - icon: "doc_background"
      title: "<% "{index-content-java.features.feature_8.title}" %>"
      content: "<% "{index-content-java.features.feature_8.content}" %>"

    # feature loop
    - icon: "unreadable_characters"
      title: "<% "{index-content-java.features.feature_9.title}" %>"
      content: "<% "{index-content-java.features.feature_9.content}" %>"

    # feature loop
    - icon: "watermark_text_search"
      title: "<% "{index-content-java.features.feature_10.title}" %>"
      content: "<% "{index-content-java.features.feature_10.content}" %>"

    # feature loop
    - icon: "watermark_image_search"
      title: "<% "{index-content-java.features.feature_11.title}" %>"
      content: "<% "{index-content-java.features.feature_11.content}" %>"

    # feature loop
    - icon: "document_info"
      title: "<% "{index-content-java.features.feature_12.title}" %>"
      content: "<% "{index-content-java.features.feature_12.content}" %>"

############################# Code samples ############################
code_samples:
  enable: true
  title: "<% "{index-content.code_samples.title}" %>"
  description: "<% "{index-content-java.code_samples_description}" %>"
  items:
    # code sample loop
    - title: "<% "{index-content-java.code_title_sample_1}" %>"
      content: |
        <% "{index-content-java.code_samples_sample_1_content}" %>
        {{< landing/code title="<% "{index-content.code_samples.sample_1.code_title}" %>">}}
        ```csharp {style=abap}
        // <% "{index-content.code_samples.sample_1.comment_1}" %>
        Watermarker watermarker = new Watermarker("document.pdf");
        
        // <% "{index-content.code_samples.sample_1.comment_2}" %>
        ImageWatermark watermark = new ImageWatermark("watermark.jpg");

        // <% "{index-content.code_samples.sample_1.comment_3}" %>
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "<% "{index-content-java.code_title_sample_2}" %>"
      content: |
        <% "{index-content-java.code_samples_sample_2_content}" %>
        {{< landing/code title="<% "{index-content.code_samples.sample_2.code_title}" %>">}}
        ```csharp {style=abap}   
        // <% "{index-content.code_samples.sample_2.comment_1}" %>
        Watermarker watermarker = new Watermarker("document.pdf");

        // <% "{index-content.code_samples.sample_2.comment_2}" %>
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);                               
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);                             

        // <% "{index-content.code_samples.sample_2.comment_3}" %>
        for (PossibleWatermark watermark : watermarks)                                                           
        {  
            watermark.setText("New Text");
        }

        // <% "{index-content.code_samples.sample_2.comment_4}" %>
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
