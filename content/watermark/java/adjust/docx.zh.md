
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:35
draft: false
lang: zh
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "调整 DOCX 个文档中的水印-GroupDocs.Watermark"
head_description: "使用 GroupDocs.Watermark 高效编辑不同文档格式的水印。增强文档的真实性。"

############################# Header ############################
title: "调整 DOCX 水印：无缝自定义" 
description: "使用我们高效的水印编辑工具无缝自定义您的文档。毫不费力地提升您的品牌形象。"
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
    title: "GroupDocs.Watermark for Java API"
    link: "/watermark/java/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **编辑水印**：使用我们强大的编辑工具无缝自定义您的文档。无论是调整位置还是更改内容，都可以轻松实现所需的水印效果。

############################# Steps ############################
steps:
    enable: true
    title: "使用 Java 调整 Docx 文档水印"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** 允许 Java 开发人员使用其应用程序轻松调整许多文档中的水印。这是一个快速指南：
      
      1. 首先，您需要将 Docx 文件作为 **Watermarker** 类构造函数的参数传递。提供字节或文件流或本地磁盘路径。
      2. 其次，找到需要调整的水印。使用 **SearchCriteria** 来识别具有先前添加到文档中的特定属性的水印。
      3. 搜索后，您将收到相关水印的列表。然后，您可以调整它们的属性，包括大小、页面对齐方式、文本、颜色、图像内容等。这为您的数据提供了高度的定制。
      4. 完成水印调整后，保存更新的文档。您可以使用本地文件路径或流来存储结果。
   
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
        // 调整 DOCX图片水印

        // 使用 DOCX 实例化 Watermarker
        Watermarker watermarker = new Watermarker("input.docx");
        
        // 初始化 SearchCriteria 以匹配特定图像
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);

        for (PossibleWatermark watermark : watermarks)
        {
            // 替换找到的图像
            watermark.setImageData(imageData);
        }

        // 保存调整后的文件
        watermarker.save("output.docx");
        
        ```
        
############################# More features ############################
more_features:
  enable: true
  title: "适用于 Java 应用程序的高级 DOCX 水印管理"
  description: "GroupDocs.Watermark API 使开发人员能够将水印功能无缝集成到其 Java 应用程序中。它支持添加、编辑、删除和搜索各种文档格式的水印。"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "水印调整"
  features:
    # feature loop
    - title: "轻松集成水印"
      content: "GroupDocs.Watermark 简化了向 Java 应用程序中的各种业务文档和文件添加不同水印的过程。开发人员不仅可以应用水印，还可以通过编程方式更新或删除现有的水印。"

    # feature loop
    - title: "粒度水印自定义"
      content: "该 API 为水印提供了广泛的自定义选项。开发人员可以轻松调整大小、旋转、颜色、字体、样式和其他属性，以实现所需的视觉效果。"

    # feature loop
    - title: "利用 DOCX 原生文档功能"
      content: "根据目标文档格式，开发人员可以使用本机功能来放置水印。这些功能可能包括文档页面背景、注释、标题或其他作为水印容器的对象。"
      
  code_samples:
    # code sample loop
    - title: "调整电子表格中的图像水印"
      content: |
        此示例说明如何调整 Excel 工作表中特定形状的图像。
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  将文档加载为电子表格
        SpreadsheetLoadOptions loadOptions = new SpreadsheetLoadOptions();
        Watermarker watermarker = new Watermarker("source.xlsx", loadOptions);

        //  获取新的水印字节
        File file = new File("new_watermark.png");
        byte[] imageBytes = new byte[(int) file.length()];
        FileInputStream inputStream = new FileInputStream(file);
        inputStream.read(imageBytes);
        inputStream.close();

        //  调整特定水印的内容
        for (SpreadsheetShape shape : content.getWorksheets().get_Item(0).getShapes())
        {
            if (shape.getImage() != null)
            {
                shape.setImage(new SpreadsheetWatermarkableImage(imageBytes));
            }
        }

        //  保存结果文档
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
    title: "使用 GroupDocs.Watermark for Java 修改多种格式的水印"
    exclude: "DOCX"
    description: "无缝编辑多种文档格式的水印。毫不费力地自定义您的文档，同时确保保护和真实性。"
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