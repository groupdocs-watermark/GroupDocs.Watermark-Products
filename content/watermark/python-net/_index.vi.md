---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:49
draft: false

lang: vi
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

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
    # supported_platforms loop
    - title: "Python"
      tag: "python-net"

############################# Head ############################
head_title: "Thư viện hình chìm mờ Python | Hình mờ tài liệu"
head_description: "Python bảo vệ tài liệu kinh doanh bằng hình mờ văn bản và hình ảnh. Các định dạng tệp như PDF, Word, Excel và PowerPoint đều được hỗ trợ."

############################# Header ############################
title: "Truy cập công nghệ hình mờ Python via .NET"
description: "Bảo vệ dữ liệu của bạn và ngăn chặn việc sao chép trái phép bằng giải pháp Python này. Dễ dàng thêm hình mờ vào tài liệu kinh doanh ở nhiều định dạng khác nhau, bao gồm PDF, Word, Excel, PowerPoint, hình ảnh, v.v."
words:
  for: "cho"

actions:
  main: "PyPi tải xuống miễn phí"
  main_link: "https://pypi.org/project/groupdocs-watermark-net/"
  alt: "Cấp phép"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
  title: "Sẵn sàng để bắt đầu?"
  description: "Dùng thử GroupDocs.Watermark tính năng miễn phí hoặc yêu cầu giấy phép"

release:
  title: "Phiên bản {0} đã phát hành"
  notes: "Xem những gì mới"
  downloads: "Tải xuống"
  link: "https://releases.groupdocs.com/watermark/python-net/"

code:
  title: "Thêm Hình mờ vào PDF bằng cách sử dụng Python"
  more: "Thêm ví dụ"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
  install: "pip install groupdocs-watermark-net"
  content: |
    ```python {style=abap}

    import groupdocs.watermark as gw
    import groupdocs.watermark.watermarks as gww
    import groupdocs.watermark.options.pdf as gwop
    import groupdocs.watermark.common as gwc

    # Thực hiện Watermarker đi qua đường dẫn PDF
    pdf_lo = gwop.PdfLoadOptions()
    with gw.Watermarker("source.pdf", pdf_lo) as watermarker:
        options = gwop.PdfArtifactWatermarkOptions()

        # Tùy chỉnh tùy chọn hình mờ
        text_watermark = 
            gww.TextWatermark("Approved", gww.Font("Arial", 8.0))
        text_watermark.horizontal_alignment = 
            gwc.HorizontalAlignment.RIGHT

        # Áp dụng hình mờ cho tài liệu PDF
        watermarker.add(text_watermark, options)

        # Lưu tài liệu kết quả
        watermarker.save("result.pdf")

    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark trong nháy mắt"
  description: "Thư viện Python dành cho hình chìm mờ"
  features:
    # feature loop
    - title: "Hình mờ tài liệu Python"
      content: "Bảo mật dữ liệu nhạy cảm của bạn với GroupDocs.Watermark for Python via .NET. Đặt văn bản hoặc hình ảnh trên các định dạng tệp khác nhau làm hình mờ."

    # feature loop
    - title: "Tùy chỉnh hình mờ"
      content: "Nhiều tùy chọn tùy chỉnh có sẵn trong GroupDocs.Watermark for Python via .NET. Thiết lập kiểu văn bản (đậm, in nghiêng, phông chữ) hoặc các thuộc tính hình ảnh như kích thước hoặc xoay để điều chỉnh hình mờ tài liệu."

    # feature loop
    - title: "Hỗ trợ các định dạng tệp phổ biến"
      content: "GroupDocs.Watermark for Python via .NET hỗ trợ nhiều định dạng tệp, bao gồm PDF, tài liệu MS Office như Word, Excel, PowerPoint và các hình ảnh như JPEG, PNG, GIF, BMP, sơ đồ Visio, email, v.v. bàn thắng."

    # feature loop
    - title: "Tìm kiếm và cập nhật hình mờ"
      content: "Truy xuất và cập nhật hình mờ được đặt trong tài liệu. Sửa đổi kiểu văn bản, nội dung hình ảnh hoặc xóa chúng hoàn toàn. GroupDocs.Watermark for Python via .NET cung cấp nhiều khả năng xử lý hình mờ."

############################# Platforms ############################
platforms:
  enable: true
  title: "Độc lập nền tảng"
  description: "GroupDocs.Watermark for Python via .NET tích hợp liền mạch với nhiều hệ điều hành và trình quản lý gói khác nhau."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Định dạng tập tin được hỗ trợ"
  description: |
    GroupDocs.Watermark for Python via .NET cho phép bạn xử lý nhiều định dạng tệp khác nhau. [Khám phá danh sách đầy đủ](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "Tính năng của GroupDocs.Watermark for Python via .NET"
  description: "Tăng cường bảo mật tài liệu thông qua hình mờ có lập trình. Xử lý các định dạng tệp đa dạng bao gồm PDF, DOCX, XLSX, PPTX và các định dạng hình ảnh (PNG, JPG, v.v.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Kiểm soát hình mờ chính xác"
      content: "Quản lý chính xác hình mờ bằng cách thêm hoặc xóa chúng khỏi các phần cụ thể, toàn bộ tài liệu hoặc các tệp đính kèm và hình dạng riêng lẻ trong các định dạng tệp khác nhau."

    # feature loop
    - icon: "watermark_style"
      title: "Tùy chỉnh hình mờ"
      content: "Thực hiện kiểm soát chi tiết đối với tính thẩm mỹ của hình mờ bằng cách sửa đổi các thuộc tính như màu sắc, phông chữ, độ mờ, xoay và định vị trong tài liệu."

    # feature loop
    - icon: "hidden_print"
      title: "In hình mờ PDF"
      content: "Thêm hình mờ ẩn vào tài liệu thông thường, hình mờ này chỉ hiển thị trong quá trình in, tăng cường bảo mật tài liệu một cách kín đáo."

    # feature loop
    - icon: "image_only"
      title: "Hình mờ hình ảnh cụ thể"
      content: "Tạo hình mờ cho các hình ảnh cụ thể trong tài liệu bằng giải pháp của chúng tôi. Nhúng hình mờ vào một phần được chỉ định (ví dụ: trang, trang trình bày) hoặc trên toàn bộ tài liệu."

    # feature loop
    - icon: "image_frame"
      title: "Hình mờ hình ảnh nhiều lớp"
      content: "Thêm hình mờ chính xác vào các khung cụ thể trong định dạng hình ảnh nhiều khung, đạt được khả năng kiểm soát chi tiết đối với vị trí hình mờ."

    # feature loop
    - icon: "attachments"
      title: "Bảo vệ nội dung toàn diện"
      content: "Mở rộng khả năng bảo vệ cho các thành phần tài liệu khác nhau như tệp đính kèm trong tài liệu Excel và hình ảnh trong bản trình bày, cung cấp thêm lớp bảo mật."

    # feature loop
    - icon: "pdf_objects"
      title: "Hình mờ PDF nâng cao"
      content: "Hình mờ các khu vực khác nhau của tệp PDF, bao gồm Bleed Box, Art Box, Crop Box, Trim Box, v.v."

    # feature loop
    - icon: "doc_background"
      title: "Hình mờ hình nền"
      content: "Quản lý hình mờ trong ảnh nền của bảng tính và bản trình bày, cung cấp các tùy chọn tùy chỉnh bổ sung cho các biện pháp bảo mật trực quan."

    # feature loop
    - icon: "unreadable_characters"
      title: "Hình mờ văn bản có ký tự không thể đọc được"
      content: "Sử dụng các ký tự không thể đọc được trong hình mờ văn bản được nhúng trong bản trình bày, tăng cường bảo mật bằng cách khiến việc trích xuất hình mờ trái phép trở nên khó khăn hơn đáng kể."

    # feature loop
    - icon: "watermark_text_search"
      title: "Tìm kiếm hình mờ nâng cao"
      content: "Sử dụng các tính năng tìm kiếm toàn diện để định vị hình mờ trong tài liệu dựa trên các thông số cụ thể hoặc bằng cách kết hợp nhiều tiêu chí khác nhau."

    # feature loop
    - icon: "watermark_image_search"
      title: "Phát hiện hình mờ hình ảnh tương tự"
      content: "Tìm hình ảnh hình mờ tương tự trong tài liệu trông giống với hình ảnh nguồn."

    # feature loop
    - icon: "document_info"
      title: "Phân tích thông tin tài liệu"
      content: "Trích xuất dữ liệu tài liệu cần thiết như thiết lập trang để phân tích thêm."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Mẫu mã"
  description: "Khám phá các ví dụ mã giới thiệu các chức năng phổ biến của GroupDocs.Watermark for Python via .NET."
  items:
    # code sample loop
    - title: "Hình mờ một tài liệu bằng hình ảnh"
      content: |
        Sử dụng GroupDocs.Watermark for Python via .NET để bảo vệ tài liệu bằng cách thêm hình mờ vào hình ảnh. [Tìm hiểu thêm](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Cách bảo vệ tệp bằng hình mờ hình ảnh.">}}
        ```python {style=abap}

        # Tải tài liệu nguồn vào Watermarker
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Chỉ định đường dẫn đến hình ảnh hình mờ
            watermark = groupdocs.watermark.watermarks.ImageWatermark("watermark.jpg")
            watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwgroupdocs.watermark.common.VerticalAlignment.CENTER

            # Bảo vệ tập tin và lưu nó
            watermarker.add(watermark)
            watermarker.save("result.pdf")
       
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Tìm kiếm và sửa đổi hình mờ hiện có"
      content: |
        GroupDocs.Watermark for Python via .NET trao quyền cho bạn quản lý hình mờ tài liệu. Chọn hình mờ và sửa đổi thuộc tính của chúng. [Khám phá cách thực hiện](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Tìm kiếm và sửa đổi hình mờ.">}}
        ```python {style=abap}

        # Tải tài liệu nguồn
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Tìm kiếm hình mờ để được cập nhật
            search_criteria = groupdocs.watermark.search.searchcriteria.TextSearchCriteria("annotation", False)
            watermarks = watermarker.search(search_criteria)
            
            # Cập nhật các thuộc tính mong muốn
            for watermark in watermarks:
                watermark.text = "passed"

            # Lưu tài liệu đã sửa đổi vào một đường dẫn được chỉ định
            watermarker.save("result.pdf")


        ```
        {{< /landing/code >}}

---
