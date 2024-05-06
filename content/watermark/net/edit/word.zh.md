
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:29
draft: false
lang: zh
format: Word
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "编辑 Word 个文档中的水印"
head_description: "使用 GroupDocs.Watermark for .NET 优化水印位置并确保文档安全。毫不费力地在您的解决方案中定制 Word 个水印。"

############################# Header ############################
title: "增强 Word 水印：.NET 信心" 
description: "使用 GroupDocs.Watermark for .NET 确保 Word 文档的真实性和品牌完整性。放心地使用我们的解决方案编辑水印。"
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
       **增强 Word 文档安全性：** GroupDocs.Watermark for .NET 使开发人员能够轻松增强文档安全性。自信地编辑水印以满足您的特定要求。

############################# Steps ############################
steps:
    enable: true
    title: "使用 .NET 编辑 Word 文档中的水印"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** 使 .NET 开发人员能够轻松编辑各种 Word 文档中的水印。以下是如何在您的应用程序中使用我们的 API 的简化指南：
      
      1. 首先将您的 Word 文件作为参数传递给 **Watermarker** 类构造函数。您可以以字节流、文件流或本地磁盘路径的形式提供文件。
      2. 接下来，找到需要编辑的特定水印。利用 **SearchCriteria** 来识别具有先前添加到文档中的相应属性的水印。
      3. 搜索后，您将获得相关水印的列表。然后，您可以自定义它们的属性，例如大小、页面对齐方式、文本、颜色、图像内容等。这使您能够广泛控制您的数据。
      4. 完成水印编辑后，保存更新的文档。您可以利用本地文件路径或流来存储最终结果。
   
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
        // 编辑 WORD 文本水印

        // 制作 Watermarker 提供 WORD 文件
        using (Watermarker watermarker = new Watermarker("input.docx"))
        {
            // 构造 TextSearchCriteria 并获取文本水印
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
            watermarker.Save("output.docx");
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
    title: "增强其他格式的安全性"
    exclude: "WORD"
    description: "GroupDocs.Watermark for .NET 提供有效的解决方案，以增强不同格式的文档安全性。"
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