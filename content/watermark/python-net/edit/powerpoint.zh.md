
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:16
draft: false
lang: zh
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "编辑Powerpoint文件中的水印"
head_description: "使用GroupDocs.Watermark for Python via .NET快速更改Powerpoint演示文稿中的水印内容，并确保您的文档安全。"

############################# Header ############################
title: "在Python中精确编辑Powerpoint水印" 
description: "使用GroupDocs.Watermark for Python via .NET完全控制演示文稿中水印的布局和可见性。"
subtitle: "GroupDocs.Watermark for Python via .NET库" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "从PyPi免费下载"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET API"
    link: "/watermark/python-net/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **控制Powerpoint文件中的水印布局：** 使用GroupDocs.Watermark for Python via .NET，您可以将水印放置在确切需要的位置，并轻松保护您的演示文稿。

############################# Steps ############################
steps:
    enable: true
    title: "使用Python修改Powerpoint文档中的水印"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)**帮助Python开发者高效更新各种Powerpoint文件中的水印。以下是如何在您的项目中使用它：
      
      1. 首先，通过将文件传递给**Watermarker**构造函数打开您的Powerpoint文件。您可以使用文件路径、字节流或文件流。
      2. 接下来，使用**SearchCriteria**查找您想要更改的水印，这可以让您搜索水印文本或属性。
      3. 一旦找到，您可以更改文本、字体、大小、位置、颜色等细节，这让您对水印的外观拥有完全的控制。
      4. 修改后，保存文档。您可以将结果写入流或文件路径。
   
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
        # 更新POWERPOINT中的水印文本
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # 使用POWERPOINT文件创建Watermarker
        with gw.Watermarker("input.pptx") as watermarker:

            # 设置TextSearchCriteria以查找水印文本
            search_criteria = gwss.TextSearchCriteria("test", False)

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # 修改水印文本
                        watermark.text = "passed"
                    except Exception as e:
                        pass
            
            watermarker.save("output.pptx")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "发现更新水印的更多方法"
  description: "使用我们的库，Python应用程序可以在多种文件类型中添加、查找、编辑或删除水印。"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "水印编辑"
  features:
    # feature loop
    - title: "便捷地为文件添加水印"
      content: "使用GroupDocs.Watermark for Python via .NET为您的文档添加和管理水印。使用简易的API根据需要搜索、更新或删除水印。"

    # feature loop
    - title: "根据需要自定义水印"
      content: "使用我们的灵活API调整水印设置，如字体、大小、方向和颜色，以获得所需的结果。"

    # feature loop
    - title: "使用特定格式的功能"
      content: "根据文件格式，您可以使用诸如页眉、页脚、注释或背景等本地功能作为水印区域。"
      
  code_samples:
    # code sample loop
    - title: "在Excel中编辑文本水印"
      content: |
        以下代码展示了如何在Excel电子表格中更改水印文本。
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # 打开XLSX文件
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # 读取电子表格数据
        with gw.Watermarker("source.xlsx") as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,3]

            # 更改水印文本
            watermarks = watermarker.search(search_criteria)
            for watermark in watermarks:
                try:
                    watermark.formatted_text_fragments.clear()
                    watermark.formatted_text_fragments.add(
                       "passed", 
                        gww.Font("Calibri", 19.0, gww.FontStyle.bold), 
                        gww.Color.red, 
                        gww.Color.aqua
                    )
                except Exception as e:
                    pass
        
            # 保存结果
            watermarker.save("output.xlsx")
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
    title: "编辑其他文件类型中的水印"
    exclude: "POWERPOINT"
    description: "使用GroupDocs.Watermark for Python via .NET处理不同文档格式中的水印。"
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