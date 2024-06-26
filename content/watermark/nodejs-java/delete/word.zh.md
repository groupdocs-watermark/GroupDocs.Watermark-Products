
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
head_title: "使用 Node.js via Java API 高效移除 Word 个水印"
head_description: "使用我们的 Node.js via Java API 整合 Word 个文件的水印去除功能，优化您的文档工作流程。"

############################# Header ############################
title: "Node.js via Java 用于移除 Word 水印的 API" 
description: "使用 GroupDocs.Watermark for Node.js via Java API 高效地从 Word 个文档中删除或编辑水印，是确保文档输出干净和专业的理想之选。"
subtitle: "GroupDocs.Watermark for Node.js via Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "在 NPM 免费下载"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java 图书馆"
    link: "/watermark/nodejs-java/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java 库为开发人员提供了强大的工具来处理 Word 文档中的水印。无论您需要清除、编辑还是删除水印，此 API 都有助于轻松操作文档元素，以保持文档的视觉质量和完整性，使其成为法律、学术和公司设置的完美之选。

############################# Steps ############################
steps:
    enable: true
    title: "使用 Node.js via Java 删除 Word 水印"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/nodejs-java/)** 为 Node.js via Java 开发人员提供了全面的 API，用于以编程方式删除嵌入在各种 Word 文档中的特定水印。本指南深入探讨了技术流程：
      
      1. 通过实例化 **Watermarker** 类并提供 Word 文件作为构造函数参数来启动工作流程。该文件可以作为字节流、文件流或本地磁盘位置的路径引用提供。
      2. 要实现精确的水印定位，请利用 **SearchCriteria** 对象的功能。该对象有助于根据先前嵌入文档中的属性构建复杂的过滤器。您可以将图像与文本或格式属性一起用作搜索参数，以实现高度精细的选择过程。
      3. 执行搜索后，您将收到一组已识别的水印。这些水印可以轻松删除。
      4. 成功删除水印后，保留修改后的文档。 API 提供了存储灵活性，允许您利用本地文件路径或流对象来进行最终输出。
   
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

        // 删除 Word 文档中的文本水印

        // 使用 Word 文档实例化 Watermarker
        const watermarker = new groupdocs.watermark.Watermarker("input.docx");
        
        // 明文水印适合搜索条件
        const criteria = new groupdocs.watermark.TextFormattingSearchCriteria();
        criteria.setFontBold(true);
        const watermarks = watermarker.search(criteria);
        watermarks.clear();

        // 保存处理后的文件
        watermarker.save("output.docx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Node.js via Java 用于高效去除水印的 API"
  description: "利用我们的 Node.js via Java API 无缝删除或清除各种文档格式中的水印，包括 PDF 和 Office 文件。该API专为开发人员设计，可轻松与您的 Node.js via Java 个应用程序集成，确保文档干净清晰。"
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "移除水印"
  features:
    # feature loop
    - title: "Node.js via Java 去除水印"
      content: "使用我们的 Node.js via Java API 精确、轻松地删除水印。非常适合需要无标记文档进行演示或进一步处理的应用程序。"

    # feature loop
    - title: "批量去除水印处理"
      content: "使用我们的批量水印去除功能高效处理多个文档。通过在 Node.js via Java 应用程序中同时处理大批文件来节省时间和服务器资源。"

    # feature loop
    - title: "灵活地编辑和删除水印"
      content: "我们的API允许灵活地编辑和删除水印元素，以满足各种业务需求和文档类型。调整文档以保持专业外观，同时确保内容完整性。"
      
  code_samples:
    # code sample loop
    - title: "删除 PDF 个超链接水印"
      content: |
        此示例说明如何从 PDF 中删除所有带有正确超链接的水印
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  在 Watermarker 中加载 PDF
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  使用超链接搜索水印
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria('someurl.com');
            const watermarks = watermarker.search(searchCriteria);
  
            //  删除所选水印
            for (let i = watermarks.getCount() - 1; i >= 0; i--) {
                if (watermarks.get_Item(i) instanceof groupdocsWatermark.HyperlinkPossibleWatermark) {
                    console.log(watermarks.get_Item(i).getText());
                    watermarks.removeAt(i);
                }
            }

            //  在文档中保存更改
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
    title: "使用 Node.js via Java 在 Word 中进行有效的水印管理"
    exclude: "WORD"
    description: "探索 GroupDocs.Watermark for Node.js via Java API 管理和删除 Word 文档中的水印的功能，确保所有重要文件的清晰度和可读性。"
    items: 
        # format loop 1
        - name: "水印 PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/delete//pdf/"
          description: "Adobe Portable 文档格式"

        # format loop 2
        - name: "水印 Word"
          format: "WORD"
          link: "/watermark/nodejs-java/delete//word/"
          description: "MS Word 和 Open Office 文档"
          
        # format loop 3
        - name: "水印 Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/delete//excel/"
          description: "MS Excel 和 Open Office 电子表格"

        # format loop 4
        - name: "水印 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/delete//powerpoint/"
          description: "MS PowerPoint 和开放办公室演示"

        # format loop 5
        - name: "水印 DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/delete//docx/"
          description: "微软 Word 打开 XML 文档"
          
        # format loop 6
        - name: "水印 PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/delete//pptx/"
          description: "PowerPoint 打开 XML 演示文稿"
          
        # format loop 7
        - name: "水印 XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/delete//xlsx/"
          description: "微软 Excel 打开 XML 电子表格"

        # format loop 8
        - name: "水印 DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/delete//doc/"
          description: "微软 Word 97-2007 文档"

        # format loop 9
        - name: "水印 XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/delete//xls/"
          description: "微软 Excel 工作簿 97-2003"

        # format loop 10
        - name: "水印 PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/delete//ppt/"
          description: "PowerPoint 演示 97-2003"

        # format loop 11
        - name: "水印 RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/delete//rtf/"
          description: "富文本格式"

---