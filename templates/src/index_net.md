<% configRef "..\\configs\\index\\index_net.yml" %>
<% include "..\\data\\platform_data.md" %>
---
############################# Static ############################
layout: "landing"
date: <% date "utcnow" %>
draft: false

lang: <% lower ( get "lang") %>
product: "Watermark"
product_tag: "watermark"
platform: "Net"
platform_tag: "net"

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
head_title: "<% "{index-content-net.head_title}" %>"
head_description: "<% "{index-content-net.head_description}" %>"

############################# Header ############################
title: "<% "{index-content-net.title}" %>"
description: "<% "{index-content-net.description}" %>"
words:
  for: "<% "{index-content.words_for}" %>"

actions:
  main: "<% "{index-content-net.actions_main}" %>"
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
  title: "<% "{index-content-net.code_title}" %>"
  more: "<% "{index-content.code_more}" %>"
  more_link: "<% dict "products.net.more_link" %>"
  install: "dotnet add package GroupDocs.Watermark"
  content: |
    ```csharp {style=abap}   
    // <% "{index-content.code_comment_1}" %>
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    using (Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions))
    {
        // <% "{index-content.code_comment_2}" %>
        TextWatermark textWatermark = 
            new TextWatermark("Approved", new Font("Arial", 8));
        
        // <% "{index-content.code_comment_3}" %>
        watermarker.Add(textWatermark);

        // <% "{index-content.code_comment_4}" %>
        watermarker.Save("result.pdf");
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "<% "{index-content.overview_title}" %>"
  description: "<% "{index-content-net.overview_description}" %>"
  features:
    # feature loop
    - title: "<% "{index-content-net.overview_feature_1.title}" %>"
      content: "<% "{index-content-net.overview_feature_1.description}" %>"

    # feature loop
    - title: "<% "{index-content-net.overview_feature_2.title}" %>"
      content: "<% "{index-content-net.overview_feature_2.description}" %>"

    # feature loop
    - title: "<% "{index-content-net.overview_feature_3.title}" %>"
      content: "<% "{index-content-net.overview_feature_3.description}" %>"

    # feature loop
    - title: "<% "{index-content-net.overview_feature_4.title}" %>"
      content: "<% "{index-content-net.overview_feature_4.description}" %>"

############################# Platforms ############################
platforms:
  enable: true
  title: "<% "{index-content.platforms.title}" %>"
  description: "<% "{index-content-net.platforms_description}" %>"
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "<% "{index-content.formats_title}" %>"
  description: |
    <% "{index-content-net.formats_description}" %>
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
  title: "<% "{index-content-net.features.title}" %>"
  description: "<% "{index-content-net.features.description}" %>"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "<% "{index-content-net.features.feature_1.title}" %>"
      content: "<% "{index-content-net.features.feature_1.content}" %>"

    # feature loop
    - icon: "watermark_style"
      title: "<% "{index-content-net.features.feature_2.title}" %>"
      content: "<% "{index-content-net.features.feature_2.content}" %>"

    # feature loop
    - icon: "hidden_print"
      title: "<% "{index-content-net.features.feature_3.title}" %>"
      content: "<% "{index-content-net.features.feature_3.content}" %>"

    # feature loop
    - icon: "image_only"
      title: "<% "{index-content-net.features.feature_4.title}" %>"
      content: "<% "{index-content-net.features.feature_4.content}" %>"

    # feature loop
    - icon: "image_frame"
      title: "<% "{index-content-net.features.feature_5.title}" %>"
      content: "<% "{index-content-net.features.feature_5.content}" %>"

    # feature loop
    - icon: "attachments"
      title: "<% "{index-content-net.features.feature_6.title}" %>"
      content: "<% "{index-content-net.features.feature_6.content}" %>"

    # feature loop
    - icon: "pdf_objects"
      title: "<% "{index-content-net.features.feature_7.title}" %>"
      content: "<% "{index-content-net.features.feature_7.content}" %>"

    # feature loop
    - icon: "doc_background"
      title: "<% "{index-content-net.features.feature_8.title}" %>"
      content: "<% "{index-content-net.features.feature_8.content}" %>"

    # feature loop
    - icon: "unreadable_characters"
      title: "<% "{index-content-net.features.feature_9.title}" %>"
      content: "<% "{index-content-net.features.feature_9.content}" %>"

    # feature loop
    - icon: "watermark_text_search"
      title: "<% "{index-content-net.features.feature_10.title}" %>"
      content: "<% "{index-content-net.features.feature_10.content}" %>"

    # feature loop
    - icon: "watermark_image_search"
      title: "<% "{index-content-net.features.feature_11.title}" %>"
      content: "<% "{index-content-net.features.feature_11.content}" %>"

    # feature loop
    - icon: "document_info"
      title: "<% "{index-content-net.features.feature_12.title}" %>"
      content: "<% "{index-content-net.features.feature_12.content}" %>"

############################# Code samples ############################
code_samples:
  enable: true
  title: "<% "{index-content.code_samples.title}" %>"
  description: "<% "{index-content-net.code_samples_description}" %>"
  items:
    # code sample loop
    - title: "<% "{index-content-net.code_title_sample_1}" %>"
      content: |
        <% "{index-content-net.code_samples_sample_1_content}" %>
        {{< landing/code title="<% "{index-content.code_samples.sample_1.code_title}" %>">}}
        ```csharp {style=abap}
        // <% "{index-content.code_samples.sample_1.comment_1}" %>
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // <% "{index-content.code_samples.sample_1.comment_2}" %>
            using (ImageWatermark watermark = new ImageWatermark("watermark.jpg"))
            {
                // <% "{index-content.code_samples.sample_1.comment_3}" %>
                watermarker.Add(watermark);

                watermarker.Save("result.pdf");
            }
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "<% "{index-content-net.code_title_sample_2}" %>"
      content: |
        <% "{index-content-net.code_samples_sample_2_content}" %>
        {{< landing/code title="<% "{index-content.code_samples.sample_2.code_title}" %>">}}
        ```csharp {style=abap}   
        // <% "{index-content.code_samples.sample_2.comment_1}" %>
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // <% "{index-content.code_samples.sample_2.comment_2}" %>
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                // <% "{index-content.code_samples.sample_2.comment_3}" %>
                watermark.Text = "New Text";
            }

            // <% "{index-content.code_samples.sample_2.comment_4}" %>
            watermarker.Save("document.pdf");
        }
        ```
        {{< /landing/code >}}

---
