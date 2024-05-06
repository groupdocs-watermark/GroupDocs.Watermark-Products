
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:32
draft: false
lang: vi
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Khám phá Powerpoint Bản trình bày Hình mờ ẩn"
head_description: "Khám phá các hình mờ ẩn trong tài liệu bằng cách sử dụng GroupDocs.Watermark."

############################# Header ############################
title: "Khám phá các hình mờ được đặt trong Powerpoint bài thuyết trình" 
description: "Khám phá và tiết lộ các hình mờ ẩn trong tài liệu của bạn với GroupDocs.Watermark for Node.js via Java."
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống miễn phí NPM"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Tìm hiểu thêm về GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       Khám phá khả năng của GroupDocs.Watermark for Node.js via Java trong việc quản lý hình mờ liền mạch trên Node.js via Java. Dễ dàng xử lý các thao tác hình mờ như tạo, cập nhật, lấy và xóa trên các định dạng tệp khác nhau.

############################# Steps ############################
steps:
    enable: true
    title: "Nhận hình mờ trong tệp Powerpoint một cách hiệu quả của GroupDocs.Watermark"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** hợp lý hóa quy trình truy xuất hình mờ được nhúng trong các định dạng tài liệu kinh doanh khác nhau. Tích hợp liền mạch GroupDocs.Watermark vào các ứng dụng Node.js via Java của bạn để trang bị cho chúng khả năng phát hiện hình mờ mạnh mẽ.
      
      1. Để tận dụng các chức năng của GroupDocs.Watermark, hãy khởi tạo lớp **Watermarker** và cung cấp đường dẫn tệp Powerpoint, luồng tệp hoặc luồng byte làm đầu vào. Hành động này tải tài liệu để phân tích hình mờ.
      2. Để nhận dạng hình mờ được nhắm mục tiêu, hãy sử dụng đối tượng **SearchCriteria**. Chỉ định một hình ảnh để định vị các hình mờ tương tự. Ngoài ra, đối với hình mờ văn bản, hãy xác định nội dung văn bản, thuộc tính phông chữ, thuộc tính màu sắc và các thông số liên quan khác để tinh chỉnh tiêu chí tìm kiếm.
      3. Sử dụng phương thức **Search** của đối tượng **Watermarker** để bắt đầu quá trình phát hiện hình mờ trong tài liệu được tải. Hàm này trả về một tập hợp các đối tượng đại diện cho các hình mờ tiềm năng, cho phép xử lý thêm.
      4. Bộ sưu tập các đối tượng hình mờ được truy xuất mang lại cho bạn rất nhiều khả năng. Bạn có thể xóa hình mờ không mong muốn hoặc sửa đổi thuộc tính của chúng. Thay đổi nội dung, di chuyển hình mờ trên một trang và nhiều nội dung khác.
   
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

        // Nhận danh sách hình mờ văn bản cho POWERPOINT

        // Khởi tạo lớp Watermarker
        const watermarker = new groupdocs.watermark.Watermarker("input.pptx");
        
        // Nhận hình mờ theo tiêu chí văn bản
        const searchCriteria = new groupdocs.watermark.TextSearchCriteria("test", false);
        const watermarks = watermarker.search(searchCriteria);

        // Sử dụng thông tin hình mờ
        console.log(`Found ${watermarks.getCount()} possible watermark(s).`);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Hợp lý hóa tìm kiếm hình mờ của bạn với GroupDocs.Watermark trong Node.js"
  description: "Tìm hiểu cách triển khai các chức năng tìm kiếm hình mờ nâng cao trong các ứng dụng Node.js của bạn với GroupDocs.Watermark, tối ưu hóa quản lý tài liệu trong Node.js via Java."
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "Tìm kiếm Hình mờ trong Node.js"
  features:
    # feature loop
    - title: "Phát hiện hình mờ nâng cao trong Node.js"
      content: "Sử dụng GroupDocs.Watermark để tăng cường khả năng phát hiện và xác định hình mờ ở bất kỳ định dạng tài liệu nào. Tìm kiếm hiệu quả bằng cách sử dụng các tùy chọn lọc tinh vi."

    # feature loop
    - title: "API Node.js cho tìm kiếm hình mờ tùy chỉnh"
      content: "Tùy chỉnh hoạt động tìm kiếm của bạn với API Node.js của chúng tôi. Tìm hình mờ bằng cách chỉ định các tham số chi tiết như vị trí, độ mờ và loại nội dung, tối ưu hóa quy trình công việc tài liệu của bạn."

    # feature loop
    - title: "Truy xuất và phân tích hình mờ hiệu quả"
      content: "Với GroupDocs.Watermark, nhanh chóng trích xuất và phân tích hình mờ từ các tài liệu khác nhau. API của chúng tôi hỗ trợ truy xuất nhanh chóng, giúp bạn duy trì sự tuân thủ và tính nhất quán về thương hiệu."
      
  code_samples:
    # code sample loop
    - title: "Ví dụ Node.js: Tìm kiếm hình mờ hiệu quả"
      content: |
        Khám phá cách sử dụng Node.js với GroupDocs.Watermark để tìm kiếm hình mờ trên các loại tài liệu khác nhau, thể hiện việc sử dụng tiêu chí tìm kiếm động để có kết quả chính xác.
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Khởi tạo môi trường Node.js và tải tài liệu đích
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  Thiết lập truy vấn tìm kiếm bằng tiêu chí linh hoạt để tìm hình mờ cụ thể
            const criteria = new groupdocsWatermark.TextFormattingSearchCriteria();
            criteria.setForegroundColorRange(new groupdocsWatermark.ColorRange());
            criteria.getForegroundColorRange().setMinHue(-5);
            criteria.getForegroundColorRange().setMaxHue(10);
            criteria.setBackgroundColorRange(new groupdocsWatermark.ColorRange());
            criteria.getBackgroundColorRange().setEmpty(true);
            criteria.setFontName("Arial");
            criteria.setMinFontSize(19);
            criteria.setMaxFontSize(42);
            criteria.setFontBold(true);
  
            //  Thực hiện tìm kiếm và thu thập hình mờ đáp ứng các tiêu chí
            const watermarks = watermarker.search(criteria);

            //  Xử lý và phân tích kết quả để xác định các hành động cần thiết
            console.log(`Found ${watermarks.getCount()} possible watermark(s).`);
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
    title: "Khám phá hình mờ trên các định dạng"
    exclude: "POWERPOINT"
    description: "Dễ dàng khám phá hình mờ trên các định dạng tệp khác nhau với GroupDocs.Watermark for Node.js via Java."
    items: 
        # format loop 1
        - name: "Hình mờ PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/get//pdf/"
          description: "Định dạng tài liệu Adobe Portable"

        # format loop 2
        - name: "Hình mờ Word"
          format: "WORD"
          link: "/watermark/nodejs-java/get//word/"
          description: "MS Word và tài liệu Open Office"
          
        # format loop 3
        - name: "Hình mờ Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/get//excel/"
          description: "MS Excel và bảng tính Open Office"

        # format loop 4
        - name: "Hình mờ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/get//powerpoint/"
          description: "MS PowerPoint và các bài thuyết trình Open Office"

        # format loop 5
        - name: "Hình mờ DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/get//docx/"
          description: "Microsoft Word Tài liệu XML mở"
          
        # format loop 6
        - name: "Hình mờ PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/get//pptx/"
          description: "PowerPoint Bản trình bày XML mở"
          
        # format loop 7
        - name: "Hình mờ XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/get//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Hình mờ DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/get//doc/"
          description: "Tài liệu Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Hình mờ XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/get//xls/"
          description: "Microsoft Excel Sổ làm việc 97-2003"

        # format loop 10
        - name: "Hình mờ PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/get//ppt/"
          description: "PowerPoint Bài thuyết trình 97-2003"

        # format loop 11
        - name: "Hình mờ RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/get//rtf/"
          description: "Định dạng văn bản phong phú"

---