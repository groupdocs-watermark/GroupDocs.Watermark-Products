
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:20
draft: false
lang: zh
format: Word
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "轻松更新 WORD 中的水印"
head_description: "使用 Node.js via Java 使用 GroupDocs.Watermark 简化 WORD 文档格式中的水印更新。为您的业务解决方案提供支持。"

############################# Header ############################
title: "简化 WORD 文档水印更新" 
description: "使用 GroupDocs.Watermark for Node.js via Java 解锁高效的水印更新功能。使用各种水印保护您的业务文档。更新水印属性，如大小、对齐方式、旋转角度和位置以满足您的需求。"
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "在 NPM 免费下载"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java 个技能"
    link: "/watermark/nodejs-java/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java 为使用 Node.js via Java 应用程序管理水印提供了无缝解决方案。这种多功能工具使开发人员能够毫不费力地编辑各种文件格式的文档中的水印，包括 PDF、微软 Word、Excel、PowerPoint、Visio、电子邮件和图像格式。GroupDocs.Watermark 支持所有主要操作系统和 Node.js via Java 版本。

############################# Steps ############################
steps:
    enable: true
    title: "通过 Node.js via Java 更新 WORD 中的水印"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** 为 Node.js via Java 开发人员提供强大的 API，用于以编程方式更新各种 WORD 文档中的水印。本指南概述了该过程：
      
      1. 通过将您的 WORD 文件作为参数提供给 **Watermarker** 类构造函数来开始该过程。根据您的需求，文件可以作为流或对本地磁盘位置的引用提供。
      2. 随后，利用 **SearchCriteria** 对象来识别需要修改的特定水印。该对象可以根据所需的属性精确定位水印。
      3. 成功执行搜索后，您将收到一组相关水印。这些水印提供精细控制，允许您更新尺寸、页面定位、文本内容、配色方案、图像数据等属性。
      4. 水印更新完成后，保留修改后的文档。 API 使用本地文件路径或流对象促进存储。
   
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

        // 更新 WORD 文本水印

        // 为 WORD 文件提供 Watermarker 实例
        const watermarker = new groupdocs.watermark.Watermarker("input.docx");

        // 使用 TextSearchCriteria 查找文本水印
        const searchCriteria = 
            new groupdocs.watermark.TextSearchCriteria("test", false);
        const watermarks = watermarker.search(searchCriteria);
        
        // 更新文字水印
        for (const watermark of watermarks.getInnerList().toArray())
        {
            watermark.setText("passed");
        }

        // 享受结果
        watermarker.save("output.docx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "使用 GroupDocs.Watermark 在 PDF 秒内掌握水印编辑"
  description: "探索用于在 Node.js via Java 个应用程序中调整和管理 PDF 的水印的全面 API 功能。"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "编辑水印"
  features:
    # feature loop
    - title: "在 PDF 秒内轻松编辑水印"
      content: "GroupDocs.Watermark 在 Node.js via Java 中提供了强大的工具，可无缝编辑 PDF 文档中的现有水印。轻松调整位置、透明度等。"

    # feature loop
    - title: "优化水印细节以提高精度"
      content: "控制细节。我们的 API 允许您微调水印的外观，从而可以精确修改 PDF 的大小、不透明度和颜色。"

    # feature loop
    - title: "简化的水印管理"
      content: "我们的 API 简化了水印管理。无论是更新还是删除，您都可以高效地管理水印，保持文档完整性，同时满足您的品牌需求。"
      
  code_samples:
    # code sample loop
    - title: "Java 示例：编辑 PDF 水印"
      content: |
        这个 Java 示例演示了如何编辑 PDF 文档中的现有水印，展示了如何以编程方式调整其属性。
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  加载 PDF 文档进行处理
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  搜索符合您条件的特定水印
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria("test", false);
            const watermarks = watermarker.search(searchCriteria);
  
            //  编辑水印的设置，例如大小、颜色和位置
            for (const watermark of watermarks.getInnerList().toArray()) {
                watermark.getFormattedTextFragments().clear();
                watermark.getFormattedTextFragments().add("passed", 
                    new groupdocsWatermark.Font("Calibri", 19, groupdocsWatermark.FontStyle.Bold), 
                    groupdocsWatermark.Color.getRed(), groupdocsWatermark.Color.getAqua());
            }

            //  将更新后的文档保存到本地系统或直接流式传输
            watermarker.save("result.pdf");
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
    title: "更新其他文件格式的水印"
    exclude: "WORD"
    description: "使用 GroupDocs.Watermark for Node.js via Java 简化 PDF、Word、Excel 等中的水印编辑。支持所有流行的业务格式。"
    items: 
        # format loop 1
        - name: "水印 PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/update//pdf/"
          description: "Adobe Portable 文档格式"

        # format loop 2
        - name: "水印 Word"
          format: "WORD"
          link: "/watermark/nodejs-java/update//word/"
          description: "MS Word 和 Open Office 文档"
          
        # format loop 3
        - name: "水印 Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/update//excel/"
          description: "MS Excel 和 Open Office 电子表格"

        # format loop 4
        - name: "水印 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/update//powerpoint/"
          description: "MS PowerPoint 和开放办公室演示"

        # format loop 5
        - name: "水印 DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/update//docx/"
          description: "微软 Word 打开 XML 文档"
          
        # format loop 6
        - name: "水印 PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/update//pptx/"
          description: "PowerPoint 打开 XML 演示文稿"
          
        # format loop 7
        - name: "水印 XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/update//xlsx/"
          description: "微软 Excel 打开 XML 电子表格"

        # format loop 8
        - name: "水印 DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/update//doc/"
          description: "微软 Word 97-2007 文档"

        # format loop 9
        - name: "水印 XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/update//xls/"
          description: "微软 Excel 工作簿 97-2003"

        # format loop 10
        - name: "水印 PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/update//ppt/"
          description: "PowerPoint 演示 97-2003"

        # format loop 11
        - name: "水印 RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/update//rtf/"
          description: "富文本格式"

---