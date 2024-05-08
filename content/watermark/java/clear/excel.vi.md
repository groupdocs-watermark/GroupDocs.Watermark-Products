
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
head_title: "Xóa hình mờ khỏi Excel bằng Java API"
head_description: "Dễ dàng xóa, xóa hoặc chỉnh sửa hình mờ khỏi tệp Excel bằng API GroupDocs.Watermark for Java. Tăng cường tính toàn vẹn của tài liệu và trình bày."

############################# Header ############################
title: "Java Excel Quản lý hình mờ" 
description: "Sử dụng GroupDocs.Watermark for Java để xóa hoặc chỉnh sửa hình mờ trong Excel bảng tính một cách hiệu quả và chính xác."
subtitle: "GroupDocs.Watermark for Java CÁ" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống miễn phí tại Maven"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java thư viện"
    link: "/watermark/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       Với thư viện GroupDocs.Watermark for Java, các nhà phát triển có thể quản lý hình mờ trong Excel tệp một cách liền mạch. Công cụ này hỗ trợ các thao tác như xóa, điều chỉnh và tìm kiếm cả hình mờ văn bản và hình ảnh. Lý tưởng cho các ứng dụng yêu cầu trình bày dữ liệu trực quan rõ ràng mà không ảnh hưởng đến bảo mật hoặc bố cục của tài liệu.

############################# Steps ############################
steps:
    enable: true
    title: "Xóa hình mờ trong tài liệu Excel bằng cách sử dụng Java"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/)** giúp dễ dàng xóa các hình mờ đã thêm trước đó trong tài liệu kinh doanh. Trao quyền cho ứng dụng Java của bạn bằng cách cài đặt thư viện của chúng tôi và thực hiện việc đó trong một vài bước đơn giản:
      
      1. Trước hết, khởi tạo lớp chính có tên **Watermarker** bằng tài liệu Excel. API của chúng tôi hỗ trợ chuyển tài liệu để xử lý dưới dạng luồng hoặc đường dẫn cục bộ.
      2. Sử dụng **SearchCriteria** để giới hạn tập hợp hình mờ cần xử lý. Có thể sử dụng hình ảnh làm tham số tìm kiếm cũng như các tính năng văn bản hoặc định dạng. Sau đó, bạn cung cấp các thông số tìm kiếm cụ thể hơn thì bạn sẽ nhận được kết quả chính xác hơn.
      3. Xử lý danh sách các hình mờ tài liệu mà bạn đã thu được dưới dạng kết quả tìm kiếm. Xóa tài liệu.
      4. Sau khi xóa kết quả lưu tài liệu dưới dạng tệp cục bộ hoặc luồng byte.
   
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

        // Xóa hình mờ văn bản trong tài liệu Excel

        // Khởi tạo Watermarker bằng tài liệu Excel
        Watermarker watermarker = new Watermarker("input.xslx");
        
        // Xóa hình mờ cụ thể
        PossibleWatermarkCollection possibleWatermarks = watermarker.search();
        possibleWatermarks.removeAt(0);

        // Lưu tập tin đã xử lý
        watermarker.save("output.xslx");
        
        ```    
        
############################# More features ############################
more_features:
  enable: true
  title: "Loại bỏ hình mờ hiệu quả thông qua Java API"
  description: "Khám phá khả năng mạnh mẽ của API Java của chúng tôi để xóa hoặc xóa hình mờ khỏi các loại tài liệu khác nhau, bao gồm PDF s và tệp Office. Hoàn hảo cho các nhà phát triển muốn duy trì hình ảnh sạch sẽ và bảo vệ tính toàn vẹn của tài liệu."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "Hình mờ rõ ràng"
  features:
    # feature loop
    - title: "Xóa hình mờ với độ chính xác"
      content: "Sử dụng API Java của chúng tôi để nhắm mục tiêu và xóa hình mờ chính xác mà không làm gián đoạn bố cục tài liệu gốc. Lý tưởng cho các tài liệu nhạy cảm hoặc chính thức, nơi sự rõ ràng và chính xác là tối quan trọng."

    # feature loop
    - title: "Xóa hình mờ hàng loạt"
      content: "Nâng cao hiệu quả xử lý tài liệu của bạn bằng cách xóa hình mờ khỏi nhiều tệp cùng một lúc. API của chúng tôi hỗ trợ các hoạt động hàng loạt, tiết kiệm thời gian và tài nguyên cho các tác vụ quy mô lớn."

    # feature loop
    - title: "Chỉnh sửa các yếu tố hình mờ"
      content: "Các công cụ chỉnh sửa nâng cao của chúng tôi cho phép bạn chỉnh sửa có chọn lọc các thành phần hình mờ, mang lại sự linh hoạt trong việc quản lý bản trình bày tài liệu đồng thời đảm bảo bảo mật nội dung."
      
  code_samples:
    # code sample loop
    - title: "PDF hình mờ văn bản rõ ràng"
      content: |
        Ví dụ này cho thấy cách tìm và xóa tất cả các chú thích chứa văn bản có định dạng cụ thể khỏi tài liệu PDF.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Tải tài liệu PDF
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Nhận nội dung tài liệu
        PdfContent pdfContent = watermarker.getContent(PdfContent.class);

        //  Hình mờ văn bản rõ ràng với phông chữ cụ thể
        for (PdfPage page : pdfContent.getPages()){
            for (int i = page.getAnnotations().getCount() - 1; i >= 0; i--){
                for (FormattedTextFragment fragment : page.getAnnotations().get_Item(i).getFormattedTextFragments()){
                    if (fragment.getFont().getFamilyName() == "Verdana"){
                        page.getAnnotations().removeAt(i);
                        break;
                    }
                }
            }
        }

        //  Lưu tài liệu
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
    title: "Quản lý hình mờ Excel trong Java"
    exclude: "EXCEL"
    description: "Tìm hiểu cách Excel API đơn giản hóa việc xóa hình mờ khỏi tài liệu Excel, duy trì tính toàn vẹn và rõ ràng của tệp."
    items: 
        # format loop 1
        - name: "Hình mờ PDF"
          format: "PDF"
          link: "/watermark/java/clear//pdf/"
          description: "Định dạng tài liệu Adobe Portable"

        # format loop 2
        - name: "Hình mờ Word"
          format: "WORD"
          link: "/watermark/java/clear//word/"
          description: "MS Word và tài liệu Open Office"
          
        # format loop 3
        - name: "Hình mờ Excel"
          format: "EXCEL"
          link: "/watermark/java/clear//excel/"
          description: "MS Excel và bảng tính Open Office"

        # format loop 4
        - name: "Hình mờ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/clear//powerpoint/"
          description: "MS PowerPoint và các bài thuyết trình Open Office"

        # format loop 5
        - name: "Hình mờ DOCX"
          format: "DOCX"
          link: "/watermark/java/clear//docx/"
          description: "Microsoft Word Tài liệu XML mở"
          
        # format loop 6
        - name: "Hình mờ PPTX"
          format: "PPTX"
          link: "/watermark/java/clear//pptx/"
          description: "PowerPoint Bản trình bày XML mở"
          
        # format loop 7
        - name: "Hình mờ XLSX"
          format: "XLSX"
          link: "/watermark/java/clear//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Hình mờ DOC"
          format: "DOC"
          link: "/watermark/java/clear//doc/"
          description: "Tài liệu Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Hình mờ XLS"
          format: "XLS"
          link: "/watermark/java/clear//xls/"
          description: "Microsoft Excel Sổ làm việc 97-2003"

        # format loop 10
        - name: "Hình mờ PPT"
          format: "PPT"
          link: "/watermark/java/clear//ppt/"
          description: "PowerPoint Bài thuyết trình 97-2003"

        # format loop 11
        - name: "Hình mờ RTF"
          format: "RTF"
          link: "/watermark/java/clear//rtf/"
          description: "Định dạng văn bản phong phú"

---