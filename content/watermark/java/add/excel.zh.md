
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:18
draft: false
lang: zh
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "在 Excel 电子表格中为 Java 生成水印"
head_description: "使用 Java 轻松在 Excel 中生成文本和图像水印，以保护您的 Excel 数据电子表格"

############################# Header ############################
title: "使用 Java 代码自动化 Excel 个水印" 
description: "使用 Java 在 Excel 电子表格中实现自定义文本或图像水印。本指南提供了针对各种专业需求量身定制的增强文档安全性和品牌的分步说明。"
subtitle: "GroupDocs.Watermark for Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费 Maven 下载"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java 图书馆"
    link: "/watermark/java/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java 在 Excel 电子表格中提供全面的水印管理，使开发人员能够轻松生成、调整和清除水印。它支持所有流行的 Excel 文件格式，允许嵌入文本和图像水印，这些水印可以在字体、颜色、大小和位置上进行自定义。GroupDocs.Watermark 还包括水印搜索功能，可确保您的水印完好无损且防篡改。非常适合需要在 Java 环境中增强文档安全性的应用程序。

############################# Steps ############################
steps:
    enable: true
    title: "通过 Java 将水印添加到 Excel 文档"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** 使 Java 开发人员可以轻松地将各种类型的水印添加到流行的商业文件格式中。只需几个简单的步骤即可将我们的库添加到您的应用程序和水印文档中，如下所示。
      
      1. 我们 API 的主类是 **Watermarker**。您需要在文档处理之前实例化它。不要忘记将 Excel 文件作为路径或流对象传递给构造函数。
      2. 下一步是构造所需类型的 **Watermark** 对象。它不仅可以放置在特定文档页面上，还可以放置在附件或标题等本机文档部分中。
      3. 设置水印属性，例如高度和宽度、页面对齐方式（顶部、左侧、中央等）、字体系列和颜色等等。
      4. 调用 **Watermarker** 方法添加新水印。您可以根据需要添加任意数量的水印。建议将处理后的文档保存到其他位置。
   
    code:
      platform: "net"
      copy_title: "复制"
      install:
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-watermark</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "点击复制"
        copy_done: "复制的"
      links:
        #  loop
        - title: "更多例子"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
        #  loop
        - title: "文档"
          link: "https://docs.groupdocs.com/watermark/java/"
          
      content: |
        ```java {style=abap}

        // 添加文本水印到EXCEL

        // 将要加水印的文件传递给 Watermarker
        Watermarker watermarker = new Watermarker("input.xslx");
        
        // 创建文本水印并设置属性
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        watermark.setForegroundColor(Color.getRed());

        // 保存带水印的文件
        watermarker.add(watermark);
        watermarker.save("output.xslx");
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "轻松增强您的水印"
  description: "利用 GroupDocs.Watermark 的强大功能生成、撰写和添加多种文档格式的水印。该API不仅可以增强文档安全性，还可以通过嵌入功能强大且可自定义的水印来保护您的知识产权。"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "添加水印"
  features:
    # feature loop
    - title: "多功能水印选项。"
      content: "使用 GroupDocs.Watermark 探索各种水印选项。从调整不透明度和旋转角度到按比例缩放大小，我们的 API 可让您精确地根据需要自定义水印，确保水印与您的文档无缝融合，同时保持内容的完整性。"

    # feature loop
    - title: "高级水印样式。"
      content: "GroupDocs.Watermark 允许您使用各种字体、颜色和阴影来设置水印样式，使其与众不同且更难移除。使用反映您品牌形象和专业精神的时尚水印增强受保护文档和图像的美学吸引力。"

    # feature loop
    - title: "水印拼贴和定位"
      content: "使用 GroupDocs.Watermark，实现平铺效果以覆盖整个文档，确保全面保护。将水印精确放置在您需要的位置，例如中心、角落或自定义位置。我们灵活的定位选项有助于保护您的文件免遭未经授权的使用和复制。"
      
  code_samples:
    # code sample loop
    - title: "PDF 注释水印"
      content: |
        此示例说明如何向 PDF 文档添加水印注释
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  将文档加载为 PDF
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  基于 PDF 注解创建水印
        PdfAnnotationWatermarkOptions options = new PdfAnnotationWatermarkOptions();
        TextWatermark textWatermark = new TextWatermark("Annotation watermark", new Font("Arial", 8));

        //  设置水印选项
        textWatermark.setHorizontalAlignment(HorizontalAlignment.Left);
        textWatermark.setVerticalAlignment(VerticalAlignment.Top);

        //  在结果文档中添加文本水印
        watermarker.add(textWatermark, options);
        watermarker.save("result.pdf");

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "准备好开始了吗？"
  description: "免费试用 GroupDocs.Watermark 项功能或申请许可证"
  items:
    #  loop
    - title: "Maven 下载"
      link: "https://releases.groupdocs.com/watermark/java/"
      color: "red"
        #  loop
    - title: "许可"
      link: "https://purchase.groupdocs.com/pricing/watermark/java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Java Excel 水印技术"
    exclude: "EXCEL"
    description: "使用 GroupDocs.Watermark for Java，可以轻松地将基于文本或图像的水印应用于 Excel 个电子表格，从而在业务工作流程中显著提高文档安全性和品牌知名度。"
    items: 
        # format loop 1
        - name: "水印 PDF"
          format: "PDF"
          link: "/watermark/java/add//pdf/"
          description: "Adobe Portable 文档格式"

        # format loop 2
        - name: "水印 Word"
          format: "WORD"
          link: "/watermark/java/add//word/"
          description: "MS Word 和 Open Office 文档"
          
        # format loop 3
        - name: "水印 Excel"
          format: "EXCEL"
          link: "/watermark/java/add//excel/"
          description: "MS Excel 和 Open Office 电子表格"

        # format loop 4
        - name: "水印图片"
          format: "IMAGE"
          link: "/watermark/java/add//image/"
          description: "流行的图像格式"

        # format loop 5
        - name: "水印照片"
          format: "PHOTO"
          link: "/watermark/java/add//photo/"
          description: "照片格式"

        # format loop 6
        - name: "水印 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/add//powerpoint/"
          description: "MS PowerPoint 和开放办公室演示"

        # format loop 7
        - name: "水印 DOCX"
          format: "DOCX"
          link: "/watermark/java/add//docx/"
          description: "微软 Word 打开 XML 文档"
          
        # format loop 8
        - name: "水印 PPTX"
          format: "PPTX"
          link: "/watermark/java/add//pptx/"
          description: "PowerPoint 打开 XML 演示文稿"
          
        # format loop 9
        - name: "水印 XLSX"
          format: "XLSX"
          link: "/watermark/java/add//xlsx/"
          description: "微软 Excel 打开 XML 电子表格"

        # format loop 10
        - name: "水印 JPEG"
          format: "JPEG"
          link: "/watermark/java/add//jpeg/"
          description: "JPEG 图片"

        # format loop 11
        - name: "水印 PNG"
          format: "PNG"
          link: "/watermark/java/add//png/"
          description: "Portable 网络图形"

        # format loop 12
        - name: "水印 TIFF"
          format: "TIFF"
          link: "/watermark/java/add//tiff/"
          description: "标记图像文件格式"

        # format loop 13
        - name: "WEBP 水印"
          format: "WEBP"
          link: "/watermark/java/add//webp/"
          description: "网络图片"

        # format loop 14
        - name: "水印 DOC"
          format: "DOC"
          link: "/watermark/java/add//doc/"
          description: "微软 Word 97-2007 文档"

        # format loop 15
        - name: "水印 XLS"
          format: "XLS"
          link: "/watermark/java/add//xls/"
          description: "微软 Excel 工作簿 97-2003"

        # format loop 16
        - name: "水印 PPT"
          format: "PPT"
          link: "/watermark/java/add//ppt/"
          description: "PowerPoint 演示 97-2003"

        # format loop 17
        - name: "水印 RTF"
          format: "RTF"
          link: "/watermark/java/add//rtf/"
          description: "富文本格式"

---