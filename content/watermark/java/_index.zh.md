---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:29
draft: false

lang: zh
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
head_title: "Java 水印库 | 为文档添加水印"
head_description: "原生 Java 软件，用于在 PDF、Word、Excel、演示文稿、Visio 图表、电子邮件和图像文件中添加和操作文本和图像水印。"

############################# Header ############################
title: "在 Java 个项目中轻松实现文档水印"
description: "借助 GroupDocs.Watermark 库为文件添加水印的功能，增强您的 Java 个应用程序。我们的 API 为各种流行的文件格式提供可自定义的水印。"
words:
  for: "为了"

actions:
  main: "从 Maven 免费下载"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "许可"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java/"
  title: "准备好开始了吗？"
  description: "免费试用 GroupDocs.Watermark 项功能或申请许可证"

release:
  title: "版本 {0} 已发布"
  notes: "查看新增内容"
  downloads: "下载"

code:
  title: "通过 Java 对 PDF 加水印"
  more: "更多例子"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-watermark</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // 通过 PDF 路径实例化 Watermarker
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // 自定义水印选项
    TextWatermark textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // 向 PDF 文档应用水印
    watermarker.add(textWatermark);

    // 保存结果文档
    watermarker.save("result.pdf");
    watermarker.close();
      
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark 一览"
  description: "专为使用 Java 技术添加水印而设计的库"
  features:
    # feature loop
    - title: "通过 Java 为文件添加水印"
      content: "使用 GroupDocs.Watermark for Java 保护您的商业文档。将文本、图像、图表或电子邮件附件作为水印添加到各种文件格式。"

    # feature loop
    - title: "根据特定需求自定义水印"
      content: "GroupDocs.Watermark for Java 为水印提供了大量的自定义选项。调整文本样式（粗体、斜体、字体）和图像属性（旋转等），根据您的特定目标定制水印流程。"

    # feature loop
    - title: "广泛格式支持"
      content: "GroupDocs.Watermark for Java 可与多种文件格式无缝集成，包括：PDF、Microsoft Office（Word、Excel、Excel、PowerPoint）、图像（JPEG、PNG、GIF、BMP）、Visio 图表和电子邮件。增强不同文件类型的文档安全性。"

    # feature loop
    - title: "轻松的水印搜索和管理"
      content: "高效管理文档中的现有水印。找到特定的水印，修改其文本、样式或图像，或将其完全删除。GroupDocs.Watermark for Java 简化了水印工作流程。"

############################# Platforms ############################
platforms:
  enable: true
  title: "平台独立性"
  description: "GroupDocs.Watermark for Java 支持各种操作系统和包管理器。"
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
  title: "支持的文件格式"
  description: |
    GroupDocs.Watermark for Java 支持处理各种文件格式。[查看完整列表](https://docs.groupdocs.com/watermark/java/supported-document-formats/)。
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office 和 OpenDocument 格式
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### 图像和图形
        * **流行的图像格式:** BMP, JPG, JPEG, PNG
        * **多页图片:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### 其他
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark for Java：功能"
  description: "通过添加水印来保护您的文件。支持各种格式，包括 PDF、Office 文档和图像。"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "文件水印"
      content: "为各种支持的文件格式在特定部分或整个文档中添加或删除水印。"

    # feature loop
    - icon: "watermark_style"
      title: "水印自定义"
      content: "使用颜色、字体、旋转等选项自定义水印的外观。"

    # feature loop
    - icon: "hidden_print"
      title: "PDF 的隐藏打印水印"
      content: "添加仅在打印 PDF 文档时出现的水印。"

    # feature loop
    - icon: "image_only"
      title: "选择性图像水印"
      content: "为特定部分、页面、幻灯片或整个文档中的所有图像添加水印。"

    # feature loop
    - icon: "image_frame"
      title: "为特定图像帧添加水印"
      content: "将水印应用于多帧图像中的特定框架。"

    # feature loop
    - icon: "attachments"
      title: "为附件和形状加水印"
      content: "为 Excel 个文档中的所有附件或演示文稿中的所有图像形状添加水印。"

    # feature loop
    - icon: "pdf_objects"
      title: "PDF 中的水印对齐"
      content: "将水印与 PDF 文档的不同区域对齐，包括出血框、艺术框、裁剪框和修剪框。"

    # feature loop
    - icon: "doc_background"
      title: "通过背景图像添加水印"
      content: "在电子表格或演示文稿中添加或删除背景图像水印。"

    # feature loop
    - icon: "unreadable_characters"
      title: "使用不可读字符进行保护"
      content: "使用带有不可读字符的文本水印保护演示文稿。"

    # feature loop
    - icon: "watermark_text_search"
      title: "搜索水印"
      content: "使用包括正则表达式在内的各种参数获取文件中显示的水印列表。"

    # feature loop
    - icon: "watermark_image_search"
      title: "查找相似的图像水印"
      content: "找到看起来像特定图像的图像水印。"

    # feature loop
    - icon: "document_info"
      title: "提取文档信息"
      content: "获取各种文档数据，例如支持的文件格式的页面设置。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "代码示例"
  description: "浏览说明典型 GroupDocs.Watermark for Java 功能的代码示例"
  items:
    # code sample loop
    - title: "使用图像给文档加水印"
      content: |
        利用 GroupDocs.Watermark for Java 通过添加图像水印来增强文档安全性。了解更多：[图片水印](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/)。
        {{< landing/code title="如何通过图像水印保护文件。">}}
        ```java {style=abap}
        // 将源文档加载到 Watermarker
        Watermarker watermarker = new Watermarker("document.pdf");
        
        // 指定水印图像的路径
        ImageWatermark watermark = new ImageWatermark("watermark.jpg");

        // 保护文件并将其保存
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "修改水印"
      content: |
        GroupDocs.Watermark for Java 使您能够管理文档中的现有水印。找到特定的水印并 [修改其属性](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/)。
        {{< landing/code title="水印搜索和修改。">}}
        ```java {style=abap}   
        // 加载源文档
        Watermarker watermarker = new Watermarker("document.pdf");

        // 搜索要更新的水印
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);                               
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);                             

        // 更新所需的属性
        for (PossibleWatermark watermark : watermarks)                                                           
        {  
            watermark.setText("New Text");
        }

        // 将修改后的文档保存到指定路径
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
