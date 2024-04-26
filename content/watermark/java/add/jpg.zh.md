
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:39:01
draft: false
lang: zh
format: Jpg
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "使用 Java 进行高级 JPG 水印"
head_description: "使用 Java 简化您的 JPG 水印流程，以增强图像保护和版权声明。"

############################# Header ############################
title: "Java-为 JPG 个文件添加水印" 
description: "使用可自定义的水印提升 JPG 文件的安全性。利用 Java 无缝集成水印，确保最佳保护和品牌一致性。"
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
       GroupDocs.Watermark for Java 为 Java 名开发人员配备了专为 JPG 张图像设计的强大水印功能。该API允许添加将文本和图形结合在一起的多层水印，从而在不影响图像质量的情况下确保强大的版权保护。功能包括灵活的缩放、旋转和透明度设置，使水印可以根据用户需求隐蔽或突出。使用 GroupDocs.Watermark 增强数字媒体的完整性和真实性，完全兼容 Java 8 或更高版本。

############################# Steps ############################
steps:
    enable: true
    title: "高级技巧：通过 Java 向 Jpg 文档添加水印"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** 探索 Jpg 文档的高级水印技术
      
      1. **水印器**类来启动水印过程。这一基本步骤为使用水印增强 Jpg 个文档奠定了基础。将 Jpg 文件作为路径或流对象提供给构造函数。
      2. **水印**物体，进入下一个级别。这些多功能实体不仅可以在指定的文档页面上精确定位，还可以在附件或标题等本机元素中精确定位。
      3. 通过微调尺寸、对齐方式、字体样式和颜色等属性来完善水印流程。这种自定义级别使您能够创建水印，完美地补充您的文档美感。
      4. **水印**方法将新创建的水印应用到您的文档上。享受根据您的要求添加多个水印的灵活性。要保存文档，请考虑将其保存在安全的位置。
   
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
        // 向 JPG 添加图像水印

        // 将要添加水印的文件传递给 Watermarker
        Watermarker watermarker = new Watermarker("input.jpg");
        
        // 提供带水印的图像路径
        ImageWatermark watermark = new ImageWatermark("watermark.png");

        // 保存结果
        watermarker.add(watermark);
        watermarker.save("output.jpg");
        
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
    title: "通过 Java 保护 JPG 张图片"
    exclude: "JPG"
    description: "利用 Java 在 JPG 张图像上部署复杂的水印。量身定制水印特征以强化您的版权并增强图像安全性。"
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