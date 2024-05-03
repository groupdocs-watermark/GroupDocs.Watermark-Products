
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:15
draft: false
lang: zh
format: Xls
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "找出隐藏的 XLS 电子表格水印"
head_description: "使用 GroupDocs.Watermark for .NET 轻松发现文档中隐藏的水印。"

############################# Header ############################
title: "发现并管理 XLS 电子表格中的隐藏水印" 
description: "使用 GroupDocs.Watermark for .NET 快速发现和管理隐藏的水印。"
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
       GroupDocs.Watermark for .NET 为使用 .NET 管理水印提供了全面的解决方案。轻松生成、编辑、查找和删除各种文档格式的水印，例如 PDF、微软 Word、Excel 等。使用 GroupDocs.Watermark for .NET 为您的应用程序添加水印搜索功能。

############################# Steps ############################
steps:
    enable: true
    title: "使用 .NET 高效查找 Xls 水印"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/)** 提供了一个强大的解决方案，用于以编程方式在各种业务文档格式中查找水印。将我们的软件包集成到您的 .NET 应用程序中，为它们提供水印查找功能。
      
      1. 要利用我们库的功能，请实例化 **Watermarker** 类并提供 Xls 文件路径、文件流或字节流作为输入。此操作加载文档以进行水印分析。
      2. 对于有针对性的水印识别，请利用 **SearchCriteria** 对象。指定图像以查找相似图像水印。或者，对于文本水印，定义文本内容、字体属性、颜色属性和其他相关参数以细化搜索条件。
      3. 使用 **Watermarker** 对象的 **Search** 方法在加载的文档中启动水印检测过程。此函数返回表示潜在水印的对象集合，以便进行进一步处理。
      4. 检索到的水印对象集合使您能够精确控制。您可以通过编程方式删除不需要的水印或动态修改其属性，例如调整其大小或文本内容，以满足您的特定要求。
   
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
        // 查找放置在 XLS 中的图像水印

        // 构造 Watermarker 传递 XLS 路径
        using (Watermarker watermarker = new Watermarker("input.xls"))
        {
            // 使用搜索选项查找水印
            ImageSearchCriteria imageSearchCriteria = new ImageDctHashSearchCriteria("watermark.jpeg");
            imageSearchCriteria.MaxDifference = 0.9;
            PossibleWatermarkCollection possibleWatermarks = watermarker.Search(imageSearchCriteria);

            // 处理水印信息
            Console.WriteLine("Found {0} possible watermark(s).", possibleWatermarks.Count);
        }
        
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "使用 C# 和 GroupDocs.Watermark 的高级水印搜索技术"
  description: "使用 GroupDocs.Watermark C# API 深入研究强大的水印搜索功能，该API专为 .NET 平台内的开发人员量身定制。"
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "C# 水印搜索"
  features:
    # feature loop
    - title: "简化了 C# 中的水印检测"
      content: "利用 GroupDocs.Watermark 在 C# 应用程序中实现简化的水印检测。受益于高级搜索功能，可以快速准确地找到水印。"

    # feature loop
    - title: "使用 C# 进行精确的水印搜索"
      content: "通过在 C# 中精确搜索水印来增强您的文档安全协议。配置 GroupDocs.Watermark 以根据大小、颜色和位置等特定特征查找水印。"

    # feature loop
    - title: "C# 集成实现有效的水印管理"
      content: "将 GroupDocs.Watermark 集成到您的 C# 项目中以有效管理文档水印。我们的 API 提供了强大的工具来搜索、分析和报告水印使用情况，从而确保合规性和品牌一致性。"
      
  code_samples:
    # code sample loop
    - title: "C# 示例：全面的水印搜索"
      content: |
        浏览此详细示例，了解如何使用 C# 和 GroupDocs.Watermark 实现全面的水印搜索功能，包括处理多种文档类型和复杂的搜索条件。
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  初始化 C# 应用程序并准备文档加载机制
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  设置搜索参数以定位特定的水印属性
                ImageSearchCriteria criteria = new ImageDctHashSearchCriteria("watermark.png");
                PossibleWatermarkCollection possibleWatermarks = watermarker.Search(criteria);

                //  对文档进行搜索并收集水印详细信息
                foreach (PossibleWatermark watermark in watermarks)
                {
                    //...
                }

                //  分析和处理水印数据，以采取进一步的管理或合规措施
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
    title: "在支持的格式中找出水印"
    exclude: "XLS"
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