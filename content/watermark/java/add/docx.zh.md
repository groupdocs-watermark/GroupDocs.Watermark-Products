
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:21
draft: false
lang: zh
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "使用 Java 水印增强 DOCX"
head_description: "通过 Java 向 DOCX 文件添加复杂的水印。毫不费力地保护和设计您的文档。"

############################# Header ############################
title: "使用 Java 个水印保护 DOCX 个文件" 
description: "探索 Java 将安全、可自定义的水印嵌入到 DOCX 文件中的强大功能。非常适合需要保护其知识内容的企业。"
subtitle: "GroupDocs.Watermark for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "在 Maven 免费下载"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java"
    link: "/watermark/java/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java 使 Java 开发人员能够将高级水印技术无缝集成到其 DOCX 文档工作流程中。该API具有插入、修改和删除水印的功能，有助于保护版权和增强文档安全性。它专为 DOCX 格式量身定制，提供基于内容敏感度的水印自动化、大小、透明度和旋转等水印属性的动态调整以及在批处理文档上应用水印等功能。GroupDocs.Watermark 可有效确保合规性并防止未经授权的文件流通，从版本 8 开始与 Java 环境兼容。

############################# Steps ############################
steps:
    enable: true
    title: "高级技术：通过 Java 添加水印到 Docx 文档"
    content: |
      使用 **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** 探索 Docx 文档的高级水印技术
      
      1. 通过初始化 **Watermarker** 类来启动水印过程。这一基础步骤为增强带有水印的 Docx 文档奠定了基础。将 Docx 文件作为路径或流对象提供给构造函数。
      2. 通过制作根据您的规格定制的 **Watermark** 对象，进入下一级别。这些多功能实体不仅可以在指定的文档页面上提供精确的放置，还可以在附件或标题等本机元素内提供精确的放置。
      3. 通过微调尺寸、对齐方式、字体样式和颜色等属性来优化水印过程。这种级别的自定义使您能够创建完美补充文档美观的水印。
      4. 利用 **Watermarker** 方法将新创建的水印应用到您的文档上。享受根据您的要求添加多个水印的灵活性。要保存文档，请考虑将它们保存在安全的位置。
   
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
        // 添加图片水印到 DOCX

        // 将要加水印的文件传递给 Watermarker
        Watermarker watermarker = new Watermarker("input.docx");
        
        // 提供带有水印的图像的路径
        ImageWatermark watermark = new ImageWatermark("watermark.png");

        // 保存结果
        watermarker.add(watermark);
        watermarker.save("output.docx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "掌握文档水印"
  description: "使用我们为 .NET 开发人员量身定制的复杂水印 API 来提升您的文档管理。该工具为应用、自定义和管理各种文档格式的水印提供了全面的解决方案，确保了美观和增强的安全性。"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "高级文档水印"
  features:
    # feature loop
    - title: "灵活的水印旋转"
      content: "使用我们灵活的旋转设置，调整您的水印以适应任何文档方向。无论您的文档是纵向还是横向，都可以轻松调整水印角度，以保持一致的外观，与文档布局相得益彰。"

    # feature loop
    - title: "完美的透明度控制"
      content: "精确控制水印的透明度，允许在不影响文档内容的情况下进行细致而安全的标记。此功能非常适合保持文档的原始美感，同时增加一层安全性。"

    # feature loop
    - title: "用于强调的阴影效果"
      content: "增强水印的可见性，或通过可自定义的阴影效果将其巧妙地集成到文档中。此功能允许使用不同的模糊、散布和颜色的阴影，从而根据需要使水印更加独特或隐蔽。"
      
  code_samples:
    # code sample loop
    - title: "MS Word 锁定水印"
      content: |
        此示例说明如何锁定 DOCX 所有页面中的水印
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  以 MS Word doc 格式加载文档
        WordProcessingLoadOptions loadOptions = new WordProcessingLoadOptions();
        Watermarker watermarker = new Watermarker("source.docx", loadOptions);

        //  创建水印
        TextWatermark watermark = new TextWatermark("Watermark text", new Font("Arial", 19));
        watermark.setForegroundColor(Color.getRed());

        //  调整原生 Word 选项
        WordProcessingWatermarkPagesOptions options = new WordProcessingWatermarkPagesOptions();
        options.setLocked(true);
        options.setLockType(WordProcessingLockType.AllowOnlyFormFields);

        //  为结果文档页面添加水印
        watermarker.add(textWatermark, options);
        watermarker.save("result.docx");
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
    title: "DOCX 的基于 Java 的水印"
    exclude: "DOCX"
    description: "利用 Java 在 DOCX 文件中实现动态和安全的水印，确保全面的版权保护。"
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