
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:58
draft: false
lang: fa
format: Image
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "تصاویر واترمارک با .NET C#"
head_description: "یاد بگیرید که علامت های بدون درز را روی تصاویر با استفاده از .NET C# اعمال کنید. از دارایی های خود بدون به خطر انداختن کیفیت محافظت کنید."

############################# Header ############################
title: "علامت گذاری سریع سفارشی برای تصاویر با استفاده از .NET" 
description: "ابزار .NET C# ما یک راه حل سریع برای جاسازی واترمارک ها در تصاویر فراهم می کند. پشتیبانی از فرمت های تصویر گسترده پوشش کامل از عکس ها تا آثار هنری دیجیتال را تضمین می کند."
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
       GroupDocs.Watermark for .NET برای خودکار کردن فرآیند علامت گذاری تصاویر طراحی شده است و از مجموعه گسترده ای از فرمت ها مانند JPEG، PNG، BMP و TIFF پشتیبانی می کند. این API قوی امکان وارد کردن سریع واترمارک های متن و تصویر را فراهم می کند که از نظر کدورت، اندازه و موقعیت قابل تنظیم هستند، متناسب با نیازهای خاص شما. چه برای حفاظت از کپی رایت باشد و چه برای تقویت مطالب بازاریابی، جعبه ابزار ما تضمین می کند که واترمارک ها با وفاداری بالا و حداقل تأثیر بر کیفیت تصویر اصلی اعمال می شوند.

############################# Steps ############################
steps:
    enable: true
    title: "اسناد خود را بهبود ببخشید: با استفاده از .NET واترمارک برای Image ایجاد کنید"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** یک کتابخانه است که افزودن واترمارک به فرمت های مختلف فایل تجاری را برای .NET توسعه دهندگان ساده می کند. کتابخانه ما را با استفاده از این مراحل زیر در برنامه خود ادغام کنید و اسناد را بدون زحمت علامت گذاری کنید:
      
      1. **شروع سفر علامت گذاری:** با آشنایی خود با کلاس **Watermarker**، سنگ بنای API ما، شروع کنید. برای شروع فرآیند، اطمینان حاصل کنید که قبل از پردازش سند، آن را نمونه سازی می کنید. اهمیت ارائه فایل Image به سازنده را نادیده نگیرید، چه یک مسیر باشد یا یک شیء جریان.
      2. **ساخت واترمارک های سفارشی:** با ایجاد شیء **Watermark** متناسب با مشخصات شما، به مرحله بعدی بروید. این ابزار همه کاره محدود به صفحات خاص سند نیست. همچنین می تواند به طور یکپارچه در عناصر اسناد بومی مانند پیوست ها یا هدر ادغام شود.
      3. **تنظیمات دقیق ویژگی های واترمارک:** تجربه علامت گذاری خود را با تنظیم خواص مانند ارتفاع، عرض، تراز صفحه، خانواده فونت و رنگ اصلاح کنید. این سطح سفارشی سازی تضمین می کند که واترمارک های شما به طور یکپارچه با اسناد شما ترکیب می شوند.
      4. **استفاده از واترمارک های خود:** از روش **Watermarker** استفاده کنید تا به راحتی واترمارک های سفارشی خود را روی اسناد خود اعمال کنید. چه نیاز به اضافه کردن یک یا چند واترمارک داشته باشید، این فرآیند انعطاف پذیری را ارائه می دهد. برای امنیت بیشتر، اسناد پردازش شده خود را در یک مکان جداگانه ذخیره کنید.
   
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
        // تولید علامت متن در فایل IMAGE

        // پرونده را برای علامت گذاری کنید
        using (Watermarker watermarker = new Watermarker("input.جی پی جی پی"))
        {
            // نمونه واترمارک متن تولید کنید
            Font font = new Font("Arial", 19, FontStyle.Bold | FontStyle.Italic);
            TextWatermark watermark = new TextWatermark("my watermark", font);
            watermark.ForegroundColor = Color.Red;
            watermark.BackgroundColor = Color.Blue;
            watermarker.Add(watermark);

            // ذخیره IMAGE نتیجه
            watermarker.Save("output.جی پی جی پی");
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
    title: "واترمارک ها را به سرعت در سراسر فرمت های تصویر از طریق C# پیاده سازی کنید"
    exclude: "IMAGE"
    description: "حفاظت از تصویر خود را با ابزار .NET C# که قادر به مدیریت فرمت های مختلف تصویر با سرعت و کارایی است، افزایش دهید. واترمارک های خود را طوری تنظیم کنید تا کاملاً با محتوای بصری شما ترکیب شود."
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