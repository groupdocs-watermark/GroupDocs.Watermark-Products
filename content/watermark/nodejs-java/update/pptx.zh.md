
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:27
draft: false
lang: zh
format: Pptx
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "无缝更新 PPTX 个文档中的水印"
head_description: "通过 GroupDocs.Watermark for Node.js via Java 无缝修改 PPTX 演示文稿中的水印。将我们的库整合到您的应用程序中。"

############################# Header ############################
title: "更新 PPTX 演示文稿中的水印" 
description: "使用 GroupDocs.Watermark for Node.js via Java 轻松高效地修改水印。使用精选的水印保护您的业务文档的安全。轻松自定义水印属性，如大小、对齐方式、旋转角度和位置。"
subtitle: "GroupDocs.Watermark for Node.js via Java 图书馆" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "NPM 软件包下载"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java 解决方案"
    link: "/watermark/nodejs-java/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java 支持无缝修改文档中的水印。使用这种多功能工具，开发人员可以轻松修改和更新各种文件格式的水印，包括 PDF、微软 Word、Excel、PowerPoint、Visio、电子邮件和图像格式。GroupDocs.Watermark for Node.js via Java 可用于所有流行的操作系统。

############################# Steps ############################
steps:
    enable: true
    title: "Node.js via Java 中 PPTX 的动态水印编辑"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** 为 Node.js via Java 开发者提供了强大的 API，用于编辑不同 PPTX 文档的水印。以下是简化工作流程的综合指南：
      
      1. **开始流程：** 首先将您的 PPTX 文件作为参数提供给 **Watermarker** 类构造函数。根据您的要求，文件可以作为流或本地磁盘位置获取。
      2. **精确水印：** 使用 **SearchCriteria** 对象来识别需要修改的水印。这种多功能工具可以根据特定属性进行有针对性的水印选择。
      3. **精确细化：** 成功执行搜索后，即可访问相关水印的集合。享受对每个元素的精细控制，能够更新尺寸、页面定位、文本内容、颜色、图像数据等。
      4. **无缝持久性：** 水印更新完成后，安全地存储修改后的文档。该 API 提供灵活的存储选项，允许您保存到本地文件路径或作为流对象。
   
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

        // 更新图片 PPTX 水印

        // 为 PPTX 文件编写 Watermarker
        const watermarker = new groupdocs.watermark.Watermarker("input.pptx");

        // 使用 SearchCriteria 查找特定图像
        const searchCriteria = 
            new groupdocs.watermark.ImageDctHashSearchCriteria("logo.png");
        const watermarks = watermarker.search(searchCriteria);
        
        // 更新图片内容
        for (const watermark of watermarks.getInnerList().toArray())
        {
            watermark.setImageData(imageData);
        }

        // 保存更新的文件
        watermarker.save("output.pptx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "深入了解如何添加水印"
  description: "用于在 .NET 应用程序中呈现、显示、转换文档、幻灯片、图表和许多其他文档类型的 API"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "添加水印"
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
    - title: "更新演示水印内容"
      content: |
        此示例说明如何更新演示文稿水印的文本内容
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  加载 PDF 文档进行处理
            const watermarker = new groupdocsWatermark.Watermarker("source.pptx");

            //  搜索符合您条件的特定水印
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria("denied", false);
            const watermarks = watermarker.search(searchCriteria);
  
            //  编辑水印的设置，例如大小、颜色和位置
            for (const watermark of watermarks.getInnerList().toArray()) {
                watermark.setText("accepted");
            }

            //  将更新后的文档保存到本地系统或直接流式传输
            watermarker.save("result.pptx");
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
    title: "更新支持的文件格式水印"
    exclude: "PPTX"
    description: "使用 GroupDocs.Watermark for Node.js via Java 无缝修改 PDF、Word、Excel 等中的水印。增强您的文档品牌知名度。"
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