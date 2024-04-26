
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:39:08
draft: false
lang: zh
format: Rtf
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "毫不费力地移除 RTF 中的水印"
head_description: "使用 GroupDocs.Watermark 水印删除功能简化文档编辑。"

############################# Header ############################
title: "轻松删除 RTF 个水印" 
description: "使用 GroupDocs.Watermark 轻松去除文档中不需要的水印。"
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
    title: "GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java 为使用 .NET 环境从文档中删除水印提供了无缝解决方案。开发人员可以毫不费力地集成此功能，从各种文件格式（包括 PDF、Word、Excel 等）中删除不必要或过时的水印。使用 GroupDocs.Watermark 高效删除水印，增强文档管理流程。

############################# Steps ############################
steps:
    enable: true
    title: "通过 Node.js via Java 轻松删除 Rtf 中的水印"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/nodejs-java/)** 简化了从业务文档中删除水印的过程。通过无缝集成我们的库并遵循以下简单步骤，提升您的 Node.js via Java 应用程序级别：
      
      1. **Watermarker**来启动该过程。我们的多功能 API 可以无缝处理文档，无论是以直播形式还是本地路径提供。
      2. **搜索条件**精确定位要解决的水印。利用图像、文本或格式化功能等各种参数来优化搜索。您的标准越详细，结果就越准确。
      3. 对通过搜索检索到的文档水印列表执行删除流程。毫不费力地将它们从文档中删除。
      4. 成功删除水印后，将生成的文档安全地保存为本地文件或字节流，以保持其完整性。
   
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

        // 删除 RTF 文档中的图像水印

        // 获取 Watermarker 传递 RTF 路径作为参数
        const watermarker = new groupdocs.watermark.Watermarker("input.rtf");
        
        // 按搜索条件清除图像水印
        const searchCriteria = 
            new groupdocs.watermark.ImageDctHashSearchCriteria("logo.png");
        const watermarks = watermarker.search(searchCriteria);
        watermarks.clear();

        // 保存已处理的文件
        watermarker.save("output.rtf");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Node.js via Java 去除水印的 API | GroupDocs.Watermark"
  description: "集成我们的 Node.js via Java API，轻松去除文档中的水印，增强文档的清晰度和美观性。该API专为 Node.js via Java 环境量身定制，非常适合需要处理和呈现无水印的干净文档的应用程序。"
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "移除水印"
  features:
    # feature loop
    - title: "简化了 Node.js via Java 的水印去除流程"
      content: "我们的 API 提供专为 Node.js via Java 应用程序设计的简化水印去除工具，使开发人员无需复杂编码即可增强文档的可读性和专业外观。"

    # feature loop
    - title: "Node.js via Java 批量水印清理"
      content: "利用我们的批处理功能，一次性清除多个文档中的水印。这对于需要快速高效地处理大型文档流的应用程序特别有用。"

    # feature loop
    - title: "通过 Node.js via Java 灵活编辑水印"
      content: "使用我们灵活的编辑工具调整、修改或完全删除水印。此功能允许 Node.js via Java 开发人员根据特定的业务需求或客户请求定制文档处理，从而确保最佳结果。"
      
  code_samples:
    # code sample loop
    - title: "删除电子表格标题水印"
      content: |
        此示例说明如何删除放在 XLSX 标题中的水印
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  加载电子表格工作簿
            const loadOptions = new groupdocsWatermark.SpreadsheetLoadOptions();
            const watermarker = new groupdocsWatermark.Watermarker("source.xlsx", loadOptions);

            //  获取标题栏目列表
            const content = watermarker.getContent(groupdocsWatermark.SpreadsheetContent.class);
            const sections = content.getWorksheets().get_Item(0).getHeadersFooters()
                .getByOfficeHeaderFooterType(groupdocsWatermark.OfficeHeaderFooterType.HeaderPrimary).getSections();
  
            //  从标题中删除水印
            for (const section of sections.getInnerList().toArray()) {
                section.setScript(null);
                section.setImage(null);
            }

            //  保存已清除的工作簿
            watermarker.save("result.xlsx");
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
    title: "跨格式删除水印"
    exclude: "RTF"
    description: "使用 GroupDocs.Watermark 去除各种文档类型的水印。"
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