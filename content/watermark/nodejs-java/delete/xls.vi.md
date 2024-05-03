
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:18
draft: false
lang: vi
format: Xls
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Loại bỏ hình mờ chính xác trong XLS Bảng tính"
head_description: "GroupDocs.Watermark cung cấp khả năng kiểm soát chi tiết đối với việc xóa các hình mờ cụ thể."

############################# Header ############################
title: "Hình mờ XLS dành riêng cho mục tiêu" 
description: "Chọn lọc loại bỏ hình mờ không mong muốn trong khi vẫn giữ các hình mờ mong muốn với GroupDocs.Watermark."
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
       GroupDocs.Watermark trao quyền cho các nhà phát triển khả năng nhắm mục tiêu và xóa các hình mờ cụ thể trong tài liệu. Điều khiển chi tiết này đảm bảo chỉnh sửa tài liệu chính xác, cho phép bạn loại bỏ các hình mờ lỗi thời hoặc không liên quan trong khi vẫn duy trì thông tin quan trọng. GroupDocs.Watermark tích hợp liền mạch với môi trường .NET, hợp lý hóa việc xóa hình mờ cho các định dạng tệp khác nhau.

############################# Steps ############################
steps:
    enable: true
    title: "Xóa hình mờ khỏi Xls một cách dễ dàng bởi Node.js via Java"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/nodejs-java/)** hợp lý hóa quy trình xóa hình mờ khỏi tài liệu kinh doanh. Nâng cao ứng dụng Node.js via Java của bạn bằng cách tích hợp liền mạch thư viện của chúng tôi và làm theo các bước đơn giản sau:
      
      1. Bắt đầu quá trình bằng cách khởi tạo lớp lõi, **Watermarker**, bằng tài liệu Xls. API linh hoạt của chúng tôi xử lý liền mạch các tài liệu, cho dù được cung cấp dưới dạng luồng hay đường dẫn cục bộ.
      2. Tận dụng **SearchCriteria** để xác định chính xác hình mờ cần xử lý. Sử dụng nhiều thông số khác nhau như hình ảnh, văn bản hoặc tính năng định dạng để tinh chỉnh tìm kiếm của bạn. Tiêu chí của bạn càng chi tiết thì kết quả của bạn càng chính xác.
      3. Thực hiện quá trình xóa trên danh sách hình mờ tài liệu được truy xuất thông qua tìm kiếm của bạn. Dễ dàng xóa chúng khỏi tài liệu.
      4. Sau khi xóa thành công hình mờ, hãy lưu tài liệu kết quả một cách an toàn dưới dạng tệp cục bộ hoặc luồng byte, duy trì tính toàn vẹn của nó.
   
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

        // Xóa hình mờ trong tài liệu XLS

        // Lấy đường dẫn Watermarker truyền vào XLS làm đối số
        const watermarker = new groupdocs.watermark.Watermarker("input.xls");
        
        // Xóa hình mờ hình ảnh theo tiêu chí tìm kiếm
        const searchCriteria = 
            new groupdocs.watermark.ImageDctHashSearchCriteria("logo.png");
        const watermarks = watermarker.search(searchCriteria);
        watermarks.clear();

        // Lưu tập tin đã xử lý
        watermarker.save("output.xls");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Node.js via Java API để xóa hình mờ | GroupDocs.Watermark"
  description: "Tích hợp API Node.js via Java của chúng tôi để dễ dàng xóa hình mờ khỏi tài liệu, nâng cao độ rõ ràng và thẩm mỹ của tài liệu. Được thiết kế riêng cho môi trường Node.js via Java, API này hoàn hảo cho các ứng dụng cần xử lý và trình bày các tài liệu sạch không có hình mờ."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "Xóa hình mờ"
  features:
    # feature loop
    - title: "Loại bỏ hình mờ được sắp xếp hợp lý cho Node.js via Java"
      content: "API của chúng tôi cung cấp các công cụ xóa hình mờ hợp lý được thiết kế đặc biệt cho Node.js via Java ứng dụng, cho phép các nhà phát triển nâng cao khả năng đọc tài liệu và giao diện chuyên nghiệp mà không cần mã hóa phức tạp."

    # feature loop
    - title: "Node.js via Java Dọn dẹp hình mờ hàng loạt"
      content: "Tận dụng khả năng xóa hình mờ khỏi nhiều tài liệu cùng một lúc với tính năng xử lý hàng loạt của chúng tôi. Điều này đặc biệt hữu ích cho các ứng dụng cần xử lý các luồng tài liệu lớn một cách nhanh chóng và hiệu quả."

    # feature loop
    - title: "Chỉnh sửa hình mờ linh hoạt thông qua Node.js via Java"
      content: "Điều chỉnh, sửa đổi hoặc xóa hoàn toàn hình mờ bằng các công cụ chỉnh sửa linh hoạt của chúng tôi. Tính năng này cho phép Node.js via Java nhà phát triển điều chỉnh xử lý tài liệu theo nhu cầu kinh doanh cụ thể hoặc yêu cầu của khách hàng, đảm bảo kết quả tối ưu."
      
  code_samples:
    # code sample loop
    - title: "Xóa hình mờ tiêu đề bảng tính"
      content: |
        Ví dụ này cho thấy cách xóa hình mờ đã được đưa vào tiêu đề XLSX
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Tải sổ làm việc Bảng tính
            const loadOptions = new groupdocsWatermark.SpreadsheetLoadOptions();
            const watermarker = new groupdocsWatermark.Watermarker("source.xlsx", loadOptions);

            //  Nhận danh sách các phần tiêu đề
            const content = watermarker.getContent(groupdocsWatermark.SpreadsheetContent.class);
            const sections = content.getWorksheets().get_Item(0).getHeadersFooters()
                .getByOfficeHeaderFooterType(groupdocsWatermark.OfficeHeaderFooterType.HeaderPrimary).getSections();
  
            //  Xóa hình mờ khỏi tiêu đề
            for (const section of sections.getInnerList().toArray()) {
                section.setScript(null);
                section.setImage(null);
            }

            //  Lưu sổ làm việc đã xóa
            watermarker.save("result.xlsx");
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
    title: "Xóa chính xác trên các định dạng"
    exclude: "XLS"
    description: "Nhắm mục tiêu hình mờ cụ thể trong các loại tài liệu khác nhau với GroupDocs.Watermark."
    items: 
        # format loop 1
        - name: "Hình mờ PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/delete//pdf/"
          description: "Định dạng tài liệu Adobe Portable"

        # format loop 2
        - name: "Hình mờ Word"
          format: "WORD"
          link: "/watermark/nodejs-java/delete//word/"
          description: "MS Word và tài liệu Open Office"
          
        # format loop 3
        - name: "Hình mờ Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/delete//excel/"
          description: "MS Excel và bảng tính Open Office"

        # format loop 4
        - name: "Hình mờ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/delete//powerpoint/"
          description: "MS PowerPoint và các bài thuyết trình Open Office"

        # format loop 5
        - name: "Hình mờ DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/delete//docx/"
          description: "Microsoft Word Tài liệu XML mở"
          
        # format loop 6
        - name: "Hình mờ PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/delete//pptx/"
          description: "PowerPoint Bản trình bày XML mở"
          
        # format loop 7
        - name: "Hình mờ XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/delete//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Hình mờ DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/delete//doc/"
          description: "Tài liệu Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Hình mờ XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/delete//xls/"
          description: "Microsoft Excel Sổ làm việc 97-2003"

        # format loop 10
        - name: "Hình mờ PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/delete//ppt/"
          description: "PowerPoint Bài thuyết trình 97-2003"

        # format loop 11
        - name: "Hình mờ RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/delete//rtf/"
          description: "Định dạng văn bản phong phú"

---