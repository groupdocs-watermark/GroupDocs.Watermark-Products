
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:20
draft: false
lang: zh
format: Image
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "用于图像保护的动态水印"
head_description: "使用 Node.js 动态水印保护您的图像版权。支持 JPG、PNG、WEBP 等。"

############################# Header ############################
title: "使用 Node.js 为图像保护添加动态水印" 
description: "使用我们的 Node.js 工具包为您的图像生成动态、安全的水印，支持 JPG、PNG 和 WEBP 等格式。使用高级保护功能确保您的图像版权。"
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
       使用 GroupDocs.Watermark for Node.js via Java，对图像应用水印既简单又可自定义。该工具包支持多种图像格式，包括 JPG 和 PNG 等传统光栅图像，以及 WEBP 等新格式。它允许开发人员动态添加水印，这些水印不仅安全，而且可以自然地与图像内容融为一体，从而在不影响图像原始吸引力的前提下提供强大的版权侵权保护。

############################# Steps ############################
steps:
    enable: true
    title: "保护商业文档：为 Image 格式生成水印"
    content: |
      使用 **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/) 提高文档安全性：** 将我们的 API 注入您的应用程序并为许多支持的文件格式生成水印。
      
      1. **启动水印：** 使用提供主要功能的 **Watermarker** 类开始文档处理。通过将 Image 文件传递​​给构造函数来实例化它，该文件应该由生成的水印保护。
      2. **创建主要水印对象：** 通过雕刻定制的 **Watermark** 对象来提升您的文档。除了单纯的页面之外，它们还无缝集成到附件或标题等本机元素中，从而增加了安全性和专业性。
      3. **优化水印属性：** 精确调整水印，调整尺寸、对齐方式和配色方案。每个细节都增强了文档的完整性，使您的文件毫无疑问是您的。
      4. **精确实施：** 利用 **Watermarker** 方法完美地应用您的自定义水印。无论是单个还是多个，每个水印都会增加一层额外的保护。为了提高安全性，请考虑将已处理的文档存储在单独的安全位置。
   
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

        // 为 IMAGE 生成文本水印

        // 将源文件传递给 Watermarker 实例
        const watermarker = new groupdocs.watermark.Watermarker("input.jpeg");
        
        // 生成文本水印并设置其选项
        const  watermark = new groupdocs.watermark.TextWatermark
            ("My Watermark", groupdocs.watermark.new Font("Arial", 36));

        // 获取 IMAGE 结果
        watermarker.add(watermark);
        watermarker.save("output.jpeg");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "高级水印技术"
  description: "使用我们强大的 API 探索尖端的水印技术，该技术旨在无缝集成到 .NET 环境中。非常适合为各种文档类型（包括演示文稿、法律文档和技术图表）添加复杂而安全的水印。"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "精致的水印"
  features:
    # feature loop
    - title: "动态水印放置"
      content: "我们的 API 提供动态放置选项，可根据文档内容调整水印定位。此功能非常适合演示和技术图表中的复杂布局，可确保水印始终处于最佳位置，而不会干扰基础信息的可读性。"

    # feature loop
    - title: "使用隐形水印增强安全性"
      content: "使用隐形水印，在不改变文档外观的情况下提供强有力的保护。这些水印设计为只能通过特定的软件工具进行检测，因此非常适合保护法律和财务文件中的敏感信息。"

    # feature loop
    - title: "自动水印工作流程"
      content: "使用自动水印工作流程简化您的文档安全流程。根据文档类型、内容敏感度和用户访问级别配置规则，以自动应用水印，确保在所有文档中保持一致的安全协议。"
      
  code_samples:
    # code sample loop
    - title: "为 PDF 个附件生成水印"
      content: |
        此示例说明如何在所有 PDF 个附件中生成水印
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  加载 PDF 个文档
            const loadOptions = new groupdocsWatermark.PdfLoadOptions();
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf", loadOptions);
            const pdfContent = watermarker.getContent(groupdocsWatermark.PdfContent.class);

            //  生成文字水印
            const watermark = new groupdocsWatermark.TextWatermark('WaterMark', new groupdocsWatermark.Font('Arial', 19));
  
            //  为合适的附件添加水印
            for (const attachment of pdfContent.getAttachments().getInnerList().toArray()) {
                const info = attachment.getDocumentInfo();
                if (info.getFileType() !== groupdocsWatermark.FileType.Unknown && !info.isEncrypted()) {
                    const attachedWatermarker = attachment.createWatermarker();
                    attachedWatermarker.add(watermark);
                    attachment.updateContent(attachedWatermarker);
                    attachedWatermarker.close();
                }
            }

            //  保存已处理 PDF
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
    title: "通过 JavaScript 在图像中实现惊人的水印"
    exclude: "IMAGE"
    description: "使用我们的 Node.js API 有效保护您的图片版权。为 JPG、PNG 和 WEBP 文件动态添加水印，确保每张图像均为其合法所有者标记。"
    items: 
        # format loop 1
        - name: "水印 PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/generate//pdf/"
          description: "Adobe Portable 文档格式"

        # format loop 2
        - name: "水印 Word"
          format: "WORD"
          link: "/watermark/nodejs-java/generate//word/"
          description: "MS Word 和 Open Office 文档"
          
        # format loop 3
        - name: "水印 Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/generate//excel/"
          description: "MS Excel 和 Open Office 电子表格"

        # format loop 4
        - name: "水印图片"
          format: "IMAGE"
          link: "/watermark/nodejs-java/generate//image/"
          description: "流行的图像格式"

        # format loop 5
        - name: "水印照片"
          format: "PHOTO"
          link: "/watermark/nodejs-java/generate//photo/"
          description: "照片格式"

        # format loop 6
        - name: "水印 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/generate//powerpoint/"
          description: "MS PowerPoint 和开放办公室演示"

        # format loop 7
        - name: "水印 DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/generate//docx/"
          description: "微软 Word 打开 XML 文档"
          
        # format loop 8
        - name: "水印 PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/generate//pptx/"
          description: "PowerPoint 打开 XML 演示文稿"
          
        # format loop 9
        - name: "水印 XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/generate//xlsx/"
          description: "微软 Excel 打开 XML 电子表格"

        # format loop 10
        - name: "水印 JPEG"
          format: "JPEG"
          link: "/watermark/nodejs-java/generate//jpeg/"
          description: "JPEG 图片"

        # format loop 11
        - name: "水印 PNG"
          format: "PNG"
          link: "/watermark/nodejs-java/generate//png/"
          description: "Portable 网络图形"

        # format loop 12
        - name: "水印 TIFF"
          format: "TIFF"
          link: "/watermark/nodejs-java/generate//tiff/"
          description: "标记图像文件格式"

        # format loop 13
        - name: "WEBP 水印"
          format: "WEBP"
          link: "/watermark/nodejs-java/generate//webp/"
          description: "网络图片"

        # format loop 14
        - name: "水印 DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/generate//doc/"
          description: "微软 Word 97-2007 文档"

        # format loop 15
        - name: "水印 XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/generate//xls/"
          description: "微软 Excel 工作簿 97-2003"

        # format loop 16
        - name: "水印 PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/generate//ppt/"
          description: "PowerPoint 演示 97-2003"

        # format loop 17
        - name: "水印 RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/generate//rtf/"
          description: "富文本格式"

---