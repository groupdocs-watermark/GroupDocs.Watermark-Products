
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: fa
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "اضافه کردن واترمارک به ارائه‌ها"
head_description: "به راحتی واترمارک‌ها را به اسلایدهای PowerPoint خود برای امنیت بیشتر اضافه کنید."

############################# Header ############################
title: "واترمارک‌گذاری پیشرفته برای ارائه‌ها در Python" 
description: "واترمارک‌های متنی و تصویری را به اسلایدهای PowerPoint با API Python ما اضافه کنید. مناسب برای حفظ امنیت و حرفه‌ای بودن ارائه‌های شما."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود PyPi به صورت رایگان"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "بیشتر بدانید"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET به شما این امکان را می‌دهد که واترمارک‌های پیشرفته به ارائه‌های PowerPoint در Python اضافه کنید. اطلاعات محرمانه را محافظت کنید یا لوگوی شرکت خود را به اسلایدها اضافه کنید. می‌توانید واترمارک‌ها را به اسلایدهای منفرد یا کل ارائه اضافه کنید و نحوه نمایش آن‌ها و مکان ظهور آن‌ها را تنظیم کنید.

############################# Steps ############################
steps:
    enable: true
    title: "اضافه کردن واترمارک‌ها: واترمارک‌گذاری Python برای Powerpoint"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** یک کتابخانه است که افزودن واترمارک به بسیاری از انواع فایل‌های تجاری را تسهیل می‌کند. مراحل زیر را دنبال کنید تا به سرعت واترمارک‌ها را به مستندات خود در Python اضافه کنید:
      
      1. **شروع با واترمارک‌گذاری:** با ایجاد یک نمونه از کلاس **Watermarker** شروع کنید. فایل Powerpoint خود را (به عنوان مسیر یا استریم) به سازنده پاس دهید تا برای واترمارک‌گذاری باز شود.
      2. **واترمارک خود را بسازید:** یک شی **Watermark** با متن و تنظیمات دلخواه خود ایجاد کنید. می‌توانید واترمارک‌ها را به هر صفحه یا حتی به عناصر документی مانند سرصفحه‌ها یا پیوست‌ها اضافه کنید.
      3. **واترمارک را سفارشی کنید:** اندازه، موقعیت، فونت، رنگ و تراز واترمارک را مطابق نیازهای خود تنظیم کنید. این کمک می‌کند واترمارک شما در سند به درستی نمایان شود.
      4. **اعمال و ذخیره:** از متد **Watermarker** برای افزودن واترمارک‌ها به سند استفاده کنید. نتیجه را ذخیره کنید، به‌خصوص به‌عنوان یک فایل جدید برای ایمنی.
   
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
        # یک واترمارک متنی به فایل POWERPOINT اضافه کنید
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # فایلی که می‌خواهید واترمارک کنید را انتخاب کنید
        with gw.Watermarker("input.pptx") as watermarker:

            # یک شی واترمارک متنی بسازید
            font = gww.Font("Arial", 36.0)
            watermark = gww.TextWatermark("top secret", font)
            watermark.foreground_color = gww.Color.red
            watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
            watermark.opacity = 0.4

            watermarker.add(watermark)

            # فایل POWERPOINT به‌روز شده را ذخیره کنید
            watermarker.save("output.pptx")
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "ویژگی‌های بیشتر واترمارک‌گذاری را بررسی کنید"
  description: "از API Python ما برای افزودن، مشاهده، تبدیل و مدیریت واترمارک‌ها در مستندات، اسلایدها، نمودارها و غیره استفاده کنید. GroupDocs.Watermark for Python via .NET به شما کمک می‌کند تا فایل‌های خود را محافظت کرده و اطلاعات حق کپی را به سادگی اضافه کنید."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "اضافه کردن واترمارک"
  features:
    # feature loop
    - title: "اضافه کردن واترمارک به سادگی"
      content: "GroupDocs.Watermark به توسعه‌دهندگان Python این امکان را می‌دهد که به سرعت واترمارک‌های متنی، تصویری یا پویا به مستندات تجاری اضافه کنند. فایل‌های خود را با حداقل تلاش ایمن و برند کنید."

    # feature loop
    - title: "واترمارک‌های کاملاً قابل تنظیم"
      content: "اندازه، چرخش، شفافیت، رنگ و فونت واترمارک را با GroupDocs.Watermark تغییر دهید. واترمارک شما می‌تواند به طور دقیق با سند شما هماهنگ شود و محتویات مهم قابل مشاهده بمانند."

    # feature loop
    - title: "استفاده از ویژگی‌های مستندات برای واترمارک‌گذاری"
      content: "از ویژگی‌های داخلی مستندات مانند حاشیه‌نویسی‌های PDF، پس‌زمینه‌های Word یا سرصفحه‌های Excel برای افزودن واترمارک‌ها بهره ببرید. GroupDocs.Watermark با ساختارهای مستنداتی برای واترمارک‌گذاری مؤثر و غیرتهاجمی کار می‌کند."
      
  code_samples:
    # code sample loop
    - title: "اضافه کردن واترمارک تصویری به DOCX"
      content: |
        این مثال نشان می‌دهد چگونه می‌توانید اثرات تصویری را به واترمارک‌های شکلی اعمال کنید.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.wordprocessing as gwow

        # یک سند Word را باز کنید
        load_options = gwow.WordProcessingLoadOptions()
        with gw.Watermarker("source.docx", load_options) as watermarker:

            # گزینه‌های واترمارک را تنظیم کنید
            with gww.ImageWatermark("logo.png") as watermark:

                effects = gwow.WordProcessingImageEffects()
                effects.brightness = 0.7
                effects.contrast = 0.6
                effects.chroma_key = gww.Color.red

                options = gwow.WordProcessingWatermarkSectionOptions()
                options.Effects = effects;

                # واترمارک را ایجاد کنید
                watermarker.add(watermark, options)

                # سند را با واترمارک ذخیره کنید
                watermarker.save("result.docx")
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
    title: "واترمارک‌گذاری ارائه‌ها با Python"
    exclude: "POWERPOINT"
    description: "از ابزار Python ما برای اضافه کردن سریع واترمارک‌ها به فایل‌های PowerPoint استفاده کنید. اسلایدهای خود را ایمن و واضح نگه دارید."
    items: 
        # format loop 1
        - name: "واترمارک PDF"
          format: "PDF"
          link: "/watermark/python-net/add//pdf/"
          description: "ادوبی Portable فرمت سند"

        # format loop 2
        - name: "واترمارک Word"
          format: "WORD"
          link: "/watermark/python-net/add//word/"
          description: "MS Word و اسناد آفیس باز"
          
        # format loop 3
        - name: "واترمارک Excel"
          format: "EXCEL"
          link: "/watermark/python-net/add//excel/"
          description: "MS Excel و صفحات گسترده آفیس باز"

        # format loop 4
        - name: "تصویر واترمارک"
          format: "IMAGE"
          link: "/watermark/python-net/add//image/"
          description: "فرمت های تصویر محبوب"

        # format loop 5
        - name: "عکس واترمارک"
          format: "PHOTO"
          link: "/watermark/python-net/add//photo/"
          description: "فرمت های عکس"

        # format loop 6
        - name: "واترمارک PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/add//powerpoint/"
          description: "MS PowerPoint و ارائه های آفیس باز"

        # format loop 7
        - name: "واترمارک DOCX"
          format: "DOCX"
          link: "/watermark/python-net/add//docx/"
          description: "مایکروسافت Word سند XML باز"
          
        # format loop 8
        - name: "واترمارک PPTX"
          format: "PPTX"
          link: "/watermark/python-net/add//pptx/"
          description: "PowerPoint ارائه اکس‌ام‌ال باز"
          
        # format loop 9
        - name: "واترمارک XLSX"
          format: "XLSX"
          link: "/watermark/python-net/add//xlsx/"
          description: "مایکروسافت Excel صفحه گسترده XML باز"

        # format loop 10
        - name: "واترمارک JPEG"
          format: "JPEG"
          link: "/watermark/python-net/add//jpeg/"
          description: "JPEG تصویر"

        # format loop 11
        - name: "واترمارک PNG"
          format: "PNG"
          link: "/watermark/python-net/add//png/"
          description: "Portable گرافیک شبکه"

        # format loop 12
        - name: "واترمارک TIFF"
          format: "TIFF"
          link: "/watermark/python-net/add//tiff/"
          description: "برچسب فرمت فایل تصویر"

        # format loop 13
        - name: "واترمارک WEBP"
          format: "WEBP"
          link: "/watermark/python-net/add//webp/"
          description: "تصویر WEB"

        # format loop 14
        - name: "واترمارک DOC"
          format: "DOC"
          link: "/watermark/python-net/add//doc/"
          description: "سند مایکروسافت Word 97 - 2007"

        # format loop 15
        - name: "واترمارک XLS"
          format: "XLS"
          link: "/watermark/python-net/add//xls/"
          description: "مایکروسافت Excel کتاب کار 97-2003"

        # format loop 16
        - name: "واترمارک PPT"
          format: "PPT"
          link: "/watermark/python-net/add//ppt/"
          description: "PowerPoint ارائه ۹۷—۲۰۰۳"

        # format loop 17
        - name: "واترمارک RTF"
          format: "RTF"
          link: "/watermark/python-net/add//rtf/"
          description: "فرمت متن غنی"

---