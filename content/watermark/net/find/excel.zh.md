
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
head_title: "查找不可见的 Excel 电子表格水印"
head_description: "使用 GroupDocs.Watermark 轻松发现文档中不可见的水印。"

############################# Header ############################
title: "立即查找 Excel 电子表格水印" 
description: "使用 GroupDocs.Watermark for .NET 轻松揭开和管理隐藏的水印。"
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费 Nuget 下载"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "获取信息 GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET 为使用 .NET 管理水印提供了全面的解决方案。轻松生成、编辑、查找和删除各种文档格式的水印，例如 PDF、微软 Word、Excel 等。使用 GroupDocs.Watermark for .NET 将水印管理无缝集成到您的应用程序中。

############################# Steps ############################
steps:
    enable: true
    title: "使用 .NET 在 Excel 文件中查找水印"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/)** 简化了在业务文档中查找水印的过程。将我们的软件包集成到您的 .NET 应用程序中以释放其优势。
      
      1. 要利用我们的库功能，请将 Excel 文件加载到 **Watermarker** 类实例中。您可以提供文件路径、文件流或字节流。
      2. 要细化潜在水印列表，请使用 **SearchCriteria** 对象。例如，提供图像来查找相似的图像水印。如果查找文本水印，请提供文本、字体、颜色和其他相关选项。
      3. 使用 **Watermarker** 对象的 **Search** 方法检索文档中放置的水印。您将收到代表潜在水印的对象集合，以供进一步处理。
      4. 最后，您可以根据需要灵活地操作搜索结果。您可以删除找到的水印或编辑其属性，例如更改大小或文本。
   
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
        // 在 EXCEL 中查找文本水印

        // 使用 EXCEL 路径创建 Watermarker
        using (Watermarker watermarker = new Watermarker("input.xslx"))
        {
            // 查找水印
            PossibleWatermarkCollection possibleWatermarks = watermarker.Search();

            // 使用找到的水印信息
            foreach (PossibleWatermark possibleWatermark in possibleWatermarks)
            {
                Console.WriteLine(possibleWatermark.Text);
                Console.WriteLine(possibleWatermark.Width);
                Console.WriteLine(possibleWatermark.Height);
            }
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "使用 GroupDocs.Watermark 高效搜索和查找水印"
  description: "利用 GroupDocs.Watermark 的强大功能，在 .NET 中使用 C# 在任何文档类型中搜索和定位水印。"
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "搜索水印"
  features:
    # feature loop
    - title: "使用高级搜索发现水印"
      content: "使用 GroupDocs.Watermark 可以毫不费力地在多种文档类型中查找水印。我们的工具允许您按内容、大小和不透明度等参数进行搜索。"

    # feature loop
    - title: "通过自定义参数查找水印"
      content: "使用 GroupDocs.Watermark 定制您的搜索条件，根据特定属性查找水印，确保您可以有效地管理和查看它们。"

    # feature loop
    - title: "高效检索和管理水印"
      content: "通过快速检索文档中的所有水印，简化文档管理流程。我们的API允许快速识别和分析水印。"
      
  code_samples:
    # code sample loop
    - title: "C# 示例：搜索水印"
      content: |
        此 C# 示例演示如何使用 GroupDocs.Watermark 在任何文档中搜索水印，并说明如何利用参数获得精确结果。
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  从本地或网络来源加载文档进行处理
            var loadOptions = new WordProcessingLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.docx", loadOptions))
            {
                //  定义水印搜索的参数，例如类型或可见性
                Regex regex = new Regex(@"^© \d{4}$");

                //  检索所有符合指定条件的水印
                TextSearchCriteria textSearchCriteria = new TextSearchCriteria(regex);
                PossibleWatermarkCollection possibleWatermarks = watermarker.Search(textSearchCriteria);

                //  查看和管理找到的水印清单以评估其影响
                Console.WriteLine("Found {0} possible watermark(s).", possibleWatermarks.Count);
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
    title: "发现各种格式的水印"
    exclude: "EXCEL"
    description: "轻松搜索和识别各种支持的文件格式中的水印。"
    items: 
        # format loop 1
        - name: "水印 PDF"
          format: "PDF"
          link: "/watermark/net/find//pdf/"
          description: "Adobe Portable 文档格式"

        # format loop 2
        - name: "水印 Word"
          format: "WORD"
          link: "/watermark/net/find//word/"
          description: "MS Word 和 Open Office 文档"
          
        # format loop 3
        - name: "水印 Excel"
          format: "EXCEL"
          link: "/watermark/net/find//excel/"
          description: "MS Excel 和 Open Office 电子表格"

        # format loop 4
        - name: "水印 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/find//powerpoint/"
          description: "MS PowerPoint 和开放办公室演示"

        # format loop 5
        - name: "水印 DOCX"
          format: "DOCX"
          link: "/watermark/net/find//docx/"
          description: "微软 Word 打开 XML 文档"
          
        # format loop 6
        - name: "水印 PPTX"
          format: "PPTX"
          link: "/watermark/net/find//pptx/"
          description: "PowerPoint 打开 XML 演示文稿"
          
        # format loop 7
        - name: "水印 XLSX"
          format: "XLSX"
          link: "/watermark/net/find//xlsx/"
          description: "微软 Excel 打开 XML 电子表格"

        # format loop 8
        - name: "水印 DOC"
          format: "DOC"
          link: "/watermark/net/find//doc/"
          description: "微软 Word 97-2007 文档"

        # format loop 9
        - name: "水印 XLS"
          format: "XLS"
          link: "/watermark/net/find//xls/"
          description: "微软 Excel 工作簿 97-2003"

        # format loop 10
        - name: "水印 PPT"
          format: "PPT"
          link: "/watermark/net/find//ppt/"
          description: "PowerPoint 演示 97-2003"

        # format loop 11
        - name: "水印 RTF"
          format: "RTF"
          link: "/watermark/net/find//rtf/"
          description: "富文本格式"

---