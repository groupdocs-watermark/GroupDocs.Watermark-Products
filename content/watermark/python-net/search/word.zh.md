
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:16
draft: false
lang: zh
format: Word
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "识别 Word 文档中的隐藏水印"
head_description: "使用 GroupDocs.Watermark 轻松搜索文档中的隐藏水印。"

############################# Header ############################
title: "快速查找 Word 文档中的水印" 
description: "使用 GroupDocs.Watermark for Python via .NET 揭示和审查隐藏的水印内容。"
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费获取 PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "了解 GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET 是一款强大的水印操作工具，适用于 Python。无论您是添加、删除还是搜索水印，它支持 DOCX、XLSX、PDF 等格式。

############################# Steps ############################
steps:
    enable: true
    title: "如何通过 Python 检测 Word 文件中的水印"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/python-net/)** 使在商业文档中识别嵌入式水印变得简单。将其功能融入您的 Python 工作流程，实现无缝检测。
      
      1. 首先，将 Word 文档加载到 **Watermarker** 类的实例中。可以接受的输入方式包括路径、流或字节数组。
      2. 使用 **SearchCriteria** 对象缩小搜索范围。要查找基于图像的标记，使用示例图像；对于文本水印，指定内容、样式或颜色等特征。
      3. 调用 **Search** 方法，从 **Watermarker** 对象提取水印数据。将返回一系列水印实例以供检查。
      4. 获取结果后，您可以管理它们：删除不需要的标记，或更新尺寸、内容等详细信息。
   
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
        # 检测 WORD 格式中的文本水印
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # 使用 WORD 文件初始化 Watermarker
        with gw.Watermarker("input.docx") as watermarker:

            # 执行水印搜索
            search_criteria = gwss.TextSearchCriteria("test", False)
            possible_watermarks = watermarker.search(search_criteria)

            # 处理检测到的水印列表
            print("\nFound {0} possible watermark(s).".format(len(possible_watermarks)))
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "借助 GroupDocs.Watermark 强大的水印检测"
  description: "在您的 Python 项目中使用 GroupDocs.Watermark，高效扫描和定位各种文档类型中的水印元素。"
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "检测水印"
  features:
    # feature loop
    - title: "智能过滤器的高级检测"
      content: "轻松识别各种文档格式中的水印。GroupDocs.Watermark 支持通过视觉和文本特征（包括形状、透明度等）进行过滤。"

    # feature loop
    - title: "灵活的搜索标准"
      content: "使用 GroupDocs.Watermark 定义个性化的水印搜索参数。这种精准度使隐蔽或定制水印数据的检索变得更为高效。"

    # feature loop
    - title: "访问和整理检测到的水印"
      content: "通过提取所有嵌入水印简化文档审计。我们的工具能够高效提取、显示和管理找到的项目。"
      
  code_samples:
    # code sample loop
    - title: "代码示例：检测水印"
      content: |
        查看如何使用 GroupDocs.Watermark 根据灵活的检测规则搜索文档中的嵌入水印内容。
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # 从磁盘或流中打开目标文档
        load_options = gwos.SpreadsheetLoadOptions()
        with gw.Watermarker("source.xlsx", load_options) as watermarker:

            # 定义搜索中使用的特定水印属性
            criteria = gwss.TextFormattingSearchCriteria()
            criteria.foreground_color_range = gwss.ColorRange()
            criteria.foreground_color_range.min_hue = -5.0
            criteria.foreground_color_range.max_hue = 10.0
            criteria.foreground_color_range.min_brightness = 0.01
            criteria.foreground_color_range.max_brightness = 0.99
            criteria.background_color_range = gwss.ColorRange()
            criteria.background_color_range.is_empty = True
            criteria.font_name = "Arial"
            criteria.min_font_size = 19.0
            criteria.max_font_size = 42.0
            criteria.font_bold = True

            # 执行搜索并收集匹配项
            possible_watermarks = watermarker.search(criteria)

            # 利用找到的结果进行进一步操作
            print("Found {0} possible watermark(s).".format(len(possible_watermarks)))
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
    title: "跨格式检测能力"
    exclude: "WORD"
    description: "支持对多种广泛使用的文件类型进行水印分析。"
    items: 
        # format loop 1
        - name: "水印 PDF"
          format: "PDF"
          link: "/watermark/python-net/search//pdf/"
          description: "Adobe Portable 文档格式"

        # format loop 2
        - name: "水印 Word"
          format: "WORD"
          link: "/watermark/python-net/search//word/"
          description: "MS Word 和 Open Office 文档"
          
        # format loop 3
        - name: "水印 Excel"
          format: "EXCEL"
          link: "/watermark/python-net/search//excel/"
          description: "MS Excel 和 Open Office 电子表格"

        # format loop 4
        - name: "水印 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/search//powerpoint/"
          description: "MS PowerPoint 和开放办公室演示"

        # format loop 5
        - name: "水印 DOCX"
          format: "DOCX"
          link: "/watermark/python-net/search//docx/"
          description: "微软 Word 打开 XML 文档"
          
        # format loop 6
        - name: "水印 PPTX"
          format: "PPTX"
          link: "/watermark/python-net/search//pptx/"
          description: "PowerPoint 打开 XML 演示文稿"
          
        # format loop 7
        - name: "水印 XLSX"
          format: "XLSX"
          link: "/watermark/python-net/search//xlsx/"
          description: "微软 Excel 打开 XML 电子表格"

        # format loop 8
        - name: "水印 DOC"
          format: "DOC"
          link: "/watermark/python-net/search//doc/"
          description: "微软 Word 97-2007 文档"

        # format loop 9
        - name: "水印 XLS"
          format: "XLS"
          link: "/watermark/python-net/search//xls/"
          description: "微软 Excel 工作簿 97-2003"

        # format loop 10
        - name: "水印 PPT"
          format: "PPT"
          link: "/watermark/python-net/search//ppt/"
          description: "PowerPoint 演示 97-2003"

        # format loop 11
        - name: "水印 RTF"
          format: "RTF"
          link: "/watermark/python-net/search//rtf/"
          description: "富文本格式"

---