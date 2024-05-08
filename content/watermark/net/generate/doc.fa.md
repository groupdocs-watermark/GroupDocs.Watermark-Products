
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:23
draft: false
lang: fa
format: Doc
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "واترمارک DOC فایل ها با .NET C #"
head_description: "برای محافظت و مدیریت موثر از Word اسناد خود، علامت های C# .NET را در فایل DOC پیاده سازی کنید."

############################# Header ############################
title: "افزایش امنیت DOC با واترمارک های C#" 
description: "از .NET C # برای جاسازی واترمارک های امن در DOC فایل استفاده کنید، مناسب برای محافظت از MS Word اسناد در تنظیمات قانونی و شرکتی."
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
       GroupDocs.Watermark for .NET از .NET C # برای ارائه یک راه حل پیشرفته واترمارک برای DOC فایل استفاده می کند که معمولاً در مایکروسافت Word استفاده می شود. این API به توسعه دهندگان اجازه می دهد تا هر دو واترمارک متنی و گرافیکی را وارد کنند که برای کدورت، رنگ و موقعیت قابل تنظیم هستند. امنیت اسناد را با واترمارک هایی که می توانند شامل برچسب های زمانی، آرم ها یا برچسب های محرمانه باشند، به طور موثر از استفاده غیر مجاز جلوگیری کرده و از صحت سند اطمینان حاصل کنند، افزایش دهید. این API برای ادغام یکپارچه با چارچوب .NET طراحی شده است و آن را برای برنامه های کاربردی در اسناد حقوقی، ارتباطات شرکتی و مدیریت اطلاعات حساس ایده آل می کند. سازگار با محیط های C# .NET، GroupDocs.Watermark یک مجموعه ابزار قوی برای حفاظت جامع از اسناد ارائه می دهد.

############################# Steps ############################
steps:
    enable: true
    title: "بدون زحمت واترمارک برای اسناد Doc ایجاد کنید"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/):** کتابخانه واترمارک پیشرفته برای برنامه های کاربردی .NET. راه حل خود را قدرتمند کنید و اسناد خود را با واترمارک ها به موقع امن کنید.
      
      1. **کلاس اصلی: واترمارکر.** کلاس اصلی API ما **Watermarker** است. قبل از پردازش سند باید آن را نمونه برداری کنید. فراموش نکنید که فایل Doc را به عنوان یک مسیر یا یک شی جریان به سازنده ارسال کنید.
      2. ** ساخت واترمارک شما.** مرحله بعدی ساخت یک آبجکت واترمارک از نوع دلخواه است. می‌توان آن را نه تنها در یک صفحه سند خاص، بلکه در بخش‌های سند بومی مانند تصاویر یا هدرها قرار داد.
      3. **ظاهر تنظیم دقیق.** ویژگی های واترمارک مانند ارتفاع و عرض، بالا، چپ، ترازهای مرکزی، فونت ها و رنگ ها و غیره را تنظیم کنید.
      4. **در حال اعمال و ذخیره.** از روش **Watermarker** برای افزودن واترمارک جدید استفاده کنید. با خیال راحت هر تعداد که نیاز دارید واترمارک اضافه کنید. می توانید سند واترمارک شده را در هر مکانی ذخیره کنید.
   
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
        // ایجاد واترمارک تصویر در فایل DOC

        // مسیر فایل منبع را برای سازنده Watermarker ارائه دهید
        using (Watermarker watermarker = new Watermarker("input.doc"))
        {
            // نمونه واترمارک تصویر را با فایل تصویری ایجاد کنید
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // نتیجه DOC دارای واترمارک را ذخیره کنید
            watermarker.Save("output.doc");
        }
        
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "بازی علامت گذاری خود را بالا ببرید"
  description: "قابلیت های پیشرفته علامت گذاری با GroupDocs.Watermark API ما برای .NET باز کنید. این ابزار قدرتمند امکان سفارشی سازی دقیق و استفاده از واترمارک ها را در انواع مختلف سند فراهم می کند تا حداکثر امنیت و رعایت کپی رایت با حداقل اختلال بصری اطمینان حاصل شود."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "راه حل های واترمارک جامع"
  features:
    # feature loop
    - title: "گزینه های کاشی کاری پیشرفته"
      content: "با گزینه های کاشی کاری ما، واترمارک های خود را به طور یکپارچه در کل اسناد گسترش دهید. این ویژگی به واترمارک ها اجازه می دهد تا ناحیه کامل سند را پوشش دهند، از حذف و حفاظت کامل از سند را بدون به خطر انداختن طراحی یا خوانایی اطمینان حاصل کنند."

    # feature loop
    - title: "سفارشی سازی رنگ پر جنب و جوش"
      content: "یک تکه رنگ به علامت های آب خود اضافه کنید! API ما سفارشی سازی رنگ طیف کامل را امکان پذیر می کند و به شما امکان می دهد واترمارک هایی را اعمال کنید که کاملاً با نام تجاری شرکت یا سبک سند شما مطابقت دارد. ضمن حفظ ویژگی های امنیتی قوی، جذابیت بصری را افزایش دهید."

    # feature loop
    - title: "تنظیمات امنیتی پیشرفته"
      content: "با تنظیمات پیشرفته واترمارک، امنیت اسناد را به سطح بعدی برسانید. واترمارک های چند لایه را با ترکیب عناصر قابل مشاهده و نامرئی پیکربندی کنید تا در برابر کپی کردن غیر مجاز محافظت شود و اطمینان حاصل شود که فقط گیرندگان مورد نظر می توانند به اطلاعات مهم دسترسی داشته باشند."
      
  code_samples:
    # code sample loop
    - title: "تولید علامت PowerPoint"
      content: |
        این مثال نحوه افزودن واترمارک به PPTX تصاویر پس زمینه را نشان می دهد
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  بارگذاری PPTX ارائه
            var loadOptions = new PresentationLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pptx", loadOptions))
            {
                //  ویژگی های واترمارک را تنظیم کنید
                TextWatermark watermark = new TextWatermark("Protected image", new Font("Arial", 8));
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermark.RotateAngle = 45;
                watermark.SizingType = SizingType.ScaleToParentDimensions;
                watermark.ScaleFactor = 1;

                //  پس زمینه اسلاید واترمارک
                PresentationContent content = watermarker.GetContent<PresentationContent>();
                foreach (PresentationSlide slide in content.Slides)
                {
                    if (slide.ImageFillFormat.BackgroundImage != null)
                    {
                        slide.ImageFillFormat.BackgroundImage.Add(watermark);
                    }
                }

                //  ذخیره ارائه پردازش شده
                watermarker.save("result.pptx");
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
    title: "علامت گذاری C# برای Word اسناد"
    exclude: "DOC"
    description: ".NET C# را برای اعمال علامت های دقیق و قابل تنظیم در فایل DOC استفاده کنید و امنیت و یکپارچگی اسناد MS Word شما را تقویت کنید."
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