
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:18
draft: false
lang: vi
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Khám phá Excel Bảng tính Hình mờ Tìm kiếm"
head_description: "Khám phá cách GroupDocs.Watermark for Java cho phép bạn dễ dàng tìm kiếm, tìm và quản lý hình mờ ở các định dạng tài liệu khác nhau."

############################# Header ############################
title: "Ra mắt khả năng tìm kiếm hình mờ của bảng tính Excel" 
description: "Tìm hiểu sức mạnh của GroupDocs.Watermark for Java để tìm kiếm, chỉnh sửa và thao tác hình mờ một cách dễ dàng."
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
    title: "Thông tin cơ sở GroupDocs.Watermark for Java"
    link: "/watermark/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java là một giải pháp toàn diện để quản lý Excel hình mờ bằng cách sử dụng Java. Với công cụ này, các nhà phát triển có thể dễ dàng thực hiện các thao tác như tạo, chỉnh sửa, tìm kiếm và xóa hình mờ khỏi tài liệu ở các định dạng tệp phổ biến. Nó hỗ trợ làm việc với cả hình mờ văn bản và hình ảnh trong nhiều tài liệu, bao gồm PDF, Microsoft Word, Excel, PowerPoint, Visio, email và định dạng hình ảnh. GroupDocs.Watermark for Java hỗ trợ tất cả các hệ điều hành chính và Java phiên bản.

############################# Steps ############################
steps:
    enable: true
    title: "Tìm kiếm hình mờ trong tệp Excel bằng cách sử dụng Java"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/)** giúp bạn dễ dàng tìm kiếm các hình mờ đã được đặt trong tài liệu kinh doanh. Tải xuống gói của chúng tôi và đưa gói đó vào ứng dụng Java của bạn để tận dụng các lợi ích của gói đó.
      
      1. Để sử dụng các tính năng thư viện của chúng tôi, bạn cần tải tệp Excel vào phiên bản lớp **Watermarker**. Có thể chỉ cung cấp đường dẫn tệp, luồng tệp hoặc luồng byte.
      2. Để thu hẹp danh sách các hình mờ có thể sử dụng đối tượng **SearchCriteria**. Cung cấp hình ảnh làm ví dụ để có được hình mờ hình ảnh tương tự. Nếu bạn muốn tìm kiếm hình mờ văn bản, hãy cung cấp văn bản, phông chữ, màu sắc và các tùy chọn khác.
      3. Để lấy hình mờ được đặt trong tài liệu, hãy sử dụng phương thức **Search** của đối tượng **Watermarker**. Bạn sẽ được cung cấp bộ sưu tập các đối tượng có thể được xử lý dưới dạng hình mờ.
      4. Cuối cùng, bạn có thể tự do thực hiện bất cứ điều gì bạn muốn với kết quả tìm kiếm. Hoàn toàn có thể xóa các hình mờ được tìm thấy hoặc chỉnh sửa thuộc tính của chúng. Thay đổi kích thước hoặc văn bản, ví dụ.
   
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

        // Tìm kiếm hình mờ văn bản trong tài liệu EXCEL

        // Lấy phiên bản Watermarker cho tài liệu EXCEL
        Watermarker watermarker = new Watermarker("input.xslx");

        // Tìm kiếm hình mờ theo tiêu chí
        ImageSearchCriteria imageSearchCriteria = new ImageDctHashSearchCriteria("watermark.jpeg");
        imageSearchCriteria.setMaxDifference(0.9);
        PossibleWatermarkCollection possibleWatermarks = watermarker.search(imageSearchCriteria);

        // Xử lý hình mờ
        System.out.println("Found " + possibleWatermarks.getCount() + " possible watermark(s).");
        
        ```   
        
############################# More features ############################
more_features:
  enable: true
  title: "Khai thác Java để tìm kiếm hình mờ nâng cao với GroupDocs.Watermark"
  description: "Sử dụng GroupDocs.Watermark Java API để thực hiện các tìm kiếm tinh vi cho hình mờ trong tài liệu trên các định dạng khác nhau trong Java."
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "Tìm kiếm hình mờ nâng cao"
  features:
    # feature loop
    - title: "Java - Kỹ thuật tìm kiếm hình mờ nâng cao"
      content: "Hỗ trợ Java ứng dụng của bạn với các kỹ thuật tìm kiếm nâng cao bằng cách sử dụng GroupDocs.Watermark. API của chúng tôi cho phép tìm kiếm sâu các hình mờ nhúng trên các loại tài liệu khác nhau, mang lại độ chính xác và hiệu quả."

    # feature loop
    - title: "Xác định hình mờ với truy vấn tùy chỉnh Java"
      content: "Tùy chỉnh truy vấn Java của bạn để phát hiện hình mờ hiệu quả hơn. Sử dụng GroupDocs.Watermark để sắp xếp và lọc hình mờ theo các thuộc tính như độ trong suốt, phương pháp nhúng và nội dung văn bản hoặc hình ảnh."

    # feature loop
    - title: "Quản lý hiệu quả các hình mờ tài liệu"
      content: "Hợp lý hóa việc quản lý hình mờ trong Java ứng dụng của bạn. Với GroupDocs.Watermark, nhanh chóng tìm, xem xét và phân tích hình mờ để đảm bảo tính toàn vẹn của tài liệu và tuân thủ các nguyên tắc xây dựng thương hiệu."
      
  code_samples:
    # code sample loop
    - title: "Java Ví dụ về mã: Tìm kiếm hình mờ thông minh"
      content: |
        Tìm hiểu cách triển khai tìm kiếm hình mờ thông minh bằng cách sử dụng Java với GroupDocs.Watermark, thể hiện khả năng xử lý các hoạt động tìm kiếm phức tạp và quản lý kết quả của API.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Thiết lập môi trường Java và tải tài liệu từ nhiều nguồn khác nhau
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Xác định các tham số tìm kiếm nâng cao để xác định vị trí các loại hình mờ cụ thể
        TextSearchCriteria textSearchCriteria = new TextSearchCriteria("Company Name");

        //  Thực hiện tìm kiếm và xử lý các hình mờ tìm thấy để xem xét chi tiết
        RotateAngleSearchCriteria rotateAngleSearchCriteria = new RotateAngleSearchCriteria(30, 60);
        SearchCriteria combinedSearchCriteria = imageSearchCriteria.or(textSearchCriteria)
                                                                   .and(rotateAngleSearchCriteria);

        //  Lưu hoặc cập nhật tài liệu dựa trên kết quả tìm kiếm hình mờ
        PossibleWatermarkCollection possibleWatermarks = watermarker.search(combinedSearchCriteria);
        System.out.println("Found " + possibleWatermarks.getCount() + " possible watermark(s).");
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
    title: "Mở khóa sức mạnh của Tìm kiếm Hình mờ"
    exclude: "EXCEL"
    description: "Trao quyền cho bản thân để tìm và quản lý hình mờ ở các định dạng tệp được hỗ trợ khác nhau với GroupDocs.Watermark for Java."
    items: 
        # format loop 1
        - name: "Hình mờ PDF"
          format: "PDF"
          link: "/watermark/java/search//pdf/"
          description: "Định dạng tài liệu Adobe Portable"

        # format loop 2
        - name: "Hình mờ Word"
          format: "WORD"
          link: "/watermark/java/search//word/"
          description: "MS Word và tài liệu Open Office"
          
        # format loop 3
        - name: "Hình mờ Excel"
          format: "EXCEL"
          link: "/watermark/java/search//excel/"
          description: "MS Excel và bảng tính Open Office"

        # format loop 4
        - name: "Hình mờ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/search//powerpoint/"
          description: "MS PowerPoint và các bài thuyết trình Open Office"

        # format loop 5
        - name: "Hình mờ DOCX"
          format: "DOCX"
          link: "/watermark/java/search//docx/"
          description: "Microsoft Word Tài liệu XML mở"
          
        # format loop 6
        - name: "Hình mờ PPTX"
          format: "PPTX"
          link: "/watermark/java/search//pptx/"
          description: "PowerPoint Bản trình bày XML mở"
          
        # format loop 7
        - name: "Hình mờ XLSX"
          format: "XLSX"
          link: "/watermark/java/search//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Hình mờ DOC"
          format: "DOC"
          link: "/watermark/java/search//doc/"
          description: "Tài liệu Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Hình mờ XLS"
          format: "XLS"
          link: "/watermark/java/search//xls/"
          description: "Microsoft Excel Sổ làm việc 97-2003"

        # format loop 10
        - name: "Hình mờ PPT"
          format: "PPT"
          link: "/watermark/java/search//ppt/"
          description: "PowerPoint Bài thuyết trình 97-2003"

        # format loop 11
        - name: "Hình mờ RTF"
          format: "RTF"
          link: "/watermark/java/search//rtf/"
          description: "Định dạng văn bản phong phú"

---