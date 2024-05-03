
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:17
draft: false
lang: vi
format: Pptx
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Cập nhật hình mờ trong PPTX tài liệu một cách liền mạch"
head_description: "Sửa đổi hình mờ liền mạch trong PPTX bản trình bày thông qua GroupDocs.Watermark for Node.js via Java. Kết hợp thư viện của chúng tôi với các ứng dụng của bạn."

############################# Header ############################
title: "Cập nhật hình mờ trong PPTX bài thuyết trình" 
description: "Sửa đổi hình mờ một cách dễ dàng và hiệu quả bằng cách sử dụng GroupDocs.Watermark for Node.js via Java. Giữ tài liệu doanh nghiệp của bạn an toàn bằng cách sử dụng một lựa chọn hình mờ. Tùy chỉnh các thuộc tính hình mờ như kích thước, căn chỉnh, góc xoay và vị trí một cách dễ dàng."
subtitle: "GroupDocs.Watermark for Node.js via Java Thư viện" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "NPM Tải xuống gói"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java Giải pháp"
    link: "/watermark/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java cho phép sửa đổi liền mạch hình mờ trong tài liệu. Với công cụ linh hoạt này, các nhà phát triển có thể dễ dàng sửa đổi và cập nhật hình mờ ở các định dạng tệp khác nhau, bao gồm PDF, Microsoft Word, Excel, PowerPoint, Visio, email và định dạng hình ảnh. GroupDocs.Watermark for Node.js via Java có thể được sử dụng với tất cả các hệ điều hành phổ biến.

############################# Steps ############################
steps:
    enable: true
    title: "Chỉnh sửa hình mờ động cho PPTX trong Node.js via Java"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** cung cấp cho nhà phát triển Node.js via Java một API mạnh mẽ để chỉnh sửa hình mờ trên các tài liệu PPTX đa dạng. Dưới đây là hướng dẫn toàn diện để hợp lý hóa quy trình làm việc của bạn:
      
      1. **Bắt đầu quá trình:** Bắt đầu bằng cách cung cấp tệp PPTX của bạn làm đối số cho hàm tạo của lớp **Watermarker**. Tùy thuộc vào yêu cầu của bạn, tệp có thể được lấy nguồn dưới dạng luồng hoặc từ vị trí đĩa cục bộ.
      2. **Xác định hình mờ:** Sử dụng đối tượng **SearchCriteria** để xác định các hình mờ cần sửa đổi. Công cụ linh hoạt này cho phép lựa chọn hình mờ được nhắm mục tiêu dựa trên các thuộc tính cụ thể.
      3. **Tinh chỉnh với độ chính xác:** Sau khi thực hiện tìm kiếm thành công, có quyền truy cập vào bộ sưu tập hình mờ có liên quan. Tận hưởng khả năng kiểm soát chi tiết đối với từng thành phần, với khả năng cập nhật kích thước, vị trí trang, nội dung văn bản, màu sắc, dữ liệu hình ảnh, v.v.
      4. **Tính bền vững liền mạch:** Sau khi cập nhật hình mờ hoàn tất, hãy lưu trữ tài liệu đã sửa đổi một cách an toàn. API cung cấp các tùy chọn lưu trữ linh hoạt, cho phép bạn lưu vào đường dẫn tệp cục bộ hoặc dưới dạng đối tượng luồng.
   
    code:
      platform: "net"
      copy_title: "Sao chép"
      install:
        command: "npm i @groupdocs/groupdocs.watermark"
        copy_tip: "bấm để sao chép"
        copy_done: "sao chép"
      links:
        #  loop
        - title: "Thêm ví dụ"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
        #  loop
        - title: "Tài liệu"
          link: "https://docs.groupdocs.com/watermark/nodejs-java/"
          
      content: |
        ```javascript {style=abap}

        // Cập nhật hình mờ PPTX

        // Soạn Watermarker cho tệp PPTX
        const watermarker = new groupdocs.watermark.Watermarker("input.pptx");

        // Sử dụng SearchCriteria để tìm một hình ảnh cụ thể
        const searchCriteria = 
            new groupdocs.watermark.ImageDctHashSearchCriteria("logo.png");
        const watermarks = watermarker.search(searchCriteria);
        
        // Cập nhật nội dung hình ảnh
        for (const watermark of watermarks.getInnerList().toArray())
        {
            watermark.setImageData(imageData);
        }

        // Lưu tập tin cập nhật
        watermarker.save("output.pptx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tìm hiểu sâu về việc thêm Watermark"
  description: "API để hiển thị, hiển thị, chuyển đổi tài liệu, trang trình bày, sơ đồ và nhiều loại tài liệu khác trong .NET ứng dụng"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Thêm hình mờ"
  features:
    # feature loop
    - title: "Dễ dàng chỉnh sửa hình mờ trong PDF s"
      content: "GroupDocs.Watermark cung cấp các công cụ mạnh mẽ trong Node.js via Java để chỉnh sửa liền mạch hình mờ hiện có trong PDF tài liệu. Điều chỉnh vị trí, độ trong suốt và hơn thế nữa một cách dễ dàng."

    # feature loop
    - title: "Tinh chỉnh chi tiết hình mờ cho độ chính xác"
      content: "Kiểm soát các chi tiết. API của chúng tôi cho phép bạn tinh chỉnh giao diện của hình mờ, cho phép sửa đổi chính xác kích thước, độ mờ và màu sắc trong PDF s của bạn."

    # feature loop
    - title: "Quản lý hình mờ hợp lý"
      content: "API của chúng tôi đơn giản hóa việc quản lý hình mờ. Cho dù cập nhật hay xóa, bạn có thể quản lý hình mờ hiệu quả, duy trì tính toàn vẹn của tài liệu đồng thời đáp ứng nhu cầu xây dựng thương hiệu của bạn."
      
  code_samples:
    # code sample loop
    - title: "Cập nhật nội dung hình mờ bản trình bày"
      content: |
        Ví dụ này cho thấy cách cập nhật nội dung văn bản của hình mờ Bản trình bày
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Tải tài liệu PDF để xử lý
            const watermarker = new groupdocsWatermark.Watermarker("source.pptx");

            //  Tìm kiếm hình mờ cụ thể đáp ứng tiêu chí của bạn
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria("denied", false);
            const watermarks = watermarker.search(searchCriteria);
  
            //  Chỉnh sửa cài đặt hình mờ, chẳng hạn như kích thước, màu sắc và vị trí
            for (const watermark of watermarks.getInnerList().toArray()) {
                watermark.setText("accepted");
            }

            //  Lưu tài liệu đã cập nhật vào hệ thống cục bộ hoặc truyền trực tiếp
            watermarker.save("result.pptx");
            watermarker.close();

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Sẵn sàng để bắt đầu?"
  description: "Dùng thử GroupDocs.Watermark tính năng miễn phí hoặc yêu cầu giấy phép"
  items:
    #  loop
    - title: "NPM tải về"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      color: "red"
        #  loop
    - title: "Cấp phép"
      link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Cập nhật hình mờ định dạng tệp được hỗ trợ"
    exclude: "PPTX"
    description: "Sửa đổi hình mờ liền mạch trong PDF, Word, Excel và nhiều hơn nữa với GroupDocs.Watermark for Node.js via Java. Tăng cường xây dựng thương hiệu tài liệu của bạn."
    items: 
        # format loop 1
        - name: "Hình mờ PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/update//pdf/"
          description: "Định dạng tài liệu Adobe Portable"

        # format loop 2
        - name: "Hình mờ Word"
          format: "WORD"
          link: "/watermark/nodejs-java/update//word/"
          description: "MS Word và tài liệu Open Office"
          
        # format loop 3
        - name: "Hình mờ Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/update//excel/"
          description: "MS Excel và bảng tính Open Office"

        # format loop 4
        - name: "Hình mờ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/update//powerpoint/"
          description: "MS PowerPoint và các bài thuyết trình Open Office"

        # format loop 5
        - name: "Hình mờ DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/update//docx/"
          description: "Microsoft Word Tài liệu XML mở"
          
        # format loop 6
        - name: "Hình mờ PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/update//pptx/"
          description: "PowerPoint Bản trình bày XML mở"
          
        # format loop 7
        - name: "Hình mờ XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/update//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Hình mờ DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/update//doc/"
          description: "Tài liệu Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Hình mờ XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/update//xls/"
          description: "Microsoft Excel Sổ làm việc 97-2003"

        # format loop 10
        - name: "Hình mờ PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/update//ppt/"
          description: "PowerPoint Bài thuyết trình 97-2003"

        # format loop 11
        - name: "Hình mờ RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/update//rtf/"
          description: "Định dạng văn bản phong phú"

---