
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
head_title: "使用 Python 从 Word 中删除水印"
head_description: "使用我们的 Python API 快速删除或编辑 Word 文件中的水印，以实现清晰、专业的文档。"

############################# Header ############################
title: "Word 水印清除器，适用于 Python" 
description: "利用 GroupDocs.Watermark for Python via .NET API 从 Word 文件中清除水印，保持法律和商务文件的整洁。"
subtitle: "GroupDocs.Watermark for Python via .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "在 PyPi 免费获取"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET 库"
    link: "/watermark/python-net/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       通过 GroupDocs.Watermark for Python via .NET，您可以轻松查找并移除 Word 文件中的水印。在保持文档布局完好的同时，检测、修改或删除文本和图像水印。

############################# Steps ############################
steps:
    enable: true
    title: "如何在 Python 中从 Word 文件中移除水印"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/python-net/)** 可以帮助您轻松地从商务文档中清除水印。在您的 Python 项目中添加我们的库并按照以下步骤操作：
      
      1. 首先，创建一个 **Watermarker** 对象，传入您的 Word 文件。您可以使用文件路径或流作为输入。
      2. 使用 **SearchCriteria** 来过滤您想要移除的水印。您可以按文本、图像或格式进行搜索。提供的细节越多，搜索结果越准确。
      3. 遍历找到的水印，移除文档中您不需要的水印。
      4. 完成后，将清理后的文档保存为文件或流。
   
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
        # 从 Word 文件中删除文本水印
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # 使用 Watermarker 实例打开 Word 文件
        with gw.Watermarker("input.docx") as watermarker:

            # 查找并移除选中的水印
            search_criteria = gwss.TextFormattingSearchCriteria("test", False)
            criteria.ForegroundColorRange = gwss.ColorRange()
            criteria.FontBold = True

            possible_watermarks = watermarker.search(search_criteria)
            watermarks.clear()

            # 将更新后的文件保存到您选择的位置
            watermarker.save("output.docx")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "使用 Python 高效移除水印"
  description: "我们的 Python API 可帮助您快速从 PDF 和办公文件中移除水印，保持文档的清晰和原始。"
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "清除水印"
  features:
    # feature loop
    - title: "精准的水印删除"
      content: "Python API 允许您删除水印，而不会损坏文档的布局或质量。此工具专为需要可靠结果的开发者设计。"

    # feature loop
    - title: "批量删除水印"
      content: "可以轻松从多个文件中同时清除水印。这非常适合需要快速安全处理大量文档的公司。"

    # feature loop
    - title: "水印的高级编辑"
      content: "使用高级选项在删除水印之前进行微调或编辑。这有助于保持文档的专业外观和安全性。"
      
  code_samples:
    # code sample loop
    - title: "从 Excel 中删除文本水印"
      content: |
        此示例展示了如何删除 Excel 文件中特殊格式的文本水印。
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # 打开 Excel 文件
        with gw.Watermarker("source.xlsx") as watermarker:

            # 搜索水印
            search_criteria = gwss.TextSearchCriteria("someurl.com")

            # 删除水印
            watermarks = watermarker.search(search_criteria)

            for i in range(len(watermarks) - 1, -1, -1):
                if isinstance(watermarks[i], gws.HyperlinkPossibleWatermark):
                    del watermarks[i]

            # 保存清理后的 XLSX 文件
            watermarker.save("result.xlsx");
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
    title: "在 Word 中的水印管理，适用于 Python"
    exclude: "WORD"
    description: "发现如何使用我们的 Python API 管理和移除 Word 文件中的水印，以提升文档质量。"
    items: 
        # format loop 1
        - name: "水印 PDF"
          format: "PDF"
          link: "/watermark/python-net/remove//pdf/"
          description: "Adobe Portable 文档格式"

        # format loop 2
        - name: "水印 Word"
          format: "WORD"
          link: "/watermark/python-net/remove//word/"
          description: "MS Word 和 Open Office 文档"
          
        # format loop 3
        - name: "水印 Excel"
          format: "EXCEL"
          link: "/watermark/python-net/remove//excel/"
          description: "MS Excel 和 Open Office 电子表格"

        # format loop 4
        - name: "水印 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/remove//powerpoint/"
          description: "MS PowerPoint 和开放办公室演示"

        # format loop 5
        - name: "水印 DOCX"
          format: "DOCX"
          link: "/watermark/python-net/remove//docx/"
          description: "微软 Word 打开 XML 文档"
          
        # format loop 6
        - name: "水印 PPTX"
          format: "PPTX"
          link: "/watermark/python-net/remove//pptx/"
          description: "PowerPoint 打开 XML 演示文稿"
          
        # format loop 7
        - name: "水印 XLSX"
          format: "XLSX"
          link: "/watermark/python-net/remove//xlsx/"
          description: "微软 Excel 打开 XML 电子表格"

        # format loop 8
        - name: "水印 DOC"
          format: "DOC"
          link: "/watermark/python-net/remove//doc/"
          description: "微软 Word 97-2007 文档"

        # format loop 9
        - name: "水印 XLS"
          format: "XLS"
          link: "/watermark/python-net/remove//xls/"
          description: "微软 Excel 工作簿 97-2003"

        # format loop 10
        - name: "水印 PPT"
          format: "PPT"
          link: "/watermark/python-net/remove//ppt/"
          description: "PowerPoint 演示 97-2003"

        # format loop 11
        - name: "水印 RTF"
          format: "RTF"
          link: "/watermark/python-net/remove//rtf/"
          description: "富文本格式"

---