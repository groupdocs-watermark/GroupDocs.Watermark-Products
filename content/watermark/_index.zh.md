---
############################# Static ############################
layout: "family"
date:  2024-02-16T13:08:05
draft: false

product: "Watermark"
product_tag: "watermark"

lang: zh

############################# Head ############################
head_title: "{index-content.head_title}"
head_description: "{index-content.head_description}"

############################# Header ############################
title: "{index-content.title}"
description:  |
  {index-content.description_1}

  {index-content.description_2}

  {index-content.description_3}

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "{index-content.platforms.head_title}"
  title: "{index-content.platforms.title}"
  description: "{index-content.platforms.description}"
  details_link_title: "{index-content.platforms.learn_more}"

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
                    .NET Framework 4.6.2 or higher <br> .NET Core 2.0 or higher <br> .NET 6.0 or higher
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider
      
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
      features_link: "https://docs.groupdocs.com/watermark/nodejs-java/system-requirements/"
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
                    Atom <br> Visual Studio Code <br> {index-content.platforms.any_other_text_editor}
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

############################# Features ###############################
features:
  enable: true
  title: "{index-content.features.title}"
  description: "{index-content.features.description}"

  items:
    # items loop
    - icon: "protect"
      title: "{index-content.features.feature_1.title}"
      content: "{index-content.features.feature_1.content}"

    # items loop
    - icon: "search"
      title: "{index-content.features.feature_2.title}"
      content: "{index-content.features.feature_2.content}"

    # items loop
    - icon: "manipulate"
      title: "{index-content.features.feature_3.title}"
      content: "{index-content.features.feature_3.content}"

    # items loop
    - icon: "additional"
      title: "{index-content.features.feature_4.title}"
      content: "{index-content.features.feature_4.content}"

############################# Code Samples ###############################
code_samples:
  enable: true
  title: "{index-content.code_samples.index_title}"
  description: "{index-content.code_samples.index_description}"

  items:
    # items loop
    - title: "{index-content.code_samples.sample_index.title}"
      content: "{index-content.code_samples.sample_index.content}"
      samples:
          # samples loop
          - language: "C#"
            color: "blue"
            content: |
                    <code class="language-csharp" data-lang="csharp">
                        // {index-content.code_samples.sample_index.comment_1}

                        using (Watermarker watermarker = new Watermarker("source.docx"))
                        {
                          // {index-content.code_samples.sample_index.comment_2}
                          TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                          // {index-content.code_samples.sample_index.comment_3}
                          watermark.ForegroundColor = Color.Red;
                          watermark.HorizontalAlignment = HorizontalAlignment.Center;
                          watermark.VerticalAlignment = VerticalAlignment.Center;

                          // {index-content.code_samples.sample_index.comment_4}
                          watermarker.Add(watermark);
                          watermarker.Save("result.docx");
                        }                    
                    </code>

          # samples loop
          - language: "Java"
            color: "red"
            content: |
                    <code class="language-java" data-lang="java">
                        // {index-content.code_samples.sample_index.comment_1}

                        Watermarker watermarker = new Watermarker("source.docx");

                        // {index-content.code_samples.sample_index.comment_2}
                        TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // {index-content.code_samples.sample_index.comment_3}
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // {index-content.code_samples.sample_index.comment_4}
                        watermarker.add(watermark);
                        watermarker.save("result.docx");
                        watermarker.close();

                    </code>

          # samples loop
          - language: "TypeScript"
            color: "green"
            content: |
                    <code class="language-java" data-lang="javascript">
                        // {index-content.code_samples.sample_index.comment_1}

                        const watermarker = new Watermarker("source.docx");
    
                        // {index-content.code_samples.sample_index.comment_2}
                        const watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // {index-content.code_samples.sample_index.comment_3}
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // {index-content.code_samples.sample_index.comment_4}
                        watermarker.add(watermark);
                        watermarker.save("result.docx");                        

                    </code>

############################# Supported Formats ###############################
formats:
  enable: true
  title: "{index-content.formats.title}"
  description: "{index-content.formats.description}"

############################# Metrics ###############################
metrics:
  enable: true
  title: "{index-content.metrics.title}"
  description: "{index-content.metrics.description}"

  items:
    # items loop
    - number: "50+"
      title: "{index-content.metrics.item_1.title}"
      content: "{index-content.metrics.item_1.description}"

    # items loop
    - number: "800k"
      title: "{index-content.metrics.item_2.title}"
      content: "{index-content.metrics.item_2.description}"

    # items loop
    - number: "15k"
      title: "{index-content.metrics.item_3.title}"
      content: "{index-content.metrics.item_3.description}"

    # items loop
    - number: "140+"
      title: "{index-content.metrics.item_4.title}"
      content: "{index-content.metrics.item_4.description}"


############################# Customers ###############################
customers:
  enable: true
  title: "{index-content.customers.title}"
  description: "{index-content.customers.description}"

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
  title: "{index-content.actions.title}"
  description: "{index-content.actions.description_index}"

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
  title: "{index-content.faq.title}"
  description: "{index-content.faq.description}"

  items:
    # items loop
    - question: "{index-content.faq.item_1.question}"
      answer: "{index-content.faq.item_1.answer}"

    # items loop
    - question: "{index-content.faq.item_2.question}"
      answer: "{index-content.faq.item_2.answer}"

    # items loop
    - question: "{index-content.faq.item_3.question}"
      answer: "{index-content.faq.item_3.answer}"

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "{index-content.cloud_links.title}"
  description: "{index-content.cloud_links.description}"
  
  items:
    # items loop
    - title: "GroupDocs.Watermark Cloud for cURL"
      content: "{index-content.cloud_links.item_1.content}"
      icon: "groupdocs_watermark-for-curl"
      link: "https://products.groupdocs.cloud/watermark/curl"

    # items loop
    - title: "GroupDocs.Watermark Cloud for .NET"
      content: "{index-content.cloud_links.item_2.content}"
      icon: "groupdocs_watermark-for-net"
      link: "https://products.groupdocs.cloud/watermark/net"

    # items loop
    - title: "GroupDocs.Watermark Cloud for Java"
      content: "{index-content.cloud_links.item_3.content}"
      icon: "groupdocs_watermark-for-java"
      link: "https://products.groupdocs.cloud/watermark/java"

############################# App links ###############################
app_links:
  enable: true
  title: "{index-content.app_links.title}"
  description: "{index-content.app_links.description}"

  items:
    # items loop
    - title: "GroupDocs.Watermark Total"
      content: "{index-content.app_links.item_1.content}"
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/watermark/total"

    # items loop
    - title: "GroupDocs.Watermark DOCX"
      content: "{index-content.app_links.item_2.content}"
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/watermark/docx"

    # items loop
    - title: "GroupDocs.Watermark PDF"
      content: "{index-content.app_links.item_3.content}"
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/watermark/pdf"


      


---