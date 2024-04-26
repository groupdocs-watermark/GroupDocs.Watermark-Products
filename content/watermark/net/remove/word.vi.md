
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:58
draft: false
lang: vi
format: Word
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C# .NET API để loại bỏ hình mờ Word"
head_description: "Xóa, xóa hoặc chỉnh sửa hiệu quả hình mờ từ Word tài liệu bằng cách sử dụng API C# .NET của chúng tôi để trình bày tài liệu hoàn hảo."

############################# Header ############################
title: "Word Loại bỏ hình mờ cho C# .NET" 
description: "Sử dụng API GroupDocs.Watermark for .NET C# để xóa hình mờ khỏi tài liệu Word, hoàn hảo để duy trì tính toàn vẹn và sạch sẽ của các tài liệu pháp lý và công ty."
subtitle: "GroupDocs.Watermark for .NET C# CÁ" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống tại Nuget miễn phí"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET C# thư viện"
    link: "/watermark/net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       Với thư viện GroupDocs.Watermark for .NET C# .NET, các nhà phát triển có thể dễ dàng quản lý và xóa hình mờ trong các tệp Microsoft Word. Công cụ này hỗ trợ một loạt các thao tác hình mờ, bao gồm phát hiện, sửa đổi và xóa cả hình mờ văn bản và hình ảnh, đảm bảo tài liệu không có dấu không mong muốn trong khi vẫn giữ nguyên bố cục và định dạng.

############################# Steps ############################
steps:
    enable: true
    title: "Xóa hình mờ khỏi tài liệu Word bằng cách sử dụng .NET"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/)** đơn giản hóa nhiệm vụ xóa hình mờ khỏi tài liệu kinh doanh. Tăng cường ứng dụng .NET của bạn bằng cách tích hợp thư viện của chúng tôi và làm theo các bước đơn giản sau:
      
      1. **Watermarker**, với tài liệu Word. API của chúng tôi hỗ trợ xử lý tài liệu được cung cấp dưới dạng luồng hoặc đường dẫn cục bộ.
      2. **Tiêu chí tìm kiếm** để thu hẹp tập hợp hình mờ cần xử lý. Bạn có thể sử dụng các tham số khác nhau như hình ảnh, văn bản hoặc các tính năng định dạng. Các tham số tìm kiếm bạn cung cấp càng cụ thể, kết quả bạn nhận được càng chính xác.
      3. Xử lý danh sách hình mờ tài liệu thu được dưới dạng kết quả tìm kiếm và xóa chúng khỏi tài liệu.
      4. Sau khi xóa hình mờ, lưu tài liệu kết quả dưới dạng tệp cục bộ hoặc luồng byte.
   
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
        // Xóa hình mờ văn bản khỏi tài liệu Word

        // Cung cấp phiên bản Watermarker cho tài liệu nguồn tài liệu Word
        using (Watermarker watermarker = new Watermarker("input.docx"))
        {
            // Xóa hình mờ đã chọn khỏi tài liệu
            TextFormattingSearchCriteria criteria = new TextFormattingSearchCriteria();
            criteria.ForegroundColorRange = new ColorRange();
            criteria.FontBold = true;
            PossibleWatermarkCollection watermarks = watermarker.Search(criteria);
            watermarks.Clear();

            // Lưu tệp vào đường dẫn được cung cấp
            watermarker.Save("output.docx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Hợp lý hóa việc loại bỏ hình mờ với C# .NET API"
  description: "Khám phá khả năng xóa hình mờ mạnh mẽ của API C# .NET của chúng tôi, được thiết kế để tích hợp liền mạch với các ứng dụng .NET của bạn. Xóa hoặc xóa hình mờ khỏi PDF s và tài liệu văn phòng một cách hiệu quả trong khi vẫn giữ được chất lượng tệp gốc."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "Xóa hình mờ"
  features:
    # feature loop
    - title: "Xóa hình mờ chính xác"
      content: "API .NET của chúng tôi cung cấp các công cụ chính xác để xóa sạch hình mờ khỏi bất kỳ tài liệu nào. Được thiết kế riêng cho các nhà phát triển, tính năng này đảm bảo rằng việc xóa hình mờ không ảnh hưởng đến chất lượng hoặc bố cục tài liệu."

    # feature loop
    - title: "Tự động loại bỏ hình mờ hàng loạt"
      content: "Tự động hóa quá trình xóa hình mờ khỏi bộ tài liệu lớn với API .NET của chúng tôi. Lý tưởng cho các doanh nghiệp xử lý khối lượng lớn tài liệu, nâng cao cả hiệu quả và bảo mật tài liệu."

    # feature loop
    - title: "Tính năng chỉnh sửa hình mờ nâng cao"
      content: "Tận dụng các tính năng nâng cao để chỉnh sửa hoặc sửa đổi hình mờ có chọn lọc. API của chúng tôi hỗ trợ điều chỉnh chi tiết để đảm bảo tài liệu của bạn duy trì vẻ ngoài chuyên nghiệp trong khi bảo mật thông tin nhạy cảm."
      
  code_samples:
    # code sample loop
    - title: "Xóa hình mờ văn bản bảng tính"
      content: |
        Cách xóa hình mờ văn bản với định dạng đặc biệt trong Excel tài liệu.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Tải sổ làm việc Excel
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  Nhận nội dung và tìm hình mờ phù hợp
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();
                foreach (SpreadsheetWorksheet section in content.Worksheets)
                {
                    for (int i = section.Shapes.Count - 1; i >= 0; i--)
                    {
                        foreach (FormattedTextFragment fragment in section.Shapes[i].FormattedTextFragments)
                        {
                            if (fragment.ForegroundColor.Equals(Color.Red) && fragment.Font.FamilyName == "Arial")
                            {
                                //  Xóa hình mờ văn bản
                                section.Shapes.RemoveAt(i);
                                break;
                            }
                        }
                    }
                }

                //  Lưu đã xử lý XLSX
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
    title: "Quản lý hình mờ Word với .NET"
    exclude: "WORD"
    description: "Khám phá các tính năng mạnh mẽ để quản lý hình mờ trong tài liệu Word bằng API C# .NET của chúng tôi, được thiết kế để tăng cường bảo mật tài liệu và trình bày mà không ảnh hưởng đến chất lượng."
    items: 
        # format loop 1
        - name: "Hình mờ PDF"
          format: "PDF"
          link: "/watermark/net/remove//pdf/"
          description: "Định dạng tài liệu Adobe Portable"

        # format loop 2
        - name: "Hình mờ Word"
          format: "WORD"
          link: "/watermark/net/remove//word/"
          description: "MS Word và tài liệu Open Office"
          
        # format loop 3
        - name: "Hình mờ Excel"
          format: "EXCEL"
          link: "/watermark/net/remove//excel/"
          description: "MS Excel và bảng tính Open Office"

        # format loop 4
        - name: "Hình mờ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/remove//powerpoint/"
          description: "MS PowerPoint và các bài thuyết trình Open Office"

        # format loop 5
        - name: "Hình mờ DOCX"
          format: "DOCX"
          link: "/watermark/net/remove//docx/"
          description: "Microsoft Word Tài liệu XML mở"
          
        # format loop 6
        - name: "Hình mờ PPTX"
          format: "PPTX"
          link: "/watermark/net/remove//pptx/"
          description: "PowerPoint Bản trình bày XML mở"
          
        # format loop 7
        - name: "Hình mờ XLSX"
          format: "XLSX"
          link: "/watermark/net/remove//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Hình mờ DOC"
          format: "DOC"
          link: "/watermark/net/remove//doc/"
          description: "Tài liệu Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Hình mờ XLS"
          format: "XLS"
          link: "/watermark/net/remove//xls/"
          description: "Microsoft Excel Sổ làm việc 97-2003"

        # format loop 10
        - name: "Hình mờ PPT"
          format: "PPT"
          link: "/watermark/net/remove//ppt/"
          description: "PowerPoint Bài thuyết trình 97-2003"

        # format loop 11
        - name: "Hình mờ RTF"
          format: "RTF"
          link: "/watermark/net/remove//rtf/"
          description: "Định dạng văn bản phong phú"

---