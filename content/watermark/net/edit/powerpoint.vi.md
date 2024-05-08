
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:19
draft: false
lang: vi
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Chỉnh sửa hình mờ trong Powerpoint tài liệu"
head_description: "Đơn giản hóa việc chỉnh sửa hình mờ Powerpoint và bảo vệ tài liệu của bạn với Thư viện GroupDocs.Watermark for .NET. Đạt được sự kiểm soát chính xác và tính linh hoạt."

############################# Header ############################
title: "Chỉnh sửa Powerpoint Vị trí hình mờ: .NET Độ chính xác" 
description: "Đạt được quyền kiểm soát chính xác vị trí hình mờ và bảo mật tài liệu với Giải pháp GroupDocs.Watermark for .NET. Chỉnh sửa Powerpoint Hình mờ một cách chính xác."
subtitle: "GroupDocs.Watermark for .NET Thư viện" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải về tại Nuget"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET CÁ"
    link: "/watermark/net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Chỉnh sửa Powerpoint Vị trí hình mờ:** Đạt được kiểm soát chính xác vị trí hình mờ và bảo mật tài liệu với GroupDocs.Watermark for .NET Nhà phát triển. Hợp lý hóa quy trình làm việc của bạn và đảm bảo tính xác thực dễ dàng.

############################# Steps ############################
steps:
    enable: true
    title: "Chỉnh sửa hình mờ trong tài liệu Powerpoint bằng cách sử dụng .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** trao quyền cho nhà phát triển .NET dễ dàng chỉnh sửa hình mờ trong nhiều tài liệu Powerpoint khác nhau. Dưới đây là hướng dẫn đơn giản về cách sử dụng API của chúng tôi trong ứng dụng của bạn:
      
      1. Bắt đầu bằng cách chuyển tệp Powerpoint của bạn làm tham số cho hàm tạo của lớp **Watermarker**. Bạn có thể cung cấp tệp dưới dạng luồng byte, luồng tệp hoặc đường dẫn đĩa cục bộ.
      2. Tiếp theo, xác định vị trí các hình mờ cụ thể cần chỉnh sửa. Sử dụng **SearchCriteria** để xác định hình mờ có thuộc tính tương ứng đã được thêm vào tài liệu trước đó.
      3. Sau khi tìm kiếm, bạn sẽ nhận được danh sách các hình mờ có liên quan. Sau đó, bạn có thể tùy chỉnh các thuộc tính của chúng, chẳng hạn như kích thước, căn chỉnh trang, văn bản, màu sắc, nội dung hình ảnh, v.v. Điều này cấp cho bạn quyền kiểm soát rộng rãi đối với dữ liệu của bạn.
      4. Khi bạn đã hoàn tất việc chỉnh sửa hình mờ, hãy lưu tài liệu đã cập nhật. Bạn có thể sử dụng đường dẫn tệp cục bộ hoặc luồng để lưu trữ kết quả cuối cùng.
   
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
        // Chỉnh sửa hình mờ văn bản POWERPOINT

        // Yêu cầu Watermarker cung cấp tệp POWERPOINT
        using (Watermarker watermarker = new Watermarker("input.pptx"))
        {
            // Xây dựng TextSearchCriteria và nhận hình mờ văn bản
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                 // Chỉnh sửa hình mờ văn bản
                 watermark.FormattedTextFragments.Clear();
                 watermark.FormattedTextFragments.Add("passed", 
                    new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
            }

            // Lưu tài liệu
            watermarker.Save("output.pptx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tìm hiểu thêm về sửa đổi hình mờ"
  description: "Hỗ trợ .NET ứng dụng của bạn với thư viện của chúng tôi và thêm, chỉnh sửa, xóa hoặc tìm kiếm hình mờ trong các định dạng tệp khác nhau."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Chỉnh sửa hình mờ"
  features:
    # feature loop
    - title: "Tệp hình mờ cho doanh nghiệp của bạn"
      content: "Sử dụng GroupDocs.Watermark for .NET để tô mờ các tệp và tài liệu. Thêm và quản lý hình mờ mà không cần nỗ lực thêm để triển khai API của chúng tôi trong các ứng dụng của bạn. Tìm kiếm, chỉnh sửa và xóa hình mờ đã thêm trước đó."

    # feature loop
    - title: "Tinh chỉnh hình mờ cho yêu cầu của bạn"
      content: "API của chúng tôi cung cấp một bộ tùy chọn tùy chỉnh toàn diện. Dễ dàng sửa đổi các khía cạnh như kích thước, hướng, bảng màu, họ phông chữ và hơn thế nữa để tạo hình mờ lý tưởng."

    # feature loop
    - title: "Tận dụng các tính năng cụ thể cho tài liệu"
      content: "Tùy thuộc vào định dạng tệp bạn đang sử dụng, bạn có thể kết hợp các chức năng tích hợp. Chúng có thể bao gồm nền tài liệu, chú thích, tiêu đề hoặc các yếu tố khác để đóng vai trò là vùng chứa hình mờ."
      
  code_samples:
    # code sample loop
    - title: "Excel chỉnh sửa văn bản hình mờ"
      content: |
        Ví dụ này cho thấy cách chỉnh sửa văn bản cho các hình mờ cụ thể trong Excel Bảng tính
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Tải bảng tính XLSX
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  Tải nội dung bảng tính
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();

                //  Chỉnh sửa văn bản bên trong hình mờ
                foreach (SpreadsheetShape shape in content.Worksheets[0].Shapes)
                {
                    if (shape.Text == "GroupDocs 2016")
                    {
                        shape.Text = "GroupDocs 2017";
                    }
                }

                //  Lưu kết quả đầu ra
                watermarker.save("result.xlsx");
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
    title: "Tinh chỉnh hình mờ trong các định dạng khác"
    exclude: "POWERPOINT"
    description: "Chỉnh sửa hình mờ ở các định dạng tài liệu khác nhau với GroupDocs.Watermark for .NET."
    items: 
        # format loop 1
        - name: "Hình mờ PDF"
          format: "PDF"
          link: "/watermark/net/edit//pdf/"
          description: "Định dạng tài liệu Adobe Portable"

        # format loop 2
        - name: "Hình mờ Word"
          format: "WORD"
          link: "/watermark/net/edit//word/"
          description: "MS Word và tài liệu Open Office"
          
        # format loop 3
        - name: "Hình mờ Excel"
          format: "EXCEL"
          link: "/watermark/net/edit//excel/"
          description: "MS Excel và bảng tính Open Office"

        # format loop 4
        - name: "Hình mờ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/edit//powerpoint/"
          description: "MS PowerPoint và các bài thuyết trình Open Office"

        # format loop 5
        - name: "Hình mờ DOCX"
          format: "DOCX"
          link: "/watermark/net/edit//docx/"
          description: "Microsoft Word Tài liệu XML mở"
          
        # format loop 6
        - name: "Hình mờ PPTX"
          format: "PPTX"
          link: "/watermark/net/edit//pptx/"
          description: "PowerPoint Bản trình bày XML mở"
          
        # format loop 7
        - name: "Hình mờ XLSX"
          format: "XLSX"
          link: "/watermark/net/edit//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Hình mờ DOC"
          format: "DOC"
          link: "/watermark/net/edit//doc/"
          description: "Tài liệu Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Hình mờ XLS"
          format: "XLS"
          link: "/watermark/net/edit//xls/"
          description: "Microsoft Excel Sổ làm việc 97-2003"

        # format loop 10
        - name: "Hình mờ PPT"
          format: "PPT"
          link: "/watermark/net/edit//ppt/"
          description: "PowerPoint Bài thuyết trình 97-2003"

        # format loop 11
        - name: "Hình mờ RTF"
          format: "RTF"
          link: "/watermark/net/edit//rtf/"
          description: "Định dạng văn bản phong phú"

---