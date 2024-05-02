
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:26:57
draft: false
lang: vi
format: Word
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Soạn hình mờ phù hợp cho Word với Java"
head_description: "Tích hợp hình mờ tùy chỉnh trong Word tài liệu bằng cách sử dụng Java. Tăng cường bảo mật và thêm nét chuyên nghiệp."

############################# Header ############################
title: "Tạo hình mờ tùy chỉnh trong Word Tài liệu" 
description: "Bảo mật tệp Word của bạn với Java bằng cách nhúng hình mờ văn bản hoặc hình ảnh phù hợp. Tài nguyên này lý tưởng cho những người cần tăng cường bảo mật tài liệu và sự hấp dẫn trực quan với nỗ lực tối thiểu."
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
       GroupDocs.Watermark for Java cho phép tạo hình mờ chính xác và linh hoạt trong Word tài liệu. Công cụ này cho phép Java nhà phát triển thêm hình mờ tùy chỉnh có thể bao gồm văn bản, hình ảnh hoặc logo, phù hợp với nhu cầu xây dựng thương hiệu cụ thể của bạn. Nó hỗ trợ tất cả các định dạng tài liệu Word chính và cung cấp các tính năng toàn diện để chỉnh sửa và xóa hình mờ, cũng như tìm kiếm thông qua các tài liệu để xác minh tính toàn vẹn của hình mờ. Tương thích với tất cả các hệ điều hành được hỗ trợ Java, API này hoàn hảo cho các doanh nghiệp muốn củng cố các giao thức bảo mật tài liệu của họ.

############################# Steps ############################
steps:
    enable: true
    title: "Thêm hình mờ vào tài liệu Word qua Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** giúp các nhà phát triển Java dễ dàng thêm hình mờ các loại khác nhau vào các định dạng tệp doanh nghiệp phổ biến. Thêm thư viện của chúng tôi vào ứng dụng và tài liệu hình mờ của bạn trong một vài bước đơn giản như được liệt kê bên dưới.
      
      1. **Watermarker**. Bạn cần khởi tạo nó trước khi xử lý tài liệu. Đừng quên truyền tệp Word cho hàm tạo dưới dạng đường dẫn hoặc đối tượng luồng.
      2. **Watermark** thuộc loại mong muốn. Nó có thể được đặt không chỉ trên một trang tài liệu cụ thể mà còn trong các phần tài liệu gốc như tệp đính kèm hoặc tiêu đề.
      3. Đặt các thuộc tính hình mờ như chiều cao và chiều rộng, căn chỉnh trang (trên cùng, bên trái, trung tâm, v.v.), họ phông chữ và màu sắc, và nhiều thứ khác.
      4. **Watermarker** để thêm hình mờ mới. Bạn có thể thêm nhiều hình mờ như bạn cần. Nên lưu tài liệu đã xử lý vào một vị trí khác.
   
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

        // Thêm hình mờ văn bản vào WORD

        // Chuyển tệp để được đánh dấu vào Watermarker
        Watermarker watermarker = new Watermarker("input.docx");
        
        // Tạo hình mờ văn bản và thiết lập thuộc tính
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        watermark.setForegroundColor(Color.getRed());

        // Lưu tệp có hình mờ
        watermarker.add(watermark);
        watermarker.save("output.docx");
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Nâng cao hình mờ của bạn một cách dễ dàng"
  description: "Khai thác sức mạnh của GroupDocs.Watermark để tạo, soạn và thêm hình mờ trên nhiều định dạng tài liệu. API này không chỉ tăng cường bảo mật tài liệu mà còn bảo vệ tài sản trí tuệ của bạn bằng cách nhúng hình mờ có thể tùy chỉnh vừa linh hoạt vừa mạnh mẽ."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Thêm hình mờ"
  features:
    # feature loop
    - title: "Tùy chọn hình mờ đa năng."
      content: "Khám phá một loạt các tùy chọn hình mờ với GroupDocs.Watermark. Từ việc điều chỉnh độ mờ đục và xoay chuyển đến tỷ lệ kích thước theo tỷ lệ, API của chúng tôi cho phép bạn tùy chỉnh hình mờ chính xác theo nhu cầu của mình, đảm bảo rằng chúng kết hợp liền mạch với tài liệu của bạn trong khi vẫn duy trì tính toàn vẹn của nội dung."

    # feature loop
    - title: "Kiểu dáng hình mờ nâng cao."
      content: "GroupDocs.Watermark cho phép bạn tạo kiểu hình mờ của mình với nhiều phông chữ, màu sắc và bóng khác nhau, làm cho chúng trở nên đặc biệt và khó xóa hơn. Nâng cao tính thẩm mỹ của các tài liệu và hình ảnh được bảo vệ của bạn với hình mờ thời trang phản ánh bản sắc và tính chuyên nghiệp của thương hiệu của bạn."

    # feature loop
    - title: "Ốp lát và định vị hình mờ"
      content: "Với GroupDocs.Watermark, triển khai các hiệu ứng ốp lát để bao phủ toàn bộ tài liệu của bạn, đảm bảo bảo vệ hoàn toàn. Đặt hình mờ chính xác ở vị trí bạn cần — vị trí trung tâm, góc hoặc tùy chỉnh. Các tùy chọn định vị linh hoạt của chúng tôi giúp bảo vệ tài liệu của bạn khỏi việc sử dụng và sao chép trái phép."
      
  code_samples:
    # code sample loop
    - title: "PDF hình mờ chú thích"
      content: |
        Ví dụ này cho thấy cách thêm chú thích hình mờ vào tài liệu PDF
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Tải tài liệu dưới dạng PDF
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Tạo hình mờ dựa trên chú thích PDF
        PdfAnnotationWatermarkOptions options = new PdfAnnotationWatermarkOptions();
        TextWatermark textWatermark = new TextWatermark("Annotation watermark", new Font("Arial", 8));

        //  Thiết lập tùy chọn hình mờ
        textWatermark.setHorizontalAlignment(HorizontalAlignment.Left);
        textWatermark.setVerticalAlignment(VerticalAlignment.Top);

        //  Thêm hình mờ văn bản vào tài liệu kết quả
        watermarker.add(textWatermark, options);
        watermarker.save("result.pdf");

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
    title: "Cá nhân hóa tệp MS Word của bạn bằng cách tạo hình mờ Java."
    exclude: "WORD"
    description: "GroupDocs.Watermark for Java cho phép các nhà phát triển dễ dàng chèn hình mờ văn bản hoặc hình ảnh tùy chỉnh vào tài liệu Word. Những cải tiến này không chỉ tăng cường bảo mật tài liệu mà còn làm phong phú thêm giao tiếp kinh doanh với một nét chuyên nghiệp."
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