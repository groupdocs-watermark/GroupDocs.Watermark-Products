
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:35
draft: false
lang: vi
format: Xlsx
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Điều chỉnh và quản lý hình mờ XLSX - GroupDocs.Watermark"
head_description: "Hợp lý hóa quy trình quản lý hình mờ của bạn với GroupDocs.Watermark. Đơn giản hóa việc bảo vệ tài liệu và xây dựng thương hiệu."

############################# Header ############################
title: "Streamline XLSX Quản lý hình mờ: Kiểm soát đơn giản" 
description: "Đơn giản hóa quy trình quản lý hình mờ của bạn với giải pháp hợp lý của chúng tôi. Tập trung vào nội dung của bạn một cách dễ dàng."
subtitle: "GroupDocs.Watermark for Java Thư viện" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống tại Maven miễn phí"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java Thư viện"
    link: "/watermark/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Điều chỉnh tùy chọn hình mương**: Di chuyển hình mờ trên trang bằng giải pháp chính xác của chúng tôi. GroupDocs.Watermark cung cấp nhiều tùy chọn để điều chỉnh hình mờ và đảm bảo bảo mật tài liệu.

############################# Steps ############################
steps:
    enable: true
    title: "Điều chỉnh hình mờ tài liệu Xlsx bằng cách sử dụng Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** cho phép các nhà phát triển Java dễ dàng điều chỉnh hình mờ trong nhiều tài liệu bằng ứng dụng của họ. Đây là hướng dẫn nhanh:
      
      1. Trước tiên, bạn cần truyền tệp Xlsx làm tham số của hàm tạo lớp **Watermarker**. Cung cấp luồng byte hoặc tệp hoặc đường dẫn đĩa cục bộ.
      2. Thứ hai, xác định vị trí các hình mờ cần điều chỉnh. Sử dụng **SearchCriteria** để xác định hình mờ có thuộc tính cụ thể đã được thêm trước đó vào tài liệu.
      3. Sau khi tìm kiếm, bạn sẽ nhận được danh sách các hình mờ có liên quan. Sau đó, bạn có thể điều chỉnh các thuộc tính của chúng, bao gồm kích thước, căn chỉnh trang, văn bản, màu sắc, nội dung hình ảnh, v.v. Điều này cung cấp mức độ tùy chỉnh cao cho dữ liệu của bạn.
      4. Sau khi bạn điều chỉnh xong hình mờ, hãy lưu tài liệu đã cập nhật. Bạn có thể sử dụng đường dẫn tệp cục bộ hoặc luồng để lưu trữ kết quả.
   
    code:
      platform: "net"
      copy_title: "Sao chép"
      install:
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-watermark</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "bấm để sao chép"
        copy_done: "sao chép"
      links:
        #  loop
        - title: "Thêm ví dụ"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
        #  loop
        - title: "Tài liệu"
          link: "https://docs.groupdocs.com/watermark/java/"
          
      content: |
        ```java {style=abap}
        // Điều chỉnh hình mờ hình ảnh XLSX

        // Khởi tạo Watermarker bằng XLSX
        Watermarker watermarker = new Watermarker("input.xlsx");
        
        // Khởi tạo SearchCriteria để khớp với một hình ảnh cụ thể
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);

        for (PossibleWatermark watermark : watermarks)
        {
            // Thay thế hình ảnh được tìm thấy
            watermark.setImageData(imageData);
        }

        // Lưu tập tin đã điều chỉnh
        watermarker.save("output.xlsx");
        
        ```
        
############################# More features ############################
more_features:
  enable: true
  title: "Quản lý hình mờ nâng cao XLSX cho Java Ứng dụng"
  description: "API GroupDocs.Watermark cho phép các nhà phát triển tích hợp liền mạch chức năng hình mờ vào ứng dụng Java của họ. Nó hỗ trợ thêm, chỉnh sửa, xóa và tìm kiếm hình mờ trên một loạt các định dạng tài liệu."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Điều chỉnh hình mờ"
  features:
    # feature loop
    - title: "Tích hợp hình mờ dễ dàng"
      content: "GroupDocs.Watermark đơn giản hóa quá trình thêm hình mờ đa dạng vào các tài liệu và tệp kinh doanh khác nhau trong Java ứng dụng. Các nhà phát triển không chỉ có thể áp dụng hình mờ mà còn cập nhật hoặc xóa các hình mờ hiện có theo chương trình."

    # feature loop
    - title: "Tùy chỉnh hình mờ dạng hạt"
      content: "API cung cấp các tùy chọn tùy chỉnh mở rộng cho hình mờ. Các nhà phát triển có thể dễ dàng điều chỉnh kích thước, xoay, màu sắc, phông chữ, kiểu dáng và các thuộc tính khác để đạt được hiệu ứng hình ảnh mong muốn."

    # feature loop
    - title: "Tận dụng các tính năng tài liệu gốc XLSX"
      content: "Tùy thuộc vào định dạng tài liệu mục tiêu, các nhà phát triển có thể sử dụng các chức năng gốc để đặt hình mờ. Các chức năng này có thể bao gồm nền trang tài liệu, chú thích, tiêu đề hoặc các đối tượng khác làm vùng chứa hình mờ."
      
  code_samples:
    # code sample loop
    - title: "Điều chỉnh hình mờ hình ảnh trong Bảng tính"
      content: |
        Ví dụ này cho thấy cách điều chỉnh hình ảnh của các hình dạng cụ thể trong Bảng tính Excel.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Tải tài liệu dưới dạng Bảng tính
        SpreadsheetLoadOptions loadOptions = new SpreadsheetLoadOptions();
        Watermarker watermarker = new Watermarker("source.xlsx", loadOptions);

        //  Nhận byte hình mờ mới
        File file = new File("new_watermark.png");
        byte[] imageBytes = new byte[(int) file.length()];
        FileInputStream inputStream = new FileInputStream(file);
        inputStream.read(imageBytes);
        inputStream.close();

        //  Điều chỉnh nội dung của hình mờ cụ thể
        for (SpreadsheetShape shape : content.getWorksheets().get_Item(0).getShapes())
        {
            if (shape.getImage() != null)
            {
                shape.setImage(new SpreadsheetWatermarkableImage(imageBytes));
            }
        }

        //  Lưu tài liệu kết quả
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
    - title: "Maven tải về"
      link: "https://releases.groupdocs.com/watermark/java/"
      color: "red"
        #  loop
    - title: "Cấp phép"
      link: "https://purchase.groupdocs.com/pricing/watermark/java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Sử dụng GroupDocs.Watermark for Java để chỉnh sửa hình mờ trong các định dạng tệp khác"
    exclude: "XLSX"
    description: "Đơn giản hóa quy trình quản lý hình mờ của bạn trên các định dạng tài liệu khác nhau. Tập trung vào nội dung của bạn một cách dễ dàng trong khi đảm bảo bảo vệ và xây dựng thương hiệu."
    items: 
        # format loop 1
        - name: "Hình mờ PDF"
          format: "PDF"
          link: "/watermark/java/adjust//pdf/"
          description: "Định dạng tài liệu Adobe Portable"

        # format loop 2
        - name: "Hình mờ Word"
          format: "WORD"
          link: "/watermark/java/adjust//word/"
          description: "MS Word và tài liệu Open Office"
          
        # format loop 3
        - name: "Hình mờ Excel"
          format: "EXCEL"
          link: "/watermark/java/adjust//excel/"
          description: "MS Excel và bảng tính Open Office"

        # format loop 4
        - name: "Hình mờ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/adjust//powerpoint/"
          description: "MS PowerPoint và các bài thuyết trình Open Office"

        # format loop 5
        - name: "Hình mờ DOCX"
          format: "DOCX"
          link: "/watermark/java/adjust//docx/"
          description: "Microsoft Word Tài liệu XML mở"
          
        # format loop 6
        - name: "Hình mờ PPTX"
          format: "PPTX"
          link: "/watermark/java/adjust//pptx/"
          description: "PowerPoint Bản trình bày XML mở"
          
        # format loop 7
        - name: "Hình mờ XLSX"
          format: "XLSX"
          link: "/watermark/java/adjust//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Hình mờ DOC"
          format: "DOC"
          link: "/watermark/java/adjust//doc/"
          description: "Tài liệu Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Hình mờ XLS"
          format: "XLS"
          link: "/watermark/java/adjust//xls/"
          description: "Microsoft Excel Sổ làm việc 97-2003"

        # format loop 10
        - name: "Hình mờ PPT"
          format: "PPT"
          link: "/watermark/java/adjust//ppt/"
          description: "PowerPoint Bài thuyết trình 97-2003"

        # format loop 11
        - name: "Hình mờ RTF"
          format: "RTF"
          link: "/watermark/java/adjust//rtf/"
          description: "Định dạng văn bản phong phú"

---