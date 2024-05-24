---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:29
draft: false

lang: zh
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Node.js 水印库 | 文档水印"
head_description: "Node.js 解决方案使用文本和图像水印保护业务文档。支持 PDF、Word、Excel、PowerPoint 等流行格式。"

############################# Header ############################
title: "通过 Java 解决方案访问 Node.js 中的水印技术"
description: "使用此 Node.js 解决方案保护您的知识产权并防止未经授权的复制。它允许用户轻松地为各种格式的业务文档添加水印，包括 PDF、Word、Excel、PowerPoint、图像等。"
words:
  for: "为了"

actions:
  main: "使用 NPM 免费下载"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.watermark"
  alt: "许可"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
  title: "准备好开始了吗？"
  description: "免费试用 GroupDocs.Watermark 项功能或申请许可证"

release:
  title: "版本 {0} 已发布"
  notes: "查看新增内容"
  downloads: "下载"
  link: "https://releases.groupdocs.com/watermark/nodejs-java/"

code:
  title: "使用 TypeScript 向 PDF 添加水印"
  more: "更多例子"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.watermark"
  content: |
    ```javascript {style=abap}

    // 通过 PDF 路径实例化 Watermarker
    let loadOptions = new PdfLoadOptions();
    let watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // 自定义水印选项
    let textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // 向 PDF 文档应用水印
    watermarker.add(textWatermark);

    // 保存结果文档
    watermarker.save("result.pdf");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark 一览"
  description: "Node.js 用于水印的 TypeScript 库"
  features:
    # feature loop
    - title: "Node.js 文件水印"
      content: "使用 GroupDocs.Watermark for Node.js via Java 保护您的业务文档。将文本、图像、图表或电子邮件附件作为水印添加到各种文件格式。"

    # feature loop
    - title: "根据您的需求自定义水印"
      content: "GroupDocs.Watermark for Node.js via Java 为水印提供了大量的自定义选项。微调文本样式（粗体、斜体、字体）和图像属性（旋转等）允许自定义文档处理。"

    # feature loop
    - title: "全面的格式支持"
      content: "GroupDocs.Watermark for Node.js via Java 可与多种文件格式无缝集成，包括：PDF、MS Office 如 Word、Excel、PowerPoint、JPEG、PNG、GIF、GIF、BMP、Visio 图表、电子邮件等。支持文档处理以实现业务目标。"

    # feature loop
    - title: "强大的水印搜索和更新"
      content: "获取和更新带水印的文档中的现有水印。修改文本、样式、图像内容或将其完全删除。GroupDocs.Watermark for Node.js via Java 提供广泛的水印处理。"

############################# Platforms ############################
platforms:
  enable: true
  title: "平台独立性"
  description: "GroupDocs.Watermark for Node.js via Java 可轻松与各种操作系统和包管理器集成。"
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "支持的文件格式"
  description: |
    GroupDocs.Watermark for Node.js via Java 使您能够处理各种文件格式。[浏览完整列表](https://docs.groupdocs.com/watermark/java/supported-document-formats/)。
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office 和 OpenDocument 格式
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### 图像和图形
        * **流行的图像格式:** BMP, JPG, JPEG, PNG
        * **多页图片:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### 其他
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark for Node.js via Java：功能集"
  description: "通过程序化水印增强强大的文档安全性。支持多种文件格式，包括：PDF、DOCX、XLSX、PPTX 和图像格式（PNG、JPG 等）。"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "精确的水印控制"
      content: "通过在特定部分、整个文档或不同文件格式中的单个附件和形状中添加或删除水印来精确处理水印。"

    # feature loop
    - icon: "watermark_style"
      title: "自定义水印外观"
      content: "通过修改文档中的颜色、字体、不透明度、旋转和位置等属性，对水印美观进行精细控制。"

    # feature loop
    - icon: "hidden_print"
      title: "打印 PDF 水印"
      content: "部署隐身水印，该水印在常规文档查看期间保持不可见状态，但仅在打印过程中才会显现出来，从而谨慎地增强文档安全性。"

    # feature loop
    - icon: "image_only"
      title: "特定图像水印"
      content: "使用我们的解决方案，为文档中的特定图像添加水印。选择在指定部分（例如页面、幻灯片）或整个文档中嵌入水印。"

    # feature loop
    - icon: "image_frame"
      title: "多帧图像水印"
      content: "有选择地将水印应用于多帧图像格式中的特定帧，确保对水印位置进行精细控制。"

    # feature loop
    - icon: "attachments"
      title: "全面的内容保护"
      content: "将保护扩展到各种文档元素，例如 Excel 个文档中的附件和演示文稿中的图像形状，从而提供额外的安全层。"

    # feature loop
    - icon: "pdf_objects"
      title: "PDF 中的高级水印"
      content: "在 PDF 的不同区域添加水印，包括出血盒、艺术盒、裁剪盒、修剪框等。"

    # feature loop
    - icon: "doc_background"
      title: "背景图像水印"
      content: "管理电子表格和演示文稿背景图像中的水印，为视觉安全措施提供额外的自定义选项。"

    # feature loop
    - icon: "unreadable_characters"
      title: "带有不可读字符的文本水印"
      content: "在演示文稿中嵌入的文本水印中使用不可读的字符，通过使未经授权的水印提取变得更具挑战性来增强安全性。"

    # feature loop
    - icon: "watermark_text_search"
      title: "高级水印搜索"
      content: "利用全面的搜索功能，根据特定参数或组合各种标准在文档中定位水印，从而实现高效的检索和管理。"

    # feature loop
    - icon: "watermark_image_search"
      title: "相似图像水印检测"
      content: "在视觉上与源图像相似的文档中查找相似的水印图像。"

    # feature loop
    - icon: "document_info"
      title: "编程文档信息提取"
      content: "以编程方式提取有价值的元数据，包括页面设置详细信息以及支持的文件格式的其他文档信息。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "代码示例"
  description: "深入了解展示常见 GroupDocs.Watermark for Node.js via Java 功能的代码示例"
  items:
    # code sample loop
    - title: "用图像给文档加水印"
      content: |
        利用 GroupDocs.Watermark for Node.js via Java 通过添加图像水印来增强文档安全性。了解更多：[图片水印](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/)。
        {{< landing/code title="如何通过图像水印保护文件。">}}
        ```javascript {style=abap}
        // 将源文档加载到 Watermarker
        let watermarker = new Watermarker("document.pdf");
        
        // 指定水印图像的路径
        let watermark = new ImageWatermark("watermark.jpg");

        // 保护文件并将其保存
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "搜索和修改现有水印"
      content: |
        GroupDocs.Watermark for Node.js via Java 允许您管理文档水印。选择水印，修改其属性。了解如何做：[修改水印](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/)。
        {{< landing/code title="水印搜索和修改。">}}
        ```javascript {style=abap}   
        // 加载源文档
        let watermarker = new Watermarker("document.pdf");

        // 搜索要更新的水印
        let searchCriteria = new TextSearchCriteria("test", false);                               
        let watermarks = watermarker.search(searchCriteria); 

        // 更新所需的属性
        watermarks.forEach((watermark)
        {  
            watermark.setText("New Text");
        }

        // 将修改后的文档保存到指定路径
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
