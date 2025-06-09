
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: zh
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "向 Excel 文件添加水印"
head_description: "使用 Python 自动向 Excel 文件添加图片水印。一次处理多个文件以保持一致的保护。"

############################# Header ############################
title: "使用 Python 向 Excel 添加水印" 
description: "使用 Python 轻松向 Excel 文件添加文本或图像水印。我们的指南向您展示如何保持电子表格的专业性和安全性，几乎无需手动操作。"
subtitle: "GroupDocs.Watermark for Python via .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费下载 PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET 库"
    link: "/watermark/python-net/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET 使您能够在 Python 中向 Excel 电子表格添加水印。您可以使用不同的水印类型并自定义不透明度、旋转和对齐方式。该库还帮助您查找和管理现有水印，以确保文件的安全性。

############################# Steps ############################
steps:
    enable: true
    title: "轻松添加水印：为 Excel 的 Python 水印处理"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** 是一个库，使您能够轻松地向许多商业文件类型添加水印。按照以下步骤快速在 Python 中为您的文档添加水印：
      
      1. **开始水印处理：** 通过创建 **Watermarker** 类的实例来开始。将您的 Excel 文件（作为路径或流）传递给构造函数，以便为水印处理打开该文件。
      2. **创建水印：** 用所需的文本和设置创建一个 **Watermark** 对象。您可以向任何页面或文档元素（如页眉或附件）添加水印。
      3. **自定义水印：** 调整水印的大小、位置、字体、颜色和对齐方式，以满足您的需要。这可以帮助您的水印在文档中看起来恰到好处。
      4. **应用并保存：** 使用 **Watermarker** 方法将水印添加到文档中。保存结果，最好保存在新文件中以确保安全。
   
    code:
      platform: "python-net"
      copy_title: "复制"
      install:
        command: |
        command: "pip install groupdocs-watermark-net"
        copy_tip: "点击复制"
        copy_done: "复制的"
      links:
        #  loop
        - title: "更多例子"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
        #  loop
        - title: "文档"
          link: "https://docs.groupdocs.com/watermark/python-net/"
          
      content: |
        ```python {style=abap}
        # 向 EXCEL 文件添加文本水印
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # 选择您要添加水印的文件
        with gw.Watermarker("input.xslx") as watermarker:

            # 创建文本水印对象
            font = gww.Font("Arial", 36.0)
            watermark = gww.TextWatermark("top secret", font)
            watermark.foreground_color = gww.Color.red
            watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
            watermark.opacity = 0.4

            watermarker.add(watermark)

            # 保存更新后的 EXCEL 文件
            watermarker.save("output.xslx")
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "探索更多水印功能"
  description: "使用我们的 Python API 在文档、幻灯片、图表等中添加、查看、转换和管理水印。GroupDocs.Watermark for Python via .NET 帮助您保护文件并轻松添加版权信息。"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "添加水印"
  features:
    # feature loop
    - title: "轻松添加水印"
      content: "GroupDocs.Watermark 使 Python 开发者能够快速向商业文件添加文本、水印或动态水印。以最小的努力保护您的文件和品牌。"

    # feature loop
    - title: "完全可自定义的水印"
      content: "使用 GroupDocs.Watermark 更改水印的大小、旋转、透明度、颜色和字体。确保您的水印完美适配文档，同时保持重要内容的可见性。"

    # feature loop
    - title: "利用文档特性进行水印处理"
      content: "利用 PDF 注释、Word 背景或 Excel 页眉等内置文档特性来添加水印。GroupDocs.Watermark 与文档结构协作，实现有效且不干扰的水印处理。"
      
  code_samples:
    # code sample loop
    - title: "向 DOCX 添加图像水印"
      content: |
        此示例展示如何将图像效果应用于形状水印。
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.wordprocessing as gwow

        # 打开 Word 文档
        load_options = gwow.WordProcessingLoadOptions()
        with gw.Watermarker("source.docx", load_options) as watermarker:

            # 设置水印选项
            with gww.ImageWatermark("logo.png") as watermark:

                effects = gwow.WordProcessingImageEffects()
                effects.brightness = 0.7
                effects.contrast = 0.6
                effects.chroma_key = gww.Color.red

                options = gwow.WordProcessingWatermarkSectionOptions()
                options.Effects = effects;

                # 创建水印
                watermarker.add(watermark, options)

                # 保存带水印的文档
                watermarker.save("result.docx")
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "准备好开始了吗？"
  description: "免费试用 GroupDocs.Watermark 项功能或申请许可证"
  items:
    #  loop
    - title: "PyPi 下载"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      color: "red"
        #  loop
    - title: "许可"
      link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "使用 Python 向 Excel 添加文本和图像水印"
    exclude: "EXCEL"
    description: "使用 GroupDocs.Watermark 快速向 Excel 文件添加自定义水印。通过灵活的水印工具提高文档的安全性和品牌影响力。"
    items: 
        # format loop 1
        - name: "水印 PDF"
          format: "PDF"
          link: "/watermark/python-net/add//pdf/"
          description: "Adobe Portable 文档格式"

        # format loop 2
        - name: "水印 Word"
          format: "WORD"
          link: "/watermark/python-net/add//word/"
          description: "MS Word 和 Open Office 文档"
          
        # format loop 3
        - name: "水印 Excel"
          format: "EXCEL"
          link: "/watermark/python-net/add//excel/"
          description: "MS Excel 和 Open Office 电子表格"

        # format loop 4
        - name: "水印图片"
          format: "IMAGE"
          link: "/watermark/python-net/add//image/"
          description: "流行的图像格式"

        # format loop 5
        - name: "水印照片"
          format: "PHOTO"
          link: "/watermark/python-net/add//photo/"
          description: "照片格式"

        # format loop 6
        - name: "水印 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/add//powerpoint/"
          description: "MS PowerPoint 和开放办公室演示"

        # format loop 7
        - name: "水印 DOCX"
          format: "DOCX"
          link: "/watermark/python-net/add//docx/"
          description: "微软 Word 打开 XML 文档"
          
        # format loop 8
        - name: "水印 PPTX"
          format: "PPTX"
          link: "/watermark/python-net/add//pptx/"
          description: "PowerPoint 打开 XML 演示文稿"
          
        # format loop 9
        - name: "水印 XLSX"
          format: "XLSX"
          link: "/watermark/python-net/add//xlsx/"
          description: "微软 Excel 打开 XML 电子表格"

        # format loop 10
        - name: "水印 JPEG"
          format: "JPEG"
          link: "/watermark/python-net/add//jpeg/"
          description: "JPEG 图片"

        # format loop 11
        - name: "水印 PNG"
          format: "PNG"
          link: "/watermark/python-net/add//png/"
          description: "Portable 网络图形"

        # format loop 12
        - name: "水印 TIFF"
          format: "TIFF"
          link: "/watermark/python-net/add//tiff/"
          description: "标记图像文件格式"

        # format loop 13
        - name: "WEBP 水印"
          format: "WEBP"
          link: "/watermark/python-net/add//webp/"
          description: "网络图片"

        # format loop 14
        - name: "水印 DOC"
          format: "DOC"
          link: "/watermark/python-net/add//doc/"
          description: "微软 Word 97-2007 文档"

        # format loop 15
        - name: "水印 XLS"
          format: "XLS"
          link: "/watermark/python-net/add//xls/"
          description: "微软 Excel 工作簿 97-2003"

        # format loop 16
        - name: "水印 PPT"
          format: "PPT"
          link: "/watermark/python-net/add//ppt/"
          description: "PowerPoint 演示 97-2003"

        # format loop 17
        - name: "水印 RTF"
          format: "RTF"
          link: "/watermark/python-net/add//rtf/"
          description: "富文本格式"

---