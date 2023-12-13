<% configRef "..\\configs\\index\\index_new.yml" %>
---
############################# Static ############################
layout: "family"
date:  <% date "utcnow" %>
draft: false

############################# Head ############################
head_title: "<% "{index-content.head_title}" %>"
head_description: "<% "{index-content.head_description}" %>"

############################# Header ############################
title: "<% "{index-content.title}" %>"
description: | 
            "<% "{index-content.description}" %>"
            "<% "{index-content.description}" %>"
            "<% "{index-content.description}" %>"

############################# Supported Platforms ###############################
supported_platforms:
  head_title: Choose your platform

  items:
    # items loop
    - link: "/watermark/net/"
      color: "blue"
      title: ".NET"
      description: "GroupDocs.Watermark for .NET"

    # items loop
    - link: "/watermark/java/"
      color: "red"
      title: "Java"
      description: "GroupDocs.Watermark for Java"

############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Watermark at a glance"
  description: "API to combine, split, swap, reorder or remove document pages, slides, and diagrams."

  items:
    # items loop
    - icon: "merge"
      title: "Merge multiple file formats"
      content: "Seamlessly combine multiple PDF and Office files into a single document, with support for a wide range of formats"

    # items loop
    - icon: "split"
      title: "Split large documents"
      content: "Split documents based on specific pages, ranges, or even extract individual pages"

    # items loop
    - icon: "structure"
      title: "Customize document structure"
      content: "Take control of your documents by rearranging pages, removing unwanted pages, or adding new ones"

    # items loop
    - icon: "preview"
      title: "Preview document pages"
      content: "Generate image representations of document pages to understand the content and structure better"

############################# Code Samples ###############################
code_samples:
  enable: true
  title: "Practical code showcase"
  description: "Some use cases of typical GroupDocs.Merger operations."

  items:
    # items loop
    - title: "Merging several files"
      content: "GroupDocs.Merger allows you to combine several files together into a single file. You can merge whole documents or particular pages from your documents."
      samples:
          # samples loop
          - language: "C#"
            color: "blue"
            content: |
                    <code class="language-csharp" data-lang="csharp">
                    <span style="display:flex"><span><span style="color:#888;font-style:italic">// Specify desired page numbers or page range to join</span></span></span>
                    <span style="display:flex"><span><span style="color:#000">PageJoinOptions joinOptions</span> = <span style="color:#00f">new</span> <span style="color:#000">PageJoinOptions</span> (<span style="color:#00f">1</span>, <span style="color:#00f">4</span>, <span style="color:#000">RangeMode.OddPages</span>);</span></span>
                    <span style="display:flex"><span></span></span>
                    <span style="display:flex"><span><span style="color:#888;font-style:italic">// Load the source DOCX file</span></span></span>
                    <span style="display:flex"><span><span style="color:#00f">using</span> (<span style="color:#000">Merger</span> <span style="color:#000">merger</span> = <span style="color:#00f">new</span> <span style="color:#000">Merger</span>(<span style="color:#5a2">@"c:\sample.docx"</span>))</span></span>
                    <span style="display:flex"><span>{</span></span>
                    <span style="display:flex"><span><span style="color:#888;font-style:italic">// Add another DOCX file to merge</span></span></span>
                    <span style="display:flex"><span><span style="color:#000">merger</span>.<span style="color:#000">Join</span>(<span style="color:#5a2">@"c:\sample2.docx"</span>, <span style="color:#000">joinOptions</span>);</span></span>
                    <span style="display:flex"><span></span></span>
                    <span style="display:flex"><span><span style="color:#888;font-style:italic">// Merge DOCX files and save result</span></span></span>
                    <span style="display:flex"><span><span style="color:#000">merger</span>.<span style="color:#000">Save</span>(<span style="color:#5a2">@"c:\result.docx"</span>);</span></span>
                    <span style="display:flex"><span>}</span></span>
                    </code>
          # samples loop
          - language: "Java"
            color: "red"
            content: |
                    <code class="language-csharp" data-lang="java">
                    <span style="display:flex"><span><span style="color:#888;font-style:italic">// Specify desired page numbers or page range to join</span></span></span>
                    <span style="display:flex"><span><span style="color:#000">PageJoinOptions joinOptions</span> = <span style="color:#00f">new</span> <span style="color:#000">PageJoinOptions</span> (<span style="color:#00f">1</span>, <span style="color:#00f">4</span>, <span style="color:#000">RangeMode.OddPages</span>);</span></span>
                    <span style="display:flex"><span></span></span>
                    <span style="display:flex"><span><span style="color:#888;font-style:italic">// Load the source DOCX file</span></span></span>
                    <span style="display:flex"><span><span style="color:#000">Merger</span> <span style="color:#000">merger</span> = <span style="color:#00f">new</span> <span style="color:#000">Merger</span>(<span style="color:#5a2">@"c:\sample.docx"</span>);</span></span>
                    <span style="display:flex"><span></span></span>
                    <span style="display:flex"><span><span style="color:#888;font-style:italic">// Add another DOCX file to merge</span></span></span>
                    <span style="display:flex"><span><span style="color:#000">merger</span>.<span style="color:#000">join</span>(<span style="color:#5a2">@"c:\sample2.docx"</span>, <span style="color:#000">joinOptions</span>);</span></span>
                    <span style="display:flex"><span></span></span>
                    <span style="display:flex"><span><span style="color:#888;font-style:italic">// Merge DOCX files and save result</span></span></span>
                    <span style="display:flex"><span><span style="color:#000">merger</span>.<span style="color:#000">save</span>(<span style="color:#5a2">@"c:\result.docx"</span>);</span></span>
                    </code>


############################# Supported Formats ###############################
formats:
  enable: true
  title: "60+ file formats supported"
  description: "GroupDocs.Merger supports operations with a wide range of document formats."


############################# Metrics ###############################
metrics:
  enable: true
  title: "In-depth metrics and statistical insights"
  description: "Dive into a detailed breakdown of our key figures, providing comprehensive metrics and statistical insights into our achievements, impact, and growth."

  items:
    # items loop
    - number: "60+"
      title: "Supported formats"
      content: "Each library supports processing more than 50 of most popular file and document formats."

    # items loop
    - number: "274k"
      title: "NuGet downloads"
      content: "GroupDocs.Merger for .NET has more than 274K downloads from the NuGet package manager."

    # items loop
    - number: "5.5k"
      title: "Maven downloads"
      content: "GroupDocs.Merger for Java has more than 5.5K downloads from our Maven repository."

    # items loop
    - number: "140+"
      title: "Happy customers"
      content: "Our libraries are used by both small individual developers as well as by leading companies all over the world."


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


############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  title: "Platform independence"
  description: "GroupDocs.Merger library supports the following operating systems and frameworks:"
  details_link_title: "Learn more"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      features_link: "https://docs.groupdocs.com/watermark/net/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    .NET Framework 4.6.2 or higher
                    .NET Core 2.0 or higher
                    .NET 6.0 or higher
                    Mono Framework 2.6.7 or higher
      
          # features loop
          - rows: "1"
            content: |
                    Windows, Linux, Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio
                    Xamarin (Android, iOS, Mac)
                    MonoDevelop
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats
      

    # items loop
    - title: "Java"
      color: "red"
      features_link: "https://docs.groupdocs.com/watermark/java/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    J2SE 8.0 or higher
      
          # features loop
          - rows: "1"
            content: |
                    Windows, Linux, Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA
                    Eclipse
                    NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats


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
     

############################# FAQ ###############################
faq:
  enable: true
  title: "Frequently asked questions"
  description: "Answers to most commonly asked questions."

  items:
    # items loop
    - question: "Does the GroupDocs.Merger library need any other third-party software to manipulate documents?"
      answer: "GroupDocs.Merger does not require any external software to be installed such as Adobe Acrobat, Microsoft Office, or any other."

    # items loop
    - question: "Can I try the GroupDocs.Merger library before purchasing it?"
      answer: "Yes, you can try GroupDocs.Merger without buying a license. Once installed without a license, the library works in trial mode. In this mode, trial badges are added to the resultant document, and it is trimmed to the first 3 pages. If you wish to test GroupDocs.Merger without the limitations of the trial version, you can also request a 30-day temporary license. For more details, see "

    # items loop
    - question: "What licenses do you have?"
      answer: "We offer several license types to fit the needs of particular developers or companies. License types depend on the number of developers, the number of developer site locations, and whether you need to deliver our SDK/API to your end customers. Alternatively, you can choose Metered licenses based on monthly usage of the product. Learn more at "


############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Merger low code APIs"
  description: "Accelerate documents merging in any type of application with our cloud-based REST API."

  items:
    # items loop
    - title: "GroupDocs.Merger Cloud for cURL"
      content: "Simple cURL commands for RESTful document merger Cloud API to merge and split documents."
      icon: "groupdocs_merger-for-curl"
      link: "https://products.groupdocs.cloud/merger/curl"

    # items loop
    - title: "GroupDocs.Merger Cloud for .NET"
      content: "Cloud SDK for Microsoft .NET to implement quick merge and split feature in .NET based applications."
      icon: "groupdocs_merger-for-net"
      link: "https://products.groupdocs.cloud/merger/net"

    # items loop
    - title: "GroupDocs.Merger Cloud for Java"
      content: "Combine multiple documents into one, split any document to multiple in your Java applications."
      icon: "groupdocs_merger-for-java"
      link: "https://products.groupdocs.cloud/merger/java"


############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Merger NoCode apps"
  description: "Online application allowing you to merge and split 170+ popular file formats in browser."

  items:
    # items loop
    - title: "GroupDocs.Merger Total"
      content: "Try our free online app to concatenate more than 30 types of files without leaving your favorite web browser."
      icon: "groupdocs_merger-app"
      link: "https://products.groupdocs.app/merger/total"

    # items loop
    - title: "GroupDocs.Merger DOCX"
      content: "Concatenate multiple DOCX files to generate a single document."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/merger/docx"

    # items loop
    - title: "GroupDocs.Merger PDF"
      content: "Merge multiple PDF files to generate a single document directly from the web browser."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/merger/pdf"


      


---