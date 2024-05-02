
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:27:02
draft: false
lang: zh
format: Word
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "从 Word 个文档中提取主水印"
head_description: "成为使用 GroupDocs.Watermark 从文档中提取水印的专家。"

############################# Header ############################
title: "专家 Word 文档水印检索" 
description: "让自己掌握使用 GroupDocs.Watermark for Node.js via Java 检索水印的专业知识。"
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "下载 NPM 软件包"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "关于 GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       使用 GroupDocs.Watermark for Node.js via Java 掌握水印管理的艺术。轻松处理多种文件格式的水印任务，包括 PDF、Word、Excel 等。

############################# Steps ############################
steps:
    enable: true
    title: "通过 GroupDocs.Watermark 高效获取 Word 个文件中的水印"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** 简化了检索嵌入在各种业务文档格式中的水印的过程。将 GroupDocs.Watermark 无缝集成到您的 Node.js via Java 应用程序中，为它们提供强大的水印检测功能。
      
      1. **Watermarker**类并提供 Word 文件路径、文件流或字节流作为输入。此操作加载文档以进行水印分析。
      2. **SearchCriteria** 对象。指定用于定位相似图像水印的图像。或者，对于文本水印，定义文本内容、字体属性、颜色属性和其他相关参数以细化搜索条件。
      3. **Watermarker**对象的**获取**方法在加载的文档中启动水印检测过程。此函数返回代表潜在水印的对象集合，从而可以进行进一步处理。
      4. 检索到的水印对象集合为您提供了很多可能性。您可以删除不需要的水印或修改其属性。更改内容、在页面上移动水印等。
   
    code:
      platform: "net"
      copy_title: "复制"
      install:
        command: "npm i @groupdocs/groupdocs.watermark"
        copy_tip: "点击复制"
        copy_done: "复制的"
      links:
        #  loop
        - title: "更多例子"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
        #  loop
        - title: "文档"
          link: "https://docs.groupdocs.com/watermark/nodejs-java/"
          
      content: |
        ```javascript {style=abap}

        // 获取 WORD 的文字水印列表

        // 实例化 Watermarker 类
        const watermarker = new groupdocs.watermark.Watermarker("input.docx");
        
        // 按文本条件获取水印
        const searchCriteria = new groupdocs.watermark.TextSearchCriteria("test", false);
        const watermarks = watermarker.search(searchCriteria);

        // 使用水印信息
        console.log(`Found ${watermarks.getCount()} possible watermark(s).`);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "在 Node.js 中使用 GroupDocs.Watermark 简化水印搜索"
  description: "学习使用 GroupDocs.Watermark 在 Node.js 应用程序中实现高级水印搜索功能，优化 Node.js via Java 中的文档管理。"
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "在 Node.js 中搜索水印"
  features:
    # feature loop
    - title: "Node.js 中的高级水印检测"
      content: "利用 GroupDocs.Watermark 增强您检测和识别任何文档格式的水印的能力。使用复杂的筛选选项进行高效搜索。"

    # feature loop
    - title: "用于自定义水印搜索的 Node.js API"
      content: "使用我们的 Node.js API 自定义您的搜索操作。通过指定位置、不透明度和内容类型等详细参数来查找水印，优化文档工作流程。"

    # feature loop
    - title: "高效的水印检索和分析"
      content: "使用 GroupDocs.Watermark 快速提取和分析各种文档中的水印。我们的 API 支持快速检索，帮助您保持合规性和品牌一致性。"
      
  code_samples:
    # code sample loop
    - title: "Node.js 示例：高效的水印搜索"
      content: |
        探索如何使用 Node.js 和 GroupDocs.Watermark 搜索不同文档类型的水印，演示如何使用动态搜索条件获得精确结果。
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  初始化 Node.js 环境并加载目标文档
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  使用灵活的条件设置搜索查询以查找特定的水印
            const criteria = new groupdocsWatermark.TextFormattingSearchCriteria();
            criteria.setForegroundColorRange(new groupdocsWatermark.ColorRange());
            criteria.getForegroundColorRange().setMinHue(-5);
            criteria.getForegroundColorRange().setMaxHue(10);
            criteria.setBackgroundColorRange(new groupdocsWatermark.ColorRange());
            criteria.getBackgroundColorRange().setEmpty(true);
            criteria.setFontName("Arial");
            criteria.setMinFontSize(19);
            criteria.setMaxFontSize(42);
            criteria.setFontBold(true);
  
            //  执行搜索并收集符合条件的水印
            const watermarks = watermarker.search(criteria);

            //  处理和分析结果以确定必要的行动
            console.log(`Found ${watermarks.getCount()} possible watermark(s).`);
            watermarker.close();

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "准备好开始了吗？"
  description: "免费试用 GroupDocs.Watermark 项功能或申请许可证"
  items:
    #  loop
    - title: "NPM 下载"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      color: "red"
        #  loop
    - title: "许可"
      link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "高效的文件格式处理"
    exclude: "WORD"
    description: "使用 GroupDocs.Watermark for Node.js via Java 高效处理各种文件格式的水印。"
    items: 
        # format loop 1
        - name: "水印 PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/get//pdf/"
          description: "Adobe Portable 文档格式"

        # format loop 2
        - name: "水印 Word"
          format: "WORD"
          link: "/watermark/nodejs-java/get//word/"
          description: "MS Word 和 Open Office 文档"
          
        # format loop 3
        - name: "水印 Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/get//excel/"
          description: "MS Excel 和 Open Office 电子表格"

        # format loop 4
        - name: "水印 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/get//powerpoint/"
          description: "MS PowerPoint 和开放办公室演示"

        # format loop 5
        - name: "水印 DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/get//docx/"
          description: "微软 Word 打开 XML 文档"
          
        # format loop 6
        - name: "水印 PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/get//pptx/"
          description: "PowerPoint 打开 XML 演示文稿"
          
        # format loop 7
        - name: "水印 XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/get//xlsx/"
          description: "微软 Excel 打开 XML 电子表格"

        # format loop 8
        - name: "水印 DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/get//doc/"
          description: "微软 Word 97-2007 文档"

        # format loop 9
        - name: "水印 XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/get//xls/"
          description: "微软 Excel 工作簿 97-2003"

        # format loop 10
        - name: "水印 PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/get//ppt/"
          description: "PowerPoint 演示 97-2003"

        # format loop 11
        - name: "水印 RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/get//rtf/"
          description: "富文本格式"

---