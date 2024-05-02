
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:27:09
draft: false
lang: zh
format: Jpg
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "使用 Node.js 向 JPG 添加水印"
head_description: "使用 Node.js 将水印无缝集成到 JPG 张图像中，从而增强版权安全性。"

############################# Header ############################
title: "通过 Node.js 为 JPG 个文件创建水印" 
description: "实现 Node.js 在 JPG 文件中生成自定义水印，保护您的图像免遭滥用和版权侵害。"
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
       GroupDocs.Watermark for Node.js via Java 使 Node.js 开发人员能够高效地在 JPG 张图像上撰写和应用水印。此 API 便于插入根据内容需求量身定制的水印，无论是用于个人用途还是专业展示。开发人员可以自定义水印功能，包括不透明度、大小和位置，以确保它们有效且不显眼。GroupDocs.Watermark 在 Node.js 环境中提供强大的保护功能，确保您的知识产权安全和视觉完好无损，是保护照片内容、数字艺术品和其他媒体资产免受未经授权的复制的理想之选。

############################# Steps ############################
steps:
    enable: true
    title: "保护业务文档：生成 Jpg 个水印"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/) 增强文档安全性：**-适用于 Node.js via Java 的强大水印生成解决方案。
      
      1. **简化您的 Node.js via Java 个应用程序中的安全水印：** **水印** 类作为 GroupDocs.Watermark API 的核心组件。该库简化了各种文档格式的水印生成，包括 Jpg。首先，请在处理您的文档之前创建一个 Watermarker 实例。在初始化期间向构造函数提供 Jpg 文件路径或流对象。
      2. **生成水印以增强保护：** 增强水印，使其完全符合您的安全需求。构造一个指定所需类型的**水印**对象。与传统的页面放置方式不同，您可以在标题或附件等原生文档元素中嵌入水印，从而增强文档安全性并增添专业风格。
      3. **微调水印外观以获得最佳效果：** 控制水印的视觉方面。自定义高度、宽度、对齐方式（上、左、居中等）、字体系列和颜色等属性，以获得视觉效果和一致的结果，增强文档的合法性。
      4. **水印应用程序和安全存储**：使用**水印工具**方法合并您的水印。该库允许您在必要时添加多个水印以增强保护。建议将修改后的 Jpg 文档保存到单独的安全位置，以保留原始文件并保护带水印的文档。
   
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

        // 为 JPG 生成图像水印

        // 实例化 Watermarker 传递源文件
        const watermarker = new groupdocs.watermark.Watermarker("input.jpg");
        
        // 通过提供图像文件生成水印
        const watermark = new groupdocs.watermark.ImageWatermark("watermark.png");

        // 获取 JPG 个结果
        watermarker.add(watermark);
        watermarker.save("output.jpg");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "精细水印集成"
  description: "我们面向 .NET 开发人员的 GroupDocs.Watermark API 为将水印无缝集成到任何文档中提供了完善的解决方案。该工具旨在创建复杂、不显眼的水印，确保版权保护，同时保持文档美感。"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "精确水印集成"
  features:
    # feature loop
    - title: "渐变水印效果"
      content: "实现渐变水印，在文档中顺畅融合。此功能允许采用线性或径向渐变，为安全功能增添现代外观，在不影响内容的情况下增强保护和视觉参与度。"

    # feature loop
    - title: "图案水印可增强安全性"
      content: "使用基于模式的水印来增加额外的安全层。我们的 API 支持各种模式，这些模式可以精心设计并在文档中重复，从而使水印更耐篡改和删除。"

    # feature loop
    - title: "特定文档的水印"
      content: "为不同的文档类型专门定制水印。无论是法律合同、商业计划还是科学报告，都可以根据文档的目的和读者的可访问性自定义水印，从而确保最佳的集成和安全性。"
      
  code_samples:
    # code sample loop
    - title: "生成 PDF 图像水印"
      content: |
        为 PDF 文档中显示的所有图像生成图像水印
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  将文档加载为 PDF
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  基于 PDF 注解创建水印
            const imageWatermark = new groupdocsWatermark.ImageWatermark("watermark.jpg");
            imageWatermark.setHorizontalAlignment(groupdocsWatermark.HorizontalAlignment.Center);
            imageWatermark.setVerticalAlignment(groupdocsWatermark.VerticalAlignment.Center);
            imageWatermark.setRotateAngle(-45);
            imageWatermark.setSizingType(groupdocsWatermark.SizingType.ScaleToParentDimensions);
            imageWatermark.setScaleFactor(1);
  
            //  设置水印选项
            const images = watermarker.getImages();
            for (let i = 0; i < images.getCount(); i++) {
                if (images.get_Item(i).getWidth() > 100 && images.get_Item(i).getHeight() > 100) {
                    images.get_Item(i).add(imageWatermark);
                }
            }

            //  在结果文档中添加文本水印
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
    title: "使用 Node.js 水印保护 JPG 张图片"
    exclude: "JPG"
    description: "利用 Node.js 嵌入水印，保护您的 JPG 张图像，在确保版权保护的同时保持其原始质量。"
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