---
############################# Static ############################
layout: "landing"
date: 2023-12-04T15:21:06
draft: false
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "{index-content.head_title}"
head_description: "{index-content.head_description}"

############################# Header ############################
title: "{index-content.title_1}<br>{index-content-java.title_2}"
description: "{index-content.description}"
words:
  for: "{index-content.words_for}"

actions:
  main: "{index-content-java.actions_main}"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "{index-content.actions_alt}"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java"
  title: "{index-content.actions_title}"
  description: "{index-content.actions_description}"

release:
  title: "{index-content.release_title}"
  notes: "{index-content.release_notes}"
  downloads: "{index-content.release_downloads}"

code:
  title: "{index-content-java.code_title}"
  more: "{index-content.code_more}"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // {index-content.code_comment_1}
    Signature signature = new Signature("sample.pdf");
    
    // {index-content.code_comment_2}
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // {index-content.code_comment_4}
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "{index-content.overview_title}"
  description: "{index-content-java.overview_description}"
  features:
    # feature loop
    - title: "{index-content-java.overview_feature_1.title}"
      content: "{index-content-java.overview_feature_1.description}"

    # feature loop
    - title: "{index-content-java.overview_feature_2.title}"
      content: "{index-content-java.overview_feature_2.description}"

    # feature loop
    - title: "{index-content-java.overview_feature_3.title}"
      content: "{index-content-java.overview_feature_3.description}"

############################# Platforms ############################
platforms:
  enable: true
  title: "{index-content.platforms_title}"
  description: "{index-content-java.platforms_description}"
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
  title: "{index-content.formats_title}"
  description: |
    {index-content-java.formats_description}
  groups:
    # group loop
    - color: "green"
      content: |
        ### {index-content.formats_groups.title_1}
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### {index-content.formats_groups.title_2}
        * **{index-content.formats_groups.format_portable}:** PDF
        * **{index-content.formats_groups.format_images}:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **{index-content.formats_groups.format_other_office}:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### {index-content.formats_groups.title_3}
        * **{index-content.formats_groups.format_web}:** HTML, MHTML
        * **{index-content.formats_groups.format_archives}:** ZIP, TAR, 7Z
        * **{index-content.formats_groups.format_certificates}:** PFX

############################# Features ############################
features:
  enable: true
  title: "{index-content-java.features.title}"
  description: "{index-content-java.features.description}"

  items:
    # feature loop
    - icon: "sign"
      title: "{index-content-java.features.feature_1.title}"
      content: "{index-content-java.features.feature_1.content}"

    # feature loop
    - icon: "custom"
      title: "{index-content-java.features.feature_2.title}"
      content: "{index-content-java.features.feature_2.content}"

    # feature loop
    - icon: "password"
      title: "{index-content-java.features.feature_3.title}"
      content: "{index-content-java.features.feature_3.content}"

    # feature loop
    - icon: "protect"
      title: "{index-content-java.features.feature_4.title}"
      content: "{index-content-java.features.feature_4.content}"

    # feature loop
    - icon: "convert"
      title: "{index-content-java.features.feature_5.title}"
      content: "{index-content-java.features.feature_5.content}"

    # feature loop
    - icon: "preview"
      title: "{index-content-java.features.feature_6.title}"
      content: "{index-content-java.features.feature_6.content}"

    # feature loop
    - icon: "search"
      title: "{index-content-java.features.feature_7.title}"
      content: "{index-content-java.features.feature_7.content}"

    # feature loop
    - icon: "validate"
      title: "{index-content-java.features.feature_8.title}"
      content: "{index-content-java.features.feature_8.content}"

    # feature loop
    - icon: "update"
      title: "{index-content-java.features.feature_9.title}"
      content: "{index-content-java.features.feature_9.content}"

############################# Code samples ############################
code_samples:
  enable: true
  title: "{index-content.code_samples.title}"
  description: "{index-content-java.code_samples_description}"
  items:
    # code sample loop
    - title: "{index-content-java.code_title_sample_1}"
      content: |
        {index-content-java.code_samples_sample_1_content_1} {index-content-java.code_samples_sample_1_content_2}
        {{< landing/code title="{index-content-java.code_title_sample_1}">}}
        ```java {style=abap}
        // {index-content.code_samples.sample_1.comment_1}
        Signature signature = new Signature("file_to_sign.pdf");
        
        // {index-content.code_samples.sample_1.comment_2}
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // {index-content.code_samples.sample_1.comment_3}
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // {index-content.code_samples.sample_1.comment_4}
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "{index-content-java.code_title_sample_2}"
      content: |
        {index-content-java.code_samples_sample_2_content_1} {index-content-java.code_samples_sample_2_content_2}
        {{< landing/code title="{index-content-java.code_title_sample_2}">}}
        ```java {style=abap}   
        // {index-content.code_samples.sample_2.comment_1}
        Signature signature = new Signature("file_to_sign.pdf");
        
        // {index-content.code_samples.sample_2.comment_2}
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // {index-content.code_samples.sample_2.comment_3}
        options.setPassword("1234567890");

        // {index-content.code_samples.sample_2.comment_4}
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---

