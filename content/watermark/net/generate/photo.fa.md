
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:28
draft: false
lang: fa
format: Photo
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "عکس های خود را به سرعت و به راحتی علامت بزنید"
head_description: "با علامت های .NET C # به سرعت حق چاپ عکس های خود را ایمن کنید و ادعا کنید. همین امروز حفاظت از کارتان را شروع کنید."

############################# Header ############################
title: "علامت گذاری سریع و آسان عکس با .NET" 
description: "کتابخانه قدرتمند C# ما امکان علامت گذاری سریع عکس های شما را فراهم می کند و به شما کمک می کند کپی رایت را حفظ کنید و هویت برند را بدون به خطر انداختن کیفیت تصویر افزایش دهید."
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود در Nuget به صورت رایگان"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "بیشتر بدانید"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET یک راه حل قدرتمند برای خدمات عکاس که به دنبال محافظت از کپی رایت و هویت برند خود هستند ارائه می دهد. این API امکان افزودن سریع واترمارک های متنی یا گرافیکی به عکس ها در فرمت های مختلف از جمله JPEG، PNG و RAW را فراهم می کند. واترمارک های خود را برای شفافیت، اندازه و موقعیت سفارشی کنید تا به طور یکپارچه با عکس ترکیب شود، کیفیت زیبایی شناختی را حفظ کرده و در عین حال حقوق قانونی خود را تأیید کنید و از استفاده غیر مجاز جلوگیری کنید.

############################# Steps ############################
steps:
    enable: true
    title: "اسناد خود را تقویت کنید: با استفاده از .NET برای Photo واترمارک ایجاد کنید"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** کتابخانه ای است که افزودن واترمارک به فرمت های مختلف فایل های تجاری را برای توسعه دهندگان .NET ساده می کند. کتابخانه ما را در برنامه خود ادغام کنید و اسناد را با استفاده از این مراحل زیر بدون دردسر علامت گذاری کنید:
      
      1. **آغاز سفر واترمارکینگ شما:** با آشنایی با کلاس **Watermarker** ، سنگ بنای API ما، شروع کنید. برای شروع فرآیند، مطمئن شوید که آن را قبل از پردازش سند نمونه‌برداری کرده‌اید. اهمیت ارائه فایل Photo به سازنده را نادیده نگیرید، خواه مسیر باشد یا یک شی جریان.
      2. **ساخت واترمارک های سفارشی:** با ایجاد یک شی **Watermark** متناسب با مشخصات شما، به مرحله بعدی بروید. این ابزار همه کاره به صفحات سند خاص محدود نمی شود. همچنین می تواند به طور یکپارچه در عناصر سند بومی مانند پیوست ها یا هدرها ادغام شود.
      3. **تنظیم دقیق ویژگی های واترمارک:** تجربه واترمارک خود را با تنظیم ویژگی هایی مانند ارتفاع، عرض، تراز صفحه، خانواده فونت و رنگ اصلاح کنید. این سطح از سفارشی سازی تضمین می کند که واترمارک های شما یکپارچه با اسناد شما ترکیب می شوند.
      4. **استفاده از واترمارک های خود:** از روش **Watermarker** استفاده کنید تا بدون زحمت واترمارک های سفارشی خود را روی اسناد خود اعمال کنید. چه نیاز به اضافه کردن یک یا چند واترمارک داشته باشید، این فرآیند انعطاف پذیری را ارائه می دهد. برای امنیت بیشتر، اسناد پردازش شده خود را در مکانی جداگانه ذخیره کنید.
   
    code:
      platform: "net"
      copy_title: "کپی کردن"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "برای کپی کلیک کنید"
        copy_done: "کپی شده"
      links:
        #  loop
        - title: "نمونه های بیشتر"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "مستندات"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // ایجاد واترمارک متنی در فایل PHOTO

        // ارائه فایل به واترمارک
        using (Watermarker watermarker = new Watermarker("input.png"))
        {
            // نمونه واترمارک متنی ایجاد کنید
            Font font = new Font("Arial", 19, FontStyle.Bold | FontStyle.Italic);
            TextWatermark watermark = new TextWatermark("my watermark", font);
            watermark.ForegroundColor = Color.Red;
            watermark.BackgroundColor = Color.Blue;
            watermarker.Add(watermark);

            // نتیجه PHOTO را ذخیره کنید
            watermarker.Save("output.png");
        }
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "شیوه عمیق در افزودن واترمارک ها"
  description: "از API قدرتمند ما برای رندر، نمایش، تبدیل و مدیریت اسناد، اسلاید، نمودارها و انواع مختلف سند در .NET برنامه استفاده کنید. GroupDocs.Watermark به طور یکپارچه قابلیت های واترمارک را برای افزایش امنیت اسناد و حفاظت از کپی رایت ادغام می کند."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "افزودن واترمارک"
  features:
    # feature loop
    - title: "اسناد خود را بدون زحمت علامت گذاری کنید"
      content: "GroupDocs.Watermark توسعه دهندگان را قادر می سازد تا به راحتی واترمارک را در برنامه های خود ادغام کنند. بدون زحمت متن، تصویر یا واترمارک پویا را به اسناد و فایل های تجاری محبوب اضافه کنید و اطمینان حاصل کنید که محتوای شما به طور مداوم در همه سیستم عامل ها ایمن و برند دار است."

    # feature loop
    - title: "واترمارک ها را متناسب با نیازهای شما تنظیم کنید."
      content: "با ویژگی های گسترده پشتیبانی شده توسط GroupDocs.Watermark، واترمارک ها را متناسب با نیازهای خاص خود سفارشی کنید. اندازه، چرخش، شفافیت، رنگ و فونت را تنظیم کنید تا اطمینان حاصل شود که واترمارک شما نه تنها عالی به نظر می رسد بلکه امنیت سند را نیز بدون مانع اطلاعات مهم افزایش می دهد."

    # feature loop
    - title: "از ویژگی های اسناد بومی برای علامت گذاری استفاده کنید"
      content: "از ویژگی های ذاتی فرمت های سند برای علامت گذاری پیشرفته استفاده کنید. چه از حاشیه نویسی PDF بومی، MS Word پس زمینه یا Excel هدر و پاورقی استفاده کند، GroupDocs.Watermark عمیقاً با ساختارهای سند ادغام می شود تا واترمارک هایی را اعمال کند که هم موثر و هم کم تهاجمی هستند."
      
  code_samples:
    # code sample loop
    - title: "تولید علامت تصویر برای DOCX"
      content: |
        این مثال نحوه اعمال جلوه های تصویر به علامت های شکل را نشان می دهد.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  بارگیری Word سند
            var loadOptions = new WordProcessingLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.docx", loadOptions))
            {
                //  تنظیمات علامت گذاری را تنظیم کنید
                using (ImageWatermark watermark = new ImageWatermark("logo.png"))
                {
                    WordProcessingImageEffects effects = new WordProcessingImageEffects();
                    effects.Brightness = 0.7;
                    effects.Contrast = 0.6;
                    effects.ChromaKey = Color.Red;
                    effects.BorderLineFormat.Enabled = true;
                    effects.BorderLineFormat.Weight = 1;

                    WordProcessingWatermarkSectionOptions options = new WordProcessingWatermarkSectionOptions();
                    options.Effects = effects;

                    //  تولید علامت
                    watermarker.Add(watermark, options);
                }

                //  ذخیره سند به روز شده
                watermarker.save("result.docx");
            }

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "آماده شروع هستید؟"
  description: "ویژگی های GroupDocs.Watermark را به صورت رایگان امتحان کنید یا مجوز درخواست کنید"
  items:
    #  loop
    - title: "Nuget دانلود"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "صدور مجوز"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "از عکس های خود با علامت های موثر محافظت کنید C#"
    exclude: "PHOTO"
    description: "محتوای عکاسی خود را با واترمارک های قابل تنظیم با استفاده از .NET C# API که برای ادغام یکپارچه و حفظ کیفیت تصویر طراحی شده است، ایمن و سبک سازی کنید."
    items: 
        # format loop 1
        - name: "واترمارک PDF"
          format: "PDF"
          link: "/watermark/net/generate//pdf/"
          description: "ادوبی Portable فرمت سند"

        # format loop 2
        - name: "واترمارک Word"
          format: "WORD"
          link: "/watermark/net/generate//word/"
          description: "MS Word و اسناد آفیس باز"
          
        # format loop 3
        - name: "واترمارک Excel"
          format: "EXCEL"
          link: "/watermark/net/generate//excel/"
          description: "MS Excel و صفحات گسترده آفیس باز"

        # format loop 4
        - name: "تصویر واترمارک"
          format: "IMAGE"
          link: "/watermark/net/generate//image/"
          description: "فرمت های تصویر محبوب"

        # format loop 5
        - name: "عکس واترمارک"
          format: "PHOTO"
          link: "/watermark/net/generate//photo/"
          description: "فرمت های عکس"

        # format loop 6
        - name: "واترمارک PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/generate//powerpoint/"
          description: "MS PowerPoint و ارائه های آفیس باز"

        # format loop 7
        - name: "واترمارک DOCX"
          format: "DOCX"
          link: "/watermark/net/generate//docx/"
          description: "مایکروسافت Word سند XML باز"
          
        # format loop 8
        - name: "واترمارک PPTX"
          format: "PPTX"
          link: "/watermark/net/generate//pptx/"
          description: "PowerPoint ارائه اکس‌ام‌ال باز"
          
        # format loop 9
        - name: "واترمارک XLSX"
          format: "XLSX"
          link: "/watermark/net/generate//xlsx/"
          description: "مایکروسافت Excel صفحه گسترده XML باز"

        # format loop 10
        - name: "واترمارک JPEG"
          format: "JPEG"
          link: "/watermark/net/generate//jpeg/"
          description: "JPEG تصویر"

        # format loop 11
        - name: "واترمارک PNG"
          format: "PNG"
          link: "/watermark/net/generate//png/"
          description: "Portable گرافیک شبکه"

        # format loop 12
        - name: "واترمارک TIFF"
          format: "TIFF"
          link: "/watermark/net/generate//tiff/"
          description: "برچسب فرمت فایل تصویر"

        # format loop 13
        - name: "واترمارک WEBP"
          format: "WEBP"
          link: "/watermark/net/generate//webp/"
          description: "تصویر WEB"

        # format loop 14
        - name: "واترمارک DOC"
          format: "DOC"
          link: "/watermark/net/generate//doc/"
          description: "سند مایکروسافت Word 97 - 2007"

        # format loop 15
        - name: "واترمارک XLS"
          format: "XLS"
          link: "/watermark/net/generate//xls/"
          description: "مایکروسافت Excel کتاب کار 97-2003"

        # format loop 16
        - name: "واترمارک PPT"
          format: "PPT"
          link: "/watermark/net/generate//ppt/"
          description: "PowerPoint ارائه ۹۷—۲۰۰۳"

        # format loop 17
        - name: "واترمارک RTF"
          format: "RTF"
          link: "/watermark/net/generate//rtf/"
          description: "فرمت متن غنی"

---