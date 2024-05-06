
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:39
draft: false
lang: zh
format: Xls
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "简化的 Xls 水印编辑"
head_description: "使用 GroupDocs.Watermark 简化 .NET 项目中的 Xls 水印编辑。专注于您的内容。"

############################# Header ############################
title: "简化的 Xls 水印编辑：.NET 优化" 
description: "使用 GroupDocs.Watermark 在 .NET 个项目中编辑和优化您的水印。简化工作流程，轻松专注于内容。"
subtitle: "GroupDocs.Watermark for .NET 解决方案" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "在 Nuget 免费下载"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET 软件开发工具包"
    link: "/watermark/net/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **编辑 Xls 水印：** 使用 GroupDocs.Watermark 优化 .NET 项目中的水印控制。简化工作流程，专注于内容，同时毫不费力地确保文档安全。

############################# Steps ############################
steps:
    enable: true
    title: "使用 .NET API 以编程方式编辑 Xls 文档中的水印"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** 为 .NET 开发人员提供强大的 API，用于以编程方式操作各种 Xls 文档中的水印。本指南概述了该过程：
      
      1. 通过将您的 Xls 文件作为参数提供给 **Watermarker** 类构造函数来启动工作流程。该文件可以作为字节流、文件流或对本地磁盘位置的引用提供。
      2. 随后，利用 **SearchCriteria** 对象来查明需要修改的特定水印。该对象能够识别先前嵌入到文档中的水印。
      3. 成功执行搜索后，您将收到一组相关水印。这些水印提供精细控制，允许您修改尺寸、页面定位、文本内容、配色方案、图像数据等属性。
      4. 完成水印编辑后，保留修改后的文档。 API 使用本地文件路径或流对象促进存储。
   
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
        // 在 XLS 文档中编辑图像水印

        // 通过源文件初始化Watermarker
        using (Watermarker watermarker = new Watermarker("input.xls"))
        {
            // 创建SearchCriteria用于图像水印搜索
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                // 编辑图片水印
                watermark.ImageData = imageData;
            }

            // 保存结果XLS
            watermarker.Save("output.xls");
        }
        
        ```     

############################# More features ############################
more_features:
  enable: true
  title: "使用水印管理增强您的工作流程"
  description: "使用我们强大的库，简化 .NET 应用程序中不同文件格式的水印。轻松添加、编辑、搜索或删除水印，以增强文档安全性和品牌推广。"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "无缝水印编辑"
  features:
    # feature loop
    - title: "简化应用程序中的水印流程"
      content: "利用 GroupDocs.Watermark for .NET 的强大功能将水印功能无缝集成到您的 .NET 应用程序中。我们直观的 API 简化了水印的创建、管理、搜索和编辑，无需复杂的手动流程。"

    # feature loop
    - title: "粒度水印自定义"
      content: "借助我们全面的 API，释放水印定制的全部潜力。微调每个细节，包括大小、方向、配色方案和字体选择，以创建完全符合您的品牌和安全要求的水印。"

    # feature loop
    - title: "利用文档特定功能实现灵活的水印"
      content: "在各种文档格式中释放本机功能的力量。利用文档背景、注释、标题或其他对象等元素作为独特的水印容器，满足不同的文档类型和安全需求。"
      
  code_samples:
    # code sample loop
    - title: "PDF 图像水印编辑"
      content: |
        此示例说明如何编辑图像水印的内容
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  将文档加载为 PDF
            var loadOptions = new PdfLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pdf", loadOptions))
            {
                //  加载内容
                PdfContent pdfContent = watermarker.GetContent<PdfContent>();

                //  编辑图像水印
                foreach (PdfArtifact artifact in pdfContent.Pages[0].Artifacts)
                {
                    if (artifact.Image != null)
                    {
                        artifact.Image = new PdfWatermarkableImage(File.ReadAllBytes("test.png"));
                    }
                }

                //  享受输出结果
                watermarker.save("result.pdf");
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
    title: "简化了其他格式的水印控制"
    exclude: "XLS"
    description: "使用 GroupDocs.Watermark 优化 .NET 个项目中的水印控制。"
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