
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:08
draft: false
lang: vi
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Cập nhật hình mờ cho Excel Bảng tính"
head_description: "Cập nhật hình mờ trong bảng tính có định dạng khác nhau bằng cách sử dụng GroupDocs.Watermark for Node.js via Java. Làm phong phú thêm Node.js via Java ứng dụng của bạn."

############################# Header ############################
title: "Cách mạng hóa hình mờ bảng tính bằng cách sử dụng Node.js via Java" 
description: "Trải nghiệm sức mạnh của GroupDocs.Watermark for Node.js via Java. Bảo mật tài liệu kinh doanh của bạn với nhiều hình mờ khác nhau. Cập nhật kích thước hình mờ, căn chỉnh, góc xoay, vị trí, v.v."
subtitle: "GroupDocs.Watermark for Node.js via Java CÁ" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống miễn phí NPM"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java thư viện"
    link: "/watermark/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java là một giải pháp toàn diện để quản lý hình mờ bằng môi trường Node.js via Java. Với công cụ này, các nhà phát triển có thể dễ dàng thực hiện các thao tác như thêm, chỉnh sửa, tìm kiếm và xóa hình mờ khỏi tài liệu ở các định dạng tệp khác nhau, bao gồm PDF, Microsoft Word, Excel, PowerPoint, Visio, email và định dạng hình ảnh. GroupDocs.Watermark hỗ trợ tất cả các hệ điều hành chính và các phiên bản Node.js.

############################# Steps ############################
steps:
    enable: true
    title: "Cập nhật Hình mờ trong EXCEL qua Node.js via Java"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** trang bị cho nhà phát triển Node.js via Java một API mạnh mẽ để cập nhật hình mờ theo chương trình trong nhiều tài liệu EXCEL khác nhau. Hướng dẫn này phác thảo quá trình:
      
      1. Bắt đầu quá trình bằng cách cung cấp tệp EXCEL của bạn làm đối số cho hàm tạo của lớp **Watermarker**. Tùy thuộc vào nhu cầu của bạn, tệp có thể được cung cấp dưới dạng luồng hoặc tham chiếu đến vị trí đĩa cục bộ.
      2. Sau đó, tận dụng đối tượng **SearchCriteria** để xác định các hình mờ cụ thể cần sửa đổi. Đối tượng này cho phép xác định chính xác các hình mờ dựa trên các thuộc tính mong muốn.
      3. Sau khi thực hiện tìm kiếm thành công, bạn sẽ nhận được một bộ sưu tập các hình mờ có liên quan. Những hình mờ này cung cấp khả năng kiểm soát chi tiết, cho phép bạn cập nhật các thuộc tính như kích thước, vị trí trang, nội dung văn bản, bảng màu, dữ liệu hình ảnh, v.v.
      4. Sau khi hoàn thành cập nhật hình mờ, hãy duy trì tài liệu đã sửa đổi. API hỗ trợ lưu trữ bằng cách sử dụng đường dẫn tệp cục bộ hoặc đối tượng luồng.
   
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

        // Cập nhật hình mờ văn bản EXCEL

        // Cung cấp phiên bản Watermarker cho tệp EXCEL
        const watermarker = new groupdocs.watermark.Watermarker("input.xslx");

        // Sử dụng TextSearchCriteria để tìm hình mờ văn bản
        const searchCriteria = 
            new groupdocs.watermark.TextSearchCriteria("test", false);
        const watermarks = watermarker.search(searchCriteria);
        
        // Cập nhật hình mờ văn bản
        for (const watermark of watermarks.getInnerList().toArray())
        {
            watermark.setText("passed");
        }

        // Tận hưởng kết quả
        watermarker.save("output.xslx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Làm chủ chỉnh sửa hình mờ trong PDF giây với GroupDocs.Watermark"
  description: "Khám phá các tính năng API toàn diện để điều chỉnh và quản lý hình mờ trong PDF s trong Node.js via Java ứng dụng."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Chỉnh sửa hình mờ"
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
    - title: "Java Ví dụ: Chỉnh sửa hình mờ PDF"
      content: |
        Ví dụ Java này trình bày cách chỉnh sửa hình mờ hiện có trong tài liệu PDF, hiển thị cách điều chỉnh các thuộc tính của nó theo chương trình.
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Tải tài liệu PDF để xử lý
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  Tìm kiếm hình mờ cụ thể đáp ứng tiêu chí của bạn
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria("test", false);
            const watermarks = watermarker.search(searchCriteria);
  
            //  Chỉnh sửa cài đặt hình mờ, chẳng hạn như kích thước, màu sắc và vị trí
            for (const watermark of watermarks.getInnerList().toArray()) {
                watermark.getFormattedTextFragments().clear();
                watermark.getFormattedTextFragments().add("passed", 
                    new groupdocsWatermark.Font("Calibri", 19, groupdocsWatermark.FontStyle.Bold), 
                    groupdocsWatermark.Color.getRed(), groupdocsWatermark.Color.getAqua());
            }

            //  Lưu tài liệu đã cập nhật vào hệ thống cục bộ hoặc truyền trực tiếp
            watermarker.save("result.pdf");
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
    title: "Cập nhật hình mờ trên các định dạng tệp được hỗ trợ"
    exclude: "EXCEL"
    description: "Cập nhật hiệu quả hình mờ trong PDF, Word, Excel và nhiều hơn nữa với GroupDocs.Watermark for Node.js via Java. Tài liệu có hình mờ có thể làm phong phú thêm quy trình kinh doanh của bạn."
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