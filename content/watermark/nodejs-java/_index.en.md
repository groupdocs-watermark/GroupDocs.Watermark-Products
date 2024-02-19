---
############################# Static ############################
layout: "landing"
date: 2024-02-19T11:27:09
draft: false

lang: en
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
head_title: "Node.js Watermarking Library | add watermarks to files | remove watermark | watermark files"
head_description: "Node.js-based solution allows users to protect business documents by adding text and image watermarks. Many popular formats like PDF, Word, Excel, PowerPoint are supported."

############################# Header ############################
title: "Access to watermarking technology in Node.js via Java solutions"
description: "Protect your intellectual property and prevent unauthorized copying with this Node.js solution. It allows users to easily add watermarks to business documents in various formats, including PDF, Word, Excel, PowerPoint, images etc."
words:
  for: "for"

actions:
  main: "Use NPM to download for free"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "Licensing"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java"
  title: "Ready to get started?"
  description: "Try GroupDocs.Watermark features for free or request a license"

release:
  title: "Version {0} released"
  notes: "See what’s new"
  downloads: "Downloads"
  link: "{products.nodejs-java.release_downloads}"

code:
  title: "Add watermark to MS Word DOCX with TypeScript"
  more: "More examples"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java"
  install: "npm i @groupdocs/groupdocs.comparison"
  content: |
    ```javascript {style=abap}

    // Instantiate Watermarker
    let comparer = new Comparer("source.bmp");

    // Set up watermark options
    comparer.add("target.bmp");

    // Save protected document
    comparer.compare("result.bmp"); 
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Comparison at a glance"
  description: "Node.js TypeScript library for watermarking"
  features:
    # feature loop
    - title: "Detailed output reports"
      content: "GroupDocs.Comparison identifies changes in document content (characters, words, paragraphs, tables, charts), as well as, changes in document style. It provides customers with a resulting report that contains rich information about differences, their number, and type."

    # feature loop
    - title: "Most popular file and document formats are supported"
      content: "With GroupDocs.Comparison API you can efficiently compare documents of any supported formats like PDF, HTML, e-mail, Microsoft Office Word documents, Excel spreadsheets, PowerPoint presentations, OneNote, Visio diagrams, texts, JPEG, PNG, GIF, and BMP images as well as many other formats."

    # feature loop
    - title: "Documentation and examples"
      content: "There is already a lot of documentation on using Comparison library on different platforms with code examples, so you don’t have to think hard about how to work with GroupDocs.Comparison API in your Node.js application."

    # feature loop
    - title: "Comparison summary report"
      content: "Generate a summary report that lists all changes in the compared documents."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform independence"
  description: "GroupDocs.Comparison for Node.js supports the following operating systems, frameworks and package managers"
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
  title: "Supported file formats"
  description: |
    GroupDocs.Comparison for Node.js via Java supports operations with the following [file formats](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office & OpenDocument formats
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTX, RTF, TXT
        * **Excel:** XLS, XLT, XLSX, XLTM, XLSB, XLSM, XLSX
        * **PowerPoint:** POT, POTX, PPS, PPSX, PPTX, PPT        
        * **Outlook:** EML, EMLX, MSG
        * **OneNote:** ONE
        * **OpenDocument:** ODT, ODP, OTP, ODS, OTT
        * **Fixed Page Layout:** PDF        
    # group loop
    - color: "blue"
      content: |
        ### Images, Graphics & Diagrams
        * **Raster images:** BMP, GIF, JPG, JPEG, PNG
        * **Medical Imaging:** DICOM
        * **Microsoft Visio:** VSDX, VSD, VSS, VST, VDX
        * **AutoCAD Drawing:** DWG, DXF
      # group loop
    - color: "red"
      content: |
        ### Other
        * **Text:** TXT
        * **Programming Languages:** CS, Java, CPP, JS, PY, RB, PL, ASM, GROOVY, JSON, PHP, SQL, LOG, DIFF, LESS, SCALA
        * **Web:** HTM, HTML, MHT, MHTML
        * **e-Books:** MOBI, DjVu
        * **Delimiter-Separated Values:** CSV

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Comparison for Node.js features"
  description: "Easily compare PDF and Office documents, images and other formats"

  items:
    # feature loop
    - icon: "compare"
      title: "Easy to use document comparison"
      content: "Analyze and identify differences within two documents."

    # feature loop
    - icon: "note-stack"
      title: "Compare multiple documents"
      content: "Analyze and identify differences within multiple documents simultaneously."

    # feature loop
    - icon: "stacks"
      title: "Supported formats"
      content: "Supports more than 50 popular document formats from various categories."

    # feature loop
    - icon: "rule"
      title: "Accept or reject changes"
      content: "Clear visual representation of identified changes, providing the option to accept or reject modifications."

    # feature loop
    - icon: "preview"
      title: "Generate previews"
      content: "Save the results of the comparison as images."

    # feature loop
    - icon: "two-pager"
      title: "Content comparison"
      content: "Compare text content line-by-line, by paragraphs, by words, by characters. Highlight the changes."

    # feature loop
    - icon: "format_color_text"
      title: "Style comparison"
      content: "Detect changes in formatting and styles."

    # feature loop
    - icon: "folder-managed"
      title: "Set metadata"
      content: "Keep metadata from either the source or target files or allow it to be specified by users."

    # feature loop
    - icon: "lock"
      title: "Password protection"
      content: "Analyze the encrypted documents, or secure the resulting document with a password."

    # feature loop
    - icon: "select"
      title: "Compare specific pages"
      content: "Load just the particular sections or pages of the document."

    # feature loop
    - icon: "speaker-notes"
      title: "Display comments"
      content: "When loading the source document you can choose whether to hide or show comments."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "Some use cases of typical GroupDocs.Comparison for .NET operations"
  items:
    # code sample loop
    - title: "Comparing password-protected documents."
      content: |
        To compare documents that are [protected with a password](https://docs.groupdocs.com/comparison/net/load-password-protected-documents/), you need to specify it then loading the documents:
        {{< landing/code title="How to compare password-protected documents.">}}
        ```csharp {style=abap}
        // Load the source document and specify its password
        using(Comparer comparer = new Comparer("source.docx", new LoadOptions() {Password = "1234"}))  
        {
            // Load the target document and specify its password
            comparer.Add("target.docx", new LoadOptions() {Password = "5678"});

            // Save comparison result to a specified file
            comparer.Compare("result.docx");
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Comparing multiple PDF documents."
      content: |
        GroupDocs.Comparison allows you to [compare more than two documents](https://docs.groupdocs.com/comparison/net/compare-multiple-documents/). The operation is almost the same as when comparing two files. You just need to add more target files to the `comparer` class.
        {{< landing/code title="How to compare three or more documents.">}}
        ```csharp {style=abap}   
        // Load the source document
        using(Comparer comparer = new Comparer("source.docx") 
        {
            // Specify the second file for comparison
            comparer.Add("target2.docx");
            
            // Specify the third file for comparison
            comparer.Add("target3.docx");
            
            // Save comparison result to a specified file
            comparer.Compare("result.docx");
        }
        ```
        {{< /landing/code >}}

---
