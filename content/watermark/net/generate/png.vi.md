
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:13
draft: false
lang: vi
format: Png
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Bảo mật PNG với .NET Hình mờ C #"
head_description: "Nhúng hình mờ vào PNG tệp bằng .NET C #, hoàn hảo cho bản quyền và bảo mật hình ảnh."

############################# Header ############################
title: "Hình mờ C # cho tập tin PNG" 
description: "Sử dụng .NET C # để áp dụng hình mờ nâng cao cho PNG hình ảnh, bảo vệ nội dung nghệ thuật và kỹ thuật số một cách hiệu quả."
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
       GroupDocs.Watermark for .NET cung cấp bộ công cụ .NET C# chuyên dụng để nhúng hình mờ trong tệp PNG, phục vụ cho các nghệ sĩ, nhà thiết kế và người sáng tạo nội dung, những người cần bảo vệ tài sản hình ảnh của họ. API này cho phép bổ sung liền mạch cả hình mờ trong suốt và mờ đục có thể được định vị và thu nhỏ một cách phức tạp để duy trì tính toàn vẹn của hình ảnh gốc đồng thời đảm bảo sự bảo vệ pháp lý. Các tính năng bao gồm hình mờ văn bản và hình ảnh tùy chỉnh, kiểm soát chính xác độ mờ mờ của hình mờ và khả năng thêm hình mờ nhiều lớp để tăng cường bảo mật. Cho dù cho mục đích sử dụng cá nhân hay danh mục đầu tư chuyên nghiệp, GroupDocs.Watermark đảm bảo hình ảnh PNG của bạn được bảo vệ chống lại việc tái tạo và sử dụng trái phép, được hỗ trợ đầy đủ trên .NET môi trường.

############################# Steps ############################
steps:
    enable: true
    title: "Dễ dàng tạo hình mờ cho tài liệu Png"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/):** Thư viện hình chìm mờ nâng cao dành cho ứng dụng .NET. Trao quyền cho giải pháp của bạn và bảo mật tài liệu bằng hình mờ đúng lúc.
      
      1. **Lớp cốt lõi: Watermarker.** Lớp chính của API của chúng tôi là **Watermarker**. Bạn cần khởi tạo nó trước khi xử lý tài liệu. Đừng quên chuyển tệp Png cho hàm tạo dưới dạng đường dẫn hoặc đối tượng luồng.
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
        // Tạo hình mờ hình ảnh trong tệp PNG

        // Cung cấp đường dẫn tệp nguồn tới hàm tạo Watermarker
        using (Watermarker watermarker = new Watermarker("input.png"))
        {
            // Tạo phiên bản hình mờ hình ảnh bằng tệp hình ảnh
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // Lưu kết quả PNG có hình chìm mờ
            watermarker.Save("output.png");
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
    title: "Triển khai hình mờ trong PNG với C #"
    exclude: "PNG"
    description: "Triển khai .NET C # để tạo hình mờ kín đáo hoặc đậm trong PNG hình ảnh, đảm bảo tính linh hoạt về mặt thẩm mỹ và bảo vệ bản quyền mạnh mẽ."
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