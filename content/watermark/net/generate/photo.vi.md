
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:19
draft: false
lang: vi
format: Photo
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Làm mờ ảnh của bạn một cách nhanh chóng và dễ dàng"
head_description: "Nhanh chóng bảo mật và xác nhận bản quyền trên ảnh của bạn với hình mờ .NET C #. Bắt đầu bảo vệ công việc của bạn ngay hôm nay."

############################# Header ############################
title: "Hình mờ ảnh nhanh chóng và dễ dàng với .NET" 
description: "Thư viện C # mạnh mẽ của chúng tôi cho phép đánh dấu nhanh chóng cho ảnh của bạn, giúp bạn bảo mật bản quyền và nâng cao nhận diện thương hiệu mà không ảnh hưởng đến chất lượng hình ảnh."
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống tại Nuget miễn phí"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET cung cấp một giải pháp mạnh mẽ cho các dịch vụ của nhiếp ảnh gia đang tìm cách bảo vệ bản quyền và nhận dạng thương hiệu của họ. API này cho phép bổ sung nhanh hình mờ văn bản hoặc hình ảnh vào ảnh trên nhiều định dạng bao gồm JPEG, PNG và RAW. Tùy chỉnh hình mờ của bạn về độ trong suốt, kích thước và vị trí để kết hợp liền mạch với ảnh, duy trì chất lượng thẩm mỹ đồng thời khẳng định các quyền hợp pháp của bạn và ngăn chặn việc sử dụng trái phép.

############################# Steps ############################
steps:
    enable: true
    title: "Nâng cao tài liệu của bạn: Tạo hình mờ cho Photo bằng cách sử dụng .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** là thư viện giúp đơn giản hóa việc thêm hình mờ vào các định dạng tệp doanh nghiệp khác nhau dành cho nhà phát triển .NET. Tích hợp thư viện của chúng tôi vào ứng dụng của bạn và dễ dàng tạo hình mờ cho tài liệu bằng các bước sau:
      
      1. **Bắt đầu hành trình tạo hình mờ của bạn:** Bắt đầu bằng cách làm quen với lớp **Watermarker**, nền tảng API của chúng tôi. Để bắt đầu quá trình, hãy đảm bảo bạn khởi tạo nó trước khi xử lý tài liệu. Đừng bỏ qua tầm quan trọng của việc cung cấp tệp Photo cho hàm tạo, cho dù đó là đường dẫn hay đối tượng luồng.
      2. **Tạo hình mờ tùy chỉnh:** Chuyển sang giai đoạn tiếp theo bằng cách tạo đối tượng **Watermark** phù hợp với thông số kỹ thuật của bạn. Công cụ linh hoạt này không giới hạn ở các trang tài liệu cụ thể; nó cũng có thể được tích hợp liền mạch vào các thành phần tài liệu gốc như tệp đính kèm hoặc tiêu đề.
      3. **Tinh chỉnh thuộc tính hình mờ:** Tinh chỉnh trải nghiệm hình mờ của bạn bằng cách điều chỉnh các thuộc tính như chiều cao, chiều rộng, căn chỉnh trang, họ phông chữ và màu sắc. Mức độ tùy chỉnh này đảm bảo hình mờ của bạn kết hợp hoàn hảo với tài liệu của bạn.
      4. **Áp dụng hình mờ của bạn:** Sử dụng phương pháp **Watermarker** để dễ dàng áp dụng hình mờ tùy chỉnh cho tài liệu của bạn. Cho dù bạn cần thêm một hay nhiều hình mờ, quy trình này đều mang lại sự linh hoạt. Để tăng cường bảo mật, hãy cân nhắc việc lưu tài liệu đã xử lý của bạn ở một vị trí riêng.
   
    code:
      platform: "net"
      copy_title: "Sao chép"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "bấm để sao chép"
        copy_done: "sao chép"
      links:
        #  loop
        - title: "Thêm ví dụ"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "Tài liệu"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // Tạo hình mờ văn bản trong tệp PHOTO

        // Cung cấp tập tin được đóng dấu mờ
        using (Watermarker watermarker = new Watermarker("input.png"))
        {
            // Tạo phiên bản hình mờ văn bản
            Font font = new Font("Arial", 19, FontStyle.Bold | FontStyle.Italic);
            TextWatermark watermark = new TextWatermark("my watermark", font);
            watermark.ForegroundColor = Color.Red;
            watermark.BackgroundColor = Color.Blue;
            watermarker.Add(watermark);

            // Lưu kết quả PHOTO
            watermarker.Save("output.png");
        }
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Tìm hiểu sâu về việc thêm hình mờ"
  description: "Tận dụng API mạnh mẽ của chúng tôi để hiển thị, hiển thị, chuyển đổi và quản lý tài liệu, trang trình bày, sơ đồ và nhiều loại tài liệu khác trong ứng dụng .NET. GroupDocs.Watermark tích hợp liền mạch khả năng hình mờ để tăng cường bảo mật tài liệu và bảo vệ bản quyền."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Thêm hình mờ"
  features:
    # feature loop
    - title: "Làm mờ tài liệu của bạn một cách dễ dàng."
      content: "GroupDocs.Watermark trao quyền cho .NET nhà phát triển dễ dàng tích hợp hình mờ vào ứng dụng của họ. Thêm văn bản, hình ảnh hoặc hình mờ động vào các tài liệu và tệp kinh doanh phổ biến một cách dễ dàng, đảm bảo nội dung của bạn được bảo mật và có thương hiệu nhất quán trên tất cả các nền tảng."

    # feature loop
    - title: "Điều chỉnh hình mờ để đáp ứng nhu cầu của bạn."
      content: "Tùy chỉnh hình mờ để phù hợp với yêu cầu cụ thể của bạn với các tính năng mở rộng được hỗ trợ bởi GroupDocs.Watermark. Điều chỉnh kích thước, xoay, độ trong suốt, màu sắc và phông chữ để đảm bảo hình mờ của bạn không chỉ trông hoàn hảo mà còn tăng cường bảo mật tài liệu mà không cản trở thông tin quan trọng."

    # feature loop
    - title: "Khai thác các tính năng tài liệu gốc để tạo hình mờ"
      content: "Sử dụng các tính năng vốn có của định dạng tài liệu để tạo hình mờ tinh vi. Cho dù đó là sử dụng PDF chú thích gốc, MS Word hình nền hoặc Excel đầu trang và chân trang, GroupDocs.Watermark tích hợp sâu với cấu trúc tài liệu để áp dụng hình mờ vừa hiệu quả vừa xâm lấn tối thiểu."
      
  code_samples:
    # code sample loop
    - title: "Tạo hình mờ hình ảnh cho DOCX"
      content: |
        Ví dụ này cho thấy cách áp dụng hiệu ứng hình ảnh cho hình mờ hình dạng.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Tải tài liệu Word
            var loadOptions = new WordProcessingLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.docx", loadOptions))
            {
                //  Thiết lập tùy chọn hình mờ
                using (ImageWatermark watermark = new ImageWatermark("logo.png"))
                {
                    WordProcessingImageEffects effects = new WordProcessingImageEffects();
                    effects.Brightness = 0.7;
                    effects.Contrast = 0.6;
                    effects.ChromaKey = Color.Red;
                    effects.BorderLineFormat.Enabled = true;
                    effects.BorderLineFormat.Weight = 1;

                    WordProcessingWatermarkSectionOptions options = new WordProcessingWatermarkSectionOptions();
                    options.Effects = effects;

                    //  Tạo hình mờ
                    watermarker.Add(watermark, options);
                }

                //  Lưu tài liệu cập nhật
                watermarker.save("result.docx");
            }

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Sẵn sàng để bắt đầu?"
  description: "Dùng thử GroupDocs.Watermark tính năng miễn phí hoặc yêu cầu giấy phép"
  items:
    #  loop
    - title: "Nuget tải về"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "Cấp phép"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Bảo vệ ảnh của bạn với hình mờ hiệu quả C#"
    exclude: "PHOTO"
    description: "Bảo mật và cách điệu nội dung ảnh của bạn với hình mờ có thể tùy chỉnh bằng cách sử dụng .NET C# API của chúng tôi, được thiết kế để tích hợp liền mạch và duy trì chất lượng hình ảnh."
    items: 
        # format loop 1
        - name: "Hình mờ PDF"
          format: "PDF"
          link: "/watermark/net/generate//pdf/"
          description: "Định dạng tài liệu Adobe Portable"

        # format loop 2
        - name: "Hình mờ Word"
          format: "WORD"
          link: "/watermark/net/generate//word/"
          description: "MS Word và tài liệu Open Office"
          
        # format loop 3
        - name: "Hình mờ Excel"
          format: "EXCEL"
          link: "/watermark/net/generate//excel/"
          description: "MS Excel và bảng tính Open Office"

        # format loop 4
        - name: "Hình ảnh hình mờ"
          format: "IMAGE"
          link: "/watermark/net/generate//image/"
          description: "Định dạng hình ảnh phổ biến"

        # format loop 5
        - name: "Ảnh hình mờ"
          format: "PHOTO"
          link: "/watermark/net/generate//photo/"
          description: "Định dạng ảnh"

        # format loop 6
        - name: "Hình mờ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/generate//powerpoint/"
          description: "MS PowerPoint và các bài thuyết trình Open Office"

        # format loop 7
        - name: "Hình mờ DOCX"
          format: "DOCX"
          link: "/watermark/net/generate//docx/"
          description: "Microsoft Word Tài liệu XML mở"
          
        # format loop 8
        - name: "Hình mờ PPTX"
          format: "PPTX"
          link: "/watermark/net/generate//pptx/"
          description: "PowerPoint Bản trình bày XML mở"
          
        # format loop 9
        - name: "Hình mờ XLSX"
          format: "XLSX"
          link: "/watermark/net/generate//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 10
        - name: "Hình mờ JPEG"
          format: "JPEG"
          link: "/watermark/net/generate//jpeg/"
          description: "JPEG Hình ảnh"

        # format loop 11
        - name: "Hình mờ PNG"
          format: "PNG"
          link: "/watermark/net/generate//png/"
          description: "Portable Đồ họa mạng"

        # format loop 12
        - name: "Hình mờ TIFF"
          format: "TIFF"
          link: "/watermark/net/generate//tiff/"
          description: "Nhãn định dạng tệp hình ảnh"

        # format loop 13
        - name: "Hình mờ WEBP"
          format: "WEBP"
          link: "/watermark/net/generate//webp/"
          description: "Hình ảnh WEB"

        # format loop 14
        - name: "Hình mờ DOC"
          format: "DOC"
          link: "/watermark/net/generate//doc/"
          description: "Tài liệu Microsoft Word 97 - 2007"

        # format loop 15
        - name: "Hình mờ XLS"
          format: "XLS"
          link: "/watermark/net/generate//xls/"
          description: "Microsoft Excel Sổ làm việc 97-2003"

        # format loop 16
        - name: "Hình mờ PPT"
          format: "PPT"
          link: "/watermark/net/generate//ppt/"
          description: "PowerPoint Bài thuyết trình 97-2003"

        # format loop 17
        - name: "Hình mờ RTF"
          format: "RTF"
          link: "/watermark/net/generate//rtf/"
          description: "Định dạng văn bản phong phú"

---