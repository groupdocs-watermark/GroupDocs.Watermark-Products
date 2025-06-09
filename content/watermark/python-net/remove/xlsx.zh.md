
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:30
draft: false
lang: zh
format: Xlsx
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "使用 Python 从 XLSX 文件中移除水印"
head_description: "轻松使用我们的 Python API 清除 XLSX 表格中的水印，确保数据清晰专业。"

############################# Header ############################
title: "使用 Python 管理 XLSX 文件中的水印" 
description: "利用 GroupDocs.Watermark for Python via .NET API 删除或编辑 XLSX 表格中的水印，使您的数据保持最佳状态。"
subtitle: "GroupDocs.Watermark for Python via .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "从 PyPi 免费下载"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET 库"
    link: "/watermark/python-net/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET 库为您提供管理 XLSX 表格中的水印所需的所有工具。删除、编辑或调整水印，保持数据整洁和专业。

############################# Steps ############################
steps:
    enable: true
    title: "在 Python 中轻松移除 Xlsx 文件中的水印"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/python-net/)** 使 Python 开发人员能够快速清除 Xlsx 文件中的水印。以下是操作方法：
      
      1. 首先，将您的 Xlsx 文件传递给 **Watermarker** 构造函数。您可以使用文件路径、字节流或文件流。
      2. 使用 **SearchCriteria** 对象搜索要移除的水印。可以按图像、文本或格式进行筛选以获得精准结果。
      3. 搜索完成后，您将获得水印列表。选择并移除您不需要的水印。
      4. 完成后，将文档保存到文件或流中。
   
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
        # 从 XLSX 文件中删除图像水印
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # 使用您的 XLSX 文件创建一个 Watermarker 实例
        with gw.Watermarker("input.xlsx") as watermarker:

            # 查找并移除检测到的水印
            search_criteria = gwss.ImageDctHashSearchCriteria("logo.png")

            possible_watermarks = watermarker.search(search_criteria)
            del possible_watermarks[i]

            # 保存您的更新文件
            watermarker.save("output.xlsx")
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "使用 Python 的强大水印移除功能 | GroupDocs.Watermark"
  description: "利用我们的 Python API 从 PDF 和办公文件中移除水印。获取整洁专业的文档，适用于任何用途。"
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "擦除水印"
  features:
    # feature loop
    - title: "在 Python 中精确删除水印"
      content: "我们的 Python API 专为精准水印移除而设计，因此您的文件保持其原始外观和格式。非常适合商业、法律或学术文档。"

    # feature loop
    - title: "使用 Python 批量移除水印"
      content: "通过一次性从多个文件中删除水印来加快工作流程。非常适合高效处理大量文档。"

    # feature loop
    - title: "灵活的水印编辑和清除"
      content: "根据需要编辑或移除水印。该 API 为您的文档提供保持完美外观的选项以满足任何需求。"
      
  code_samples:
    # code sample loop
    - title: "从演示文稿中移除背景"
      content: |
        此示例展示了如何删除超链接水印。
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.presentation as gwop

        # 打开演示文稿
        load_options = gwop.PresentationLoadOptions()
        with gw.Watermarker("source.pptx", load_options) as watermarker:

            # 访问幻灯片内容
            search_criteria = gwss.TextSearchCriteria("Lorem ipsum")

            # 移除超链接水印
            watermarks = watermarker.search(search_criteria)

            for i in range(len(watermarks) - 1, -1, -1):
                if isinstance(watermarks[i], gws.HyperlinkPossibleWatermark):
                    del watermarks[i]

            # 保存演示文稿
            watermarker.save("result.pptx");
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
    title: "在 Python 中从 XLSX 表格中移除水印"
    exclude: "XLSX"
    description: "查看GroupDocs.Watermark for Python via .NET API 如何帮助您清除 XLSX 表格中的水印，提升数据体验。"
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