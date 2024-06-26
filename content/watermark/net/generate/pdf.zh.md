
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:24
draft: false
lang: zh
format: Pdf
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "安全 PDF 文档的 C# 水印"
head_description: "使用 .NET C# 在 PDF 中嵌入水印，保护官方文档和敏感信息。"

############################# Header ############################
title: "使用 C# 水印增强 PDF 安全性" 
description: "实施 .NET C# 在 PDF 个文档中应用水印，确保保护法律、财务和官方记录。"
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "在 Nuget 免费下载"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET 为 .NET C# 开发人员提供了一个强大的 API，用于在 PDF 文件中插入水印，这是企业、法律和政府部门文档安全的必备工具。此 API 支持全面的水印自定义选项，包括文本格式、图像集成和动态放置，以适应各种文档布局。无论是保护机密协议、保护版权材料还是标记专有信息，GroupDocs.Watermark 都可确保所有 PDF 清晰、专业地传达所有权。其他功能包括水印旋转、透明度控制和分层功能，与所有现代 .NET 框架兼容。

############################# Steps ############################
steps:
    enable: true
    title: "轻松为 Pdf 文档生成水印"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/):** .NET 应用程序的高级水印库。及时为您的解决方案提供支持并使用水印保护文档。
      
      1. **核心类：Watermarker。** 我们 API 的主类是 **Watermarker**。您需要在文档处理之前实例化它。不要忘记将 Pdf 文件作为路径或流对象传递给构造函数。
      2. **制作您的水印。** 下一步是构造所需类型的水印对象。它不仅可以放置在特定的文档页面上，还可以放置在图像或标题等本机文档部分中。
      3. **微调外观。** 设置水印属性，例如高度和宽度、顶部、左侧、中心对齐、字体和颜色等。
      4. **应用并保存。** 使用 **Watermarker** 方法添加新水印。您可以根据需要随意添加任意数量的水印。您可以将带水印的文档保存到任何位置。
   
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
        // 在 PDF 文件中生成图像水印

        // 为 Watermarker 构造函数提供源文件路径
        using (Watermarker watermarker = new Watermarker("input.pdf"))
        {
            // 用图像文件生成图像水印实例
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // 保存带水印的 PDF 结果
            watermarker.Save("output.pdf");
        }
        
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "提升您的水印游戏体验"
  description: "使用我们适用于 .NET 的 GroupDocs.Watermark API 解锁高级水印功能。这个强大的工具允许在各种文档类型中精确自定义和应用水印，从而在最大限度地减少视觉干扰的情况下确保最大的安全性和版权依从性。"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "全面的水印解决方案"
  features:
    # feature loop
    - title: "复杂的平铺选项"
      content: "使用我们的拼贴选项，将水印无缝扩展到整个文档。此功能允许水印覆盖整个文档区域，防止移除，并在不影响设计或可读性的前提下确保全面的文档保护。"

    # feature loop
    - title: "鲜艳的色彩定制"
      content: "为你的水印增添一抹色彩！我们的 API 支持全光谱颜色自定义，允许您应用与您的公司品牌或文档风格完美匹配的水印。增强视觉吸引力，同时保持强大的安全功能。"

    # feature loop
    - title: "增强的安全设置"
      content: "使用高级水印设置，将文档安全性提升到一个新的水平。配置包含可见和不可见元素的多层水印，以防止未经授权的复制，并确保只有预期的收件人才能访问关键信息。"
      
  code_samples:
    # code sample loop
    - title: "生成 PowerPoint 个水印"
      content: |
        此示例说明如何向 PPTX 背景图像添加水印
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  加载 PPTX 演示文稿
            var loadOptions = new PresentationLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pptx", loadOptions))
            {
                //  设置水印属性
                TextWatermark watermark = new TextWatermark("Protected image", new Font("Arial", 8));
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermark.RotateAngle = 45;
                watermark.SizingType = SizingType.ScaleToParentDimensions;
                watermark.ScaleFactor = 1;

                //  水印幻灯片背景
                PresentationContent content = watermarker.GetContent<PresentationContent>();
                foreach (PresentationSlide slide in content.Slides)
                {
                    if (slide.ImageFillFormat.BackgroundImage != null)
                    {
                        slide.ImageFillFormat.BackgroundImage.Add(watermark);
                    }
                }

                //  保存处理后的演示文稿
                watermarker.save("result.pptx");
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
    title: "使用 .NET C# 水印保护 PDF 个文件"
    exclude: "PDF"
    description: "使用 .NET C# 在 PDF 个文档中嵌入安全的定制水印，是保护官方和敏感信息的理想之选。"
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