
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:27
draft: false
lang: zh
format: Word
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "轻松调整 Word 水印-GroupDocs.Watermark"
head_description: "使用 GroupDocs.Watermark 无缝调整多种文档格式的水印。增强您的文件安全性。"

############################# Header ############################
title: "Adjust Word 水印：毫不费力地确保安全" 
description: "借助我们强大的水印修改功能，轻松保护您的文档。放心地保护您的内容。"
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
       **修改水印**：GroupDocs.Watermark 使用户能够无缝修改各种文档格式的水印。借助精确的控制和多功能选项，您可以放心地自定义文档。

############################# Steps ############################
steps:
    enable: true
    title: "使用 Java 调整 Word 文档中的水印"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** 使 Java 开发人员可以通过执行几个简单的步骤轻松调整应用程序中的文本水印：
      
      1. 将您的 Word 文件加载到我们名为 **Watermarker** 的 API 的主要对象。您可以以流或本地磁盘上的路径形式提供文件以供进一步处理。
      2. 下一步是找到必须调整的水印。 **SearchCriteria** 有助于识别先前添加到文档中的具有正确属性的水印。
      3. 通过 **Search** 过程获取合适水印的列表。调整找到的水印属性，例如大小、页面对齐、文本、颜色、图像内容等。自定义数据的方法有很多。
      4. 完成水印调整过程后，您需要保存更新的文档。使用本地文件路径、文件或字节流来存储结果。
   
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

        // 调整 WORD 文本水印

        // 使用输入 WORD 文档实例化 Watermarker
        Watermarker watermarker = new Watermarker("input.docx");

        // 初始化 TextSearchCriteria 并查找文本水印
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        
        // 调整文本水印属性
        for (PossibleWatermark watermark : watermarks)
        {
            watermark.getFormattedTextFragments().clear();
            watermark.getFormattedTextFragments().
                add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
        }

        // 保存更新后的文档
        watermarker.save("output.docx");
        
        ```            
        
############################# More features ############################
more_features:
  enable: true
  title: "深入研究 WORD 水印调整"
  description: "我们的 API 使 Java 个应用程序能够在常见文档格式中添加、编辑、删除和搜索水印。"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "调整水印"
  features:
    # feature loop
    - title: "毫不费力地为您的文档添加水印"
      content: "GroupDocs.Watermark 简化了 Java 开发者的水印流程。为各种业务文档和文件添加不同的水印。您不仅可以应用水印，还可以更新或删除现有的水印。"

    # feature loop
    - title: "根据您的需求自定义水印"
      content: "我们的 API 提供了广泛的自定义选项。轻松调整大小、旋转、颜色、字体、样式等，以获得完美的水印。"

    # feature loop
    - title: "使用 WORD 原生文档功能"
      content: "根据具体的文档格式，您可以使用本机功能。其中可能包括文档页面背景、注释、标题或其他作为水印容器的对象。"
      
  code_samples:
    # code sample loop
    - title: "PDF 调整文字水印"
      content: |
        此示例说明如何调整特定工件的文本。
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  加载 PDF 个文档
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  获取文档内容
        PdfContent pdfContent = watermarker.getContent(PdfContent.class);

        //  调整特定的水印文本
        for (PdfArtifact artifact : pdfContent.getPages().get_Item(0).getArtifacts())
        {
            if (artifact.getText().contains("Test"))
            {
                artifact.setText("Passed");
            }
        }

        //  保存文档
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
    title: "使用 GroupDocs.Watermark for Java 调整常用格式的水印"
    exclude: "WORD"
    description: "GroupDocs.Watermark 支持无缝修改各种格式的水印。量身定制水印策略以满足您的特定需求。"
    items: 
        # format loop 1
        - name: "水印 PDF"
          format: "PDF"
          link: "/watermark/java/adjust//pdf/"
          description: "Adobe Portable 文档格式"

        # format loop 2
        - name: "水印 Word"
          format: "WORD"
          link: "/watermark/java/adjust//word/"
          description: "MS Word 和 Open Office 文档"
          
        # format loop 3
        - name: "水印 Excel"
          format: "EXCEL"
          link: "/watermark/java/adjust//excel/"
          description: "MS Excel 和 Open Office 电子表格"

        # format loop 4
        - name: "水印 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/adjust//powerpoint/"
          description: "MS PowerPoint 和开放办公室演示"

        # format loop 5
        - name: "水印 DOCX"
          format: "DOCX"
          link: "/watermark/java/adjust//docx/"
          description: "微软 Word 打开 XML 文档"
          
        # format loop 6
        - name: "水印 PPTX"
          format: "PPTX"
          link: "/watermark/java/adjust//pptx/"
          description: "PowerPoint 打开 XML 演示文稿"
          
        # format loop 7
        - name: "水印 XLSX"
          format: "XLSX"
          link: "/watermark/java/adjust//xlsx/"
          description: "微软 Excel 打开 XML 电子表格"

        # format loop 8
        - name: "水印 DOC"
          format: "DOC"
          link: "/watermark/java/adjust//doc/"
          description: "微软 Word 97-2007 文档"

        # format loop 9
        - name: "水印 XLS"
          format: "XLS"
          link: "/watermark/java/adjust//xls/"
          description: "微软 Excel 工作簿 97-2003"

        # format loop 10
        - name: "水印 PPT"
          format: "PPT"
          link: "/watermark/java/adjust//ppt/"
          description: "PowerPoint 演示 97-2003"

        # format loop 11
        - name: "水印 RTF"
          format: "RTF"
          link: "/watermark/java/adjust//rtf/"
          description: "富文本格式"

---