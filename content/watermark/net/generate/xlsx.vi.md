
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:13
draft: false
lang: vi
format: Xlsx
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Nhúng hình mờ trong XLSX với C #"
head_description: "Tận dụng .NET C # để tạo và áp dụng hình mờ trong XLSX tệp, bảo mật Excel tài liệu của bạn."

############################# Header ############################
title: "Bảo mật XLSX trang tính với .NET C #" 
description: "Sử dụng .NET C # để tạo hình mờ tùy chỉnh cho XLSX tệp, hoàn hảo để tăng cường tính toàn vẹn của tài liệu và bảo vệ thông tin nhạy cảm."
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
       GroupDocs.Watermark for .NET cung cấp một giải pháp mạnh mẽ cho các nhà phát triển C# .NET để tạo, thêm và quản lý hình mờ trong XLSX tệp. API này rất cần thiết để duy trì tính bảo mật và tính xác thực của Excel tài liệu, đặc biệt là trong môi trường công ty, tài chính và pháp lý. Tùy chỉnh hình mờ của bạn với nhiều tùy chọn, bao gồm lớp phủ văn bản và hình ảnh, được thiết kế vừa có chức năng vừa tinh tế. Các tính năng bổ sung cho phép tạo hình mờ tự động dựa trên thuộc tính tài liệu và điều kiện do người dùng xác định, đảm bảo rằng hình mờ của bạn được áp dụng nhất quán và chỉ khi cần thiết. GroupDocs.Watermark tương thích với các nền tảng .NET hiện đại và hỗ trợ các chức năng nâng cao Excel.

############################# Steps ############################
steps:
    enable: true
    title: "Dễ dàng tạo hình mờ cho tài liệu Xlsx"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/):** Thư viện hình chìm mờ nâng cao dành cho ứng dụng .NET. Trao quyền cho giải pháp của bạn và bảo mật tài liệu bằng hình mờ đúng lúc.
      
      1. **Lớp cốt lõi: Watermarker.** Lớp chính của API của chúng tôi là **Watermarker**. Bạn cần khởi tạo nó trước khi xử lý tài liệu. Đừng quên chuyển tệp Xlsx cho hàm tạo dưới dạng đường dẫn hoặc đối tượng luồng.
      2. **Tạo Hình mờ của bạn.** Bước tiếp theo là xây dựng đối tượng Hình mờ thuộc loại mong muốn. Nó có thể được đặt không chỉ trên một trang tài liệu cụ thể mà còn trong các phần tài liệu gốc như hình ảnh hoặc tiêu đề.
      3. **Tinh chỉnh giao diện.** Đặt các thuộc tính hình mờ như chiều cao và chiều rộng, trên cùng, bên trái, căn chỉnh giữa, phông chữ và màu sắc, v.v.
      4. **Áp dụng và lưu.** Sử dụng phương pháp **Watermarker** để thêm hình mờ mới. Hãy thoải mái thêm bao nhiêu hình mờ tùy thích. Bạn có thể lưu tài liệu có hình mờ vào bất kỳ vị trí nào.
   
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
        // Tạo hình mờ hình ảnh trong tệp XLSX

        // Cung cấp đường dẫn tệp nguồn tới hàm tạo Watermarker
        using (Watermarker watermarker = new Watermarker("input.xlsx"))
        {
            // Tạo phiên bản hình mờ hình ảnh bằng tệp hình ảnh
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // Lưu kết quả XLSX có hình chìm mờ
            watermarker.Save("output.xlsx");
        }
        
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "Nâng cao trò chơi hình mờ của bạn"
  description: "Mở khóa khả năng tạo hình mờ nâng cao với GroupDocs.Watermark API của chúng tôi cho .NET. Công cụ mạnh mẽ này cho phép tùy chỉnh chính xác và áp dụng hình mờ trên các loại tài liệu khác nhau để đảm bảo bảo mật tối đa và tuân thủ bản quyền với sự gián đoạn hình ảnh tối thiểu."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Giải pháp chấm mờ toàn diện"
  features:
    # feature loop
    - title: "Tùy chọn ốp lát tinh vi"
      content: "Mở rộng hình mờ của bạn trên toàn bộ tài liệu một cách liền mạch với các tùy chọn ốp lát của chúng tôi. Tính năng này cho phép hình mờ bao phủ toàn bộ khu vực tài liệu, ngăn chặn việc xóa và đảm bảo bảo vệ tài liệu hoàn toàn mà không ảnh hưởng đến thiết kế hoặc khả năng đọc."

    # feature loop
    - title: "Tùy chỉnh màu sắc rực rỡ"
      content: "Thêm một chút màu sắc vào hình mờ của bạn! API của chúng tôi cho phép tùy chỉnh màu sắc toàn phổ, cho phép bạn áp dụng hình mờ phù hợp hoàn hảo với thương hiệu công ty hoặc phong cách tài liệu của bạn. Tăng cường sức hấp dẫn trực quan trong khi vẫn duy trì các tính năng bảo mật mạnh mẽ."

    # feature loop
    - title: "Cài đặt bảo mật nâng cao"
      content: "Đưa bảo mật tài liệu lên cấp độ tiếp theo với cài đặt hình mờ nâng cao. Định cấu hình hình mờ nhiều lớp, kết hợp cả các yếu tố hiển thị và vô hình, để bảo vệ chống lại việc sao chép trái phép và đảm bảo chỉ người nhận dự định mới có thể truy cập thông tin quan trọng."
      
  code_samples:
    # code sample loop
    - title: "Tạo hình mờ PowerPoint"
      content: |
        Ví dụ này cho thấy cách thêm hình mờ vào hình nền PPTX
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Tải bài thuyết trình PPTX
            var loadOptions = new PresentationLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pptx", loadOptions))
            {
                //  Thiết lập thuộc tính hình mờ
                TextWatermark watermark = new TextWatermark("Protected image", new Font("Arial", 8));
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermark.RotateAngle = 45;
                watermark.SizingType = SizingType.ScaleToParentDimensions;
                watermark.ScaleFactor = 1;

                //  Hình nền slide hình mờ
                PresentationContent content = watermarker.GetContent<PresentationContent>();
                foreach (PresentationSlide slide in content.Slides)
                {
                    if (slide.ImageFillFormat.BackgroundImage != null)
                    {
                        slide.ImageFillFormat.BackgroundImage.Add(watermark);
                    }
                }

                //  Lưu bản trình bày đã xử lý
                watermarker.save("result.pptx");
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
    title: "Triển khai hình mờ trong XLSX với C #"
    exclude: "XLSX"
    description: "Triển khai .NET C # để thêm hiệu quả hình mờ nâng cao, an toàn vào XLSX tệp, bảo vệ dữ liệu chuyên nghiệp Excel của bạn."
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