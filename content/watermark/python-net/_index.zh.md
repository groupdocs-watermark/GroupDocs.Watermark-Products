---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:49
draft: false

lang: zh
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

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
    # supported_platforms loop
    - title: "Python"
      tag: "python-net"

############################# Head ############################
head_title: "Python 水印库 |文档水印"
head_description: "Python 使用文本和图像水印保护商业文档。支持 PDF、Word、Excel 和 PowerPoint 等文件格式。"

############################# Header ############################
title: "访问 Python via .NET 水印技术"
description: "使用此 Python 解决方案保护您的数据并防止未经授权的复制。轻松为各种格式的商业文档添加水印，包括PDF、Word、Excel、PowerPoint、图像等。"
words:
  for: "为了"

actions:
  main: "PyPi 免费下载"
  main_link: "https://pypi.org/project/groupdocs-watermark-net/"
  alt: "许可"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
  title: "准备好开始了吗？"
  description: "免费试用 GroupDocs.Watermark 项功能或申请许可证"

release:
  title: "版本 {0} 已发布"
  notes: "查看新增内容"
  downloads: "下载"
  link: "https://releases.groupdocs.com/watermark/python-net/"

code:
  title: "使用 Python 添加水印到 PDF"
  more: "更多例子"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
  install: "pip install groupdocs-watermark-net"
  content: |
    ```python {style=abap}

    import groupdocs.watermark as gw
    import groupdocs.watermark.watermarks as gww
    import groupdocs.watermark.options.pdf as gwop
    import groupdocs.watermark.common as gwc

    # 通过 PDF 路径实例化 Watermarker
    pdf_lo = gwop.PdfLoadOptions()
    with gw.Watermarker("source.pdf", pdf_lo) as watermarker:
        options = gwop.PdfArtifactWatermarkOptions()

        # 自定义水印选项
        text_watermark = 
            gww.TextWatermark("Approved", gww.Font("Arial", 8.0))
        text_watermark.horizontal_alignment = 
            gwc.HorizontalAlignment.RIGHT

        # 向 PDF 文档应用水印
        watermarker.add(text_watermark, options)

        # 保存结果文档
        watermarker.save("result.pdf")

    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark 一览"
  description: "用于水印的 Python 库"
  features:
    # feature loop
    - title: "Python 文档水印"
      content: "使用 GroupDocs.Watermark for Python via .NET 保护您的敏感数据。将文本或图像作为水印放置在各种文件格式上。"

    # feature loop
    - title: "自定义水印"
      content: "GroupDocs.Watermark for Python via .NET 中提供了许多自定义选项。设置文本样式（粗体、斜体、字体）或图像属性（例如大小或旋转）以调整文档水印。"

    # feature loop
    - title: "流行的文件格式支持"
      content: "GroupDocs.Watermark for Python via .NET支持多种文件格式，包括 PDF、Word、Excel、PowerPoint 等 MS Office 文档以及 JPEG、PNG、GIF、BMP、Visio 图表、电子邮件等图像。增强文档处理以满足业务需求目标。"

    # feature loop
    - title: "水印搜索和更新"
      content: "检索和更新文档中放置的水印。修改文本样式、图像内容或完全删除它们。 GroupDocs.Watermark for Python via .NET 提供广泛的水印处理功能。"

############################# Platforms ############################
platforms:
  enable: true
  title: "平台独立性"
  description: "GroupDocs.Watermark for Python via .NET 与各种操作系统和包管理器无缝集成。"
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "支持的文件格式"
  description: |
    GroupDocs.Watermark for Python via .NET 使您能够处理各种文件格式。 [探索完整列表](https://docs.groupdocs.com/watermark/net/supported-document-formats/)。
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
  title: "GroupDocs.Watermark for Python via .NET 功能"
  description: "通过程序化水印增强文档安全性。处理多种文件格式，包括 PDF、DOCX、XLSX、PPTX 和图像格式（PNG、JPG 等）。"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "精确的水印控制"
      content: "通过在不同文件格式的特定部分、整个文档或单个附件和形状中添加或删除水印来精确管理水印。"

    # feature loop
    - icon: "watermark_style"
      title: "自定义水印外观"
      content: "通过修改文档中的颜色、字体、不透明度、旋转和位置等属性，对水印美观进行细粒度控制。"

    # feature loop
    - icon: "hidden_print"
      title: "打印 PDF 水印"
      content: "将隐藏水印添加到常规文档中，这些水印仅在打印过程中可见，从而谨慎地增强文档安全性。"

    # feature loop
    - icon: "image_only"
      title: "特定图像水印"
      content: "使用我们的解决方案为文档中的特定图像添加水印。将水印嵌入指定部分（例如页面、幻灯片）或整个文档。"

    # feature loop
    - icon: "image_frame"
      title: "多层图像水印"
      content: "将水印精确添加到多帧图像格式中的特定帧，实现对水印放置的精细控制。"

    # feature loop
    - icon: "attachments"
      title: "全面的内容保护"
      content: "将保护范围扩展到各种文档元素，例如 Excel 文档中的附件和演示文稿中的图像形状，从而提供额外的安全层。"

    # feature loop
    - icon: "pdf_objects"
      title: "高级 PDF 水印"
      content: "对PDF的不同区域添加水印，包括出血框、艺术框、裁剪框、裁切框等。"

    # feature loop
    - icon: "doc_background"
      title: "背景图像水印"
      content: "管理电子表格和演示文稿背景图像中的水印，为视觉安全措施提供额外的自定义选项。"

    # feature loop
    - icon: "unreadable_characters"
      title: "带有不可读字符的文本水印"
      content: "在演示文稿中嵌入的文本水印中使用不可读的字符，通过使未经授权的水印提取更具挑战性来增强安全性。"

    # feature loop
    - icon: "watermark_text_search"
      title: "高级水印搜索"
      content: "使用全面的搜索功能根据特定参数或组合各种条件来查找文档中的水印。"

    # feature loop
    - icon: "watermark_image_search"
      title: "相似图像水印检测"
      content: "在文档中查找视觉上与源图像相似的相似水印图像。"

    # feature loop
    - icon: "document_info"
      title: "分析文档信息"
      content: "提取页面设置等基本文档数据以进行进一步分析。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "代码示例"
  description: "探索展示常见 GroupDocs.Watermark for Python via .NET 功能的代码示例。"
  items:
    # code sample loop
    - title: "使用图像为文档添加水印"
      content: |
        使用 GroupDocs.Watermark for Python via .NET 通过添加图像水印来保护文档。 [了解更多](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/)。
        {{< landing/code title="如何通过图像水印保护文件。">}}
        ```python {style=abap}

        # 将源文档加载到 Watermarker
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # 指定水印图像的路径
            watermark = groupdocs.watermark.watermarks.ImageWatermark("watermark.jpg")
            watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwgroupdocs.watermark.common.VerticalAlignment.CENTER

            # 保护文件并将其保存
            watermarker.add(watermark)
            watermarker.save("result.pdf")
       
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "搜索和修改现有水印"
      content: |
        GroupDocs.Watermark for Python via .NET 使您能够管理文档水印。选择水印并修改其属性。 [了解如何](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/)。
        {{< landing/code title="水印搜索和修改。">}}
        ```python {style=abap}

        # 加载源文档
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # 搜索要更新的水印
            search_criteria = groupdocs.watermark.search.searchcriteria.TextSearchCriteria("annotation", False)
            watermarks = watermarker.search(search_criteria)
            
            # 更新所需的属性
            for watermark in watermarks:
                watermark.text = "passed"

            # 将修改后的文档保存到指定路径
            watermarker.save("result.pdf")


        ```
        {{< /landing/code >}}

---
