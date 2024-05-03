
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:10
draft: false
lang: vi
format: Png
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Giải pháp hình mờ cho tập tin PNG"
head_description: "Áp dụng hình mờ động cho PNG hình ảnh bằng cách sử dụng Java để bảo vệ và xác thực tài sản kỹ thuật số của bạn."

############################# Header ############################
title: "Bảo mật và tùy chỉnh PNG với Java" 
description: "Sử dụng Java để nhúng hình mờ an toàn, có thể điều chỉnh trong tệp PNG, hoàn hảo cho các nhiếp ảnh gia và nhà thiết kế đang tìm cách bảo vệ các tác phẩm sáng tạo của họ."
subtitle: "GroupDocs.Watermark for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống tại Maven miễn phí"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java"
    link: "/watermark/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java cung cấp cho Java nhà phát triển một khuôn khổ tinh vi để áp dụng hình mờ cho PNG hình ảnh. API này được thiết kế để tích hợp liền mạch vào bất kỳ ứng dụng dựa trên Java nào, cho phép chèn hình mờ trong suốt hoặc mờ kết hợp hoàn hảo với hình ảnh bên dưới. Tùy chỉnh hình mờ bằng văn bản, logo hoặc biểu tượng bản quyền để tăng cường bảo mật mà không làm giảm chất lượng hình ảnh. Với các tính năng như định vị điểm ảnh hoàn hảo và kiểm soát độ mờ, GroupDocs.Watermark đảm bảo rằng hình ảnh của bạn vừa hấp dẫn về mặt thị giác vừa được bảo vệ hợp pháp. Thích hợp để sử dụng trên các trang web thương mại điện tử, danh mục đầu tư trực tuyến, v.v., và hoàn toàn tương thích với Java 8 hoặc mới hơn.

############################# Steps ############################
steps:
    enable: true
    title: "Kỹ thuật nâng cao: Thêm hình mờ vào tài liệu Png qua Java"
    content: |
      Khám phá các kỹ thuật tạo hình mờ nâng cao cho tài liệu Png với **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)**
      
      1. Bắt đầu quá trình tạo hình mờ của bạn bằng cách khởi tạo lớp **Watermarker**. Bước cơ bản này tạo tiền đề cho việc nâng cao tài liệu Png bằng hình mờ. Cung cấp tệp Png cho hàm tạo, dưới dạng đường dẫn hoặc đối tượng luồng.
      2. Tiến lên cấp độ tiếp theo bằng cách tạo các đối tượng **Watermark** phù hợp với thông số kỹ thuật của bạn. Các thực thể linh hoạt này cung cấp vị trí chính xác không chỉ trên các trang tài liệu được chỉ định mà còn trong các phần tử gốc như tệp đính kèm hoặc tiêu đề.
      3. Tinh chỉnh quy trình tạo hình mờ của bạn bằng cách tinh chỉnh các thuộc tính như kích thước, căn chỉnh, kiểu phông chữ và màu sắc. Mức độ tùy chỉnh này cho phép bạn tạo hình mờ bổ sung hoàn hảo cho tính thẩm mỹ tài liệu của bạn.
      4. Sử dụng phương pháp **Watermarker** để áp dụng hình mờ mới tạo vào tài liệu của bạn. Tận hưởng sự linh hoạt của việc thêm nhiều hình mờ theo yêu cầu của bạn. Để bảo quản tài liệu, hãy cân nhắc việc lưu chúng ở một vị trí an toàn.
   
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
        // Thêm hình mờ vào PNG

        // Chuyển tệp được đóng dấu mờ tới Watermarker
        Watermarker watermarker = new Watermarker("input.png");
        
        // Cung cấp đường dẫn đến hình ảnh có hình mờ
        ImageWatermark watermark = new ImageWatermark("watermark.png");

        // Lưu kết quả
        watermarker.add(watermark);
        watermarker.save("output.png");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Làm chủ hình mờ tài liệu"
  description: "Nâng cao khả năng quản lý tài liệu của bạn với API hình mờ tinh vi của chúng tôi, được thiết kế riêng cho .NET nhà phát triển. Công cụ này cung cấp các giải pháp toàn diện để áp dụng, tùy chỉnh và quản lý hình mờ trên nhiều định dạng tài liệu, đảm bảo cả tính thẩm mỹ và bảo mật nâng cao."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Hình mờ tài liệu nâng cao"
  features:
    # feature loop
    - title: "Xoay hình mờ linh hoạt"
      content: "Điều chỉnh hình mờ của bạn để phù hợp với bất kỳ hướng tài liệu nào với cài đặt xoay linh hoạt của chúng tôi. Cho dù tài liệu của bạn là dọc hay ngang, dễ dàng điều chỉnh góc hình mờ để duy trì giao diện nhất quán bổ sung cho bố cục tài liệu."

    # feature loop
    - title: "Kiểm soát độ trong suốt hoàn hảo"
      content: "Kiểm soát độ trong suốt của hình mờ của bạn một cách chính xác, cho phép đánh dấu tinh tế nhưng an toàn mà không làm lấn át nội dung của tài liệu. Tính năng này lý tưởng để duy trì tính thẩm mỹ ban đầu của tài liệu của bạn trong khi thêm một lớp bảo mật."

    # feature loop
    - title: "Hiệu ứng bóng tối để nhấn mạnh"
      content: "Tăng cường khả năng hiển thị hình mờ của bạn hoặc tích hợp chúng một cách tinh tế vào tài liệu của bạn với các hiệu ứng bóng có thể tùy chỉnh. Tính năng này cho phép tạo bóng mờ, lan rộng và màu sắc khác nhau, làm cho hình mờ trở nên đặc biệt hoặc kín đáo hơn theo yêu cầu."
      
  code_samples:
    # code sample loop
    - title: "MS Word hình mờ bị khóa"
      content: |
        Ví dụ này cho thấy cách khóa hình mờ trong DOCX tất cả các trang
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Tải tài liệu dưới dạng MS Word doc
        WordProcessingLoadOptions loadOptions = new WordProcessingLoadOptions();
        Watermarker watermarker = new Watermarker("source.docx", loadOptions);

        //  Tạo hình mờ
        TextWatermark watermark = new TextWatermark("Watermark text", new Font("Arial", 19));
        watermark.setForegroundColor(Color.getRed());

        //  Điều chỉnh tùy chọn gốc Word
        WordProcessingWatermarkPagesOptions options = new WordProcessingWatermarkPagesOptions();
        options.setLocked(true);
        options.setLockType(WordProcessingLockType.AllowOnlyFormFields);

        //  Thêm hình mờ vào trang tài liệu kết quả
        watermarker.add(textWatermark, options);
        watermarker.save("result.docx");
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
    title: "Tăng cường bảo mật hình ảnh PNG với Java"
    exclude: "PNG"
    description: "Nhúng hình mờ mạnh mẽ vào PNG tệp bằng Java. Tính năng này rất quan trọng để bảo vệ nội dung trực quan khỏi việc sử dụng trái phép trong khi vẫn duy trì hình ảnh rõ nét."
    items: 
        # format loop 1
        - name: "Hình mờ PDF"
          format: "PDF"
          link: "/watermark/java/add//pdf/"
          description: "Định dạng tài liệu Adobe Portable"

        # format loop 2
        - name: "Hình mờ Word"
          format: "WORD"
          link: "/watermark/java/add//word/"
          description: "MS Word và tài liệu Open Office"
          
        # format loop 3
        - name: "Hình mờ Excel"
          format: "EXCEL"
          link: "/watermark/java/add//excel/"
          description: "MS Excel và bảng tính Open Office"

        # format loop 4
        - name: "Hình ảnh hình mờ"
          format: "IMAGE"
          link: "/watermark/java/add//image/"
          description: "Định dạng hình ảnh phổ biến"

        # format loop 5
        - name: "Ảnh hình mờ"
          format: "PHOTO"
          link: "/watermark/java/add//photo/"
          description: "Định dạng ảnh"

        # format loop 6
        - name: "Hình mờ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/add//powerpoint/"
          description: "MS PowerPoint và các bài thuyết trình Open Office"

        # format loop 7
        - name: "Hình mờ DOCX"
          format: "DOCX"
          link: "/watermark/java/add//docx/"
          description: "Microsoft Word Tài liệu XML mở"
          
        # format loop 8
        - name: "Hình mờ PPTX"
          format: "PPTX"
          link: "/watermark/java/add//pptx/"
          description: "PowerPoint Bản trình bày XML mở"
          
        # format loop 9
        - name: "Hình mờ XLSX"
          format: "XLSX"
          link: "/watermark/java/add//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 10
        - name: "Hình mờ JPEG"
          format: "JPEG"
          link: "/watermark/java/add//jpeg/"
          description: "JPEG Hình ảnh"

        # format loop 11
        - name: "Hình mờ PNG"
          format: "PNG"
          link: "/watermark/java/add//png/"
          description: "Portable Đồ họa mạng"

        # format loop 12
        - name: "Hình mờ TIFF"
          format: "TIFF"
          link: "/watermark/java/add//tiff/"
          description: "Nhãn định dạng tệp hình ảnh"

        # format loop 13
        - name: "Hình mờ WEBP"
          format: "WEBP"
          link: "/watermark/java/add//webp/"
          description: "Hình ảnh WEB"

        # format loop 14
        - name: "Hình mờ DOC"
          format: "DOC"
          link: "/watermark/java/add//doc/"
          description: "Tài liệu Microsoft Word 97 - 2007"

        # format loop 15
        - name: "Hình mờ XLS"
          format: "XLS"
          link: "/watermark/java/add//xls/"
          description: "Microsoft Excel Sổ làm việc 97-2003"

        # format loop 16
        - name: "Hình mờ PPT"
          format: "PPT"
          link: "/watermark/java/add//ppt/"
          description: "PowerPoint Bài thuyết trình 97-2003"

        # format loop 17
        - name: "Hình mờ RTF"
          format: "RTF"
          link: "/watermark/java/add//rtf/"
          description: "Định dạng văn bản phong phú"

---