<% configRef "..\\configs\\index\\index_java.yml" %>
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
  main_link: "<% dict "products.java.main_link" %>"
  alt: "<% "{index-content.actions.alt}" %>"
  alt_link: "<% dict "products.java.alt_link" %>"
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
      <artifactId>groupdocs-comparison</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // <% "{index-content.code_comment_1}" %>
    try (Comparer comparer = new Comparer("source.docx"))
    {    
      // <% "{index-content.code_comment_2}" %>
      comparer.add("target.docx");

      // <% "{index-content.code_comment_3}" %>
      CompareOptions options = new CompareOptions();
      options.setShowRevisions(false);

      // <% "{index-content.code_comment_4}" %>
      final comparer.compare("result.docx", options);
    }    
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
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTX, RTF, TXT
        * **Excel:** XLS, XLT, XLSX, XLTM, XLSB, XLSM, XLSX
        * **PowerPoint:** POT, POTX, PPS, PPSX, PPTX, PPT        
        * **Outlook:** EML, EMLX, MSG
        * **OneNote:** ONE
        * **OpenDocument:** ODT, ODP, OTP, ODS, OTT
        * **<% "{index-content.formats_groups.format_fixed_page_layout}" %>:** PDF        
    # group loop
    - color: "blue"
      content: |
        ### <% "{index-content.formats_groups.title_2}" %>
        * **<% "{index-content.formats_groups.format_raster_images}" %>:** BMP, GIF, JPG, JPEG, PNG
        * **<% "{index-content.formats_groups.format_medical_imaging}" %>:** DICOM
        * **Microsoft Visio:** VSDX, VSD, VSS, VST, VDX
        * **AutoCAD Drawing:** DWG, DXF
      # group loop
    - color: "red"
      content: |
        ### <% "{index-content.formats_groups.title_3}" %>
        * **<% "{index-content.formats_groups.format_text}" %>:** TXT
        * **<% "{index-content.formats_groups.format_programming_languages}" %>:** CS, Java, CPP, JS, PY, RB, PL, ASM, GROOVY, JSON, PHP, SQL, LOG, DIFF, LESS, SCALA
        * **<% "{index-content.formats_groups.format_web}" %>:** HTM, HTML, MHT, MHTML
        * **<% "{index-content.formats_groups.format_e_books}" %>:** MOBI, DjVu
        * **<% "{index-content.formats_groups.format_delimiter_separated_values}" %>:** CSV

############################# Features ############################
features:
  enable: true
  title: "<% "{index-content-java.features.title}" %>"
  description: "<% "{index-content-java.features.description}" %>"

  items:
    # feature loop
    - icon: "compare"
      title: "<% "{index-content-java.features.feature_1.title}" %>"
      content: "<% "{index-content-java.features.feature_1.content}" %>"

    # feature loop
    - icon: "note-stack"
      title: "<% "{index-content-java.features.feature_2.title}" %>"
      content: "<% "{index-content-java.features.feature_2.content}" %>"

    # feature loop
    - icon: "stacks"
      title: "<% "{index-content-java.features.feature_3.title}" %>"
      content: "<% "{index-content-java.features.feature_3.content}" %>"

    # feature loop
    - icon: "rule"
      title: "<% "{index-content-java.features.feature_4.title}" %>"
      content: "<% "{index-content-java.features.feature_4.content}" %>"

    # feature loop
    - icon: "preview"
      title: "<% "{index-content-java.features.feature_5.title}" %>"
      content: "<% "{index-content-java.features.feature_5.content}" %>"

    # feature loop
    - icon: "two-pager"
      title: "<% "{index-content-java.features.feature_6.title}" %>"
      content: "<% "{index-content-java.features.feature_6.content}" %>"

    # feature loop
    - icon: "format_color_text"
      title: "<% "{index-content-java.features.feature_7.title}" %>"
      content: "<% "{index-content-java.features.feature_7.content}" %>"

    # feature loop
    - icon: "folder-managed"
      title: "<% "{index-content-java.features.feature_8.title}" %>"
      content: "<% "{index-content-java.features.feature_8.content}" %>"

    # feature loop
    - icon: "lock"
      title: "<% "{index-content-java.features.feature_9.title}" %>"
      content: "<% "{index-content-java.features.feature_9.content}" %>"

    # feature loop
    - icon: "select"
      title: "<% "{index-content-java.features.feature_10.title}" %>"
      content: "<% "{index-content-java.features.feature_10.content}" %>"

    # feature loop
    - icon: "speaker-notes"
      title: "<% "{index-content-java.features.feature_11.title}" %>"
      content: "<% "{index-content-java.features.feature_11.content}" %>"

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
        ```java {style=abap}
        // <% "{index-content.code_samples.sample_1.comment_1}" %>
        try (Comparer comparer = new Comparer("source.docx", new LoadOptions("1234")))
        {
            // <% "{index-content.code_samples.sample_1.comment_2}" %>
            comparer.add("target.docx", new LoadOptions("5678"));
        
            // <% "{index-content.code_samples.sample_1.comment_3}" %>
            comparer.compare("result.docx");
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "<% "{index-content-java.code_title_sample_2}" %>"
      content: |
        <% "{index-content-java.code_samples_sample_2_content}" %>
        {{< landing/code title="<% "{index-content.code_samples.sample_2.code_title}" %>">}}
        ```java {style=abap}   
        // <% "{index-content.code_samples.sample_2.comment_1}" %>
        try (Comparer comparer = new Comparer("source.docx") 
        {
            // <% "{index-content.code_samples.sample_2.comment_2}" %>
            comparer.add("target2.docx");

            // <% "{index-content.code_samples.sample_2.comment_3}" %>
            comparer.add("target3.docx");

            // <% "{index-content.code_samples.sample_2.comment_4}" %>
            comparer.compare("result.docx");
        }
        ```
        {{< /landing/code >}}

---
