---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java API 为 PDF Word Excel 图像添加搜索删除水印"
head_description: "Java 文档水印 API – 从文档中生成、搜索和删除水印：PDF、Word、Excel、演示文稿、Visio、电子邮件和图像文件格式."

############################# Header ############################
title: "用于处理水印的 Java API"
description: "开发 Java 应用程序以通过智能搜索和强大的安全性执行图像和文本水印操作."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Watermark for Java"
        image: "/border/groupdocs-watermark-java.svg"
        product: "GroupDocs.Watermark"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "概述"

            # button loop
            - link: "#features"
              text: "特征"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/watermark"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/watermark/java"
              text: "价钱"

    right:
        link_download: "https://downloads.groupdocs.com/watermark"
        link_learn: "https://docs.groupdocs.com/watermark/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# 概述 ############################
overview:
    enable: true
    content: |
      GroupDocs.Watermark for Java 允许您制作业务应用程序，使您的最终用户能够应用新水印、搜索和删除支持格式文件中的现有水印。您可以以编程方式将数字水印分配给许多文件格式，并利用其强大的智能搜索功能。 GroupDocs.Watermark for Java 提供了各种内置的安全措施，可用于避免滥用包含敏感信息或知识产权内容的数字文档。
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          以下是 Java 的 GroupDocs.Watermark 的概述：

        rright:
          enable: true
          icon: "fab fa-html5"
          title: "概述"
          content: |
            * 添加和删除水印
            * 搜索和替换水印
            * 按格式搜索
            * 按图像比较搜索
            * 使用页眉和页脚
            * 使用背景图像
            * 使用附件
            * 光栅化页面
            * 应用编辑限制
      
      ## TAB TWO ##
      tab_two:
        description: |
          下面列出了每种格式支持的[文档格式和水印类型](https://docs.groupdocs.com/watermark/java/supported-document-formats/)：

        left:
          enable: true
          table:
            # table loop
            - title: "微软办公软件"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
                * **Visio:** VSD, VDX, VSS, VSSX, VSX, VST, VSTX, VTX, VSDX, VDW, VSTM, VSSM, VSDM

            # table loop
            - title: "添加水印"
              content: |
                * **PDF**：XObject、工件、注释
                * **字**：形状
                * **Excel**：形状、页眉和页脚
                * **PowerPoint**：形状
                * **Visio**：形状
                * **光栅图像**：文本、图像
                * **多页 Tiff**：文本、图像
                * **动画 Gif**：文本、图像

        right:
          enable: true
          table:
            # table loop
            - title: "PDF 和图像文件"
              content: |
                * **便携式文档格式**：PDF
                * **打开文档**：ODT
                * **电子邮件**：EML、MSG、EMLX、OFT
                * **图像**：PNG、BMP、GIF、JPG、JPEG、JP2、TIF、TIFF、WebP

            # table loop
            - title: "去除水印"
              content: |
                * **PDF**：XObject、工件、注释、常规文本
                * **字**：形状，常规文本
                * **Excel**：单元格中的形状、页眉和页脚、背景图像、文本和公式
                * **PowerPoint**：形状
                * **Visio**：形状、图表注释
                * **电子邮件**：附加和嵌入的图像、主题和正文片段

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Watermark for Java 支持以下操作系统、框架和包管理器：
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "操作系统"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "支持的框架"
              content: |
                * Java 7 (1.7) 及更高版本

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "开发环境"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "构建自动化工具"
              content: |
                * Maven

############################# 特征 ############################
features:
    enable: true
    title: "GroupDocs.Watermark for Java 特征"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "从文件夹中提取各种格式的所有文档并应用或删除水印"

      # feature loop
      - icon: "fas fa-eye"
        content: "从特定部分或完整文档中使用或删除水印"

      # feature loop
      - icon: "fas fa-bolt"
        content: "应用水印到特定部分、页面、幻灯片或文档中的所有图像"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "将水印附加到多帧图像的选定帧"

      # feature loop
      - icon: "fas fa-code"
        content: "将隐藏的水印应用到 PDF 以在打印文档时出现"

      # feature loop
      - icon: "fas fa-cloud"
        content: "在 Excel 文档中的附件和幻灯片中的所有图像形状中使用水印"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "在幻灯片或 Excel 工作表的背景图像中放置水印或将其删除"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "在电子邮件或 PDF 文件的附件中为支持的文件设置水印"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "在 PDF 文件中添加或删除水印作为 XObject、工件和注释"

      # feature loop
      - icon: "fas fa-border-all"
        content: "删除具有特定格式的匹配文本的水印"

      # feature loop
      - icon: "fas fa-wrench"
        content: "查找类似于特定图像的图像水印"

      # feature loop
      - icon: "fas fa-columns"
        content: "即使字母之间有不可读的字符，也能识别文本水印"

      # feature loop
      - icon: "fas fa-file-word"
        content: "根据特定参数或通过分配多个条件查找水印"

      # feature loop
      - icon: "fas fa-envelope"
        content: "指定字体格式以定位匹配的文本水印"

      # feature loop
      - icon: "fas fa-print"
        content: "获取水印绝对尺寸和定位的页面、幻灯片、单元格尺寸"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "应用水印到支持文档格式的任何页眉和页脚内的图像"

      # feature loop
      - icon: "fas fa-lock"
        content: "将水印添加到 Word 文档中的图像形状并限制水印的编辑"

      # feature loop
      - icon: "fas fa-file-code"
        content: "使用不可读字符在演示文稿中保护文本水印"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "通过光栅化单页或整个文档来保护 PDF 文档水印"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "替换当前文本水印时修改文本格式"

      # feature loop
      - icon: "fas fa-heading"
        content: "将水印与 PDF 文件中的出血框、艺术框、裁剪框或裁切框对齐"

    more_feature:
      # more_feature_loop
      - title: "使用水印"
        content: |
          GroupDocs.Watermark for Java 允许您使用多种水印。添加任何类型的水印只需几行代码。以下示例分享，如何使用 Java 在 Word 文档中添加图像水印：
          
          ```java
          Document doc = Document.load(Common.mapSourceFilePath("D://test.docx"));
          Font font = new Font("Times New Roman", 12);
          TextWatermark watermark = new TextWatermark("Test watermark", font);

          // 设置尺寸类型
          watermark.setSizingType(SizingType.ScaleToParentDimensions);

          // 设置水印比例
          watermark.setScaleFactor(0.5);

          doc.addWatermark(watermark);
          doc.save(Common.mapOutputFilePath("D://test.docx"));
          doc.close();
          ```
      # more_feature_loop
      - title: "在 Go 中为不同格式的文件添加水印"
        content: "使用 GroupDocs.Watermark for Java API，您可以在批处理模式下添加或删除特定文件夹中存在的所有文档的水印。没关系，如果文档格式不同，GroupDocs.Watermark for Java 会准确地将水印应用于所有文件."

      # more_feature_loop
      - title: "为您的水印分配万无一失的安全性"
        content: "使用最少的代码，您可以为您的水印分配万无一失的安全性，并使任何第三方工具都很难从 PDF 文件中修改或删除您分配的水印。之所以如此，是因为 GroupDocs.Watermark for Java 允许您将 PDF 文件的所有页面转换为光栅化图像。这种方法使您的数字水印安全，同时保持其质量接近原始。"

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Watermark 为其他流行的开发环境提供文档查看 API"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Watermark for .NET"
          image: "/border/groupdocs-watermark-net.svg"
          product: "GroupDocs.Watermark"
          platform: ".NET"
          link: "/watermark/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---