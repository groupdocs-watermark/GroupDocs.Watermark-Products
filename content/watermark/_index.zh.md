---
############################# Static ############################
layout: "family"
date:  2024-06-26T07:20:48
draft: false

product: "Watermark"
product_tag: "watermark"

lang: zh

############################# Head ############################
head_title: "文档水印 C# Java Node.js Python |加水印"
head_description: "为 PDF、图像和文档添加水印。Microsoft Office、PDF、OpenDocument、图像等的水印解决方案"

############################# Header ############################
title: "文档水印解决方案"
description:  |
  为您的文档和图像添加文本和图像水印。

  以方便的方式搜索和修改文档水印。

  获取有关文档中显示的水印的信息。

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "选择您的平台"
  title: "平台独立性"
  description: "GroupDocs.Watermark 库支持以下操作系统和框架："
  details_link_title: "了解更多"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Watermark .NET 
      color: "blue"
      tag: "net"
      link: "/watermark/net/"
      features_link: "https://docs.groupdocs.com/watermark/net/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    .NET Framework 4.5 or higher <br> .NET Core 3.0 or higher <br> .NET 5.0 or higher
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Watermark Java
      color: "red"
      tag: "java"
      link: "/watermark/java/"
      features_link: "https://docs.groupdocs.com/watermark/java/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    Java 8 or higher <br> Kotlin
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Watermark Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/watermark/nodejs-java/"
      features_link: "https://docs.groupdocs.com/watermark/"
      features:
          # features loop
          - rows: "4"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> 任何其他文本编辑器
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Python"
      description: GroupDocs.Watermark Python
      color: "yellow"
      tag: "python-net"
      link: "/watermark/python-net/"
      features_link: "https://docs.groupdocs.com/watermark/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Python 3.9+ and .Net 6+
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "4"
            content: |
                    IDLE <br> PyCharm <br> Visual Studio Code
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Watermark 功能审查"
  description: "该库旨在添加、搜索和更新流行文档格式的各种水印类型。"

  items:
    # items loop
    - icon: "protect"
      title: "使用水印保护文件"
      content: "在您的业务文档中添加文本和图像水印。"

    # items loop
    - icon: "search"
      title: "搜索现有水印"
      content: "获取有关先前在文档中放置的水印的详细信息。"

    # items loop
    - icon: "manipulate"
      title: "操作文档水印"
      content: "控制文本、样式、图像和其他水印功能。"

    # items loop
    - icon: "additional"
      title: "各种附加功能"
      content: "获取文档信息、更新超链接或页面背景等"

############################# Code Samples ###############################
code_samples:
  enable: true
  title: "通过水印保护文档"
  description: "GroupDocs.Watermark 典型的操作代码示例。"

  items:
    # items loop
    - title: "创建水印。"
      content: "要向文档添加水印，请提供目标文件的路径。要在特定页面上获得自定义水印，您可以选择许多选项。"
      samples:
          # samples loop
          - language: "C#"
            color: "blue"
            content: |
                    <code class="language-csharp" data-lang="csharp">
                        // 指定要添加水印的文档

                        using (Watermarker watermarker = new Watermarker("source.docx"))
                        {
                          // 创建水印对象
                          TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                          // 设置水印选项
                          watermark.ForegroundColor = Color.Red;
                          watermark.HorizontalAlignment = HorizontalAlignment.Center;
                          watermark.VerticalAlignment = VerticalAlignment.Center;

                          // 添加水印并保存处理后的文件
                          watermarker.Add(watermark);
                          watermarker.Save("result.docx");
                        }                    
                    </code>

          # samples loop
          - language: "Java"
            color: "red"
            content: |
                    <code class="language-java" data-lang="java">
                        // 指定要添加水印的文档

                        Watermarker watermarker = new Watermarker("source.docx");

                        // 创建水印对象
                        TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // 设置水印选项
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // 添加水印并保存处理后的文件
                        watermarker.add(watermark);
                        watermarker.save("result.docx");
                        watermarker.close();

                    </code>

          # samples loop
          - language: "TypeScript"
            color: "green"
            content: |
                    <code class="language-java" data-lang="javascript">
                        // 指定要添加水印的文档

                        const watermarker = new Watermarker("source.docx");
    
                        // 创建水印对象
                        const watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // 设置水印选项
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // 添加水印并保存处理后的文件
                        watermarker.add(watermark);
                        watermarker.save("result.docx");                        

                    </code>

          # samples loop
          - language: "Python"
            color: "yellow"
            content: |
                    <code class="python-net" data-lang="python">
                        def run():

                            # 指定要添加水印的文档
                            with groupdocs.watermark.Watermarker("source.docx") as watermarker:
                                font = groupdocs.watermark.watermarks.Font("Arial", 36.0)

                                # 创建水印对象
                                watermark = groupdocs.watermark.watermarks.TextWatermark("top secret", font)

                                # 设置水印选项
                                watermark.foreground_color = groupdocs.watermark.watermarks.Color.red;
                                watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
                                watermark.vertical_alignment = groupdocs.watermark.common.VerticalAlignment.CENTER

                                # 添加水印并保存处理后的文件
                                watermarker.add(watermark)
                                watermarker.save("result.docx")

                    </code>

############################# Supported Formats ###############################
formats:
  enable: true
  title: "支持 50 多种文件格式"
  description: "GroupDocs.Watermark 为常用文档和文件格式提供水印。"

############################# Metrics ###############################
metrics:
  enable: true
  title: "我们的图书馆统计数据"
  description: "深入研究关键指标，深入了解我们的成就、影响力和增长。"

  items:
    # items loop
    - number: "50+"
      title: "支持的格式"
      content: "该库能够处理 50 多种最流行的文件格式。"

    # items loop
    - number: "500k"
      title: "NuGet 次下载"
      content: ".NET 的 GroupDocs.Watermark 是一个受欢迎的库，在 NuGet 上的下载量超过50万次。"

    # items loop
    - number: "15k"
      title: "Maven 下载"
      content: "GroupDocs.Watermark 在 Maven 上的下载量超过 1.5 万次，是 Java 个开发者的热门选择。"

    # items loop
    - number: "140+"
      title: "快乐的顾客"
      content: "全球的个人开发人员和顶级公司更喜欢我们的库来构建创新的解决方案。"


############################# Customers ###############################
customers:
  enable: true
  title: "我们满意的客户"
  description: "GroupDocs 个图书馆由全球知名和杰出品牌使用。"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "准备好开始了吗？"
  description: "在您的平台上免费试用 GroupDocs.Watermark 项功能"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/watermark/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/watermark/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/watermark/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "经常问的问题"
  description: "查看我们的常见问题解答"

  items:
    # items loop
    - question: "GroupDocs.Watermark 是否需要外部库来进行文档处理？"
      answer: "GroupDocs.Watermark 可独立运行，无需像 Adobe Acrobat、Microsoft Office 等第三方软件。"

    # items loop
    - question: "我可以在购买前测试 GroupDocs.Watermark 个功能吗？"
      answer: "是的，GroupDocs.Watermark 提供免费试用！安装并试用一下，但请记住：试用版会在您的文档中添加 “试用徽章”，仅处理前 3 页。想要完整的体验吗？获得 30 天免费临时许可证以获得全部功能。请参阅 [临时许可](https://purchase.groupdocs.com/temporary-license/) 下的详细信息。"

    # items loop
    - question: "提供了哪些许可证类型？"
      answer: "需要 GroupDocs.Watermark 许可证？我们有选择！根据许多选项从许可证中进行选择。您团队中的开发者人数。部署地点，例如单一办公室或远程工作场所。终端客户分发是否需要与客户共享 SDK/API？或者，还有按月使用的许可证：仅按使用计量套餐的使用量付费。深入研究，找到完美的 [价格](https://purchase.groupdocs.com/pricing/watermark/net/)。"

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Watermark 低代码 API"
  description: "您的应用程序使用我们基于云的 REST API 为文件添加水印。"
  
  items:
    # items loop
    - title: "GroupDocs.Watermark Cloud for cURL"
      content: "使用 cURL REST 完整 API 为 PDF、Word、Excel、PowerPoint、JPEG 和其他流行的文件格式添加水印。"
      icon: "groupdocs_watermark-for-curl"
      link: "https://products.groupdocs.cloud/watermark/curl"

    # items loop
    - title: "GroupDocs.Watermark Cloud for .NET"
      content: "使用适用于 .NET 的 Cloud SDK 提供的文档水印功能，为您的 .NET 个应用程序提供水印功能。自行保护业务文档。"
      icon: "groupdocs_watermark-for-net"
      link: "https://products.groupdocs.cloud/watermark/net"

    # items loop
    - title: "GroupDocs.Watermark Cloud for Java"
      content: "GroupDocs.Watermark 专为 Java 设计的 SDK 为您的 Java 个应用程序和业务文件提供了新的可能性。"
      icon: "groupdocs_watermark-for-java"
      link: "https://products.groupdocs.cloud/watermark/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Watermark 个 Web 应用程序"
  description: "GroupDocs 授予对 Web 应用程序的访问权限，以便为您的文档添加水印。超过50种流行的文件格式可以在你最喜欢的浏览器中免费添加水印。"

  items:
    # items loop
    - title: "GroupDocs.Watermark Total"
      content: "在线工具，可从任何设备向文档添加水印。"
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/watermark/total"

    # items loop
    - title: "GroupDocs.Watermark DOCX"
      content: "在线水印 MS Word DOCX。"
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/watermark/docx"

    # items loop
    - title: "GroupDocs.Watermark PDF"
      content: "在线保护 PDF 个文档。"
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/watermark/pdf"


      


---