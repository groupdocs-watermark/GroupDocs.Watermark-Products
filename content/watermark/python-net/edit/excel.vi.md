
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:16
draft: false
lang: vi
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Chỉnh sửa Watermark trong các tệp Excel"
head_description: "Với GroupDocs.Watermark for Python via .NET, bạn có thể dễ dàng điều chỉnh các cài đặt watermark để bảo vệ và cá nhân hóa tài liệu của bạn."

############################# Header ############################
title: "Cập nhật Watermark trong Bảng tính Excel Sử dụng Python" 
description: "Bảo vệ bảng tính Excel của bạn với các công cụ chỉnh sửa watermark linh hoạt của chúng tôi dành cho Python."
subtitle: "GroupDocs.Watermark for Python via .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Nhận miễn phí trên PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET Thư viện"
    link: "/watermark/python-net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Chỉnh sửa Watermark Excel Nhanh Chóng:** GroupDocs.Watermark for Python via .NET cung cấp cho các nhà phát triển Python tất cả công cụ cần thiết để quản lý watermark với nỗ lực tối thiểu, cải thiện quy trình làm việc và an toàn tài liệu của bạn.

############################# Steps ############################
steps:
    enable: true
    title: "Chỉnh sửa watermark trong tài liệu Excel với Python"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** hỗ trợ các nhà phát triển Python cập nhật watermark trong nhiều tệp Excel khác nhau. Dưới đây là cách bạn có thể sử dụng nó trong dự án của bạn:
      
      1. Đầu tiên, mở tệp Excel của bạn bằng cách truyền nó vào bộ tạo **Watermarker**. Bạn có thể sử dụng đường dẫn tệp, luồng byte, hoặc luồng tệp.
      2. Tiếp theo, tìm các watermark bạn muốn thay đổi bằng cách sử dụng **SearchCriteria**, cho phép bạn tìm kiếm văn bản hoặc thuộc tính watermark.
      3. Khi đã tìm thấy, bạn có thể thay đổi các chi tiết như văn bản, phông chữ, kích thước, vị trí, màu sắc, và nhiều hơn nữa. Điều này giúp bạn kiểm soát hoàn toàn cách watermark hiển thị.
      4. Sau khi thực hiện các thay đổi, lưu tài liệu. Bạn có thể ghi kết quả vào một luồng hoặc một đường dẫn tệp.
   
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
        # Cập nhật văn bản watermark trong EXCEL
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Tạo một Watermarker bằng cách sử dụng tệp EXCEL
        with gw.Watermarker("input.xslx") as watermarker:

            # Thiết lập TextSearchCriteria để tìm văn bản watermark
            search_criteria = gwss.TextSearchCriteria("test", False)

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # Chỉnh sửa văn bản watermark
                        watermark.text = "passed"
                    except Exception as e:
                        pass
            
            watermarker.save("output.xslx")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Khám phá thêm cách để cập nhật watermark"
  description: "Thư viện của chúng tôi giúp các ứng dụng Python có thể thêm, tìm, chỉnh sửa hoặc xóa watermark trong nhiều loại tệp."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Chỉnh sửa Watermark"
  features:
    # feature loop
    - title: "Watermark Tài liệu của Bạn một Cách Dễ Dàng"
      content: "Sử dụng GroupDocs.Watermark for Python via .NET để thêm và quản lý watermark trong tài liệu của bạn. Tìm kiếm, cập nhật hoặc xóa watermark khi cần thiết bằng một API đơn giản."

    # feature loop
    - title: "Tùy Chỉnh Watermark theo Nhu Cầu của Bạn"
      content: "Điều chỉnh các cài đặt watermark như phông chữ, kích thước, hướng và màu sắc bằng API linh hoạt của chúng tôi để đạt được kết quả chính xác như mong muốn."

    # feature loop
    - title: "Sử Dụng Các Tính Năng Theo Định Dạng"
      content: "Tùy thuộc vào định dạng tệp, bạn có thể sử dụng các tính năng gốc như tiêu đề, chân trang, chú thích, hoặc nền làm vùng watermark."
      
  code_samples:
    # code sample loop
    - title: "Chỉnh sửa Watermark Văn bản trong Excel"
      content: |
        Đoạn mã này cho thấy cách thay đổi văn bản watermark trong bảng tính Excel.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # Mở tệp XLSX
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # Đọc dữ liệu bảng tính
        with gw.Watermarker("source.xlsx") as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,3]

            # Thay đổi văn bản watermark
            watermarks = watermarker.search(search_criteria)
            for watermark in watermarks:
                try:
                    watermark.formatted_text_fragments.clear()
                    watermark.formatted_text_fragments.add(
                       "passed", 
                        gww.Font("Calibri", 19.0, gww.FontStyle.bold), 
                        gww.Color.red, 
                        gww.Color.aqua
                    )
                except Exception as e:
                    pass
        
            # Lưu kết quả
            watermarker.save("output.xlsx")
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
    title: "Cập nhật Watermark trong Các Định Dạng Khác"
    exclude: "EXCEL"
    description: "Dễ dàng tùy chỉnh các cài đặt watermark trên nhiều định dạng tệp khác nhau bằng GroupDocs.Watermark for Python via .NET."
    items: 
        # format loop 1
        - name: "Hình mờ PDF"
          format: "PDF"
          link: "/watermark/python-net/edit//pdf/"
          description: "Định dạng tài liệu Adobe Portable"

        # format loop 2
        - name: "Hình mờ Word"
          format: "WORD"
          link: "/watermark/python-net/edit//word/"
          description: "MS Word và tài liệu Open Office"
          
        # format loop 3
        - name: "Hình mờ Excel"
          format: "EXCEL"
          link: "/watermark/python-net/edit//excel/"
          description: "MS Excel và bảng tính Open Office"

        # format loop 4
        - name: "Hình mờ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/edit//powerpoint/"
          description: "MS PowerPoint và các bài thuyết trình Open Office"

        # format loop 5
        - name: "Hình mờ DOCX"
          format: "DOCX"
          link: "/watermark/python-net/edit//docx/"
          description: "Microsoft Word Tài liệu XML mở"
          
        # format loop 6
        - name: "Hình mờ PPTX"
          format: "PPTX"
          link: "/watermark/python-net/edit//pptx/"
          description: "PowerPoint Bản trình bày XML mở"
          
        # format loop 7
        - name: "Hình mờ XLSX"
          format: "XLSX"
          link: "/watermark/python-net/edit//xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop 8
        - name: "Hình mờ DOC"
          format: "DOC"
          link: "/watermark/python-net/edit//doc/"
          description: "Tài liệu Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Hình mờ XLS"
          format: "XLS"
          link: "/watermark/python-net/edit//xls/"
          description: "Microsoft Excel Sổ làm việc 97-2003"

        # format loop 10
        - name: "Hình mờ PPT"
          format: "PPT"
          link: "/watermark/python-net/edit//ppt/"
          description: "PowerPoint Bài thuyết trình 97-2003"

        # format loop 11
        - name: "Hình mờ RTF"
          format: "RTF"
          link: "/watermark/python-net/edit//rtf/"
          description: "Định dạng văn bản phong phú"

---