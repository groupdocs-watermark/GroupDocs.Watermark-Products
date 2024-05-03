
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:17
draft: false
lang: vi
format: Xlsx
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Nhúng hình mờ trong XLSX với Node.js"
head_description: "Tận dụng Node.js để tạo và áp dụng hình mờ trong XLSX tệp, bảo mật tài liệu Excel của bạn."

############################# Header ############################
title: "Bảo mật XLSX trang tính với Node.js" 
description: "Sử dụng API Node.js để tạo hình mờ tùy chỉnh cho XLSX tệp, hoàn hảo để tăng cường tính toàn vẹn của tài liệu và bảo vệ thông tin nhạy cảm."
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống tại NPM miễn phí"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java cung cấp một giải pháp mạnh mẽ cho các nhà phát triển Node.js để tạo, thêm và quản lý hình mờ trong XLSX tệp. API này rất cần thiết để duy trì tính bảo mật và tính xác thực của Excel tài liệu, đặc biệt là trong môi trường công ty, tài chính và pháp lý. Tùy chỉnh hình mờ của bạn với nhiều tùy chọn, bao gồm lớp phủ văn bản và hình ảnh, được thiết kế vừa có chức năng vừa tinh tế. Các tính năng bổ sung cho phép tạo hình mờ tự động dựa trên thuộc tính tài liệu và điều kiện do người dùng xác định, đảm bảo rằng hình mờ của bạn được áp dụng nhất quán và chỉ khi cần thiết. GroupDocs.Watermark tương thích với các nền tảng .NET hiện đại và hỗ trợ các chức năng nâng cao Excel.

############################# Steps ############################
steps:
    enable: true
    title: "Bảo vệ tài liệu doanh nghiệp: Tạo hình mờ Xlsx"
    content: |
      Tăng cường bảo mật tài liệu với **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/):** - Giải pháp tạo hình mờ mạnh mẽ cho Node.js via Java.
      
      1. **Hợp lý hóa hình chìm mờ an toàn trong các ứng dụng Node.js via Java của bạn:** Lớp **Watermarker** đóng vai trò là thành phần cốt lõi của API GroupDocs.Watermark. Thư viện này đơn giản hóa việc tạo hình mờ ở nhiều định dạng tài liệu khác nhau, bao gồm cả Xlsx. Để bắt đầu, hãy tạo phiên bản Watermarker trước khi xử lý tài liệu của bạn. Cung cấp đường dẫn tệp Xlsx hoặc đối tượng luồng cho hàm tạo trong quá trình khởi tạo.
      2. **Tạo hình mờ để tăng cường khả năng bảo vệ:** Cung cấp hình mờ hoàn toàn phù hợp với nhu cầu bảo mật của bạn. Xây dựng một đối tượng **Watermark** chỉ định loại mong muốn. Không giống như vị trí trang truyền thống, bạn có thể nhúng hình mờ vào các thành phần tài liệu gốc như tiêu đề hoặc tệp đính kèm, tăng cường bảo mật tài liệu và thêm nét chuyên nghiệp.
      3. **Tinh chỉnh giao diện hình mờ để có tác động tối ưu:** Kiểm soát khía cạnh trực quan của hình mờ của bạn. Tùy chỉnh các thuộc tính như chiều cao, chiều rộng, căn chỉnh (trên cùng, bên trái, giữa, v.v.), họ phông chữ và màu sắc để đạt được kết quả nhất quán và hiệu quả về mặt hình ảnh nhằm củng cố tính hợp pháp của tài liệu.
      4. **Ứng dụng hình mờ và lưu trữ an toàn**: Kết hợp hình mờ của bạn bằng phương pháp **Watermarker**. Thư viện cho phép bạn thêm nhiều hình mờ nếu cần thiết để tăng cường bảo vệ. Bạn nên lưu tài liệu Xlsx đã sửa đổi vào một vị trí riêng biệt, an toàn để bảo vệ tệp gốc và bảo vệ tài liệu có hình mờ của bạn.
   
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

        // Tạo hình mờ cho hình ảnh cho XLSX

        // Khởi tạo tệp nguồn truyền Watermarker
        const watermarker = new groupdocs.watermark.Watermarker("input.xlsx");
        
        // Tạo hình mờ bằng cách cung cấp tệp hình ảnh
        const watermark = new groupdocs.watermark.ImageWatermark("watermark.png");

        // Nhận kết quả XLSX
        watermarker.add(watermark);
        watermarker.save("output.xlsx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tích hợp hình mờ tinh tế"
  description: "GroupDocs.Watermark API dành cho .NET nhà phát triển của chúng tôi cung cấp các giải pháp tinh tế để tích hợp hình mờ liền mạch vào bất kỳ tài liệu nào. Công cụ này được thiết kế để tạo ra các hình mờ tinh vi, không phô trương, đảm bảo bảo vệ bản quyền trong khi vẫn duy trì tính thẩm mỹ của tài liệu."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Tích hợp hình mờ chính xác"
  features:
    # feature loop
    - title: "Hiệu ứng hình mờ Gradient"
      content: "Triển khai hình mờ gradient hòa quyện mượt mà trên các tài liệu của bạn. Tính năng này cho phép các gradient tuyến tính hoặc xuyên tâm, thêm giao diện hiện đại cho các tính năng bảo mật giúp tăng cường cả bảo vệ và tương tác trực quan mà không làm quá tải nội dung."

    # feature loop
    - title: "Hình mờ mẫu để tăng cường bảo mật"
      content: "Sử dụng hình mờ dựa trên mẫu để thêm một lớp bảo mật bổ sung. API của chúng tôi hỗ trợ các mẫu khác nhau có thể được thiết kế phức tạp và lặp lại trên toàn tài liệu, làm cho hình mờ có khả năng chống giả mạo và loại bỏ tốt hơn."

    # feature loop
    - title: "Hình mờ dành riêng cho tài liệu"
      content: "Điều chỉnh hình mờ độc đáo cho các loại tài liệu khác nhau. Cho dù đó là hợp đồng pháp lý, kế hoạch kinh doanh hay báo cáo khoa học, hãy tùy chỉnh hình mờ để phù hợp với mục đích của tài liệu và khả năng tiếp cận của người đọc, đảm bảo tích hợp và bảo mật tối ưu."
      
  code_samples:
    # code sample loop
    - title: "Tạo hình mờ hình ảnh PDF"
      content: |
        Tạo hình mờ hình ảnh cho tất cả các hình ảnh được trình bày bên trong tài liệu PDF
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Tải tài liệu dưới dạng PDF
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  Tạo hình mờ dựa trên chú thích PDF
            const imageWatermark = new groupdocsWatermark.ImageWatermark("watermark.jpg");
            imageWatermark.setHorizontalAlignment(groupdocsWatermark.HorizontalAlignment.Center);
            imageWatermark.setVerticalAlignment(groupdocsWatermark.VerticalAlignment.Center);
            imageWatermark.setRotateAngle(-45);
            imageWatermark.setSizingType(groupdocsWatermark.SizingType.ScaleToParentDimensions);
            imageWatermark.setScaleFactor(1);
  
            //  Thiết lập tùy chọn hình mờ
            const images = watermarker.getImages();
            for (let i = 0; i < images.getCount(); i++) {
                if (images.get_Item(i).getWidth() > 100 && images.get_Item(i).getHeight() > 100) {
                    images.get_Item(i).add(imageWatermark);
                }
            }

            //  Thêm hình mờ văn bản vào tài liệu kết quả
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
    title: "Triển khai hình mờ trong XLSX với Node.js"
    exclude: "XLSX"
    description: "Triển khai Node.js để thêm hiệu quả hình mờ nâng cao, an toàn vào tệp XLSX, bảo vệ dữ liệu chuyên nghiệp Excel của bạn."
    items: 
        # format loop 1
        - name: "Hình mờ PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/generate//pdf/"
          description: "Định dạng tài liệu Adobe Portable"

        # format loop 2
        - name: "Hình mờ Word"
          format: "WORD"
          link: "/watermark/nodejs-java/generate//word/"
          description: "MS Word và tài liệu Open Office"
          
        # format loop 3
        - name: "Hình mờ Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/generate//excel/"
          description: "MS Excel và bảng tính Open Office"

        # format loop 4
        - name: "Hình ảnh hình mờ"
          format: "IMAGE"
          link: "/watermark/nodejs-java/generate//image/"
          description: "Định dạng hình ảnh phổ biến"

        # format loop 5
        - name: "Ảnh hình mờ"
          format: "PHOTO"
          link: "/watermark/nodejs-java/generate//photo/"
          description: "Định dạng ảnh"

        # format loop 6
        - name: "Hình mờ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/generate//powerpoint/"
          description: "MS PowerPoint và các bài thuyết trình Open Office"

        # format loop 7
        - name: "Hình mờ DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/generate//docx/"
          description: "Microsoft Word Tài liệu XML mở"
          
        # format loop 8
        - name: "Hình mờ PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/generate//pptx/"
          description: "PowerPoint Bản trình bày XML mở"
          
        # format loop 9
        - name: "Hình mờ XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/generate//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 10
        - name: "Hình mờ JPEG"
          format: "JPEG"
          link: "/watermark/nodejs-java/generate//jpeg/"
          description: "JPEG Hình ảnh"

        # format loop 11
        - name: "Hình mờ PNG"
          format: "PNG"
          link: "/watermark/nodejs-java/generate//png/"
          description: "Portable Đồ họa mạng"

        # format loop 12
        - name: "Hình mờ TIFF"
          format: "TIFF"
          link: "/watermark/nodejs-java/generate//tiff/"
          description: "Nhãn định dạng tệp hình ảnh"

        # format loop 13
        - name: "Hình mờ WEBP"
          format: "WEBP"
          link: "/watermark/nodejs-java/generate//webp/"
          description: "Hình ảnh WEB"

        # format loop 14
        - name: "Hình mờ DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/generate//doc/"
          description: "Tài liệu Microsoft Word 97 - 2007"

        # format loop 15
        - name: "Hình mờ XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/generate//xls/"
          description: "Microsoft Excel Sổ làm việc 97-2003"

        # format loop 16
        - name: "Hình mờ PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/generate//ppt/"
          description: "PowerPoint Bài thuyết trình 97-2003"

        # format loop 17
        - name: "Hình mờ RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/generate//rtf/"
          description: "Định dạng văn bản phong phú"

---