
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:29
draft: false
lang: zh
format: Doc
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "自信地修改Doc文件中的水印"
head_description: "通过GroupDocs.Watermark for Python via .NET API，精确更改Doc水印，同时保持布局和品牌形象。"

############################# Header ############################
title: "通过Python更新Doc文件中的水印" 
description: "通过无缝的水印编辑，提升并保护您的文件，使用GroupDocs.Watermark for Python via .NET API。"
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "从PyPi获取最新版本"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET平台"
    link: "/watermark/python-net/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **简化水印编辑：** 使用GroupDocs.Watermark for Python via .NET在您的Python应用程序中简化Doc文件的水印管理。

############################# Steps ############################
steps:
    enable: true
    title: "使用Python API修改Doc文档中的水印"
    content: |
      通过**[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)**，Python开发者可以修改各种Doc文档中的水印内容。以下是快速指南：
      
      1. 首先，使用**Watermarker**类加载Doc文档，支持文件路径、内存流或字节数组作为输入。
      2. 创建一个**SearchCriteria**对象，以搜索文档中现有的水印元素，这些可以是文本或图形。
      3. 识别后，工具会提供一组匹配的水印实例，您可以更新它们——调整颜色、对齐、字体，甚至嵌入的图像数据等参数。
      4. 最后，使用内置的保存方法，将修订后的文档保存到磁盘或任何支持的输出流。
   
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
        # 更新DOC文件中的图片水印
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # 创建带有输入文件的Watermarker实例
        with gw.Watermarker("input.doc") as watermarker:

            # 使用SearchCriteria定位基于图片的水印
            search_criteria = gwss.ImageDctHashSearchCriteria("logo.png")

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # 应用对图片水印的更改
                        watermark.ImageData = imageData
                    except Exception as e:
                        pass

            # 导出更新后的DOC文件
            watermarker.save("output.doc")
        ```     

############################# More features ############################
more_features:
  enable: true
  title: "通过高级水印工具提升生产力"
  description: "通过我们的动态水印 API，加速在Python中的文档品牌化和保护。以最小的努力插入、检测、修改或删除水印层。"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "高级水印编辑工作流程"
  features:
    # feature loop
    - title: "集成水印控制"
      content: "使用GroupDocs.Watermark for Python via .NET为您的Python应用程序提供完整的水印生命周期控制。通过自动化水印的设置、更新和删除，避免重复性任务。"

    # feature loop
    - title: "水印属性的精确调节"
      content: "全面掌控水印的美学——根据我们的灵活 API 接口调整大小、重新上色、旋转或重新定位，以满足任何视觉要求。"

    # feature loop
    - title: "利用本地格式特性"
      content: "通过将水印嵌入到页眉、页脚、注释或背景中，适应任何文件格式。我们的 API 尊重本地结构，以实现最佳集成。"
      
  code_samples:
    # code sample loop
    - title: "在PDF文件中修改水印"
      content: |
        展示如何在PDF文档中更改水印属性。
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # 打开PDF文件
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.pdf as gwop

        # 读取水印内容
        load_options = gwop.PdfLoadOptions()
        with gw.Watermarker("source.pdf", load_options) as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,5,8]

            # 应用水印更新
            watermarks = watermarker.search(search_criteria)
            for watermark in watermarks:
                try:
                    watermark.formatted_text_fragments.clear()
                    watermark.formatted_text_fragments.add(
                        "New text", 
                        gww.Font("Calibri", 5.0, gww.FontStyle.bold), 
                        gww.Color.white, 
                        gww.Color.aqua
                    )
                except Exception as e:
                    pass
        
            # 保存编辑后的结果
            watermarker.save("output.pdf")
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
    title: "跨格式水印编辑"
    exclude: "DOC"
    description: "使用GroupDocs.Watermark for Python via .NET API轻松修改多种文档类型中的水印。"
    items: 
        # format loop 1
        - name: "水印 PDF"
          format: "PDF"
          link: "/watermark/python-net/edit//pdf/"
          description: "Adobe Portable 文档格式"

        # format loop 2
        - name: "水印 Word"
          format: "WORD"
          link: "/watermark/python-net/edit//word/"
          description: "MS Word 和 Open Office 文档"
          
        # format loop 3
        - name: "水印 Excel"
          format: "EXCEL"
          link: "/watermark/python-net/edit//excel/"
          description: "MS Excel 和 Open Office 电子表格"

        # format loop 4
        - name: "水印 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/edit//powerpoint/"
          description: "MS PowerPoint 和开放办公室演示"

        # format loop 5
        - name: "水印 DOCX"
          format: "DOCX"
          link: "/watermark/python-net/edit//docx/"
          description: "微软 Word 打开 XML 文档"
          
        # format loop 6
        - name: "水印 PPTX"
          format: "PPTX"
          link: "/watermark/python-net/edit//pptx/"
          description: "PowerPoint 打开 XML 演示文稿"
          
        # format loop 7
        - name: "水印 XLSX"
          format: "XLSX"
          link: "/watermark/python-net/edit//xlsx/"
          description: "微软 Excel 打开 XML 电子表格"

        # format loop 8
        - name: "水印 DOC"
          format: "DOC"
          link: "/watermark/python-net/edit//doc/"
          description: "微软 Word 97-2007 文档"

        # format loop 9
        - name: "水印 XLS"
          format: "XLS"
          link: "/watermark/python-net/edit//xls/"
          description: "微软 Excel 工作簿 97-2003"

        # format loop 10
        - name: "水印 PPT"
          format: "PPT"
          link: "/watermark/python-net/edit//ppt/"
          description: "PowerPoint 演示 97-2003"

        # format loop 11
        - name: "水印 RTF"
          format: "RTF"
          link: "/watermark/python-net/edit//rtf/"
          description: "富文本格式"

---