
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:28
draft: false
lang: fa
format: Webp
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "واترمارک به WEBP با Python"
head_description: "از Python برای افزودن واترمارک به تصاویر WEBP برای محافظت قوی استفاده کنید."

############################# Header ############################
title: "ایجاد واترمارک برای WEBP با Python" 
description: "واترمارک‌های سفارشی به فایل‌های WEBP در Python اضافه کنید—عالی برای هنرمندان و تولیدکنندگان محتوا."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "در PyPi به صورت رایگان دریافت کنید"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "بیشتر بدانید"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET به شما این امکان را می‌دهد که به تصاویر WEBP در Python واترمارک اضافه کنید. از متن، لوگوها یا امضاهای دیجیتالی استفاده کنید و نحوه نمایش آن‌ها را تنظیم کنید تا با نیازهای شما مطابقت داشته باشد. مناسب برای هر کسی که تصاویر را به صورت آنلاین به اشتراک می‌گذارد، GroupDocs.Watermark کار شما را ایمن و زیبا نگه می‌دارد.

############################# Steps ############################
steps:
    enable: true
    title: "به سرعت واترمارک‌ها را به فایل‌های Webp اضافه کنید"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/):** یک کتابخانه قدرتمند Python که به شما امکان می‌دهد به راحتی واترمارک‌ها را به اسناد خود اضافه کنید.
      
      1. **کلاس اصلی: Watermarker.** با ایجاد یک شیء **Watermarker** شروع کنید. فایل Webp خود را به آن بدهید، چه به عنوان مسیر فایل و چه به صورت جریانی، تا کار را آغاز کنید.
      2. **واترمارک خود را بسازید.** سپس یک شیء Watermark از نوع مورد نظر خود ایجاد کنید. می‌توانید آن را در هر صفحه یا حتی در عناصر اسنادی مانند تصاویر یا سرصفحه‌ها قرار دهید.
      3. **ظاهر آن را تنظیم کنید.** اندازه، موقعیت، فونت و رنگ واترمارک را بر اساس نیازهای خود تنظیم کنید.
      4. **اضافه و ذخیره کنید.** از روش **Watermarker** برای وارد کردن واترمارک خود استفاده کنید. به دلخواه تعداد زیادی واترمارک اضافه کنید و سپس فایل را در هر جا که خواستید ذخیره کنید.
   
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
        # یک واترمارک تصویری به فایل WEBP اضافه کنید
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # مسیر فایل را به سازنده Watermarker منتقل کنید
        with gw.Watermarker("input.webp") as watermarker:

            # یک واترمارک تصویری با استفاده از فایل تصویر خود ایجاد کنید
            watermark = gww.ImageWatermark("watermark.png")

            watermarker.add(watermark)

            # فایل WEBP را با واترمارک ذخیره کنید
            watermarker.save("output.webp")
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "ابزارهای بیشتری برای واترمارک کردن بیابید"
  description: "GroupDocs.Watermark for Python via .NET گزینه‌های پیشرفته‌ای برای افزودن و سفارشی‌سازی واترمارک‌ها در بسیاری از انواع فایل‌ها ارائه می‌دهد. اسناد و تصاویر خود را با ویژگی‌های قابل انعطاف و آسان برای استفاده محافظت کنید."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "واترمارک‌گذاری همه‌کاره"
  features:
    # feature loop
    - title: "تایلینگ تمام صفحه"
      content: "تمام سند خود را با واترمارک‌های تایل شده پوشش دهید. این کار حذف واترمارک‌ها را دشوار می‌کند و فایل‌های شما را بدون مخدوش کردن قالب محفوظ نگه می‌دارد."

    # feature loop
    - title: "رنگ‌های سفارشی"
      content: "هر رنگی را برای واترمارک خود انتخاب کنید تا با برند یا سبک سند شما مطابقت داشته باشد. واترمارک خود را برجسته یا به اندازه دلخواه ترکیب کنید."

    # feature loop
    - title: "گزینه‌های امنیتی اضافی"
      content: "با واترمارک‌های لایه‌ای امنیت اسناد خود را افزایش دهید. نشانه‌های قابل مشاهده و پنهان را ترکیب کنید تا از کپی‌برداری جلوگیری کنید و اطمینان حاصل کنید که تنها افراد مجاز به فایل‌های شما دسترسی دارند."
      
  code_samples:
    # code sample loop
    - title: "اضافه کردن واترمارک به پاورپوینت"
      content: |
        این نمونه نشان می‌دهد که چگونه می‌توان یک واترمارک را در پس‌زمینه اسلایدهای PPTX قرار داد.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.presentation as gwop

        # یک فایل PPTX را باز کنید
        load_options = gwop.PresentationLoadOptions()
        with gw.Watermarker("source.pptx", load_options) as watermarker:

            # جزئیات واترمارک را تنظیم کنید
            with TextWatermark("Protected image", gww.Font("Arial", 8.0)) as watermark:

                watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
                watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
                watermark.rotate_angle = 45
                watermark.scale_factor = 1

                # واترمارک را به پس‌زمینه‌های اسلاید اعمال کنید
                watermarker.add(watermark)

                # ارائه به‌روز شده را ذخیره کنید
                watermarker.save("result.pptx")
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
    title: "محافظت از تصاویر WEBP با واترمارک‌های Python"
    exclude: "WEBP"
    description: "واترمارک‌های پیشرفته و سفارشی را به تصاویر WEBP در Python اضافه کنید تا کار خلاقانه خود را محافظت کنید."
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