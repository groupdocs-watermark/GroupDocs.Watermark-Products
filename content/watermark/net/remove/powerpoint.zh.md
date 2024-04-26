
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:58
draft: false
lang: zh
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "使用 C# .NET API 清除 Powerpoint 中的水印"
head_description: "使用我们的 C# .NET API 轻松删除和管理 Powerpoint 张幻灯片中的水印，确保演示清晰且专业。"

############################# Header ############################
title: "C# .NET Powerpoint 水印去除剂" 
description: "利用 GroupDocs.Watermark for .NET C# API 的强大功能高效地去除 Powerpoint 演示文稿中的水印，在保持内容完整性的同时保持幻灯片美感。"
subtitle: "GroupDocs.Watermark for .NET C# API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Nuget 下载"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET C# 库"
    link: "/watermark/net/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET C# 库提供了复杂的工具，用于从 Powerpoint 演示文稿中删除水印。它提供了无缝删除水印的功能，确保您的演示文稿保持有影响力且整洁。适用于必须提供干净、清晰视觉效果的商业、教育和培训环境。

############################# Steps ############################
steps:
    enable: true
    title: "使用 .NET 从 Powerpoint 个文档中移除水印"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/)** 简化了从业务文档中删除水印的任务。通过集成我们的库来增强您的 .NET 应用程序，然后按照以下简单步骤操作：
      
      1. **Watermarker**。我们的 API 支持处理以流或本地路径形式提供的文档。
      2. **搜索条件**缩小要处理的水印集的范围。您可以使用各种参数，例如图像、文本或格式化功能。您提供的搜索参数越具体，获得的结果就越精确。
      3. 处理作为搜索结果获得的文档水印列表，并将其从文档中删除。
      4. 删除水印后，将生成的文档另存为本地文件或字节流。
   
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
        // 从 Powerpoint 文档中移除文字水印

        // 为文档 Powerpoint 源文档提供 Watermarker 实例
        using (Watermarker watermarker = new Watermarker("input.pptx"))
        {
            // 从文档中移除选定的水印
            TextFormattingSearchCriteria criteria = new TextFormattingSearchCriteria();
            criteria.ForegroundColorRange = new ColorRange();
            criteria.FontBold = true;
            PossibleWatermarkCollection watermarks = watermarker.Search(criteria);
            watermarks.Clear();

            // 将文件保存到提供的路径
            watermarker.Save("output.pptx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "使用 C# .NET API 简化水印去除流程"
  description: "了解我们的 C# .NET API 的强大水印去除功能，该功能旨在与您的 .NET 应用程序无缝集成。在保持原始文件质量的同时，高效地移除或清除 PDF 和办公文档中的水印。"
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "移除水印"
  features:
    # feature loop
    - title: "精确清除水印"
      content: "我们的 .NET API 提供了精确的工具，可以从任何文档中彻底删除水印。此功能专为开发人员量身定制，可确保删除水印不会影响文档质量或布局。"

    # feature loop
    - title: "自动批量去除水印"
      content: "使用我们的 .NET API 自动执行从大型文档集中删除水印的过程。非常适合处理大量文档的企业，可提高效率和文档安全性。"

    # feature loop
    - title: "高级水印编辑功能"
      content: "利用高级功能有选择地编辑或修改水印。我们的 API 支持详细调整，确保您的文档保持专业外观，同时保护敏感信息。"
      
  code_samples:
    # code sample loop
    - title: "移除电子表格文本水印"
      content: |
        如何删除 Excel 文档中具有特殊格式的文本水印。
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  加载 Excel 工作簿
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  获取内容并找到相应的水印
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();
                foreach (SpreadsheetWorksheet section in content.Worksheets)
                {
                    for (int i = section.Shapes.Count - 1; i >= 0; i--)
                    {
                        foreach (FormattedTextFragment fragment in section.Shapes[i].FormattedTextFragments)
                        {
                            if (fragment.ForegroundColor.Equals(Color.Red) && fragment.Font.FamilyName == "Arial")
                            {
                                //  移除文字水印
                                section.Shapes.RemoveAt(i);
                                break;
                            }
                        }
                    }
                }

                //  保存已处理 XLSX
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
    title: "优化 .NET 中的 Powerpoint 演示文稿"
    exclude: "POWERPOINT"
    description: "了解如何利用 GroupDocs.Watermark for .NET C# API 进行简洁专业的 Powerpoint 演示，不含分散注意力的水印元素。"
    items: 
        # format loop 1
        - name: "水印 PDF"
          format: "PDF"
          link: "/watermark/net/remove//pdf/"
          description: "Adobe Portable 文档格式"

        # format loop 2
        - name: "水印 Word"
          format: "WORD"
          link: "/watermark/net/remove//word/"
          description: "MS Word 和 Open Office 文档"
          
        # format loop 3
        - name: "水印 Excel"
          format: "EXCEL"
          link: "/watermark/net/remove//excel/"
          description: "MS Excel 和 Open Office 电子表格"

        # format loop 4
        - name: "水印 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/remove//powerpoint/"
          description: "MS PowerPoint 和开放办公室演示"

        # format loop 5
        - name: "水印 DOCX"
          format: "DOCX"
          link: "/watermark/net/remove//docx/"
          description: "微软 Word 打开 XML 文档"
          
        # format loop 6
        - name: "水印 PPTX"
          format: "PPTX"
          link: "/watermark/net/remove//pptx/"
          description: "PowerPoint 打开 XML 演示文稿"
          
        # format loop 7
        - name: "水印 XLSX"
          format: "XLSX"
          link: "/watermark/net/remove//xlsx/"
          description: "微软 Excel 打开 XML 电子表格"

        # format loop 8
        - name: "水印 DOC"
          format: "DOC"
          link: "/watermark/net/remove//doc/"
          description: "微软 Word 97-2007 文档"

        # format loop 9
        - name: "水印 XLS"
          format: "XLS"
          link: "/watermark/net/remove//xls/"
          description: "微软 Excel 工作簿 97-2003"

        # format loop 10
        - name: "水印 PPT"
          format: "PPT"
          link: "/watermark/net/remove//ppt/"
          description: "PowerPoint 演示 97-2003"

        # format loop 11
        - name: "水印 RTF"
          format: "RTF"
          link: "/watermark/net/remove//rtf/"
          description: "富文本格式"

---