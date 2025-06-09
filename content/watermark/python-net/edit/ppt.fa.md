
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:29
draft: false
lang: fa
format: Ppt
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "ویرایش سریع و دقیق واترمارک Ppt"
head_description: "سرعت ویرایش واترمارک خود را در فایل‌های Ppt با استفاده از GroupDocs.Watermark for Python via .NET افزایش دهید."

############################# Header ############################
title: "ویرایش پیشرفته واترمارک برای Ppt با قدرت Python" 
description: "از GroupDocs.Watermark for Python via .NET برای محافظت و شخصی‌سازی اسلایدها استفاده کنید که به راحتی قابل ادغام است."
subtitle: "GroupDocs.Watermark for Python via .NET Library" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود از PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET Library"
    link: "/watermark/python-net/"
    link_title: "بیشتر بدانید"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **تنظیمات سریع واترمارک:** تغییرات آنی را در واترمارک‌ها در اسناد Ppt با استفاده از ابزارهای سازگار با Python ما اعمال کنید.

############################# Steps ############################
steps:
    enable: true
    title: "استفاده از API Python برای تغییر واترمارک‌ها در اسناد Ppt"
    content: |
      با **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)**، توسعه‌دهندگان Python می‌توانند محتوای واترمارک را در انواع مختلف اسناد Ppt تغییر دهند. در اینجا یک راهنمای سریع وجود دارد:
      
      1. با بارگذاری سند Ppt با استفاده از کلاس **Watermarker** آغاز کنید که ورودی‌هایی مانند مسیرهای فایل، جریان‌های حافظه یا آرایه‌های بایت را قبول می‌کند.
      2. یک شیء **SearchCriteria** بسازید تا عناصر واترمارک موجود در سند شما، چه متنی و چه گرافیکی، را جستجو کنید.
      3. پس از شناسایی، ابزار یک مجموعه‌ای از نمونه‌های واترمارک تطبیق‌یافته را برای به‌روزرسانی فراهم می‌کند—پارامترهایی مانند رنگ، تراز، قلم یا حتی داده‌های تصویر جاسازی‌شده را تنظیم کنید.
      4. پروسه را با ذخیره سند اصلاح‌شده به دیسک یا هر جریان خروجی پشتیبانی‌شده با استفاده از متدهای ذخیره‌سازی داخلی نهایی کنید.
   
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
        # به‌روزرسانی واترمارک تصویر در فایل PPT
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # ایجاد یک نمونه Watermarker با فایل ورودی
        with gw.Watermarker("input.ppt") as watermarker:

            # استفاده از SearchCriteria برای شناسایی واترمارک‌های مبتنی بر تصویر
            search_criteria = gwss.ImageDctHashSearchCriteria("logo.png")

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # اعمال تغییرات بر روی واترمارک تصویر
                        watermark.ImageData = imageData
                    except Exception as e:
                        pass

            # صادرات فایل PPT به‌روزرسانی‌شده
            watermarker.save("output.ppt")
        ```     

############################# More features ############################
more_features:
  enable: true
  title: "افزایش بهره‌وری با ابزارهای پیشرفته واترمارک"
  description: "سرعت بخشیدن به برندسازی و حفاظت از اسناد در Python با API دینامیک واترمارک ما. لایه‌های واترمارک را با حداقل تلاش درج، شناسایی، تغییر یا حذف کنید."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "جریان کار ویرایش پیشرفته واترمارک"
  features:
    # feature loop
    - title: "کنترل یکپارچه واترمارک"
      content: "کنترل کامل چرخه عمر واترمارک را به برنامه‌های Python خود با استفاده از GroupDocs.Watermark for Python via .NET اضافه کنید. با خودکار کردن تنظیم، به‌روزرسانی و حذف واترمارک، از کارهای تکراری جلوگیری کنید."

    # feature loop
    - title: "تنظیمات دقیق خصوصیات واترمارک"
      content: "کنترل کامل بر روی ظاهر واترمارک—تغییر اندازه، رنگ، چرخش یا جایگذاری مجدد آنها مطابق با هر درخواست بصری با سطح API انعطاف‌پذیر ما."

    # feature loop
    - title: "استفاده از ویژگی‌های فرمت بومی"
      content: "با جاسازی واترمارک‌ها در سرصفحات، پاورقی‌ها، یادداشت‌ها یا پس‌زمینه‌ها به هر فرمت فایلی سازگار شوید. API ما ساختارهای بومی را برای ادغام بهینه رعایت می‌کند."
      
  code_samples:
    # code sample loop
    - title: "تغییر واترمارک در یک فایل PDF"
      content: |
        نحوه تغییر ویژگی‌های واترمارک در یک سند PDF را نشان می‌دهد.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # باز کردن فایل PDF
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.pdf as gwop

        # خواندن محتوای واترمارک
        load_options = gwop.PdfLoadOptions()
        with gw.Watermarker("source.pdf", load_options) as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,5,8]

            # اعمال به‌روزرسانی واترمارک
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
        
            # ذخیره نتیجه ویرایش‌شده
            watermarker.save("output.pdf")
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
    title: "پشتیبانی چندفرمتی واترمارک"
    exclude: "PPT"
    description: "جریان‌های مشابه واترمارک‌گذاری را در سایر انواع اسناد با GroupDocs.Watermark for Python via .NET اعمال کنید."
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