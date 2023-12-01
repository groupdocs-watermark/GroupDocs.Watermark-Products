---
############################# Static ############################
layout: "product"
date:  2023-12-01T17:51:42
draft: false

############################# Head ############################
head_title: "{index-content.head_title}"
head_description: "{index-content.head_description}"

############################# Header ############################
title: "{index-content.title}"
description: "{index-content.description}"

############################# APIs ###############################
apis:
  enable: true

  api:
    # api loop
    - title: "{index-content.api_high_title}"
      link: "/watermark/"
      label: "{index-content.api_high_label}"
      api_product:
        # api_product loop
        - link: "/watermark/net/"
          img_alt: "GroupDocs.Watermark for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-watermark-net.png"
          product: "GroupDocs.Watermark for"
          platform: ".NET"
          content: "{index-content.api_high_1_content}"

        # api_product loop
        - link: "/watermark/java/"
          img_alt: "GroupDocs.Watermark for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-watermark-java.png"
          product: "GroupDocs.Watermark for"
          platform: "Java"
          content: "{index-content.api_high_2_content}"

    # api loop
    - title: "{index-content.api_low_title}"
      link: "https://products.groupdocs.cloud/watermark"
      label: "{index-content.api_low_label}"
      api_product:
        # api_product loop
        - link: "https://products.groupdocs.cloud/watermark/net"
          img_alt: "GroupDocs.Watermark Cloud SDK for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_watermark-for-net.png"
          product: "GroupDocs.Watermark"
          platform: "Cloud SDK for .NET"
          content: "{index-content.api_low_1_content}"

        # api_product loop
        - link: "https://products.groupdocs.cloud/watermark/java"
          img_alt: "GroupDocs.Watermark Cloud SDK for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_watermark-for-java.png"
          product: "GroupDocs.Watermark"
          platform: "Cloud SDK for Java"
          content: "{index-content.api_low_2_content}"

    # api loop
    - title: "{index-content.api_nocode_title}"
      link: "https://products.groupdocs.app/watermark"
      label: "{index-content.api_nocodelabel}"
      api_product:
        # api_product loop
        - link: "https://products.groupdocs.app/watermark/total"
          img_alt: "GroupDocs.Watermark Total"
          image: "https://www.aspose.cloud/templates/asposeapp/images/products/logo/aspose_watermark-app.png"
          product: "GroupDocs.Watermark"
          platform: "Total"
          content: "{index-content.api_nocode_1_content}"

        # api_product loop
        - link: "https://products.groupdocs.app/watermark/docx"
          img_alt: "GroupDocs.Watermark DOCX"
          image: "https://www.aspose.cloud/templates/groupdocsapp/images/products/logo/groupdocs_words-app.png"
          product: "GroupDocs.Watermark"
          platform: "DOCX"
          content: "{index-content.api_nocode_2_content}"

        # api_product loop
        - link: "https://products.groupdocs.app/watermark/pdf"
          img_alt: "GroupDocs.Watermark PDF"
          image: "https://www.aspose.cloud/templates/groupdocsapp/images/products/logo/groupdocs_pdf-app.png"
          product: "GroupDocs.Watermark"
          platform: "PDF"
          content: "{index-content.api_nocode_3_content}"

############################# Back to top ###############################
back_to_top:
  enable: true
---