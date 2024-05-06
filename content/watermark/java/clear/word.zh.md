
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
head_title: "使用 Java API 移除 Word 个水印"
head_description: "使用 GroupDocs.Watermark for Java API 简化 Word 文档的水印删除、编辑和清晰度。"

############################# Header ############################
title: "Java Word 去除水印" 
description: "掌握使用 GroupDocs.Watermark for Java API 从 Word 个文档中移除水印的方法，确保文档输出完整。"
subtitle: "GroupDocs.Watermark for Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Maven 下载"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java 图书馆"
    link: "/watermark/java/"
    link_title: "了解更多"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       利用 GroupDocs.Watermark for Java 库有效管理和清除 Word 个文档中的水印。这个强大的工具提供了删除、调整和搜索文本和图像水印的功能，便于保护和管理文档的真实性和外观。

############################# Steps ############################
steps:
    enable: true
    title: "使用 Java 清除 Word 文档的水印"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/)** 可以轻松清除之前添加的水印的业务文档。通过安装我们的库来增强您的 Java 应用程序的能力，并通过几个简单的步骤完成：
      
      1. 首先使用 Word 文档实例化名为 **Watermarker** 的主类。我们的 API 支持将要处理的文档作为流或本地路径传递。
      2. 使用 **SearchCriteria** 限制要处理的水印集。可以使用图像作为搜索参数以及文本或格式化特征。然后您提供更具体的搜索参数，然后您获得更精确的结果。
      3. 处理作为搜索结果获得的文档水印列表。清除文档。
      4. 清除文档后将结果保存为本地文件或字节流。
   
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

        // Word 文档中的清除文本水印

        // 使用 Word 文档实例化 Watermarker
        Watermarker watermarker = new Watermarker("input.docx");
        
        // 清除特定水印
        PossibleWatermarkCollection possibleWatermarks = watermarker.search();
        possibleWatermarks.removeAt(0);

        // 保存处理后的文件
        watermarker.save("output.docx");
        
        ```    
        
############################# More features ############################
more_features:
  enable: true
  title: "通过 Java API 高效去除水印"
  description: "探索我们的 Java API 从各种文档类型（包括 PDF 和 Office 文件）中移除或清除水印的强大功能。非常适合希望保持清晰视觉效果和保护文档完整性的开发人员。"
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "清除水印"
  features:
    # feature loop
    - title: "精确移除水印"
      content: "利用我们的 Java API 在不中断原始文档布局的情况下精确定位和删除水印。非常适合清晰度和准确性至关重要的敏感或官方文件。"

    # feature loop
    - title: "批量删除水印"
      content: "通过同时去除多个文件中的水印来提高文档处理效率。我们的 API 支持批量操作，为大规模任务节省时间和资源。"

    # feature loop
    - title: "编辑水印元素"
      content: "我们的高级编辑工具允许您有选择地编辑水印组件，从而灵活地管理文档演示文稿，同时确保内容安全。"
      
  code_samples:
    # code sample loop
    - title: "PDF 明文水印"
      content: |
        此示例说明如何从 PDF 文档中查找和移除所有包含特定格式文本的注释。
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  加载 PDF 个文档
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  获取文档内容
        PdfContent pdfContent = watermarker.getContent(PdfContent.class);

        //  使用特定字体的清除文本水印
        for (PdfPage page : pdfContent.getPages()){
            for (int i = page.getAnnotations().getCount() - 1; i >= 0; i--){
                for (FormattedTextFragment fragment : page.getAnnotations().get_Item(i).getFormattedTextFragments()){
                    if (fragment.getFont().getFamilyName() == "Verdana"){
                        page.getAnnotations().removeAt(i);
                        break;
                    }
                }
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
    title: "使用 Java 处理 Word 个水印"
    exclude: "WORD"
    description: "探索如何高效管理和移除 Word 文件中的水印，使用 GroupDocs.Watermark for Java API 增强文档的安全性和可读性。"
    items: 
        # format loop 1
        - name: "水印 PDF"
          format: "PDF"
          link: "/watermark/java/clear//pdf/"
          description: "Adobe Portable 文档格式"

        # format loop 2
        - name: "水印 Word"
          format: "WORD"
          link: "/watermark/java/clear//word/"
          description: "MS Word 和 Open Office 文档"
          
        # format loop 3
        - name: "水印 Excel"
          format: "EXCEL"
          link: "/watermark/java/clear//excel/"
          description: "MS Excel 和 Open Office 电子表格"

        # format loop 4
        - name: "水印 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/clear//powerpoint/"
          description: "MS PowerPoint 和开放办公室演示"

        # format loop 5
        - name: "水印 DOCX"
          format: "DOCX"
          link: "/watermark/java/clear//docx/"
          description: "微软 Word 打开 XML 文档"
          
        # format loop 6
        - name: "水印 PPTX"
          format: "PPTX"
          link: "/watermark/java/clear//pptx/"
          description: "PowerPoint 打开 XML 演示文稿"
          
        # format loop 7
        - name: "水印 XLSX"
          format: "XLSX"
          link: "/watermark/java/clear//xlsx/"
          description: "微软 Excel 打开 XML 电子表格"

        # format loop 8
        - name: "水印 DOC"
          format: "DOC"
          link: "/watermark/java/clear//doc/"
          description: "微软 Word 97-2007 文档"

        # format loop 9
        - name: "水印 XLS"
          format: "XLS"
          link: "/watermark/java/clear//xls/"
          description: "微软 Excel 工作簿 97-2003"

        # format loop 10
        - name: "水印 PPT"
          format: "PPT"
          link: "/watermark/java/clear//ppt/"
          description: "PowerPoint 演示 97-2003"

        # format loop 11
        - name: "水印 RTF"
          format: "RTF"
          link: "/watermark/java/clear//rtf/"
          description: "富文本格式"

---