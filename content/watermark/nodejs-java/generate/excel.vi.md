
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:59
draft: false
lang: vi
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Tạo hình mờ duy nhất cho Excel Bảng tính"
head_description: "Tự động hóa hình mờ động trong Excel bằng Node.js. Áp dụng hình mờ nhất quán một cách dễ dàng trên nhiều tệp."

############################# Header ############################
title: "Hình mờ do Node.js điều khiển trong tài liệu bảng tính" 
description: "Sử dụng Node.js để triển khai hình mờ văn bản hoặc hình ảnh tùy chỉnh liền mạch vào Excel bảng tính, bảo mật dữ liệu tài chính và phân tích của bạn một cách dễ dàng."
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
       GroupDocs.Watermark for Node.js via Java là một công cụ mạnh mẽ được thiết kế cho các nhà phát triển phụ trợ muốn kết hợp hình mờ độc đáo vào Excel và bảng tính OpenOffice. API đa năng này cho phép nhúng hình mờ văn bản và hình ảnh có thể được tùy chỉnh hoàn toàn về phông chữ, kích thước, màu sắc và độ mờ. Tương thích với một loạt các định dạng bảng tính bao gồm XLS, XLSX và ODS, công cụ đảm bảo rằng hình mờ được áp dụng một cách chính xác, duy trì tính toàn vẹn và bố cục của bảng tính của bạn đồng thời cung cấp bảo vệ mạnh mẽ chống lại việc sử dụng trái phép.

############################# Steps ############################
steps:
    enable: true
    title: "Tài liệu kinh doanh an toàn: Tạo hình mờ cho Excel định dạng"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/) :** Chèn API của chúng tôi vào các ứng dụng của bạn và tạo hình mờ cho nhiều định dạng tệp được hỗ trợ.
      
      1. **Bắt đầu đánh dấu mờ:** Bắt đầu xử lý tài liệu với lạng**Watermarker** cung cấp các tính năng chính của chúng tôi. Tạo khởi tạo nó bằng cách chuyển cho hàm tạo tệp Excel được cho là được bảo mật bằng hình mờ được tạo ra.
      2. **Tạo đối tượng Hình mờ chính:** Nâng cao tài liệu của bạn bằng cách điêu khắc các đối tượng** Watermark** đặt riêng. Ngoài các trang đơn thuần, chúng tích hợp liền mạch vào các yếu tố gốc như tệp đính kèm hoặc tiêu đề, thêm các lớp bảo mật và tính chuyên nghiệp.
      3. **Tinh chỉnh thuộc tính hình mờ:** Tinh chỉnh hình mờ của bạn với độ chính xác, điều chỉnh kích thước, căn chỉnh và phối màu. Mỗi chi tiết nâng cao tính toàn vẹn của tài liệu, làm cho các tệp của bạn không thể nhầm lẫn với bạn.
      4. **Thực hiện với độ chính xác:** Sử dụng phương thức** Watermarker** để áp dụng hình mờ tùy chỉnh của bạn một cách hoàn hảo. Cho dù số ít hay nhiều, mỗi hình mờ sẽ thêm một lớp bảo vệ bổ sung. Để tăng cường bảo mật, hãy cân nhắc lưu trữ tài liệu đã xử lý của bạn ở một vị trí riêng biệt, an toàn.
   
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

        // Tạo hình mờ văn bản cho EXCEL

        // Chuyển tệp nguồn đến phiên bản Watermarker
        const watermarker = new groupdocs.watermark.Watermarker("input.xslx");
        
        // Tạo hình mờ văn bản và đặt các tùy chọn của nó
        const  watermark = new groupdocs.watermark.TextWatermark
            ("My Watermark", groupdocs.watermark.new Font("Arial", 36));

        // Lấy kết quả EXCEL
        watermarker.add(watermark);
        watermarker.save("output.xslx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Kỹ thuật tạo hình mờ nâng cao"
  description: "Khám phá các kỹ thuật tạo hình mờ tiên tiến với API mạnh mẽ của chúng tôi, được thiết kế để tích hợp liền mạch vào môi trường .NET. Hoàn hảo để thêm hình mờ tinh vi và an toàn vào một loạt các loại tài liệu đa dạng bao gồm bản trình bày, tài liệu pháp lý và sơ đồ kỹ thuật."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Hình mờ tinh vi"
  features:
    # feature loop
    - title: "Vị trí hình mờ động"
      content: "API của chúng tôi cung cấp các tùy chọn vị trí động điều chỉnh vị trí hình mờ dựa trên nội dung tài liệu. Lý tưởng cho các bố cục phức tạp trong bản trình bày và sơ đồ kỹ thuật, tính năng này đảm bảo rằng hình mờ luôn được đặt tối ưu mà không ảnh hưởng đến khả năng đọc của thông tin cơ bản."

    # feature loop
    - title: "Tăng cường bảo mật với hình mờ vô hình"
      content: "Triển khai hình mờ vô hình cung cấp sự bảo vệ mạnh mẽ mà không làm thay đổi giao diện của tài liệu của bạn. Những hình mờ này được thiết kế để chỉ được phát hiện thông qua các công cụ phần mềm cụ thể, làm cho chúng trở nên hoàn hảo để bảo vệ thông tin nhạy cảm trong các tài liệu pháp lý và tài chính."

    # feature loop
    - title: "Quy trình làm việc chấm mờ tự động"
      content: "Hợp lý hóa quy trình bảo mật tài liệu của bạn với quy trình làm việc chấm mờ tự động. Định cấu hình quy tắc dựa trên loại tài liệu, độ nhạy nội dung và mức truy cập của người dùng để tự động áp dụng hình mờ, đảm bảo các giao thức bảo mật nhất quán được duy trì trên tất cả các tài liệu."
      
  code_samples:
    # code sample loop
    - title: "Tạo hình mờ cho PDF tệp đính kèm"
      content: |
        Ví dụ này cho thấy cách tạo hình mờ trong tất cả các tệp đính kèm PDF
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Tải tài liệu PDF
            const loadOptions = new groupdocsWatermark.PdfLoadOptions();
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf", loadOptions);
            const pdfContent = watermarker.getContent(groupdocsWatermark.PdfContent.class);

            //  Tạo hình mờ văn bản
            const watermark = new groupdocsWatermark.TextWatermark('WaterMark', new groupdocsWatermark.Font('Arial', 19));
  
            //  Thêm hình mờ vào tệp đính kèm phù hợp
            for (const attachment of pdfContent.getAttachments().getInnerList().toArray()) {
                const info = attachment.getDocumentInfo();
                if (info.getFileType() !== groupdocsWatermark.FileType.Unknown && !info.isEncrypted()) {
                    const attachedWatermarker = attachment.createWatermarker();
                    attachedWatermarker.add(watermark);
                    attachment.updateContent(attachedWatermarker);
                    attachedWatermarker.close();
                }
            }

            //  Lưu đã xử lý PDF
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
    title: "Kỹ thuật Node.js để đánh dấu hình mờ Excel"
    exclude: "EXCEL"
    description: "Tăng cường bảo mật bảng tính và tính toàn vẹn dữ liệu với API Node.js của chúng tôi. Nhanh chóng thêm hình mờ tùy chỉnh vào tệp Excel và OpenOffice, bảo vệ chống lại các thay đổi trái phép."
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