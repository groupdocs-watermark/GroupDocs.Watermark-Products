
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:16
draft: false
lang: fa
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "شناسایی نشانه‌های پنهان در ارائه‌های Powerpoint"
head_description: "به راحتی واترمارک‌های پنهان را در اسلایدهای ارائه با GroupDocs.Watermark شناسایی کنید."

############################# Header ############################
title: "واترمارک‌ها را در ارائه‌های Powerpoint شناسایی کنید" 
description: "عناصر واترمارک را در داخل نمایش‌نامه‌ها با قابلیت‌های قابل اطمینان GroupDocs.Watermark for Python via .NET مدیریت کنید."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "نسخه آزمایشی رایگان در PyPi موجود است"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET چیست؟"
    link: "/watermark/python-net/"
    link_title: "بیشتر بدانید"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET به توسعه‌دهندگان امکان می‌دهد تا وظایف واترمارک را در Python انجام دهند. طراحی شده برای انعطاف‌پذیری، قابلیت‌های شناسایی، درج، ویرایش و حذف واترمارک‌ها را در فرمت‌هایی مانند PPTX، DOCX، و PDF فراهم می‌کند.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه به شناسایی واترمارک‌ها در فایل‌های Powerpoint از طریق Python بپردازیم"
    content: |
      با **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/python-net/)**، شناسایی واترمارک‌های جاسازی شده در اسناد تجاری شما بسیار ساده‌تر شده است. قابلیت‌های آن را به جریان‌های کاری Python خود اضافه کنید تا شناسایی بدون درز انجام شود.
      
      1. با بارگذاری سند Powerpoint به یک نمونه از کلاس **Watermarker** شروع کنید. ورودی به عنوان مسیر، جریان یا آرایه بایت پذیرفته می‌شود.
      2. محدوده جستجو را با استفاده از شی **SearchCriteria** تنگ کنید. برای پیدا کردن نشانه‌های مبتنی بر تصویر، از یک تصویر نمونه استفاده کنید. برای نشانه‌های متنی، ویژگی‌هایی مانند محتوی، سبک یا رنگ را مشخص کنید.
      3. متد **Search** را از شی **Watermarker** فراخوانی کنید تا داده‌های واترمارک استخراج شود. یک مجموعه از نمونه‌های واترمارک برای بررسی برگردانده خواهد شد.
      4. پس از بازیابی، می‌توانید نتایج را مدیریت کنید: نشانه‌های ناخواسته را حذف کرده یا جزئیاتی مانند ابعاد یا محتوای پیام را به روز کنید.
   
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
        # شناسایی واترمارک متنی در فرمت POWERPOINT
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # مقداردهی اولیه Watermarker با فایل POWERPOINT
        with gw.Watermarker("input.pptx") as watermarker:

            # اجرای جستجوی واترمارک
            search_criteria = gwss.TextSearchCriteria("test", False)
            possible_watermarks = watermarker.search(search_criteria)

            # پردازش لیست واترمارک‌های شناسایی شده
            print("\nFound {0} possible watermark(s).".format(len(possible_watermarks)))
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "شناسایی قدرتمند واترمارک با GroupDocs.Watermark"
  description: "از GroupDocs.Watermark در پروژه‌های Python خود برای اسکن و شناسایی عناصر واترمارک در انواع مختلف اسناد به طور مؤثر استفاده کنید."
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "شناسایی واترمارک‌ها"
  features:
    # feature loop
    - title: "شناسایی پیشرفته با فیلترهای هوشمند"
      content: "به راحتی واترمارک‌ها را در طیف گسترده‌ای از فرمت‌های سند شناسایی کنید. GroupDocs.Watermark از فیلتر کردن بر اساس ویژگی‌های بصری و متنی از جمله شکل، شفافیت و غیره پشتیبانی می‌کند."

    # feature loop
    - title: "معیارهای انعطاف‌پذیر برای جستجو"
      content: "پارامترهای جستجو برای واترمارک‌های شخصی‌سازی شده را با GroupDocs.Watermark تعریف کنید. این دقت امکان بازیابی هدفمند داده‌های واترمارک پنهان یا سفارشی را فراهم می‌آورد."

    # feature loop
    - title: "دسترسی و سازماندهی واترمارک‌های شناسایی شده"
      content: "با به دست آوردن تمام واترمارک‌های جاسازی شده، فرایند ممیزی اسناد را ساده کنید. ابزارهای ما امکان استخراج، نمایش و مدیریت مؤثر اقلام یافته را فراهم می‌آورند."
      
  code_samples:
    # code sample loop
    - title: "مثال کد: شناسایی واترمارک‌ها"
      content: |
        ببینید چگونه از GroupDocs.Watermark برای جستجوی اسناد برای محتوای واترمارک جاسازی شده استفاده کنید با استفاده از قوانین شناسایی انعطاف‌پذیر.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # مدارک هدف را از دیسک یا جریان باز کنید
        load_options = gwos.SpreadsheetLoadOptions()
        with gw.Watermarker("source.xlsx", load_options) as watermarker:

            # خصوصیات خاص واترمارک که باید در جستجو استفاده شود را تعریف کنید
            criteria = gwss.TextFormattingSearchCriteria()
            criteria.foreground_color_range = gwss.ColorRange()
            criteria.foreground_color_range.min_hue = -5.0
            criteria.foreground_color_range.max_hue = 10.0
            criteria.foreground_color_range.min_brightness = 0.01
            criteria.foreground_color_range.max_brightness = 0.99
            criteria.background_color_range = gwss.ColorRange()
            criteria.background_color_range.is_empty = True
            criteria.font_name = "Arial"
            criteria.min_font_size = 19.0
            criteria.max_font_size = 42.0
            criteria.font_bold = True

            # جستجو را انجام داده و مطابقت‌ها را جمع‌آوری کنید
            possible_watermarks = watermarker.search(criteria)

            # با نتایج پیدا شده برای اقدام بیشتر کار کنید
            print("Found {0} possible watermark(s).".format(len(possible_watermarks)))
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
    title: "سازگاری با فرمت‌های وسیع"
    exclude: "POWERPOINT"
    description: "از شناسایی بی‌نقص واترمارک در چندین فرمت ارائه و سند پشتیبانی شده لذت ببرید."
    items: 
        # format loop 1
        - name: "واترمارک PDF"
          format: "PDF"
          link: "/watermark/python-net/search//pdf/"
          description: "ادوبی Portable فرمت سند"

        # format loop 2
        - name: "واترمارک Word"
          format: "WORD"
          link: "/watermark/python-net/search//word/"
          description: "MS Word و اسناد آفیس باز"
          
        # format loop 3
        - name: "واترمارک Excel"
          format: "EXCEL"
          link: "/watermark/python-net/search//excel/"
          description: "MS Excel و صفحات گسترده آفیس باز"

        # format loop 4
        - name: "واترمارک PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/search//powerpoint/"
          description: "MS PowerPoint و ارائه های آفیس باز"

        # format loop 5
        - name: "واترمارک DOCX"
          format: "DOCX"
          link: "/watermark/python-net/search//docx/"
          description: "مایکروسافت Word سند XML باز"
          
        # format loop 6
        - name: "واترمارک PPTX"
          format: "PPTX"
          link: "/watermark/python-net/search//pptx/"
          description: "PowerPoint ارائه اکس‌ام‌ال باز"
          
        # format loop 7
        - name: "واترمارک XLSX"
          format: "XLSX"
          link: "/watermark/python-net/search//xlsx/"
          description: "مایکروسافت Excel صفحه گسترده XML باز"

        # format loop 8
        - name: "واترمارک DOC"
          format: "DOC"
          link: "/watermark/python-net/search//doc/"
          description: "سند مایکروسافت Word 97 - 2007"

        # format loop 9
        - name: "واترمارک XLS"
          format: "XLS"
          link: "/watermark/python-net/search//xls/"
          description: "مایکروسافت Excel کتاب کار 97-2003"

        # format loop 10
        - name: "واترمارک PPT"
          format: "PPT"
          link: "/watermark/python-net/search//ppt/"
          description: "PowerPoint ارائه ۹۷—۲۰۰۳"

        # format loop 11
        - name: "واترمارک RTF"
          format: "RTF"
          link: "/watermark/python-net/search//rtf/"
          description: "فرمت متن غنی"

---