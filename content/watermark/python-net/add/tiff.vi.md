
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:29
draft: false
lang: vi
format: Tiff
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Thêm Watermark vào TIFF bằng Python"
head_description: "Tạo và thêm watermark vào hình ảnh TIFF trong Python để bảo vệ tệp số của bạn."

############################# Header ############################
title: "Tạo Watermark cho TIFF với Python" 
description: "Thêm watermark mạnh mẽ, tùy chỉnh vào các tệp TIFF trong Python—lý tưởng cho các kho lưu trữ số và nhiếp ảnh gia."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Nhận miễn phí tại PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET là một bộ công cụ Python để thêm watermark vào các tệp TIFF. Chọn watermark văn bản hoặc hình ảnh, thiết lập độ trong suốt, kích thước và vị trí, và giữ cho hình ảnh của bạn an toàn. Với các tính năng như xếp chồng watermark và định dạng thông minh, GroupDocs.Watermark là một công cụ cần thiết cho bất kỳ ai cần bảo vệ bộ sưu tập hình ảnh của họ.

############################# Steps ############################
steps:
    enable: true
    title: "Nhanh chóng thêm Watermark vào tệp Tiff"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/):** Một thư viện Python mạnh mẽ cho phép bạn thêm watermark vào tài liệu của bạn.
      
      1. **Lớp chính: Watermarker.** Bắt đầu bằng cách tạo một đối tượng **Watermarker**. Cung cấp cho nó tệp Tiff của bạn, dưới dạng đường dẫn tệp hoặc luồng, để bắt đầu.
      2. **Xây dựng watermark của bạn.** Tiếp theo, tạo một đối tượng Watermark của loại bạn muốn. Bạn có thể đặt nó trên bất kỳ trang nào hoặc thậm chí trong các phần của tài liệu như hình ảnh hoặc tiêu đề.
      3. **Điều chỉnh diện mạo.** Thiết lập kích thước, vị trí, font chữ và màu sắc của watermark để phù hợp với nhu cầu của bạn.
      4. **Thêm và lưu.** Sử dụng phương thức **Watermarker** để chèn watermark của bạn. Thêm bất kỳ số lượng nào bạn muốn, sau đó lưu tệp ở bất kỳ đâu bạn thích.
   
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
        # Thêm một hình ảnh làm watermark vào một tệp TIFF
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # Truyền đường dẫn tệp vào chung cho Watermarker
        with gw.Watermarker("input.tiff") as watermarker:

            # Tạo một watermark hình ảnh bằng tệp hình ảnh của bạn
            watermark = gww.ImageWatermark("watermark.png")

            watermarker.add(watermark)

            # Lưu tệp TIFF với watermark
            watermarker.save("output.tiff")
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "Khám phá thêm các công cụ Watermark"
  description: "GroupDocs.Watermark for Python via .NET cung cấp các tùy chọn nâng cao để thêm và tùy chỉnh watermark trong nhiều định dạng tệp. Bảo vệ tài liệu và hình ảnh của bạn với các tính năng linh hoạt và dễ sử dụng."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Watermark tất cả trong một"
  features:
    # feature loop
    - title: "Lợp toàn trang"
      content: "Bao phủ toàn bộ tài liệu của bạn bằng các watermark lặp lại. Điều này làm cho việc loại bỏ watermark trở nên khó khăn và giữ cho tệp của bạn được bảo vệ mà không làm hỏng bố cục."

    # feature loop
    - title: "Màu tùy chỉnh"
      content: "Chọn bất kỳ màu nào cho watermark của bạn để phù hợp với thương hiệu hoặc kiểu tài liệu của bạn. Tạo cho watermark của bạn nổi bật hoặc hòa mình vào như cần thiết."

    # feature loop
    - title: "Tùy chọn bảo mật bổ sung"
      content: "Nâng cao bảo mật tài liệu của bạn với các watermark chồng lớp. Kết hợp các dấu hiệu rõ ràng và ẩn để ngăn chặn việc sao chép và đảm bảo chỉ những người phù hợp có thể truy cập tài liệu của bạn."
      
  code_samples:
    # code sample loop
    - title: "Thêm Watermark vào PowerPoint"
      content: |
        Mẫu này cho thấy cách đặt watermark trên nền của các trang PPTX.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.presentation as gwop

        # Mở một tệp PPTX
        load_options = gwop.PresentationLoadOptions()
        with gw.Watermarker("source.pptx", load_options) as watermarker:

            # Thiết lập chi tiết watermark
            with TextWatermark("Protected image", gww.Font("Arial", 8.0)) as watermark:

                watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
                watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
                watermark.rotate_angle = 45
                watermark.scale_factor = 1

                # Áp dụng watermark vào nền các trang
                watermarker.add(watermark)

                # Lưu bài thuyết trình đã cập nhật
                watermarker.save("result.pptx")
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
    title: "Bảo vệ hình ảnh TIFF với Watermark Python"
    exclude: "TIFF"
    description: "Thêm và quản lý watermark trong các tệp TIFF trong Python để giữ cho hình ảnh của bạn an toàn và dưới sự kiểm soát của bạn."
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