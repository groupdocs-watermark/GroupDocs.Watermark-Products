---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET API 为 Word Excel PDF 图像添加搜索删除水印"
head_description: "C# .NET API 从文档中添加、搜索和删除基于图像和文本的水印：PDF、Word、Excel、演示文稿、Visio、电子邮件和图像文件格式."

############################# Header ############################
title: ".NET API 用于水印处理"
description: "构建 .NET 应用程序以使用智能搜索和强大的安全特性来操作基于文本和图像的水印。"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Watermark for .NET"
        image: "/border/groupdocs-watermark-net.svg"
        product: "GroupDocs.Watermark"
        platform: ".NET"

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
            - link: "https://purchase.groupdocs.com/pricing/watermark/net"
              text: "价钱"

    right:
        link_download: "https://downloads.groupdocs.com/watermark"
        link_learn: "https://docs.groupdocs.com/watermark/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# 概述 ############################
overview:
    enable: true
    content: |
      GroupDocs.Watermark for .NET 使您能够使用 C#、ASP.NET 和其他 .NET 相关技术构建现成的业务应用程序，让您的最终用户添加新水印、搜索和删除支持文件格式的现有水印.使用 GroupDocs.Watermark for .NET，您可以以编程方式将数字水印应用于多种文件格式，并通过采用此 API 提供的各种内置安全措施来阻止未经授权使用知识产权并安全地标记敏感性质的文档。
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          以下是 .NET 的 GroupDocs.Watermark 的概述：
      
        right:
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
          下面列出了每种格式支持的[文档格式和水印类型](https://docs.groupdocs.com/watermark/net/supported-document-formats/)：

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
          GroupDocs.Watermark for .NET supports following 操作系统, Frameworks & 包管理器s:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "操作系统"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux

            # table loop
            - icon: "fas fa-code"
              title: "支持的框架"
              content: |
                * .NET Framework 2.0 或更高版本
                * Mono 框架 1.2 或更高版本
                * .NET 标准 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "包管理器"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "开发环境"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# 特征 ############################
features:
    enable: true
    title: "GroupDocs.Watermark for .NET 特征"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "从各种文件格式的特定部分或整个文档中添加或删除水印"

      # feature loop
      - icon: "fas fa-eye"
        content: "将水印附加到特定部分、页面、幻灯片或文档中的所有图像"

      # feature loop
      - icon: "fas fa-bolt"
        content: "仅将水印分配给多帧图像的特定帧"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "将隐藏水印分配给仅在打印文档时出现的 PDF"

      # feature loop
      - icon: "fas fa-code"
        content: "为 Excel 文档中的所有附件和幻灯片中的所有图像形状设置水印"

      # feature loop
      - icon: "fas fa-cloud"
        content: "在电子表格或幻灯片的背景图像中放置水印或将其删除"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "在电子邮件或 PDF 文档的所有附件中为支持的文件使用水印"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "在 PDF 文档中应用或删除水印作为 XObject、工件和注释"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "使用特定格式消除包含文本的水印"

      # feature loop
      - icon: "fas fa-border-all"
        content: "寻找与特定图像相似的图像水印"

      # feature loop
      - icon: "fas fa-wrench"
        content: "即使字母之间有不可读的字符，也能识别文本水印"

      # feature loop
      - icon: "fas fa-columns"
        content: "根据特定参数或组合多个条件搜索水印"

      # feature loop
      - icon: "fas fa-file-word"
        content: "指定字体格式以查找匹配的文本水印"

      # feature loop
      - icon: "fas fa-envelope"
        content: "以编程方式提取支持格式的页面设置和其他信息"

      # feature loop
      - icon: "fas fa-print"
        content: "在支持的文档格式中向任何页眉和页脚内的图像添加水印"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "将水印添加到 Word 文档中的图像形状并锁定水印以限制编辑"

      # feature loop
      - icon: "fas fa-lock"
        content: "使用演示文稿中的不可读字符保护文本水印"

      # feature loop
      - icon: "fas fa-file-code"
        content: "栅格化特定页面或整个 PDF 文档以保护添加的水印"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "替换现有文本水印时更改文本格式"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "将水印与 PDF 文档中的出血框、艺术框、裁剪框或裁切框对齐"

      # feature loop
      - icon: "fas fa-heading"
        content: "在 Microsoft Visio 文档中编辑形状属性"

    more_feature:
      # more_feature_loop
      - title: "添加水印s"
        content: |
          GroupDocs.Watermark for .NET 支持多种类型的水印。添加任何类型的水印只需几行代码。以下示例演示了使用 C# 将图像水印应用于 Word 文档：

          ```cs
          // 加载文档
          using (FileStream stream = File.Open("document.docx", FileMode.Open, FileAccess.ReadWrite))
          {
            using (Watermarker watermarker = new(Watermarker(stream))
            {
              // 使用图像的路径作为构造函数的参数
              using (ImageWatermark watermark = new ImageWatermark("logo.png"))
              {
                  watermark.HorizontalAlignment = HorizontalAlignment.Center;
                  watermark.VerticalAlignment = VerticalAlignment.Center;
                  watermarker.Add(watermark);
              }
              // 保存生成的文档
              watermarker.Save("document_watermarked.docx");
            }
          }
          ```
      # more_feature_loop
      - title: "应用水印 一次转到不同格式的文件"
        content: "GroupDocs.Watermark API 允许您一次性应用水印或删除特定文件夹中所有文件的水印。这些文件甚至可以是不同的格式，但水印将准确地应用于所有文件。"

      # more_feature_loop
      - title: "水印的万无一失的安全性"
        content: "只需一行代码，任何工具都很难从 PDF 文件中删除水印。这是通过将 PDF 文档的所有页面转换为光栅图像同时保持原始质量不变来实现的."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Watermark 为其他流行的开发环境提供文档查看 API"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Watermark for Java"
          image: "/border/groupdocs-watermark-java.svg"
          product: "GroupDocs.Watermark"
          platform: "Java"
          link: "/watermark/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---