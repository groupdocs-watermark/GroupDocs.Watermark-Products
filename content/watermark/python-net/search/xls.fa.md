
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:30
draft: false
lang: fa
format: Xls
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "پیدا کردن واترمارک‌های پنهان در برگه‌های XLS"
head_description: "از GroupDocs.Watermark for Python via .NET برای شناسایی سریع واترمارک‌ها در فایل‌های صفحه‌گسترده استفاده کنید."

############################# Header ############################
title: "شناسایی و مدیریت واترمارک‌ها در برگه‌های XLS" 
description: "به راحتی برای واترمارک‌ها جستجو کنید با GroupDocs.Watermark for Python via .NET."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود رایگان از PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "بیشتر درباره GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "بیشتر بدانید"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark به توسعه‌دهندگان Python کمک می‌کند تا واترمارک‌ها را در Python مدیریت کنند. از آن برای ویرایش، حذف یا یافتن واترمارک‌ها در Excel، Word، PDF و دیگر فرمت‌ها استفاده کنید.

############################# Steps ############################
steps:
    enable: true
    title: "شناسایی واترمارک‌های Xls با استفاده از Python"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/python-net/)** به شما امکان می‌دهد واترمارک‌ها را در انواع مختلف اسناد تجاری شناسایی کنید. این ابزار را به پروژه Python خود اضافه کنید تا قابلیت‌های شناسایی واترمارک را فعال کنید.
      
      1. برای شروع، کلاس **Watermarker** را مقداردهی اولیه کنید و سند Xls خود را با استفاده از مسیر فایل، جریان فایل، یا آرایه بایت بارگذاری کنید. این کار فایل را برای جستجوی واترمارک آماده می‌کند.
      2. برای محدود کردن جستجوی خود، از کلاس **SearchCriteria** استفاده کنید. برای واترمارک‌های تصویری، یک تصویر نمونه ارائه دهید. برای متن، جزئیات مانند فونت، اندازه، رنگ یا سایر ویژگی‌های مرتبط را تنظیم کنید.
      3. روش **Search** را از نمونه **Watermarker** فراخوانی کنید تا جستجو آغاز شود. این روش لیستی از آیتم‌های واترمارک پیدا شده را برای کار شما برمی‌گرداند.
      4. با لیست آیتم‌های واترمارک، می‌توانید در صورت نیاز آنها را حذف یا ویرایش کنید. برای مثال، ممکن است بخواهید اندازه یا متن آنها را به روز کنید.
   
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
        # جستجوی واترمارک‌های متنی در XLS
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # ایجاد یک نمونه از Watermarker با استفاده از مسیر XLS
        with gw.Watermarker("input.xls") as watermarker:

            # استفاده از تنظیمات جستجو برای پیدا کردن واترمارک‌ها
            search_criteria = gwss.TextSearchCriteria("Watermark text", False)
            possible_watermarks = watermarker.search(search_criteria)

            # مدیریت نتایج واترمارک‌های پیدا شده
            print("\nFound {0} possible watermark(s).".format(len(possible_watermarks)))
       
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "شناسایی پیشرفته واترمارک در Python با GroupDocs.Watermark"
  description: "گزینه‌های جستجوی قدرتمند واترمارک را در API GroupDocs.Watermark بررسی کنید که برای استفاده در پروژه‌های Python طراحی شده است."
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "جستجوی واترمارک Python"
  features:
    # feature loop
    - title: "شناسایی ساده و سریع واترمارک‌ها"
      content: "از GroupDocs.Watermark برای پیدا کردن سریع واترمارک‌ها در کد Python خود استفاده کنید. موتور جستجوی هوشمند به شما کمک می‌کند تا واترمارک‌ها را سریع پیدا کنید."

    # feature loop
    - title: "پیدا کردن واترمارک‌های خاص با دقت"
      content: "فایل‌های خود را محافظت کنید با پیدا کردن واترمارک‌ها بر اساس رنگ، اندازه یا موقعیت. GroupDocs.Watermark این امکان را به شما می‌دهد که فیلترهای جستجو را در Python پیکربندی کنید."

    # feature loop
    - title: "ابزارهای Python برای کنترل کامل واترمارک‌ها"
      content: "GroupDocs.Watermark را به برنامه‌های Python خود اضافه کنید تا واترمارک‌ها را جستجو، بررسی و پیگیری کنید. این کار برای بازبینی‌ها، برندینگ یا حفاظت از محتوا عالی است."
      
  code_samples:
    # code sample loop
    - title: "نمونه Python: جریان کامل شناسایی واترمارک"
      content: |
        ببینید چگونه از GroupDocs.Watermark در Python برای جستجو در اسناد، مدیریت چندین فرمت و استفاده از فیلترهای پیچیده استفاده کنید.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # برنامه Python خود را راه‌اندازی کنید و سند را بارگذاری کنید
        load_options = gwos.SpreadsheetLoadOptions()
        with gw.Watermarker("source.xlsx", load_options) as watermarker:

            # تعریف کنید که چه نوع واترمارکی را جستجو کنید
            criteria = gwss.ImageColorHistogramSearchCriteria("watermark.png")
            criteria.MaxDifference = 0.5
            criteria.bins_count = 2

            # جستجو را اجرا کنید و داده‌های واترمارک را جمع‌آوری کنید
            possible_watermarks = watermarker.search(criteria)

            # از اطلاعات پیدا شده برای مراحل بعدی مانند حذف یا بررسی استفاده کنید
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
    title: "جستجوی واترمارک در میان فرمت‌ها"
    exclude: "XLS"
    description: "واترمارک‌ها را در بسیاری از فرمت‌های مختلف شناسایی و مدیریت کنید."
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