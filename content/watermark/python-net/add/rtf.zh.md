
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:29
draft: false
lang: zh
format: Rtf
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Python 为 RTF 文档添加水印"
head_description: "在 Python 中为 RTF 文件添加水印，以保护您的 Word 文档。"

############################# Header ############################
title: "使用 Python 水印保护 RTF" 
description: "使用 Python 为 RTF 文件添加安全的自定义水印——非常适用于敏感的 Word 文档。"
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "在 PyPi 免费获取"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET 提供了高级工具，能在 Python 中为 RTF 文档添加水印。可以使用可见或透明的标记，调整其字体、颜色、大小和位置。非常适合法律、商业或机密文件，GroupDocs.Watermark 有助于防止复制和编辑。

############################# Steps ############################
steps:
    enable: true
    title: "快速向 Rtf 文件添加水印"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/):** 一个强大的 Python 库，可以帮助您轻松向文档添加水印。
      
      1. **主要类：Watermarker.** 首先创建一个 **Watermarker** 对象。将您的 Rtf 文件作为文件路径或流传递给它，以便开始。
      2. **构建您的水印.** 接下来，创建您想要的水印类型的 Watermark 对象。您可以将其放置在任何页面上，甚至在文档元素中，如图像或页眉。
      3. **调整外观.** 设置水印的大小、位置、字体和颜色，以满足您的需求。
      4. **添加并保存.** 使用 **Watermarker** 方法插入您的水印。您可以添加任意数量的水印，然后将文件保存到所需的位置。
   
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
        # 向 RTF 文件添加图像水印。
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # 将文件路径传递给 Watermarker 构造函数。
        with gw.Watermarker("input.rtf") as watermarker:

            # 使用您的图像文件创建图像水印。
            watermark = gww.ImageWatermark("watermark.png")

            watermarker.add(watermark)

            # 保存带水印的 RTF 文件。
            watermarker.save("output.rtf")
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "发现更多水印工具"
  description: "GroupDocs.Watermark for Python via .NET 为您提供了在多种文件类型中添加和自定义水印的高级选项。使用灵活、易于使用的功能保护您的文档和图像。"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "全方位的水印工具"
  features:
    # feature loop
    - title: "全页面铺贴"
      content: "使用平铺水印覆盖整个文档。这使得水印难以移除，保护您的文件，同时保持布局的完整性。"

    # feature loop
    - title: "自定义颜色"
      content: "为您的水印选择任意颜色，以匹配您的品牌或文档风格。根据需要让水印突出或融入。"

    # feature loop
    - title: "额外的安全选项"
      content: "通过分层水印增强文档安全性。结合可见和隐藏的标记，防止复制，并确保只有合适的人能访问您的文件。"
      
  code_samples:
    # code sample loop
    - title: "向 PowerPoint 添加水印"
      content: |
        此示例演示如何在 PPTX 幻灯片的背景上添加水印。
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.presentation as gwop

        # 打开 PPTX 文件。
        load_options = gwop.PresentationLoadOptions()
        with gw.Watermarker("source.pptx", load_options) as watermarker:

            # 设置水印细节。
            with TextWatermark("Protected image", gww.Font("Arial", 8.0)) as watermark:

                watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
                watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
                watermark.rotate_angle = 45
                watermark.scale_factor = 1

                # 将水印应用于幻灯片背景。
                watermarker.add(watermark)

                # 保存更新的演示文稿。
                watermarker.save("result.pptx")
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
    title: "使用 Python 为 RTF 添加水印"
    exclude: "RTF"
    description: "利用 Python 为 RTF 文件添加强大且细腻的水印，以提升文档安全性。"
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