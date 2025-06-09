
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: vi
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Thêm Watermark vào Thuyết Trình"
head_description: "Dễ dàng thêm watermark vào slide PowerPoint của bạn để tăng cường bảo mật."

############################# Header ############################
title: "Watermark Nâng Cao cho Thuyết Trình trong Python" 
description: "Thêm watermark văn bản và hình ảnh vào slide PowerPoint bằng API Python của chúng tôi. Tuyệt vời để giữ cho các bài thuyết trình của bạn an toàn và chuyên nghiệp."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống PyPi miễn phí"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET cho phép bạn thêm watermark nâng cao vào các bài thuyết trình PowerPoint trong Python. Bảo vệ thông tin bí mật hoặc thêm logo công ty của bạn vào các slide. Bạn có thể thêm watermark vào các slide đơn lẻ hoặc toàn bộ bài thuyết trình, và điều chỉnh cách chúng trông và vị trí xuất hiện.

############################# Steps ############################
steps:
    enable: true
    title: "Thêm Watermark: Watermarking Python cho Powerpoint"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** là một thư viện giúp thêm watermark vào nhiều loại tệp kinh doanh. Làm theo các bước sau để nhanh chóng thêm watermark vào tài liệu của bạn trong Python:
      
      1. **Bắt đầu với Watermarking:** Bắt đầu bằng cách tạo một thể hiện của lớp **Watermarker**. Truyền tệp Powerpoint của bạn (dưới dạng đường dẫn hoặc luồng) vào trình khởi tạo để mở nó cho việc thêm watermark.
      2. **Tạo Watermark của bạn:** Tạo một đối tượng **Watermark** với văn bản và cài đặt mong muốn của bạn. Bạn có thể thêm watermark vào bất kỳ trang nào hoặc thậm chí vào các phần của tài liệu như đầu trang hoặc tệp đính kèm.
      3. **Tùy chỉnh Watermark:** Điều chỉnh kích thước, vị trí, kiểu chữ, màu sắc và căn chỉnh của watermark để phù hợp với nhu cầu của bạn. Điều này giúp watermark trông thật hoàn hảo trong tài liệu của bạn.
      4. **Áp dụng và Lưu:** Sử dụng phương thức **Watermarker** để thêm watermark(s) của bạn vào tài liệu. Lưu lại kết quả, lý tưởng là vào một tệp mới để bảo đảm.
   
    code:
      platform: "python-net"
      copy_title: "Sao chép"
      install:
        command: |
        command: "pip install groupdocs-watermark-net"
        copy_tip: "bấm để sao chép"
        copy_done: "sao chép"
      links:
        #  loop
        - title: "Thêm ví dụ"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
        #  loop
        - title: "Tài liệu"
          link: "https://docs.groupdocs.com/watermark/python-net/"
          
      content: |
        ```python {style=abap}
        # Thêm một watermark văn bản vào tệp POWERPOINT
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # Chọn tệp mà bạn muốn thêm watermark
        with gw.Watermarker("input.pptx") as watermarker:

            # Tạo một đối tượng watermark văn bản
            font = gww.Font("Arial", 36.0)
            watermark = gww.TextWatermark("top secret", font)
            watermark.foreground_color = gww.Color.red
            watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
            watermark.opacity = 0.4

            watermarker.add(watermark)

            # Lưu tệp POWERPOINT đã cập nhật
            watermarker.save("output.pptx")
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Khám Phá Thêm Các Tính Năng Watermarking"
  description: "Sử dụng API Python của chúng tôi để thêm, xem, chuyển đổi và quản lý watermark trong tài liệu, slide, sơ đồ và nhiều hơn nữa. GroupDocs.Watermark for Python via .NET giúp bạn bảo vệ tệp và thêm thông tin bản quyền một cách dễ dàng."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Thêm Watermark"
  features:
    # feature loop
    - title: "Thêm Watermark Một Cách Dễ Dàng"
      content: "GroupDocs.Watermark cho phép các nhà phát triển Python nhanh chóng thêm watermark văn bản, hình ảnh hoặc động vào các tài liệu kinh doanh. Giữ cho tệp của bạn an toàn và mang thương hiệu với nỗ lực tối thiểu."

    # feature loop
    - title: "Watermark Đầy Đủ Tùy Chỉnh"
      content: "Thay đổi kích cỡ, độ xoay, độ trong suốt, màu sắc và kiểu chữ của watermark bằng GroupDocs.Watermark. Làm cho watermark của bạn phù hợp hoàn hảo với tài liệu và giữ cho nội dung quan trọng rõ ràng."

    # feature loop
    - title: "Sử Dụng Các Tính Năng Tài Liệu Để Watermarking"
      content: "Tận dụng các tính năng tài liệu tích hợp như chú thích PDF, nền Word, hoặc đầu trang Excel để thêm watermark. GroupDocs.Watermark hoạt động với cấu trúc tài liệu để tạo watermark hiệu quả, không gây ảnh hưởng."
      
  code_samples:
    # code sample loop
    - title: "Thêm Watermark Hình Ảnh vào DOCX"
      content: |
        Ví dụ này cho thấy cách áp dụng hiệu ứng hình ảnh cho watermark hình dạng.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.wordprocessing as gwow

        # Mở một tài liệu Word
        load_options = gwow.WordProcessingLoadOptions()
        with gw.Watermarker("source.docx", load_options) as watermarker:

            # Đặt các tùy chọn watermark
            with gww.ImageWatermark("logo.png") as watermark:

                effects = gwow.WordProcessingImageEffects()
                effects.brightness = 0.7
                effects.contrast = 0.6
                effects.chroma_key = gww.Color.red

                options = gwow.WordProcessingWatermarkSectionOptions()
                options.Effects = effects;

                # Tạo watermark
                watermarker.add(watermark, options)

                # Lưu tài liệu với watermark
                watermarker.save("result.docx")
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Sẵn sàng để bắt đầu?"
  description: "Dùng thử GroupDocs.Watermark tính năng miễn phí hoặc yêu cầu giấy phép"
  items:
    #  loop
    - title: "PyPi tải về"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      color: "red"
        #  loop
    - title: "Cấp phép"
      link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Watermark Các Bài Thuyết Trình với Python"
    exclude: "POWERPOINT"
    description: "Sử dụng bộ công cụ Python của chúng tôi để nhanh chóng thêm watermark vào các tệp PowerPoint. Giữ cho các slide của bạn an toàn và trông sắc nét."
    items: 
        # format loop 1
        - name: "Hình mờ PDF"
          format: "PDF"
          link: "/watermark/python-net/add//pdf/"
          description: "Định dạng tài liệu Adobe Portable"

        # format loop 2
        - name: "Hình mờ Word"
          format: "WORD"
          link: "/watermark/python-net/add//word/"
          description: "MS Word và tài liệu Open Office"
          
        # format loop 3
        - name: "Hình mờ Excel"
          format: "EXCEL"
          link: "/watermark/python-net/add//excel/"
          description: "MS Excel và bảng tính Open Office"

        # format loop 4
        - name: "Hình ảnh hình mờ"
          format: "IMAGE"
          link: "/watermark/python-net/add//image/"
          description: "Định dạng hình ảnh phổ biến"

        # format loop 5
        - name: "Ảnh hình mờ"
          format: "PHOTO"
          link: "/watermark/python-net/add//photo/"
          description: "Định dạng ảnh"

        # format loop 6
        - name: "Hình mờ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/add//powerpoint/"
          description: "MS PowerPoint và các bài thuyết trình Open Office"

        # format loop 7
        - name: "Hình mờ DOCX"
          format: "DOCX"
          link: "/watermark/python-net/add//docx/"
          description: "Microsoft Word Tài liệu XML mở"
          
        # format loop 8
        - name: "Hình mờ PPTX"
          format: "PPTX"
          link: "/watermark/python-net/add//pptx/"
          description: "PowerPoint Bản trình bày XML mở"
          
        # format loop 9
        - name: "Hình mờ XLSX"
          format: "XLSX"
          link: "/watermark/python-net/add//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 10
        - name: "Hình mờ JPEG"
          format: "JPEG"
          link: "/watermark/python-net/add//jpeg/"
          description: "JPEG Hình ảnh"

        # format loop 11
        - name: "Hình mờ PNG"
          format: "PNG"
          link: "/watermark/python-net/add//png/"
          description: "Portable Đồ họa mạng"

        # format loop 12
        - name: "Hình mờ TIFF"
          format: "TIFF"
          link: "/watermark/python-net/add//tiff/"
          description: "Nhãn định dạng tệp hình ảnh"

        # format loop 13
        - name: "Hình mờ WEBP"
          format: "WEBP"
          link: "/watermark/python-net/add//webp/"
          description: "Hình ảnh WEB"

        # format loop 14
        - name: "Hình mờ DOC"
          format: "DOC"
          link: "/watermark/python-net/add//doc/"
          description: "Tài liệu Microsoft Word 97 - 2007"

        # format loop 15
        - name: "Hình mờ XLS"
          format: "XLS"
          link: "/watermark/python-net/add//xls/"
          description: "Microsoft Excel Sổ làm việc 97-2003"

        # format loop 16
        - name: "Hình mờ PPT"
          format: "PPT"
          link: "/watermark/python-net/add//ppt/"
          description: "PowerPoint Bài thuyết trình 97-2003"

        # format loop 17
        - name: "Hình mờ RTF"
          format: "RTF"
          link: "/watermark/python-net/add//rtf/"
          description: "Định dạng văn bản phong phú"

---