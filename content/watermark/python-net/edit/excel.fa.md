
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: fa
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "واترمارک‌ها را در فایل‌های Excel ویرایش کنید"
head_description: "با GroupDocs.Watermark for Python via .NET، می‌توانید به سادگی تنظیمات واترمارک را برای حفاظت و شخصی‌سازی اسناد خود تنظیم کنید."

############################# Header ############################
title: "واترمارک‌های Excel را با استفاده از Python بروزرسانی کنید" 
description: "اسناد اکسل خود را با ابزارهای ویرایش واترمارک منعطف ما برای Python محافظت کنید."
subtitle: "GroupDocs.Watermark for Python via .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "رایگان در PyPi دریافت کنید"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET Library"
    link: "/watermark/python-net/"
    link_title: "بیشتر بدانید"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **واترمارک‌های Excel را به سرعت ویرایش کنید:** GroupDocs.Watermark for Python via .NET به توسعه‌دهندگان Python تمام ابزارهای مورد نیاز برای مدیریت واترمارک‌ها با حداقل تلاش را می‌دهد و جریان کار و ایمنی اسناد شما را بهبود می‌بخشد.

############################# Steps ############################
steps:
    enable: true
    title: "واترمارک‌ها را در اسناد Excel با Python ویرایش کنید"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** به توسعه‌دهندگان Python امکان می‌دهد تا به سادگی واترمارک‌ها را در فایل‌های مختلف Excel بروزرسانی کنند. در اینجا نحوه استفاده از آن در پروژه شما آورده شده است:
      
      1. ابتدا فایل Excel خود را با ارسال آن به سازنده **Watermarker** باز کنید. می‌توانید از مسیر فایل، جریان بایت یا جریان فایل استفاده کنید.
      2. سپس، واترمارک‌هایی را که می‌خواهید تغییر دهید با استفاده از **SearchCriteria** پیدا کنید، که به شما امکان می‌دهد متن یا ویژگی‌های واترمارک را جستجو کنید.
      3. پس از پیدا کردن، می‌توانید جزئیاتی مانند متن، فونت، اندازه، موقعیت، رنگ و موارد دیگر را تغییر دهید. این به شما کنترل کامل بر روی ظاهر واترمارک می‌دهد.
      4. پس از انجام تغییرات، مدرک را ذخیره کنید. می‌توانید نتیجه را به یک جریان یا مسیر فایل بنویسید.
   
    code:
      platform: "python-net"
      copy_title: "کپی کردن"
      install:
        command: |
        command: "pip install groupdocs-watermark-net"
        copy_tip: "برای کپی کلیک کنید"
        copy_done: "کپی شده"
      links:
        #  loop
        - title: "نمونه های بیشتر"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
        #  loop
        - title: "مستندات"
          link: "https://docs.groupdocs.com/watermark/python-net/"
          
      content: |
        ```python {style=abap}
        # متن واترمارک را در EXCEL بروزرسانی کنید
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # یک Watermarker با استفاده از فایل EXCEL ایجاد کنید
        with gw.Watermarker("input.xslx") as watermarker:

            # برای پیدا کردن متن واترمارک، TextSearchCriteria را تنظیم کنید
            search_criteria = gwss.TextSearchCriteria("test", False)

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # متن واترمارک را تغییر دهید
                        watermark.text = "passed"
                    except Exception as e:
                        pass
            
            watermarker.save("output.xslx")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "راه‌های بیشتری برای بروزرسانی واترمارک‌ها را کشف کنید"
  description: "با کتابخانه ما، برنامه‌های Python می‌توانند واترمارک‌ها را در انواع فرمت‌های فایل اضافه، پیدا، ویرایش یا حذف کنند."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "ویرایش واترمارک"
  features:
    # feature loop
    - title: "واترمارک پرونده‌های خود را به راحتی انجام دهید"
      content: "از GroupDocs.Watermark for Python via .NET برای افزودن و مدیریت واترمارک‌ها در اسناد خود استفاده کنید. واترمارک‌ها را با استفاده از یک API ساده جستجو، بروزرسانی یا حذف کنید."

    # feature loop
    - title: "واترمارک‌ها را به صورت دلخواه تنظیم کنید"
      content: "با استفاده از API انعطاف‌پذیر ما، تنظیمات واترمارک مانند فونت، اندازه، جهت‌گیری و رنگ را تنظیم کنید تا دقیقاً نتیجه‌ای که می‌خواهید را بدست آورید."

    # feature loop
    - title: "از ویژگی‌های خاص فرمت استفاده کنید"
      content: "بسته به فرمت فایل، می‌توانید از ویژگی‌های بومی مانند سربرگ‌ها، پاورقی‌ها، حاشیه‌نویسی‌ها یا پس‌زمینه‌ها به عنوان نواحی واترمارک استفاده کنید."
      
  code_samples:
    # code sample loop
    - title: "ویرایش واترمارک متنی در اکسل"
      content: |
        این کد نشان می‌دهد که چگونه متن واترمارک را در صفحات گسترده اکسل تغییر دهید.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # فایل XLSX را باز کنید
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # داده‌های صفحه گسترده را بخوانید
        with gw.Watermarker("source.xlsx") as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,3]

            # متن واترمارک را تغییر دهید
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
        
            # نتیجه را ذخیره کنید
            watermarker.save("output.xlsx")
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "آماده شروع هستید؟"
  description: "ویژگی های GroupDocs.Watermark را به صورت رایگان امتحان کنید یا مجوز درخواست کنید"
  items:
    #  loop
    - title: "PyPi دانلود"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      color: "red"
        #  loop
    - title: "صدور مجوز"
      link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "واترمارک‌ها را در فرمت‌های دیگر بروزرسانی کنید"
    exclude: "EXCEL"
    description: "با استفاده از GroupDocs.Watermark for Python via .NET، به راحتی تنظیمات واترمارک را در فرمت‌های مختلف فایل سفارشی کنید."
    items: 
        # format loop 1
        - name: "واترمارک PDF"
          format: "PDF"
          link: "/watermark/python-net/edit//pdf/"
          description: "ادوبی Portable فرمت سند"

        # format loop 2
        - name: "واترمارک Word"
          format: "WORD"
          link: "/watermark/python-net/edit//word/"
          description: "MS Word و اسناد آفیس باز"
          
        # format loop 3
        - name: "واترمارک Excel"
          format: "EXCEL"
          link: "/watermark/python-net/edit//excel/"
          description: "MS Excel و صفحات گسترده آفیس باز"

        # format loop 4
        - name: "واترمارک PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/edit//powerpoint/"
          description: "MS PowerPoint و ارائه های آفیس باز"

        # format loop 5
        - name: "واترمارک DOCX"
          format: "DOCX"
          link: "/watermark/python-net/edit//docx/"
          description: "مایکروسافت Word سند XML باز"
          
        # format loop 6
        - name: "واترمارک PPTX"
          format: "PPTX"
          link: "/watermark/python-net/edit//pptx/"
          description: "PowerPoint ارائه اکس‌ام‌ال باز"
          
        # format loop 7
        - name: "واترمارک XLSX"
          format: "XLSX"
          link: "/watermark/python-net/edit//xlsx/"
          description: "مایکروسافت Excel صفحه گسترده XML باز"

        # format loop 8
        - name: "واترمارک DOC"
          format: "DOC"
          link: "/watermark/python-net/edit//doc/"
          description: "سند مایکروسافت Word 97 - 2007"

        # format loop 9
        - name: "واترمارک XLS"
          format: "XLS"
          link: "/watermark/python-net/edit//xls/"
          description: "مایکروسافت Excel کتاب کار 97-2003"

        # format loop 10
        - name: "واترمارک PPT"
          format: "PPT"
          link: "/watermark/python-net/edit//ppt/"
          description: "PowerPoint ارائه ۹۷—۲۰۰۳"

        # format loop 11
        - name: "واترمارک RTF"
          format: "RTF"
          link: "/watermark/python-net/edit//rtf/"
          description: "فرمت متن غنی"

---