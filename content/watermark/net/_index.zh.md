---
############################# Static ############################
layout: "landing"
date: 2024-04-26T21:39:08
draft: false

lang: zh
product: "Watermark"
product_tag: "watermark"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "C# .NET 文档水印软件 | 添加水印"
head_description: "用于在文档中添加、搜索和删除水印的 C# .NET 库：PDF、Word、Excel、演示文稿、Visio 图表、电子邮件和图像文件格式。"

############################# Header ############################
title: "在 C# .NET 应用程序中轻松为文档添加水印"
description: "使用灵活的文档水印 API 为您的 C# 解决方案提供支持，该水印可为所有常用文档格式添加可自定义的水印。"
words:
  for: "为了"

actions:
  main: "免费 NuGet 下载"
  main_link: "https://www.nuget.org/packages/GroupDocs.Watermark"
  alt: "许可"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/net/"
  title: "准备好开始了吗？"
  description: "免费试用 GroupDocs.Watermark 项功能或申请许可证"

release:
  title: "版本 {0} 已发布"
  notes: "查看新增内容"
  downloads: "下载"

code:
  title: "在 C# 中给 PDF 个文件加水印"
  more: "更多例子"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
  install: "dotnet add package GroupDocs.Watermark"
  content: |
    ```csharp {style=abap}   
    // 通过 PDF 路径实例化 Watermarker
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    using (Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions))
    {
        // 自定义水印选项
        TextWatermark textWatermark = 
            new TextWatermark("Approved", new Font("Arial", 8));
        
        // 向 PDF 文档应用水印
        watermarker.Add(textWatermark);

        // 保存结果文档
        watermarker.Save("result.pdf");
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark 一览"
  description: "通过 .NET 在文档上添加水印的 API"
  features:
    # feature loop
    - title: "C# 文件水印"
      content: "使用 GroupDocs.Watermark 为您的企业文件添加水印。使用文本、图像、图表或电子邮件附件。"

    # feature loop
    - title: "根据您的目标自定义水印"
      content: "GroupDocs.Watermark for .NET 软件允许以各种方式自定义水印。粗体、斜体、字体类型等文本样式以及旋转等图像属性丰富了水印过程。"

    # feature loop
    - title: "支持所有流行的文件格式"
      content: "GroupDocs.Watermark 解决方案支持许多文件和文档格式。PDF、Microsoft Office Word、Excel、PowerPoint、JPEG、PNG、GIF、GIF、BMP、Visio、Visio 图表、电子邮件等图像可以使用我们的水印进行保护。"

    # feature loop
    - title: "搜索和更新水印"
      content: "可能会找到并重新处理已在文档中显示的水印。无需额外努力即可修改文本、样式、图像或删除显示的水印。"

############################# Platforms ############################
platforms:
  enable: true
  title: "平台独立性"
  description: "GroupDocs.Watermark for .NET 支持下面列出的操作系统、框架和包管理器"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "支持的文件格式"
  description: |
    GroupDocs.Watermark for .NET 提供以下 [文件格式](https://docs.groupdocs.com/watermark/net/supported-document-formats/) 的处理。
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office 和 OpenDocument 格式
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### 图像和图形
        * **流行的图像格式:** BMP, JPG, JPEG, PNG
        * **多页图片:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### 其他
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark 个功能"
  description: "通过水印保护 PDF、Office、图像和其他格式"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "文件水印"
      content: "在各种文件格式的特定部分或整个文档中添加或删除水印。"

    # feature loop
    - icon: "watermark_style"
      title: "设置水印样式"
      content: "自定义各种水印属性，如颜色、字体、旋转等。"

    # feature loop
    - icon: "hidden_print"
      title: "PDF 隐藏的打印水印"
      content: "为仅在打印文档时出现的 PDF 分配隐藏水印。"

    # feature loop
    - icon: "image_only"
      title: "仅为文档中的图像添加水印"
      content: "为特定部分、页面、幻灯片或文档中的所有图像添加水印。"

    # feature loop
    - icon: "image_frame"
      title: "处理选定的图像框架"
      content: "仅为多帧图像的特定帧分配水印。"

    # feature loop
    - icon: "attachments"
      title: "附件和形状"
      content: "为 Excel 文档中的所有附件和幻灯片中的所有图像形状设置水印。"

    # feature loop
    - icon: "pdf_objects"
      title: "PDF 个对象"
      content: "将水印与 PDF 文档中的出血框、艺术框、裁剪框或修剪框对齐。"

    # feature loop
    - icon: "doc_background"
      title: "文件背景"
      content: "在电子表格或幻灯片的背景图像中添加水印或将其删除。"

    # feature loop
    - icon: "unreadable_characters"
      title: "不可读字符保护"
      content: "在演示文稿中使用不可读字符保护文本水印。"

    # feature loop
    - icon: "watermark_text_search"
      title: "在文档中搜索水印"
      content: "根据特定参数或组合多个条件搜索水印。"

    # feature loop
    - icon: "watermark_image_search"
      title: "搜索相似的图片水印"
      content: "寻找与特定图像相似的图像水印。"

    # feature loop
    - icon: "document_info"
      title: "获取文件信息"
      content: "以编程方式提取支持格式的页面设置和其他信息。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "代码示例"
  description: "典型 GroupDocs.Watermark for .NET 操作的一些用例"
  items:
    # code sample loop
    - title: "通过向文档添加图像来添加水印。"
      content: |
        要保护任何文档，您可以使用 [图像水印](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/)：
        {{< landing/code title="如何通过图像水印保护文件。">}}
        ```csharp {style=abap}
        // 将源文档加载到 Watermarker
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // 指定水印图像的路径
            using (ImageWatermark watermark = new ImageWatermark("watermark.jpg"))
            {
                // 保护文件并将其保存
                watermarker.Add(watermark);

                watermarker.Save("result.pdf");
            }
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "搜索和修改现有水印。"
      content: |
        GroupDocs.Watermark 能够 [修改已在文档中显示的水印](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/)。搜索所需的项目并更新其属性。
        {{< landing/code title="水印搜索和修改。">}}
        ```csharp {style=abap}   
        // 加载源文档
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // 搜索要更新的水印
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                // 更新所需的属性
                watermark.Text = "New Text";
            }

            // 将修改后的文档保存到指定路径
            watermarker.Save("document.pdf");
        }
        ```
        {{< /landing/code >}}

---
