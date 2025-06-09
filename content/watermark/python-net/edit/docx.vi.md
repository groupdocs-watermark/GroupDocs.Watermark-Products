
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:29
draft: false
lang: vi
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Chỉnh sửa Watermark tùy chỉnh trong các tệp Docx"
head_description: "Tùy chỉnh nội dung watermark trong các tệp Docx bằng các công cụ GroupDocs.Watermark for Python via .NET để đáp ứng nhu cầu thương hiệu."

############################# Header ############################
title: "Tùy chỉnh Watermark Docx trong các Dự án Python của bạn" 
description: "Chỉnh sửa và quản lý watermark trên nhiều loại tài liệu khác nhau một cách dễ dàng với GroupDocs.Watermark for Python via .NET."
subtitle: "GroupDocs.Watermark for Python via .NET Bộ API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Truy cập qua PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Các công cụ Watermark Linh hoạt:** Thích ứng và cá nhân hóa việc watermark qua các định dạng bằng cách sử dụng GroupDocs.Watermark for Python via .NET trong quy trình Python của bạn.

############################# Steps ############################
steps:
    enable: true
    title: "Sử dụng API Python để Chỉnh sửa Watermark trong Tài liệu Docx"
    content: |
      Với **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)**, các nhà phát triển Python có thể thay đổi nội dung watermark trong nhiều tài liệu Docx khác nhau. Dưới đây là một hướng dẫn nhanh: 
      
      1. Bắt đầu bằng cách tải tài liệu Docx bằng cách sử dụng lớp **Watermarker**, chấp nhận các đường dẫn tệp, dòng bộ nhớ hoặc mảng byte làm đầu vào.
      2. Xây dựng một đối tượng **SearchCriteria** để tìm kiếm các phần tử watermark hiện có trong tài liệu của bạn, bất kể là văn bản hay đồ họa.
      3. Khi đã xác định, công cụ sẽ cung cấp một tập hợp các thể hiện watermark đã khớp mà bạn có thể cập nhật—điều chỉnh các tham số như màu sắc, căn chỉnh, phông chữ hoặc thậm chí dữ liệu hình ảnh nhúng.
      4. Hoàn thành quá trình bằng cách lưu tài liệu đã sửa đổi của bạn vào ổ đĩa hoặc bất kỳ dòng xuất hỗ trợ nào bằng cách sử dụng các phương thức lưu tích hợp.
   
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
        # Cập nhật watermark hình ảnh trong tệp DOCX
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Tạo một thể hiện Watermarker với tệp đầu vào
        with gw.Watermarker("input.docx") as watermarker:

            # Sử dụng SearchCriteria để xác định các watermark dựa trên hình ảnh
            search_criteria = gwss.ImageDctHashSearchCriteria("logo.png")

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # Áp dụng thay đổi cho watermark hình ảnh
                        watermark.ImageData = imageData
                    except Exception as e:
                        pass

            # Xuất tệp DOCX đã cập nhật
            watermarker.save("output.docx")
        ```     

############################# More features ############################
more_features:
  enable: true
  title: "Tăng hiệu suất với các công cụ watermarking nâng cao"
  description: "Thúc đẩy thương hiệu và bảo vệ tài liệu trong Python với API watermarking động của chúng tôi. Chèn, phát hiện, chỉnh sửa hoặc xóa các lớp watermark với nỗ lực tối thiểu."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Quy trình chỉnh sửa Watermark Nâng cao"
  features:
    # feature loop
    - title: "Kiểm soát Watermark Tích hợp"
      content: "Mang lại toàn bộ kiểm soát vòng đời watermark cho các ứng dụng Python của bạn bằng cách sử dụng GroupDocs.Watermark for Python via .NET. Tránh những công việc lặp đi lặp lại bằng cách tự động hóa việc thiết lập, cập nhật và xóa watermark."

    # feature loop
    - title: "Tùy chỉnh chính xác các thuộc tính Watermark"
      content: "Kiểm soát hoàn toàn các yếu tố thẩm mỹ của watermark—thay đổi kích thước, thay đổi màu, xoay hoặc điều chỉnh vị trí để đáp ứng bất kỳ yêu cầu hình ảnh nào với bề mặt API linh hoạt của chúng tôi."

    # feature loop
    - title: "Tận dụng các tính năng định dạng gốc"
      content: "Thích ứng với bất kỳ định dạng tệp nào bằng cách nhúng watermark vào tiêu đề, chân trang, chú thích hoặc nền. API của chúng tôi tôn trọng cấu trúc gốc để tích hợp tối ưu."
      
  code_samples:
    # code sample loop
    - title: "Chỉnh sửa Watermark trong một tệp PDF"
      content: |
        Minh họa cách thay đổi các thuộc tính watermark trong tài liệu PDF.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # Mở tệp PDF
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.pdf as gwop

        # Đọc nội dung watermark
        load_options = gwop.PdfLoadOptions()
        with gw.Watermarker("source.pdf", load_options) as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,5,8]

            # Áp dụng cập nhật watermark
            watermarks = watermarker.search(search_criteria)
            for watermark in watermarks:
                try:
                    watermark.formatted_text_fragments.clear()
                    watermark.formatted_text_fragments.add(
                        "New text", 
                        gww.Font("Calibri", 5.0, gww.FontStyle.bold), 
                        gww.Color.white, 
                        gww.Color.aqua
                    )
                except Exception as e:
                    pass
        
            # Lưu kết quả đã chỉnh sửa
            watermarker.save("output.pdf")
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
    title: "Kiểm soát Watermark cho các Định dạng Khác"
    exclude: "DOCX"
    description: "Sử dụng các công cụ chỉnh sửa watermark đồng nhất trên tất cả các loại tệp hỗ trợ bằng GroupDocs.Watermark for Python via .NET."
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