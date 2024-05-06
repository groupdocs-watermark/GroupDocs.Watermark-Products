---
############################# Static ############################
layout: "landing"
date: 2024-05-06T23:13:47
draft: false

lang: vi
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
head_title: "Node.js Watermarking Library | hình mờ tài liệu"
head_description: "Giải pháp Node.js bảo vệ tài liệu kinh doanh với hình mờ văn bản và hình ảnh. Các định dạng phổ biến như PDF, Word, Excel, PowerPoint được hỗ trợ."

############################# Header ############################
title: "Truy cập vào công nghệ hình mờ trong Node.js thông qua giải pháp Java"
description: "Bảo vệ tài sản trí tuệ của bạn và ngăn chặn sao chép trái phép với giải pháp Node.js này. Nó cho phép người dùng dễ dàng thêm hình mờ vào tài liệu kinh doanh ở các định dạng khác nhau, bao gồm PDF, Word, Excel, PowerPoint, hình ảnh, v.v."
words:
  for: "cho"

actions:
  main: "Sử dụng NPM để tải xuống miễn phí"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.watermark"
  alt: "Cấp phép"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
  title: "Sẵn sàng để bắt đầu?"
  description: "Dùng thử GroupDocs.Watermark tính năng miễn phí hoặc yêu cầu giấy phép"

release:
  title: "Phiên bản {0} đã phát hành"
  notes: "Xem những gì mới"
  downloads: "Tải xuống"
  link: "https://releases.groupdocs.com/watermark/nodejs-java/"

code:
  title: "Thêm hình mờ vào PDF với TypeScript"
  more: "Thêm ví dụ"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.watermarker"
  content: |
    ```javascript {style=abap}

    // Thực hiện Watermarker đi qua đường dẫn PDF
    let loadOptions = new PdfLoadOptions();
    let watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Tùy chỉnh tùy chọn hình mờ
    let textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Áp dụng hình mờ cho tài liệu PDF
    watermarker.add(textWatermark);

    // Lưu tài liệu kết quả
    watermarker.save("result.pdf");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark trong nháy mắt"
  description: "Thư viện Node.js TypeScript để tạo hình mờ"
  features:
    # feature loop
    - title: "Đánh dấu tệp Node.js"
      content: "Bảo vệ tài liệu kinh doanh của bạn với GroupDocs.Watermark for Node.js via Java. Thêm văn bản, hình ảnh, sơ đồ hoặc tệp đính kèm email dưới dạng hình mờ vào các định dạng tệp khác nhau."

    # feature loop
    - title: "Tùy chỉnh hình mờ cho nhu cầu của bạn"
      content: "GroupDocs.Watermark for Node.js via Java cung cấp các tùy chọn tùy chỉnh mở rộng cho hình mờ. Tinh chỉnh các kiểu văn bản (in đậm, in nghiêng, phông chữ) và thuộc tính hình ảnh (xoay, v.v.) cho phép tùy chỉnh xử lý tài liệu."

    # feature loop
    - title: "Hỗ trợ định dạng toàn diện"
      content: "GroupDocs.Watermark for Node.js via Java tích hợp liền mạch với một loạt các định dạng tệp, bao gồm: PDF, MS Office như Word, Excel, PowerPoint, hình ảnh như JPEG, PNG, GIF, BMP, Visio, Visio sơ đồ, email... Cho phép xử lý tài liệu để đạt được mục tiêu kinh doanh."

    # feature loop
    - title: "Tìm kiếm và cập nhật hình mờ mạnh mẽ"
      content: "Nhận và cập nhật hình mờ hiện có trong các tài liệu có hình mờ. Sửa đổi văn bản, kiểu dáng, nội dung hình ảnh hoặc xóa chúng hoàn toàn. GroupDocs.Watermark for Node.js via Java cung cấp một loạt các xử lý hình mờ."

############################# Platforms ############################
platforms:
  enable: true
  title: "Độc lập nền tảng"
  description: "GroupDocs.Watermark for Node.js via Java dễ dàng tích hợp với các hệ điều hành khác nhau và trình quản lý gói."
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
  title: "Định dạng tập tin được hỗ trợ"
  description: |
    GroupDocs.Watermark for Node.js via Java cho phép bạn xử lý một loạt các định dạng tập tin đa dạng. [Khám phá danh sách đầy đủ](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Node.js via Java: Bộ tính năng"
  description: "Tăng cường bảo mật tài liệu mạnh mẽ thông qua hình mờ theo chương trình. Hỗ trợ các định dạng tệp đa dạng bao gồm: PDF, DOCX, XLSX, PPTX và các định dạng hình ảnh (PNG, JPG, v.v.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Kiểm soát hình mờ chính xác"
      content: "Thao tác chính xác hình mờ bằng cách thêm hoặc xóa chúng khỏi các phần cụ thể, toàn bộ tài liệu hoặc các tệp đính kèm và hình dạng riêng lẻ trong các định dạng tệp khác nhau."

    # feature loop
    - icon: "watermark_style"
      title: "Tùy chỉnh giao diện hình mờ"
      content: "Thực hiện kiểm soát chi tiết đối với tính thẩm mỹ hình mờ bằng cách sửa đổi các thuộc tính như màu sắc, phông chữ, độ mờ, xoay và định vị trong tài liệu."

    # feature loop
    - icon: "hidden_print"
      title: "In PDF Hình mờ"
      content: "Triển khai hình mờ ẩn không nhìn thấy trong quá trình xem tài liệu thông thường nhưng chỉ trở nên rõ ràng trong quá trình in, tăng cường bảo mật tài liệu một cách kín đáo."

    # feature loop
    - icon: "image_only"
      title: "Hình mờ hình ảnh cụ thể"
      content: "Đánh dấu hình ảnh cụ thể trong tài liệu bằng cách sử dụng giải pháp của chúng tôi. Chọn nhúng hình mờ trong một phần được chỉ định (ví dụ: trang, trang chiếu) hoặc trên toàn bộ tài liệu."

    # feature loop
    - icon: "image_frame"
      title: "Hình ảnh đa khung hình mờ"
      content: "Áp dụng hình mờ một cách chọn lọc cho các khung cụ thể trong định dạng hình ảnh nhiều khung hình, đảm bảo kiểm soát chi tiết vị trí hình mờ."

    # feature loop
    - icon: "attachments"
      title: "Bảo vệ nội dung toàn diện"
      content: "Mở rộng bảo vệ cho các phần tử tài liệu khác nhau như tệp đính kèm trong Excel tài liệu và hình dạng hình ảnh trong Bản trình bày, cung cấp thêm một lớp bảo mật."

    # feature loop
    - icon: "pdf_objects"
      title: "Hình mờ nâng cao trong PDF"
      content: "Đánh dấu các khu vực khác nhau của PDF s, bao gồm Bleed Box, Art Box, Crop Box, Trim Box, v.v."

    # feature loop
    - icon: "doc_background"
      title: "Hình nền mờ"
      content: "Quản lý hình mờ trong hình nền của Bảng tính và Bản trình bày, cung cấp các tùy chọn tùy chỉnh bổ sung cho các biện pháp bảo mật trực quan."

    # feature loop
    - icon: "unreadable_characters"
      title: "Hình mờ văn bản với các ký tự không đọc được"
      content: "Sử dụng các ký tự không đọc được trong hình mờ văn bản được nhúng trong Bản trình bày, tăng cường bảo mật bằng cách làm cho việc trích xuất hình mờ trái phép trở nên khó khăn hơn đáng kể."

    # feature loop
    - icon: "watermark_text_search"
      title: "Tìm kiếm hình mờ nâng cao"
      content: "Sử dụng khả năng tìm kiếm toàn diện để định vị hình mờ trong tài liệu dựa trên các thông số cụ thể hoặc bằng cách kết hợp các tiêu chí khác nhau, cho phép truy xuất và quản lý hiệu quả."

    # feature loop
    - icon: "watermark_image_search"
      title: "Phát hiện hình mờ hình ảnh tương tự"
      content: "Tìm hình ảnh hình mờ tương tự trong các tài liệu giống hình ảnh nguồn một cách trực quan."

    # feature loop
    - icon: "document_info"
      title: "Trích xuất thông tin tài liệu lập trình"
      content: "Trích xuất siêu dữ liệu có giá trị theo chương trình, bao gồm chi tiết thiết lập trang và thông tin tài liệu khác cho các định dạng tệp được hỗ trợ."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Mẫu mã"
  description: "Đi sâu vào các ví dụ mã giới thiệu các chức năng GroupDocs.Watermark for Node.js via Java phổ biến"
  items:
    # code sample loop
    - title: "Đánh dấu tài liệu bằng hình ảnh"
      content: |
        Tận dụng GroupDocs.Watermark for Node.js via Java để tăng cường bảo mật tài liệu bằng cách thêm hình mờ hình ảnh. Tìm hiểu thêm: [Hình mờ hình ảnh](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Cách bảo vệ tệp bằng hình mờ hình ảnh.">}}
        ```javascript {style=abap}
        // Tải tài liệu nguồn vào Watermarker
        let watermarker = new Watermarker("document.pdf");
        
        // Chỉ định đường dẫn đến hình ảnh hình mờ
        let watermark = new ImageWatermark("watermark.jpg");

        // Bảo vệ tập tin và lưu nó
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Tìm kiếm và sửa đổi hình mờ hiện có"
      content: |
        GroupDocs.Watermark for Node.js via Java cho phép bạn quản lý hình mờ tài liệu. Chọn hình mờ, sửa đổi thuộc tính của chúng. Khám phá cách: [Sửa đổi hình mờ](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Tìm kiếm và sửa đổi hình mờ.">}}
        ```javascript {style=abap}   
        // Tải tài liệu nguồn
        let watermarker = new Watermarker("document.pdf");

        // Tìm kiếm hình mờ để được cập nhật
        let searchCriteria = new TextSearchCriteria("test", false);                               
        let watermarks = watermarker.search(searchCriteria); 

        // Cập nhật các thuộc tính mong muốn
        watermarks.forEach((watermark)
        {  
            watermark.setText("New Text");
        }

        // Lưu tài liệu đã sửa đổi vào một đường dẫn được chỉ định
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
