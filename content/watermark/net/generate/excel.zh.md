
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:19
draft: false
lang: zh
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "为 Excel 电子表格生成水印"
head_description: "使用 .NET C# 自动为图像添加水印，以实现一致的安全性。高效处理大批量图像。"

############################# Header ############################
title: "使用 .NET C# 在 Excel 中添加动态水印" 
description: "使用 C# 自动在 Excel 文件上应用动态文本或图像水印。我们的教程向您展示如何保持一致性和专业性，同时最大限度地减少人工干预。"
subtitle: "GroupDocs.Watermark for .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费 Nuget 下载"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET 图书馆"
    link: "/watermark/net/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET 支持将水印无缝集成到 Excel 电子表格中，为企业提供保护和个性化文档所需的工具。此 C# 库支持多种水印类型，并允许进行详细自定义，包括不透明度、旋转和对齐调整。此外，它还配备了高级搜索功能，可以检测和管理现有水印，确保您的电子表格免遭篡改和未经授权的披露。

############################# Steps ############################
steps:
    enable: true
    title: "增强您的文档：使用 .NET 为 Excel 生成水印"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** 是一个库，可为 .NET 开发人员简化向各种业务文件格式添加水印的过程。使用以下步骤将我们的库集成到您的应用程序中并轻松地为文档添加水印：
      
      1. **开始您的水印之旅：** 首先熟悉 **Watermarker** 类，它是我们 API 的基石。要开始该过程，请确保在文档处理之前将其实例化。不要忽视向构造函数提供 Excel 文件的重要性，无论它是路径还是流对象。
      2. **制作自定义水印：** 通过创建根据您的规范定制的 **Watermark** 对象，继续下一阶段。这种多功能工具不仅限于特定的文档页面；它还可以无缝集成到附件或标题等本机文档元素中。
      3. **微调水印属性：** 通过调整高度、宽度、页面对齐、字体系列和颜色等属性来改善您的水印体验。这种级别的自定义可确保您的水印与文档无缝融合。
      4. **应用您的水印：** 利用 **Watermarker** 方法轻松将自定义水印应用到您的文档。无论您需要添加一个还是多个水印，这一过程都提供了灵活性。为了提高安全性，请考虑将已处理的文档保存在单独的位置。
   
    code:
      platform: "net"
      copy_title: "复制"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "点击复制"
        copy_done: "复制的"
      links:
        #  loop
        - title: "更多例子"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "文档"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // 在 EXCEL 文件中生成文本水印

        // 提供要加水印的文件
        using (Watermarker watermarker = new Watermarker("input.xslx"))
        {
            // 生成文本水印实例
            Font font = new Font("Arial", 19, FontStyle.Bold | FontStyle.Italic);
            TextWatermark watermark = new TextWatermark("my watermark", font);
            watermark.ForegroundColor = Color.Red;
            watermark.BackgroundColor = Color.Blue;
            watermarker.Add(watermark);

            // 保存 EXCEL 结果
            watermarker.Save("output.xslx");
        }
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "深入了解添加水印"
  description: "利用我们强大的 API 在 .NET 应用程序中呈现、显示、转换和管理文档、幻灯片、图表和其他各种文档类型。GroupDocs.Watermark 无缝集成水印功能，以增强文档安全和版权保护。"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "添加水印"
  features:
    # feature loop
    - title: "毫不费力地为您的文档添加水印。"
      content: "GroupDocs.Watermark 使 .NET 开发人员能够轻松地将水印集成到他们的应用程序中。毫不费力地为常用业务文档和文件添加文本、图像或动态水印，确保您的内容在所有平台上均安全且品牌一致。"

    # feature loop
    - title: "量身定制水印以满足您的需求。"
      content: "使用 GroupDocs.Watermark 支持的广泛功能自定义水印以满足您的特定要求。调整大小、旋转、透明度、颜色和字体，确保您的水印不仅看起来完美，而且还能在不妨碍重要信息的情况下增强文档安全性。"

    # feature loop
    - title: "利用原生文档功能进行水印"
      content: "利用文档格式的固有功能进行复杂的水印。无论是使用原生 PDF 批注、MS Word 背景还是 Excel 页眉和页脚，GroupDocs.Watermark 都与文档结构深度集成，应用既有效又微创的水印。"
      
  code_samples:
    # code sample loop
    - title: "为 DOCX 生成图像水印"
      content: |
        此示例说明如何将图像效果应用于形状水印。
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  加载 Word 个文档
            var loadOptions = new WordProcessingLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.docx", loadOptions))
            {
                //  设置水印选项
                using (ImageWatermark watermark = new ImageWatermark("logo.png"))
                {
                    WordProcessingImageEffects effects = new WordProcessingImageEffects();
                    effects.Brightness = 0.7;
                    effects.Contrast = 0.6;
                    effects.ChromaKey = Color.Red;
                    effects.BorderLineFormat.Enabled = true;
                    effects.BorderLineFormat.Weight = 1;

                    WordProcessingWatermarkSectionOptions options = new WordProcessingWatermarkSectionOptions();
                    options.Effects = effects;

                    //  生成水印
                    watermarker.Add(watermark, options);
                }

                //  保存更新的文档
                watermarker.save("result.docx");
            }

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "准备好开始了吗？"
  description: "免费试用 GroupDocs.Watermark 项功能或申请许可证"
  items:
    #  loop
    - title: "Nuget 下载"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "许可"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "使用 C# 在 Excel 中嵌入文本和图像水印"
    exclude: "EXCEL"
    description: "利用 GroupDocs.Watermark C# API 向 Excel 电子表格高效添加自定义水印。使用专为快速灵活的水印集成而设计的工具，增强文档安全性和企业品牌推广。"
    items: 
        # format loop 1
        - name: "水印 PDF"
          format: "PDF"
          link: "/watermark/net/generate//pdf/"
          description: "Adobe Portable 文档格式"

        # format loop 2
        - name: "水印 Word"
          format: "WORD"
          link: "/watermark/net/generate//word/"
          description: "MS Word 和 Open Office 文档"
          
        # format loop 3
        - name: "水印 Excel"
          format: "EXCEL"
          link: "/watermark/net/generate//excel/"
          description: "MS Excel 和 Open Office 电子表格"

        # format loop 4
        - name: "水印图片"
          format: "IMAGE"
          link: "/watermark/net/generate//image/"
          description: "流行的图像格式"

        # format loop 5
        - name: "水印照片"
          format: "PHOTO"
          link: "/watermark/net/generate//photo/"
          description: "照片格式"

        # format loop 6
        - name: "水印 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/generate//powerpoint/"
          description: "MS PowerPoint 和开放办公室演示"

        # format loop 7
        - name: "水印 DOCX"
          format: "DOCX"
          link: "/watermark/net/generate//docx/"
          description: "微软 Word 打开 XML 文档"
          
        # format loop 8
        - name: "水印 PPTX"
          format: "PPTX"
          link: "/watermark/net/generate//pptx/"
          description: "PowerPoint 打开 XML 演示文稿"
          
        # format loop 9
        - name: "水印 XLSX"
          format: "XLSX"
          link: "/watermark/net/generate//xlsx/"
          description: "微软 Excel 打开 XML 电子表格"

        # format loop 10
        - name: "水印 JPEG"
          format: "JPEG"
          link: "/watermark/net/generate//jpeg/"
          description: "JPEG 图片"

        # format loop 11
        - name: "水印 PNG"
          format: "PNG"
          link: "/watermark/net/generate//png/"
          description: "Portable 网络图形"

        # format loop 12
        - name: "水印 TIFF"
          format: "TIFF"
          link: "/watermark/net/generate//tiff/"
          description: "标记图像文件格式"

        # format loop 13
        - name: "WEBP 水印"
          format: "WEBP"
          link: "/watermark/net/generate//webp/"
          description: "网络图片"

        # format loop 14
        - name: "水印 DOC"
          format: "DOC"
          link: "/watermark/net/generate//doc/"
          description: "微软 Word 97-2007 文档"

        # format loop 15
        - name: "水印 XLS"
          format: "XLS"
          link: "/watermark/net/generate//xls/"
          description: "微软 Excel 工作簿 97-2003"

        # format loop 16
        - name: "水印 PPT"
          format: "PPT"
          link: "/watermark/net/generate//ppt/"
          description: "PowerPoint 演示 97-2003"

        # format loop 17
        - name: "水印 RTF"
          format: "RTF"
          link: "/watermark/net/generate//rtf/"
          description: "富文本格式"

---