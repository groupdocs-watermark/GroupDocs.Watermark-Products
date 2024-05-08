
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:27
draft: false
lang: vi
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Tạo hình mờ trong DOCX với Node.js"
head_description: "Khai thác Node.js để thêm hình mờ mạnh mẽ vào tệp DOCX, tăng cường bảo mật và tính toàn vẹn của tài liệu."

############################# Header ############################
title: "Tạo hình mờ cho DOCX bằng Node.js" 
description: "Sử dụng Node.js để soạn và triển khai hình mờ tinh vi trong tệp DOCX, hoàn hảo để bảo mật các tài liệu nhạy cảm Word."
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
       GroupDocs.Watermark for Node.js via Java trang bị cho các nhà phát triển Node.js các công cụ để tạo, thêm và quản lý hình mờ trong DOCX tài liệu một cách hiệu quả. API này cho phép tích hợp liền mạch các hình mờ có thể tùy chỉnh có thể tăng cường đáng kể bảo mật tài liệu. Cho dù thêm logo công ty, văn bản hay lớp phủ đồ họa phức tạp, API cung cấp toàn quyền kiểm soát độ mờ, kích thước và vị trí. Được thiết kế đặc biệt cho các môi trường chuyên nghiệp nơi tính xác thực tài liệu và bảo vệ bản quyền là rất quan trọng, chẳng hạn như các lĩnh vực pháp lý, tài chính và chính phủ, GroupDocs.Watermark đảm bảo rằng tệp DOCX của bạn không chỉ bảo mật mà còn duy trì tiêu chuẩn trình bày cao. Tương thích với các môi trường Node.js khác nhau, nó hỗ trợ các hoạt động đồng bộ và không đồng bộ để phù hợp với các nhu cầu ứng dụng khác nhau.

############################# Steps ############################
steps:
    enable: true
    title: "Bảo vệ tài liệu doanh nghiệp: Tạo hình mờ Docx"
    content: |
      Tăng cường bảo mật tài liệu với **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/):** - Giải pháp tạo hình mờ mạnh mẽ cho Node.js via Java.
      
      1. **Hợp lý hóa hình chìm mờ an toàn trong các ứng dụng Node.js via Java của bạn:** Lớp **Watermarker** đóng vai trò là thành phần cốt lõi của API GroupDocs.Watermark. Thư viện này đơn giản hóa việc tạo hình mờ ở nhiều định dạng tài liệu khác nhau, bao gồm cả Docx. Để bắt đầu, hãy tạo phiên bản Watermarker trước khi xử lý tài liệu của bạn. Cung cấp đường dẫn tệp Docx hoặc đối tượng luồng cho hàm tạo trong quá trình khởi tạo.
      2. **Tạo hình mờ để tăng cường khả năng bảo vệ:** Cung cấp hình mờ hoàn toàn phù hợp với nhu cầu bảo mật của bạn. Xây dựng một đối tượng **Watermark** chỉ định loại mong muốn. Không giống như vị trí trang truyền thống, bạn có thể nhúng hình mờ vào các thành phần tài liệu gốc như tiêu đề hoặc tệp đính kèm, tăng cường bảo mật tài liệu và thêm nét chuyên nghiệp.
      3. **Tinh chỉnh giao diện hình mờ để có tác động tối ưu:** Kiểm soát khía cạnh trực quan của hình mờ của bạn. Tùy chỉnh các thuộc tính như chiều cao, chiều rộng, căn chỉnh (trên cùng, bên trái, giữa, v.v.), họ phông chữ và màu sắc để đạt được kết quả nhất quán và hiệu quả về mặt hình ảnh nhằm củng cố tính hợp pháp của tài liệu.
      4. **Ứng dụng hình mờ và lưu trữ an toàn**: Kết hợp hình mờ của bạn bằng phương pháp **Watermarker**. Thư viện cho phép bạn thêm nhiều hình mờ nếu cần thiết để tăng cường bảo vệ. Bạn nên lưu tài liệu Docx đã sửa đổi vào một vị trí riêng biệt, an toàn để bảo vệ tệp gốc và bảo vệ tài liệu có hình mờ của bạn.
   
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

        // Tạo hình mờ cho hình ảnh cho DOCX

        // Khởi tạo tệp nguồn truyền Watermarker
        const watermarker = new groupdocs.watermark.Watermarker("input.docx");
        
        // Tạo hình mờ bằng cách cung cấp tệp hình ảnh
        const watermark = new groupdocs.watermark.ImageWatermark("watermark.png");

        // Nhận kết quả DOCX
        watermarker.add(watermark);
        watermarker.save("output.docx");
        
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
    title: "Thêm hình mờ vào DOCX bằng Node.js"
    exclude: "DOCX"
    description: "Triển khai Node.js để tự động tạo và áp dụng hình mờ tùy chỉnh trong DOCX tệp, bảo mật và xây dựng thương hiệu chúng một cách hiệu quả."
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