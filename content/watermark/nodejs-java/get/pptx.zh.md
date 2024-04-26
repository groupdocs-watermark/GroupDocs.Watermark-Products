
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:39:08
draft: false
lang: zh
format: Pptx
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "在 PPTX 演示文稿中探索水印见解"
head_description: "使用 GroupDocs.Watermark for Node.js via Java 发现隐藏在水印中的宝贵见解。"

############################# Header ############################
title: "发现有价值的 PPTX 演示文稿水印见解" 
description: "使用 GroupDocs.Watermark for Node.js via Java 解锁隐藏在水印中的宝贵见解。"
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "NPM 免费套餐"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "获取信息 GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       发挥 GroupDocs.Watermark for Node.js via Java 的潜力，发现隐藏在 Node.js via Java 水印中的宝贵见解。轻松提取和分析各种文件格式的水印。

############################# Steps ############################
steps:
    enable: true
    title: "使用 GroupDocs.Watermark 从 Pptx 个文件中获取水印"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)**为以流行的商业文档格式添加水印提供了全面的解决方案。通过将我们的库集成到您的 Node.js via Java 应用程序中，您可以为它们配备强大的水印搜索功能。
      
      1. **水印**类并提供 Pptx 文件路径。也可以使用另存为字节流的文件。此操作实质上是加载目标文档以进行全面的水印分析。
      2. **SearchCriteria** 对象。您可以指定图像来定位相似的图像水印。或者，对于文本水印，定义文本内容、字体属性、颜色属性和其他相关参数，以完善搜索条件并获得更精确的结果。
      3. **Watermarker**对象的**Get**方法（或类似的命名惯例），在加载的文档中启动水印获取过程。此函数返回代表潜在水印的对象集合，便于根据您的特定要求进行进一步处理。
      4. 水印的结果集合允许您控制文档中标识的水印。您可以删除不需要的水印或动态修改其属性，例如调整其大小、位置或文本内容，以满足您的需求。
   
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

        // 在 PPTX 中放置图像水印

        // 使用源路径创建 Watermarker 对象
        const watermarker = new groupdocs.watermark.Watermarker("input.pptx");
        
        // 通过相似的图像哈希获取水印
        const imageSearchCriteria = 
            new groupdocs.watermark.ImageDctHashSearchCriteria("watermark.jpg");
        imageSearchCriteria.setMaxDifference(0.9);
        const possibleWatermarks = watermarker.search(imageSearchCriteria);

        // 随心所欲处理水印
        console.log(`Found ${possibleWatermarks.getCount()} possible watermark(s).`);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "利用 Node.js 使用 GroupDocs.Watermark 进行水印搜索"
  description: "在 Node.js via Java 平台中使用 GroupDocs.Watermark 在 Node.js 应用程序中实现动态高效的水印搜索功能。"
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "Node.js 水印搜索"
  features:
    # feature loop
    - title: "用于灵活水印搜索的 Node.js API"
      content: "利用 Node.js 的灵活性 GroupDocs.Watermark 搜索多种文档格式的水印。轻松配置搜索以满足特定要求，例如大小、类型或内容。"

    # feature loop
    - title: "使用 Node.js 增强水印识别"
      content: "使用 Node.js 准确识别水印，改善文档处理。利用 GroupDocs.Watermark 的 API 来检测水印，即使在复杂的文档结构中也是如此。"

    # feature loop
    - title: "可扩展的水印搜索解决方案"
      content: "使用 Node.js 扩展您的文档安全解决方案。GroupDocs.Watermark 允许高效处理大型文档批次，使其成为企业级应用程序的理想之选。"
      
  code_samples:
    # code sample loop
    - title: "Node.js 示例：搜索和检索水印"
      content: |
        这个 Node.js 示例展示了如何使用 GroupDocs.Watermark 搜索和检索水印，演示了高效且可扩展的搜索操作。
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            const files = ["source.docx", "source.xlsx", "source.pptx", "source.vsdx"];
            for (const file of files) {
                //  设置 Node.js 环境并加载必要的文档
                const settings = new groupdocsWatermark.WatermarkerSettings();
                settings.setSearchableObjects(new groupdocsWatermark.SearchableObjects());
                settings.getSearchableObjects().setWordProcessingSearchableObjects(
                    groupdocsWatermark.WordProcessingSearchableObjects.Hyperlinks | 
                    groupdocsWatermark.WordProcessingSearchableObjects.Text
                );
                settings.getSearchableObjects().setSpreadsheetSearchableObjects(
                    groupdocsWatermark.SpreadsheetSearchableObjects.HeadersFooters
                );
                settings.getSearchableObjects().setPresentationSearchableObjects(
                    groupdocsWatermark.PresentationSearchableObjects.SlidesBackgrounds |
                    groupdocsWatermark.PresentationSearchableObjects.Shapes
                );
                settings.getSearchableObjects().setDiagramSearchableObjects(groupdocsWatermark.DiagramSearchableObjects.None);
                settings.getSearchableObjects().setPdfSearchableObjects(groupdocsWatermark.PdfSearchableObjects.All);

                //  配置您的搜索以根据不同的标准识别水印
                const watermarker = new groupdocsWatermark.Watermarker(file, settings);

                //  执行水印搜索并收集已识别水印的数据
                const watermarks = watermarker.search();

                //  根据业务需求对结果进行处理以修改或删除水印
                console.log(`In ${documentPath} found ${watermarks.getCount()} possible watermark(s).`);
                watermarker.close();
            }

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
    title: "从水印中提取见解"
    exclude: "PPTX"
    description: "使用 GroupDocs.Watermark for Node.js via Java 从不同文件格式的水印中提取有价值的见解。"
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