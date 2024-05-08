---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:29
draft: false

lang: vi
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

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
head_title: "Java Thư viện hình mờ | thêm hình mờ vào tài liệu"
head_description: "Phần mềm gốc Java để thêm và thao tác hình mờ văn bản và hình ảnh trong PDF, Word, Excel, Bản trình bày, Visio sơ đồ, email và tệp hình ảnh."

############################# Header ############################
title: "Triển khai hình mờ tài liệu trong Java dự án một cách dễ dàng"
description: "Nâng cao ứng dụng Java của bạn với khả năng tạo hình mờ các tệp bằng thư viện GroupDocs.Watermark. API của chúng tôi cung cấp hình mờ có thể tùy chỉnh cho một loạt các định dạng tệp phổ biến."
words:
  for: "cho"

actions:
  main: "Tải miễn phí từ Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "Cấp phép"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java/"
  title: "Sẵn sàng để bắt đầu?"
  description: "Dùng thử GroupDocs.Watermark tính năng miễn phí hoặc yêu cầu giấy phép"

release:
  title: "Phiên bản {0} đã phát hành"
  notes: "Xem những gì mới"
  downloads: "Tải xuống"

code:
  title: "Hình mờ PDF s qua Java"
  more: "Thêm ví dụ"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-watermark</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Thực hiện Watermarker đi qua đường dẫn PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Tùy chỉnh tùy chọn hình mờ
    TextWatermark textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Áp dụng hình mờ cho tài liệu PDF
    watermarker.add(textWatermark);

    // Lưu tài liệu kết quả
    watermarker.save("result.pdf");
    watermarker.close();
      
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark trong nháy mắt"
  description: "Thư viện được thiết kế để thêm hình mờ bằng công nghệ Java"
  features:
    # feature loop
    - title: "Tệp hình mờ qua Java"
      content: "Bảo vệ tài liệu kinh doanh của bạn bằng cách sử dụng GroupDocs.Watermark for Java. Thêm văn bản, hình ảnh, sơ đồ hoặc tệp đính kèm email dưới dạng hình mờ vào các định dạng tệp khác nhau."

    # feature loop
    - title: "Tùy chỉnh hình mờ cho các nhu cầu cụ thể"
      content: "GroupDocs.Watermark for Java cung cấp các tùy chọn tùy chỉnh mở rộng cho hình mờ. Điều chỉnh kiểu văn bản (in đậm, in nghiêng, phông chữ) và thuộc tính hình ảnh (xoay, v.v.) để điều chỉnh quy trình tạo hình mờ phù hợp với mục tiêu cụ thể của bạn."

    # feature loop
    - title: "Hỗ trợ định dạng rộng"
      content: "GroupDocs.Watermark for Java tích hợp liền mạch với một loạt các định dạng tệp, bao gồm: PDF, Microsoft Office (Word, Excel, PowerPoint), hình ảnh (JPEG, PNG, GIF, BMP), Visio sơ đồ và email. Tăng cường bảo mật tài liệu trên các loại tệp khác nhau."

    # feature loop
    - title: "Tìm kiếm và quản lý hình mờ dễ dàng"
      content: "Quản lý hiệu quả các hình mờ hiện có trong tài liệu. Xác định vị trí hình mờ cụ thể, sửa đổi văn bản, kiểu dáng hoặc hình ảnh của chúng hoặc xóa chúng hoàn toàn. GroupDocs.Watermark for Java đơn giản hóa quy trình làm việc tạo hình mờ."

############################# Platforms ############################
platforms:
  enable: true
  title: "Độc lập nền tảng"
  description: "GroupDocs.Watermark for Java hỗ trợ các hệ điều hành khác nhau và trình quản lý gói."
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
  title: "Định dạng tập tin được hỗ trợ"
  description: |
    GroupDocs.Watermark for Java cho phép xử lý một loạt các định dạng tệp. [Xem danh sách đầy đủ](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office & OpenDocument định dạng
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### Hình ảnh & Đồ họa
        * **Định dạng hình ảnh phổ biến:** BMP, JPG, JPEG, PNG
        * **Hình ảnh nhiều trang:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### Khác
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark for Java: Tính năng"
  description: "Bảo vệ các tệp của bạn bằng cách thêm hình mờ. Hỗ trợ các định dạng khác nhau bao gồm PDF, tài liệu Office và hình ảnh."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Tệp Watermark"
      content: "Thêm hoặc xóa hình mờ khỏi các phần cụ thể hoặc toàn bộ tài liệu cho các định dạng tệp được hỗ trợ khác nhau."

    # feature loop
    - icon: "watermark_style"
      title: "Tùy chỉnh hình mờ"
      content: "Tùy chỉnh giao diện hình mờ của bạn với các tùy chọn như màu sắc, phông chữ, xoay và hơn thế nữa."

    # feature loop
    - icon: "hidden_print"
      title: "Hình mờ in ẩn cho PDF"
      content: "Thêm hình mờ chỉ xuất hiện khi in tài liệu PDF."

    # feature loop
    - icon: "image_only"
      title: "Đánh dấu hình ảnh chọn lọc"
      content: "Đánh mờ tất cả hình ảnh trong một phần, trang, trang chiếu hoặc toàn bộ tài liệu cụ thể."

    # feature loop
    - icon: "image_frame"
      title: "Đánh dấu khung hình ảnh cụ thể"
      content: "Áp dụng hình mờ cho các khung cụ thể trong hình ảnh nhiều khung."

    # feature loop
    - icon: "attachments"
      title: "Tệp đính kèm và hình dạng hình mờ"
      content: "Thêm hình mờ vào tất cả các tệp đính kèm trong Excel tài liệu hoặc tất cả các hình dạng hình ảnh trong Bản trình bày."

    # feature loop
    - icon: "pdf_objects"
      title: "Căn chỉnh hình mờ trong PDF"
      content: "Căn chỉnh hình mờ với các khu vực khác nhau của tài liệu PDF, bao gồm Bleed Box, Art Box, Crop Box và Trim Box."

    # feature loop
    - icon: "doc_background"
      title: "Hình mờ theo hình nền"
      content: "Thêm hoặc xóa hình mờ hình nền vào Bảng tính hoặc Bản trình bày."

    # feature loop
    - icon: "unreadable_characters"
      title: "Bảo vệ với các ký tự không đọc được"
      content: "Bảo vệ bản trình bày bằng hình mờ văn bản với các ký tự không đọc được."

    # feature loop
    - icon: "watermark_text_search"
      title: "Tìm kiếm hình mờ"
      content: "Nhận danh sách hình mờ được trình bày trong tệp, sử dụng các tham số khác nhau bao gồm các biểu thức chính quy."

    # feature loop
    - icon: "watermark_image_search"
      title: "Tìm hình mờ hình ảnh tương tự"
      content: "Xác định vị trí hình mờ hình ảnh trông giống như một hình ảnh cụ thể."

    # feature loop
    - icon: "document_info"
      title: "Trích xuất thông tin tài liệu"
      content: "Nhận dữ liệu tài liệu khác nhau như thiết lập trang cho các định dạng tệp được hỗ trợ."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Mẫu mã"
  description: "Khám phá các ví dụ mã minh họa các chức năng GroupDocs.Watermark for Java điển hình"
  items:
    # code sample loop
    - title: "Đánh dấu tài liệu bằng hình ảnh"
      content: |
        Sử dụng GroupDocs.Watermark for Java để tăng cường bảo mật tài liệu bằng cách thêm hình mờ hình ảnh. Tìm hiểu thêm: [Hình mờ hình ảnh](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Cách bảo vệ tệp bằng hình mờ hình ảnh.">}}
        ```csharp {style=abap}
        // Tải tài liệu nguồn vào Watermarker
        Watermarker watermarker = new Watermarker("document.pdf");
        
        // Chỉ định đường dẫn đến hình ảnh hình mờ
        ImageWatermark watermark = new ImageWatermark("watermark.jpg");

        // Bảo vệ tập tin và lưu nó
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Sửa đổi hình mờ"
      content: |
        GroupDocs.Watermark for Java cho phép bạn quản lý hình mờ hiện có trong tài liệu. Xác định vị trí hình mờ cụ thể và [sửa đổi thuộc tính của chúng](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Tìm kiếm và sửa đổi hình mờ.">}}
        ```csharp {style=abap}   
        // Tải tài liệu nguồn
        Watermarker watermarker = new Watermarker("document.pdf");

        // Tìm kiếm hình mờ để được cập nhật
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);                               
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);                             

        // Cập nhật các thuộc tính mong muốn
        for (PossibleWatermark watermark : watermarks)                                                           
        {  
            watermark.setText("New Text");
        }

        // Lưu tài liệu đã sửa đổi vào một đường dẫn được chỉ định
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
