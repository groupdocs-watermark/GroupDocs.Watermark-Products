---
############################# Static ############################
layout: "family"
date:  2024-07-08T15:37:04
draft: false

product: "Watermark"
product_tag: "watermark"

lang: en

############################# Head ############################
head_title: "Document Watermark C# Java Node.js Python | add watermark"
head_description: "Add watermark to PDF, images and documents. Watermarking Solution for Microsoft Office, PDF, OpenDocument, Images and etc."

############################# Header ############################
title: "Documents Watermark Solution"
description:  |
  Add text and image watermarks for your documents and images.

  Search and modify document watermarks in convenient way.

  Get info about watermarks which are presented in your documents.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Choose your platform"
  title: "Platform independence"
  description: "GroupDocs.Watermark library supports the following operating systems and frameworks:"
  details_link_title: "Learn more"

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
                    Atom <br> Visual Studio Code <br> Any other text editor
      
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
  title: "GroupDocs.Watermark features review"
  description: "The library designed to add, search and update various watermark types for popular document formats."

  items:
    # items loop
    - icon: "protect"
      title: "Protect files with watermarks"
      content: "Append text and image watermarks to your business documents."

    # items loop
    - icon: "search"
      title: "Search for existing watermarks"
      content: "Get detailed information about watermarks placed in document previously."

    # items loop
    - icon: "manipulate"
      title: "Manipulate document watermarks"
      content: "Control text, style, image and other watermark features."

    # items loop
    - icon: "additional"
      title: "Various additional features"
      content: "Get document info, update hyper-links or pages background etc."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Protect documents by watermarks"
  description: "GroupDocs.Watermark typical operations code examples."
  items:
    # code sample loop
    - title: "Creating a watermark."
      content: |
       "To append a watermark to a document, provide path to target file. You have many options to choose in order to get a customized watermark on a specific page."
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Specify the document to be watermarked
            using (Watermarker watermarker = new Watermarker("source.docx"))
            {
                // Create watermark object
                TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                // Set watermark options
                watermark.ForegroundColor = Color.Red;
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;

                // Add watermark and save processed file
                watermarker.Add(watermark);
                watermarker.Save("result.docx");

            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Specify the document to be watermarked
            Watermarker watermarker = new Watermarker("source.docx");

            // Create watermark object
            TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

            // Set watermark options
            watermark.setForegroundColor(Color.getRed());
            watermark.setHorizontalAlignment(HorizontalAlignment.Center);
            watermark.setVerticalAlignment(VerticalAlignment.Center);

            // Add watermark and save processed file
            watermarker.add(watermark);
            watermarker.save("result.docx");
            watermarker.close();
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            // Specify the document to be watermarked
            const watermarker = new Watermarker("source.docx");

            // Create watermark object
            const watermark = new TextWatermark("top secret", new Font("Arial", 36));

            // Set watermark options
            watermark.setForegroundColor(Color.getRed());
            watermark.setHorizontalAlignment(HorizontalAlignment.Center);
            watermark.setVerticalAlignment(VerticalAlignment.Center);

            // Add watermark and save processed file
            watermarker.add(watermark);
            watermarker.save("result.docx");
            ```
        - language: "Python"
          color: "yellow"
          content: |
            ```python {style=abap}  
            def run():
                # Specify the document to be watermarked
                with groupdocs.watermark.Watermarker("source.docx") as watermarker:
                    font = groupdocs.watermark.watermarks.Font("Arial", 36.0)

                    # Create watermark object
                    watermark = groupdocs.watermark.watermarks.TextWatermark("top secret", font)

                    # Set watermark options
                    watermark.foreground_color = groupdocs.watermark.watermarks.Color.red;
                    watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
                    watermark.vertical_alignment = groupdocs.watermark.common.VerticalAlignment.CENTER

                    # Add watermark and save processed file
                    watermarker.add(watermark)
                    watermarker.save("result.docx")
            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "50+ file formats supported"
  description: "GroupDocs.Watermark provides watermarking for popular document and file formats."

############################# Metrics ###############################
metrics:
  enable: true
  title: "Our library statistical data"
  description: "Dive deep into key metrics, revealing insights into our achievements, impact, and growth."

  items:
    # items loop
    - number: "50+"
      title: "Supported formats"
      content: "The Library is able to process more than 50 of the most popular file formats."

    # items loop
    - number: "500k"
      title: "NuGet downloads"
      content: "GroupDocs.Watermark for .NET is a popular library with over 500,000 downloads on NuGet."

    # items loop
    - number: "15k"
      title: "Maven downloads"
      content: "With over 15K downloads on Maven, GroupDocs.Watermark is a popular choice for Java developers."

    # items loop
    - number: "140+"
      title: "Happy customers"
      content: "Individual developers and top companies worldwide prefer our libraries to build innovative solutions."


############################# Customers ###############################
customers:
  enable: true
  title: "Our happy customers"
  description: "GroupDocs libraries are employed by globally renowned and distinguished brands across the world."

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
  title: "Ready to get started?"
  description: "Try GroupDocs.Watermark features for free on your platform"

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
  title: "Frequently asked questions"
  description: "Check out our Frequently Asked Questions"

  items:
    # items loop
    - question: "Are external libraries required by GroupDocs.Watermark for document manipulation?"
      answer: "GroupDocs.Watermark works independently, no need for third-party software like Adobe Acrobat, Microsoft Office, etc."

    # items loop
    - question: "Can I test GroupDocs.Watermark features before buying?"
      answer: "Yes, GroupDocs.Watermark offers a free trial! Install it and try it out, but keep in mind: Trial versions add 'trial badges' to your documents, only the first 3 pages are processed. Want the full experience? Get a free 30-day temporary license for full functionality. See details under [temporary license](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "What license types are provided?"
      answer: "Need a GroupDocs.Watermark license? We've got options! Choose from licenses based on many options. Number of developers in your team. Deployment locations like single office or remote workplaces. Does end-customer distribution need to share the SDK/API with clients? Alternatively, there's a license for monthly usage: Pay only for what you use with metered plans. Dive deeper and find the perfect [price](https://purchase.groupdocs.com/pricing/watermark/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Watermark low code APIs"
  description: "Add watermarks to files by your application using our cloud-based REST API."
  
  items:
    # items loop
    - title: "GroupDocs.Watermark Cloud for cURL"
      content: "Use cURL RESTful API to watermark PDF, Word, Excel, PowerPoint, JPEG and other popular file formats."
      icon: "groupdocs_watermark-for-curl"
      link: "https://products.groupdocs.cloud/watermark/curl"

    # items loop
    - title: "GroupDocs.Watermark Cloud for .NET"
      content: "Empower your .NET applications with documents watermarking features by Cloud SDK for .NET. Protect business documents on your own."
      icon: "groupdocs_watermark-for-net"
      link: "https://products.groupdocs.cloud/watermark/net"

    # items loop
    - title: "GroupDocs.Watermark Cloud for Java"
      content: "GroupDocs.Watermark SDK designed for Java grants new possibilities for your Java applications and business files."
      icon: "groupdocs_watermark-for-java"
      link: "https://products.groupdocs.cloud/watermark/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Watermark Web apps"
  description: "GroupDocs grants access to web application for adding watermarks to your documents. More than 50 popular file formats could be watermarked in your favorite browser FOR FREE."

  items:
    # items loop
    - title: "GroupDocs.Watermark Total"
      content: "On-line tool to add watermarks to documents from any device."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/watermark/total"

    # items loop
    - title: "GroupDocs.Watermark DOCX"
      content: "Watermark MS Word DOCX on-line."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/watermark/docx"

    # items loop
    - title: "GroupDocs.Watermark PDF"
      content: "Protect PDF documents on-line."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/watermark/pdf"


      


---