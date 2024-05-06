
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:28
draft: false
lang: zh
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "探索 Excel 电子表格水印搜索"
head_description: "了解 GroupDocs.Watermark for Java 如何让您毫不费力地搜索、查找和管理各种文档格式的水印。"

############################# Header ############################
title: "推出 Excel 电子表格水印搜索功能" 
description: "深入研究 GroupDocs.Watermark for Java 轻松搜索、编辑和操作水印的强大功能。"
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
    title: "基本 GroupDocs.Watermark for Java 信息"
    link: "/watermark/java/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java 是使用 Java 管理 Excel 水印的综合解决方案。使用此工具，开发人员可以轻松执行诸如创建、编辑、搜索和删除常用文件格式文档中的水印等操作。它支持在各种文档中同时使用文本和图像水印，包括 PDF、微软 Word、Excel、PowerPoint、Visio、电子邮件和图像格式。GroupDocs.Watermark for Java 支持所有主要操作系统和 Java 版本。

############################# Steps ############################
steps:
    enable: true
    title: "使用 Java 在 Excel 文件中搜索水印"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/)** 可以轻松搜索已放置在业务文档中的水印。下载我们的软件包并将其引入到您的 Java 应用程序中以利用其优势。
      
      1. 为了使用我们的库功能，您需要将 Excel 文件加载到 **Watermarker** 类实例。可以仅提供文件路径、文件流或字节流。
      2. 要缩小可能水印的列表，请使用 **SearchCriteria** 对象。提供图像作为示例以获得相似的图像水印。如果要搜索文本水印，请提供文本、字体、颜色和其他选项。
      3. 要获取放置在文档中的水印，请使用 **Watermarker** 对象的方法 **Search**。您将获得可作为水印处理的对象集合。
      4. 最后，您可以随意处理搜索结果。删除找到的水印或编辑其属性是完全可能的。例如，更改大小或文本。
   
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

        // 在 EXCEL 文档中搜索文本水印

        // 获取 EXCEL 文档的 Watermarker 实例
        Watermarker watermarker = new Watermarker("input.xslx");

        // 按条件搜索水印
        ImageSearchCriteria imageSearchCriteria = new ImageDctHashSearchCriteria("watermark.jpeg");
        imageSearchCriteria.setMaxDifference(0.9);
        PossibleWatermarkCollection possibleWatermarks = watermarker.search(imageSearchCriteria);

        // 处理水印
        System.out.println("Found " + possibleWatermarks.getCount() + " possible watermark(s).");
        
        ```   
        
############################# More features ############################
more_features:
  enable: true
  title: "利用 Java 利用 GroupDocs.Watermark 进行高级水印搜索"
  description: "利用 GroupDocs.Watermark Java API 在 Java 中对不同格式的文档中的水印进行复杂搜索。"
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "高级水印搜索"
  features:
    # feature loop
    - title: "Java-增强型水印搜索技术"
      content: "使用 GroupDocs.Watermark 为您的 Java 应用程序提供高级搜索技术。我们的API支持对各种文档类型的嵌入式水印进行深度搜索，从而提高了精度和效率。"

    # feature loop
    - title: "使用自定义 Java 查询识别水印"
      content: "自定义您的 Java 个查询以更有效地检测水印。使用 GroupDocs.Watermark 按透明度、嵌入方法以及文本或图像内容等属性对水印进行排序和过滤。"

    # feature loop
    - title: "文件水印的有效管理"
      content: "简化 Java 应用程序中水印的管理。使用 GroupDocs.Watermark 快速查找、审查和分析水印，以确保文档完整性并符合品牌推广指南。"
      
  code_samples:
    # code sample loop
    - title: "Java 代码示例：智能水印搜索"
      content: |
        学习如何使用 Java 和 GroupDocs.Watermark 实现智能水印搜索，演示 API 处理复杂搜索操作和结果管理的能力。
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  设置 Java 环境并加载来自各种来源的文档
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  定义高级搜索参数以查找特定类型的水印
        TextSearchCriteria textSearchCriteria = new TextSearchCriteria("Company Name");

        //  执行搜索并处理找到的水印以进行详细审查
        RotateAngleSearchCriteria rotateAngleSearchCriteria = new RotateAngleSearchCriteria(30, 60);
        SearchCriteria combinedSearchCriteria = imageSearchCriteria.or(textSearchCriteria)
                                                                   .and(rotateAngleSearchCriteria);

        //  根据水印搜索结果保存或更新文档
        PossibleWatermarkCollection possibleWatermarks = watermarker.search(combinedSearchCriteria);
        System.out.println("Found " + possibleWatermarks.getCount() + " possible watermark(s).");
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
    title: "解锁水印搜索的力量"
    exclude: "EXCEL"
    description: "使用 GroupDocs.Watermark for Java 让自己能够查找和管理各种支持的文件格式的水印。"
    items: 
        # format loop 1
        - name: "水印 PDF"
          format: "PDF"
          link: "/watermark/java/search//pdf/"
          description: "Adobe Portable 文档格式"

        # format loop 2
        - name: "水印 Word"
          format: "WORD"
          link: "/watermark/java/search//word/"
          description: "MS Word 和 Open Office 文档"
          
        # format loop 3
        - name: "水印 Excel"
          format: "EXCEL"
          link: "/watermark/java/search//excel/"
          description: "MS Excel 和 Open Office 电子表格"

        # format loop 4
        - name: "水印 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/search//powerpoint/"
          description: "MS PowerPoint 和开放办公室演示"

        # format loop 5
        - name: "水印 DOCX"
          format: "DOCX"
          link: "/watermark/java/search//docx/"
          description: "微软 Word 打开 XML 文档"
          
        # format loop 6
        - name: "水印 PPTX"
          format: "PPTX"
          link: "/watermark/java/search//pptx/"
          description: "PowerPoint 打开 XML 演示文稿"
          
        # format loop 7
        - name: "水印 XLSX"
          format: "XLSX"
          link: "/watermark/java/search//xlsx/"
          description: "微软 Excel 打开 XML 电子表格"

        # format loop 8
        - name: "水印 DOC"
          format: "DOC"
          link: "/watermark/java/search//doc/"
          description: "微软 Word 97-2007 文档"

        # format loop 9
        - name: "水印 XLS"
          format: "XLS"
          link: "/watermark/java/search//xls/"
          description: "微软 Excel 工作簿 97-2003"

        # format loop 10
        - name: "水印 PPT"
          format: "PPT"
          link: "/watermark/java/search//ppt/"
          description: "PowerPoint 演示 97-2003"

        # format loop 11
        - name: "水印 RTF"
          format: "RTF"
          link: "/watermark/java/search//rtf/"
          description: "富文本格式"

---