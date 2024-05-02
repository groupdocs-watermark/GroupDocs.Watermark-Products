
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:26:59
draft: false
lang: zh
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "编辑 Excel 格式的水印"
head_description: "使用 GroupDocs.Watermark for .NET 轻松自定义和保护您的文档。增强文档完整性，轻松编辑 Excel 水印。"

############################# Header ############################
title: "编辑您的 Excel 电子表格水印：.NET 效率" 
description: "使用我们专为 .NET 效率而设计的可定制水印工具，提升您的文档安全性。毫不费力地编辑 Excel 个水印。"
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
       **使用我们的工具编辑 Excel 水印：** 我们的 GroupDocs.Watermark for .NET 工具提供有效的策略来增强和保护您的文档。由于为 .NET 开发人员提供了各种功能，管理水印变得轻而易举，从而确保文档的安全性和真实性。

############################# Steps ############################
steps:
    enable: true
    title: "使用 .NET 编辑 Excel 个文档中的水印"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** 使 .NET 开发人员能够毫不费力地编辑各种 Excel 文档中的水印。以下是如何在您的应用程序中使用我们的 API 的简化指南：
      
      1. **Watermarker**类构造函数。您可以将文件作为字节流、文件流或本地磁盘路径提供。
      2. **搜索条件**来识别具有先前添加到文档中的相应属性的水印。
      3. 搜索完成后，您将获得相关水印的列表。然后，您可以自定义其属性，例如大小、页面对齐方式、文本、颜色、图像内容等。这使您可以对数据进行广泛的控制。
      4. 完成水印编辑后，保存更新后的文档。您可以使用本地文件路径或流来存储最终结果。
   
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
        // 编辑 EXCEL 文本水印

        // 让 Watermarker 提供 EXCEL 个文件
        using (Watermarker watermarker = new Watermarker("input.xslx"))
        {
            // 构建 TextSearchCriteria 并获取文本水印
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                 // 编辑文字水印
                 watermark.FormattedTextFragments.Clear();
                 watermark.FormattedTextFragments.Add("passed", 
                    new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
            }

            // 保存文档
            watermarker.Save("output.xslx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "了解有关修改水印的更多信息"
  description: "使用我们的库为您的 .NET 个应用程序提供支持，并在各种文件格式中添加、编辑、删除或搜索水印。"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "编辑水印"
  features:
    # feature loop
    - title: "为您的企业添加水印文件"
      content: "使用 GroupDocs.Watermark for .NET 为文件和文档添加水印。无需额外努力即可添加和管理水印，在您的应用程序中实现我们的 API。搜索、编辑和删除之前添加的水印。"

    # feature loop
    - title: "根据您的要求微调水印"
      content: "我们的 API 提供了一套全面的自定义选项。轻松修改大小、方向、配色方案、字体系列等方面，以创建理想的水印。"

    # feature loop
    - title: "利用特定于文档的功能"
      content: "根据您使用的文件格式，您可以合并内置功能。它们可能包括文档背景、注释、标题或其他用作水印容器的元素。"
      
  code_samples:
    # code sample loop
    - title: "Excel 水印文本编辑"
      content: |
        此示例说明如何在 Excel 工作表中编辑特定水印的文本
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  加载 XLSX 电子表格
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  加载电子表格内容
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();

                //  编辑水印内部文本
                foreach (SpreadsheetShape shape in content.Worksheets[0].Shapes)
                {
                    if (shape.Text == "GroupDocs 2016")
                    {
                        shape.Text = "GroupDocs 2017";
                    }
                }

                //  保存输出结果
                watermarker.save("result.xlsx");
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
    title: "以其他格式自定义您的水印"
    exclude: "EXCEL"
    description: "使用 GroupDocs.Watermark for .NET 为各种文档格式添加水印，以满足您的需求。"
    items: 
        # format loop 1
        - name: "水印 PDF"
          format: "PDF"
          link: "/watermark/net/edit//pdf/"
          description: "Adobe Portable 文档格式"

        # format loop 2
        - name: "水印 Word"
          format: "WORD"
          link: "/watermark/net/edit//word/"
          description: "MS Word 和 Open Office 文档"
          
        # format loop 3
        - name: "水印 Excel"
          format: "EXCEL"
          link: "/watermark/net/edit//excel/"
          description: "MS Excel 和 Open Office 电子表格"

        # format loop 4
        - name: "水印 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/edit//powerpoint/"
          description: "MS PowerPoint 和开放办公室演示"

        # format loop 5
        - name: "水印 DOCX"
          format: "DOCX"
          link: "/watermark/net/edit//docx/"
          description: "微软 Word 打开 XML 文档"
          
        # format loop 6
        - name: "水印 PPTX"
          format: "PPTX"
          link: "/watermark/net/edit//pptx/"
          description: "PowerPoint 打开 XML 演示文稿"
          
        # format loop 7
        - name: "水印 XLSX"
          format: "XLSX"
          link: "/watermark/net/edit//xlsx/"
          description: "微软 Excel 打开 XML 电子表格"

        # format loop 8
        - name: "水印 DOC"
          format: "DOC"
          link: "/watermark/net/edit//doc/"
          description: "微软 Word 97-2007 文档"

        # format loop 9
        - name: "水印 XLS"
          format: "XLS"
          link: "/watermark/net/edit//xls/"
          description: "微软 Excel 工作簿 97-2003"

        # format loop 10
        - name: "水印 PPT"
          format: "PPT"
          link: "/watermark/net/edit//ppt/"
          description: "PowerPoint 演示 97-2003"

        # format loop 11
        - name: "水印 RTF"
          format: "RTF"
          link: "/watermark/net/edit//rtf/"
          description: "富文本格式"

---