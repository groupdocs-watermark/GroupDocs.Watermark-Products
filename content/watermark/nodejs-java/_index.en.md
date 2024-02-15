---
############################# Static ############################
layout: "landing"
date: 2024-02-15T17:06:03
draft: false
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Documents Watermark Solution C# Java & Node.js | add document watermark  | watermark library | Put text & image watermarks on documents"
head_description: "Add watermark to PDF, images and documents. Watermarking Solution for Microsoft Office, PDF, OpenDocument, Images and etc."

############################# Header ############################
title: "{index-content.title_1}<br>via Java API"
description: "{index-content.description}"
words:
  for: "{index-content.words_for}"

actions:
  main: "Free Maven Download"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "{index-content.actions_alt}"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java"
  title: "{index-content.actions_title}"
  description: "{index-content.actions_description}"

release:
  title: "{index-content.release_title}"
  notes: "{index-content.release_notes}"
  downloads: "{index-content.release_downloads}"

code:
  title: "Sign PDF files in Java"
  more: "{index-content.code_more}"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // {index-content.code_comment_1}
    Signature signature = new Signature("sample.pdf");
    
    // {index-content.code_comment_2}
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // {index-content.code_comment_4}
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "{index-content.overview_title}"
  description: "API for performing document signing and related operations in Java applications"
  features:
    # feature loop
    - title: "Improved business documents with digital signatures in Java"
      content: "Swift and customizable signing: GroupDocs.Signature for Java offers a wide range of digital signature options for PDFs, images, and Office documents. You can use text, barcodes, QR-codes, digital certificates, pictures, or hidden metadata. The document processing is fast and efficient."

    # feature loop
    - title: "Manipulating signed documents"
      content: "Advanced document processing involves powerful operations on signed documents using GroupDocs.Signature for Java. You can search for and validate signatures that have been added to business documents using various useful criteria. Additionally, you can access detailed information about the document or obtain preview images of its pages."

    # feature loop
    - title: "Variety of output choices"
      content: "Robust signing options allow you to customize the output for documents signed with GroupDocs.Signature for Java. You can precisely position any signature on any document page and configure its appearance in various ways. The Java API supports saving signed business documents in numerous supported formats and provides options for securing them with passwords."

############################# Platforms ############################
platforms:
  enable: true
  title: "{index-content.platforms_title}"
  description: "GroupDocs.Signature for Java supports the following operating systems, frameworks and package managers"
  items:
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "{index-content.formats_title}"
  description: |
    GroupDocs.Signature for Java supports operations with the following [file formats](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### {index-content.formats_groups.title_1}
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### {index-content.formats_groups.title_2}
        * **{index-content.formats_groups.format_portable}:** PDF
        * **{index-content.formats_groups.format_images}:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **{index-content.formats_groups.format_other_office}:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### {index-content.formats_groups.title_3}
        * **{index-content.formats_groups.format_web}:** HTML, MHTML
        * **{index-content.formats_groups.format_archives}:** ZIP, TAR, 7Z
        * **{index-content.formats_groups.format_certificates}:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature features"
  description: "Signing PDFs, Office Documents, and images with digital signatures"

  items:
    # feature loop
    - icon: "sign"
      title: "Adding Signatures"
      content: "Sign a document using various supported signature types by placing a digital signature precisely at any position on any page."

    # feature loop
    - icon: "custom"
      title: "Customizing results"
      content: "Customize the signature appearance by adjusting color, font, border, rotation, and other features to achieve the desired result."

    # feature loop
    - icon: "password"
      title: "Securing documents with password"
      content: "For many supported document types, you can protect the signed document with a password."

    # feature loop
    - icon: "protect"
      title: "Preventing unauthorized changes"
      content: "Protect important business documents signed with a digital certificate from unauthorized modifications."

    # feature loop
    - icon: "convert"
      title: "Obtaining results in desired formats"
      content: "Easily obtain signed result files in any supported format. You can also convert MS Word documents to PDF effortlessly."

    # feature loop
    - icon: "preview"
      title: "Document preview"
      content: "Save any page of a document as an image for future processing."

    # feature loop
    - icon: "search"
      title: "Searching for signatures"
      content: "It is possible to get information about previously added signatures in specific documents."

    # feature loop
    - icon: "validate"
      title: "Validating documents"
      content: "Validate the correctness of signatures on any signed document."

    # feature loop
    - icon: "update"
      title: "Managing signatures"
      content: "Once a signature is placed on a document page, it can be deleted, moved, or updated as needed."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "Some use cases of typical GroupDocs.Signature for Java operations"
  items:
    # code sample loop
    - title: "Enchance PDF document with QR-code"
      content: |
        Enhancing business processes by adding [QR-codes](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) to specific pages of PDF documents can be valuable. There is an example of how to add a QR code using GroupDocs.Signature for Java.
        {{< landing/code title="Enchance PDF document with QR-code">}}
        ```java {style=abap}
        // Load the source document and specify its password
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Load the target document and specify its password
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Save comparison result to a specified file
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // {index-content.code_samples.sample_1.comment_4}
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Use digital signature to protect a DOCX"
      content: |
        You can [Safeguard a Document](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) using personal or corporate signatures stored as digital certificates. Documents secured with certificate cannot be altered without invalidating the signature.
        {{< landing/code title="Use digital signature to protect a DOCX">}}
        ```java {style=abap}   
        // Load the source document
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Specify the second file for comparison
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Specify the third file for comparison
        options.setPassword("1234567890");

        // Save comparison result to a specified file
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---

