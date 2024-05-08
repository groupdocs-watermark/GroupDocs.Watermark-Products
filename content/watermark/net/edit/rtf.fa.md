
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:24
draft: false
lang: fa
format: Rtf
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "ویرایش واترمارک ها در Rtf اسناد"
head_description: "با GroupDocs.Watermark for .NET SDK به برندسازی سند شفاف Rtf دست یابید. واترمارک های خود را برای اطمینان از امنیت ویرایش کنید."

############################# Header ############################
title: "جلا Rtf ویرایش واترمارک: .NET پیچیدگی" 
description: "با GroupDocs.Watermark for .NET SDK به برندسازی پیچیده اسناد دست یابید. علامت های سند خود را با دقت و اطمینان ویرایش کنید."
subtitle: "GroupDocs.Watermark for .NET آپی" 

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
       **ویرایش واترمارک های صیقلی:** با GroupDocs.Watermark for .NET SDK به برندسازی پیچیده Rtf سند دست یابید. اسناد خود را با دقت و اطمینان جلا کنید و از سازگاری و حفاظت از نام تجاری اطمینان حاصل کنید.

############################# Steps ############################
steps:
    enable: true
    title: "ویرایش برنامه‌نویسی واترمارک در اسناد Rtf با API .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** به توسعه دهندگان .NET یک API قوی برای دستکاری برنامه‌نویسی واترمارک در اسناد مختلف Rtf ارائه می‌دهد. این راهنما فرآیند را تشریح می کند:
      
      1. با ارائه فایل Rtf خود به عنوان آرگومان در سازنده کلاس **Watermarker**، گردش کار را آغاز کنید. فایل را می توان به عنوان یک جریان بایت، یک جریان فایل، یا یک مرجع به یک محل دیسک محلی ارائه کرد.
      2. پس از آن، از شیء **SearchCriteria** برای مشخص کردن واترمارک های خاص که نیاز به اصلاح دارند، استفاده کنید. این شی شناسایی واترمارک هایی را که قبلاً در سند جاسازی شده اند را قادر می سازد.
      3. پس از اجرای موفقیت آمیز جستجو، مجموعه ای از واترمارک های مربوطه را دریافت خواهید کرد. این واترمارک ها کنترل دانه ای را ارائه می دهند که به شما امکان می دهد ویژگی هایی مانند ابعاد، موقعیت صفحه، محتوای متن، طرح رنگ، داده های تصویر و موارد دیگر را تغییر دهید.
      4. پس از تکمیل ویرایش های واترمارک، سند اصلاح شده را ادامه دهید. API ذخیره سازی را با استفاده از یک مسیر فایل محلی یا یک شی جریان تسهیل می کند.
   
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
        // واترمارک تصویر را در سند RTF ویرایش کنید

        // Watermarker را با فایل منبع مقداردهی کنید
        using (Watermarker watermarker = new Watermarker("input.rtf"))
        {
            // برای جستجوی واترمارک تصویر، SearchCriteria را ایجاد کنید
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                // واترمارک تصویر را ویرایش کنید
                watermark.ImageData = imageData;
            }

            // ذخیره نتیجه RTF
            watermarker.Save("output.rtf");
        }
        
        ```     

############################# More features ############################
more_features:
  enable: true
  title: "گردش کار خود را با مدیریت واترمارک افزایش دهید"
  description: "با کتابخانه قوی ما، علامت گذاری در قالب های مختلف فایل در برنامه های .NET خود را ساده کنید. برای افزایش امنیت سند و نام تجاری، بدون زحمت، اضافه کردن، ویرایش، جستجو یا حذف واترمارک ها."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "ویرایش علامت بدون درز"
  features:
    # feature loop
    - title: "علامت گذاری واترمارک را در برنامه های خود ساده کنید"
      content: "از قدرت GroupDocs.Watermark for .NET استفاده کنید تا قابلیت واترمارک را به طور یکپارچه در .NET برنامه های خود ادغام کنید. API بصری ما ایجاد، مدیریت، جستجو و ویرایش واترمارک را ساده می کند و نیاز به فرآیندهای دستی پیچیده را از بین می برد."

    # feature loop
    - title: "سفارشی سازی علامت گرانول"
      content: "با API جامع ما از پتانسیل کامل سفارشی سازی واترمارک استفاده کنید. هر جزئیات از جمله اندازه، جهت گیری، طرح رنگ و انتخاب فونت را با جزئیات دقیق تنظیم کنید تا واترمارک هایی ایجاد کنید که کاملاً با الزامات برند و امنیتی شما هماهنگ باشد."

    # feature loop
    - title: "مهار ویژگی های خاص سند برای علامت گذاری انعطاف پذیر"
      content: "قدرت عملکردهای بومی را در قالب های مختلف سند باز کنید. از عناصری مانند پس زمینه سند، حاشیه نویسی، هدر یا سایر اشیاء به عنوان ظروف علامت واترمارک منحصر به فرد استفاده کنید و انواع مختلف اسناد و نیازهای امنیتی را تأمین می کند."
      
  code_samples:
    # code sample loop
    - title: "PDF ویرایش علامت تصویر"
      content: |
        این مثال نحوه ویرایش محتوای واترمارک تصویر را نشان می دهد
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  بارگذاری سند به عنوان PDF
            var loadOptions = new PdfLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pdf", loadOptions))
            {
                //  محتوا را بارگیری کنید
                PdfContent pdfContent = watermarker.GetContent<PdfContent>();

                //  ویرایش علامت تصویر
                foreach (PdfArtifact artifact in pdfContent.Pages[0].Artifacts)
                {
                    if (artifact.Image != null)
                    {
                        artifact.Image = new PdfWatermarkableImage(File.ReadAllBytes("test.png"));
                    }
                }

                //  از نتیجه خروجی لذت ببرید
                watermarker.save("result.pdf");
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
    title: "پردازش فرمت های دیگر"
    exclude: "RTF"
    description: "واترمارک های سند را به روشهای پیچیده با GroupDocs.Watermark for .NET SDK ویرایش کنید."
    items: 
        # format loop 1
        - name: "واترمارک PDF"
          format: "PDF"
          link: "/watermark/net/edit//pdf/"
          description: "ادوبی Portable فرمت سند"

        # format loop 2
        - name: "واترمارک Word"
          format: "WORD"
          link: "/watermark/net/edit//word/"
          description: "MS Word و اسناد آفیس باز"
          
        # format loop 3
        - name: "واترمارک Excel"
          format: "EXCEL"
          link: "/watermark/net/edit//excel/"
          description: "MS Excel و صفحات گسترده آفیس باز"

        # format loop 4
        - name: "واترمارک PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/edit//powerpoint/"
          description: "MS PowerPoint و ارائه های آفیس باز"

        # format loop 5
        - name: "واترمارک DOCX"
          format: "DOCX"
          link: "/watermark/net/edit//docx/"
          description: "مایکروسافت Word سند XML باز"
          
        # format loop 6
        - name: "واترمارک PPTX"
          format: "PPTX"
          link: "/watermark/net/edit//pptx/"
          description: "PowerPoint ارائه اکس‌ام‌ال باز"
          
        # format loop 7
        - name: "واترمارک XLSX"
          format: "XLSX"
          link: "/watermark/net/edit//xlsx/"
          description: "مایکروسافت Excel صفحه گسترده XML باز"

        # format loop 8
        - name: "واترمارک DOC"
          format: "DOC"
          link: "/watermark/net/edit//doc/"
          description: "سند مایکروسافت Word 97 - 2007"

        # format loop 9
        - name: "واترمارک XLS"
          format: "XLS"
          link: "/watermark/net/edit//xls/"
          description: "مایکروسافت Excel کتاب کار 97-2003"

        # format loop 10
        - name: "واترمارک PPT"
          format: "PPT"
          link: "/watermark/net/edit//ppt/"
          description: "PowerPoint ارائه ۹۷—۲۰۰۳"

        # format loop 11
        - name: "واترمارک RTF"
          format: "RTF"
          link: "/watermark/net/edit//rtf/"
          description: "فرمت متن غنی"

---