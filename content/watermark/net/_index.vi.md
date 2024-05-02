---
############################# Static ############################
layout: "landing"
date: 2024-04-29T14:27:13
draft: false

lang: vi
product: "Watermark"
product_tag: "watermark"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "C# .NET Phần mềm hình mờ tài liệu | thêm hình mờ"
head_description: "Thư viện C# .NET để thêm, tìm kiếm và xóa hình mờ trong tài liệu: PDF, Word, Excel, bản trình bày, Visio sơ đồ, email và định dạng tệp hình ảnh."

############################# Header ############################
title: "Hình mờ tài liệu dễ dàng trong các ứng dụng C # .NET của bạn"
description: "Tăng cường các giải pháp C# của bạn với API hình mờ tài liệu linh hoạt cung cấp thêm hình mờ tùy chỉnh cho tất cả các định dạng tài liệu phổ biến."
words:
  for: "cho"

actions:
  main: "Tải xuống miễn phí NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Watermark"
  alt: "Cấp phép"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/net/"
  title: "Sẵn sàng để bắt đầu?"
  description: "Dùng thử GroupDocs.Watermark tính năng miễn phí hoặc yêu cầu giấy phép"

release:
  title: "Phiên bản {0} đã phát hành"
  notes: "Xem những gì mới"
  downloads: "Tải xuống"

code:
  title: "Hình mờ PDF tệp trong C #"
  more: "Thêm ví dụ"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
  install: "dotnet add package GroupDocs.Watermark"
  content: |
    ```csharp {style=abap}   
    // Thực hiện Watermarker đi qua đường dẫn PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    using (Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions))
    {
        // Tùy chỉnh tùy chọn hình mờ
        TextWatermark textWatermark = 
            new TextWatermark("Approved", new Font("Arial", 8));
        
        // Áp dụng hình mờ cho tài liệu PDF
        watermarker.Add(textWatermark);

        // Lưu tài liệu kết quả
        watermarker.Save("result.pdf");
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark trong nháy mắt"
  description: "API để đặt hình mờ trên tài liệu thông qua .NET"
  features:
    # feature loop
    - title: "Hình mờ tệp C #"
      content: "Thêm hình mờ vào tệp doanh nghiệp của bạn bằng cách sử dụng GroupDocs.Watermark. Sử dụng văn bản, hình ảnh, sơ đồ hoặc tệp đính kèm email."

    # feature loop
    - title: "Tùy chỉnh hình mờ theo mục tiêu của bạn"
      content: "Phần mềm GroupDocs.Watermark for .NET cho phép tùy chỉnh hình mờ theo nhiều cách khác nhau. Các kiểu văn bản như in đậm, nghiêng, kiểu phông chữ cùng với các thuộc tính hình ảnh như xoay, v.v. làm phong phú quá trình hình mờ."

    # feature loop
    - title: "Tất cả các định dạng tệp phổ biến được hỗ trợ"
      content: "Nhiều định dạng tệp và tài liệu được hỗ trợ bởi giải pháp GroupDocs.Watermark. PDF, Microsoft Office Word, Excel, PowerPoint, hình ảnh như JPEG, PNG, GIF, BMP, Visio, Visio sơ đồ, email, v.v. có thể được bảo vệ bằng hình mờ của chúng tôi."

    # feature loop
    - title: "Tìm kiếm và cập nhật hình mờ"
      content: "Hình mờ đã được trình bày trong tài liệu có thể được tìm thấy và xử lý lại. Sửa đổi văn bản, kiểu dáng, hình ảnh hoặc xóa hình mờ lộ mà không cần nỗ lực thêm."

############################# Platforms ############################
platforms:
  enable: true
  title: "Độc lập nền tảng"
  description: "GroupDocs.Watermark for .NET hỗ trợ các hệ điều hành, khung và trình quản lý gói được liệt kê dưới đây"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Định dạng tập tin được hỗ trợ"
  description: |
    GroupDocs.Watermark for .NET cung cấp xử lý các [định dạng tệp] sau đây (https://docs.groupdocs.com/watermark/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office & OpenDocument định dạng
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### Hình ảnh & Đồ họa
        * **Định dạng hình ảnh phổ biến:** BMP, JPG, JPEG, PNG
        * **Hình ảnh nhiều trang:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### Khác
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark tính năng"
  description: "Bảo vệ PDF, Office, Hình ảnh và các định dạng khác bằng hình mờ"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Hình mờ tài liệu"
      content: "Thêm hoặc xóa hình mờ khỏi một phần cụ thể hoặc toàn bộ tài liệu của các định dạng tệp khác nhau."

    # feature loop
    - icon: "watermark_style"
      title: "Tạo kiểu hình mờ của bạn"
      content: "Tùy chỉnh các thuộc tính hình mờ khác nhau như màu sắc, phông chữ, xoay, v.v."

    # feature loop
    - icon: "hidden_print"
      title: "PDF hình mờ in ẩn"
      content: "Phân bổ Hidden Watermark cho PDF chỉ xuất hiện khi in tài liệu."

    # feature loop
    - icon: "image_only"
      title: "Hình ảnh chỉ có hình mờ trong tài liệu"
      content: "Đánh dấu tất cả hình ảnh trong một phần cụ thể, trang, trang trình chiếu hoặc tài liệu."

    # feature loop
    - icon: "image_frame"
      title: "Xử lý khung hình ảnh đã chọn"
      content: "Chỉ gán hình mờ cho các khung cụ thể của hình ảnh đa khung."

    # feature loop
    - icon: "attachments"
      title: "Tệp đính kèm & hình dạng"
      content: "Đặt Hình mờ cho tất cả các tệp đính kèm trong tài liệu Excel và tất cả Hình dạng hình ảnh trong Trang trình bày."

    # feature loop
    - icon: "pdf_objects"
      title: "PDF đối tượng"
      content: "Căn chỉnh hình mờ với Hộp Bleed, Hộp nghệ thuật, Hộp cắt hoặc Hộp cắt trong Tài liệu PDF."

    # feature loop
    - icon: "doc_background"
      title: "Tài liệu nền"
      content: "Đặt Hình mờ hoặc Xóa nó khỏi Hình nền của Bảng tính hoặc Trang trình bày."

    # feature loop
    - icon: "unreadable_characters"
      title: "Bảo vệ ký tự không thể đọc"
      content: "Bảo vệ hình mờ văn bản bằng cách sử dụng các ký tự không đọc được trong bản trình bày."

    # feature loop
    - icon: "watermark_text_search"
      title: "Tìm kiếm hình mờ trong tài liệu"
      content: "Tìm kiếm hình mờ dựa trên các tham số cụ thể hoặc bằng cách kết hợp nhiều tiêu chí."

    # feature loop
    - icon: "watermark_image_search"
      title: "Tìm hình mờ hình ảnh tương tự"
      content: "Tìm hình mờ hình ảnh giống với một hình ảnh cụ thể."

    # feature loop
    - icon: "document_info"
      title: "Nhận thông tin tài liệu"
      content: "Trích xuất thiết lập trang theo chương trình và thông tin khác cho các định dạng được hỗ trợ."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Mẫu mã"
  description: "Một số trường hợp sử dụng của hoạt động GroupDocs.Watermark for .NET điển hình"
  items:
    # code sample loop
    - title: "Hình mờ bằng cách thêm hình ảnh vào tài liệu."
      content: |
        Để bảo vệ bất kỳ tài liệu nào, bạn có thể sử dụng [hình mờ hình ảnh](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/):
        {{< landing/code title="Cách bảo vệ tệp bằng hình mờ hình ảnh.">}}
        ```csharp {style=abap}
        // Tải tài liệu nguồn vào Watermarker
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Chỉ định đường dẫn đến hình ảnh hình mờ
            using (ImageWatermark watermark = new ImageWatermark("watermark.jpg"))
            {
                // Bảo vệ tập tin và lưu nó
                watermarker.Add(watermark);

                watermarker.Save("result.pdf");
            }
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Tìm kiếm và sửa đổi hình mờ hiện có."
      content: |
        GroupDocs.Watermark có thể [sửa đổi hình mờ](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/) đã được trình bày trong tài liệu. Tìm kiếm các mục mong muốn và cập nhật thuộc tính của chúng.
        {{< landing/code title="Tìm kiếm và sửa đổi hình mờ.">}}
        ```csharp {style=abap}   
        // Tải tài liệu nguồn
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Tìm kiếm hình mờ để được cập nhật
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                // Cập nhật các thuộc tính mong muốn
                watermark.Text = "New Text";
            }

            // Lưu tài liệu đã sửa đổi vào một đường dẫn được chỉ định
            watermarker.Save("document.pdf");
        }
        ```
        {{< /landing/code >}}

---
