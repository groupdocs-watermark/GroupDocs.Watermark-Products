
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:27:00
draft: false
lang: fa
format: Word
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "علامت های پنهان را در Word اسناد پیدا کنید"
head_description: "علامت های پنهان را در اسناد بدون زحمت با GroupDocs.Watermark پیدا کنید."

############################# Header ############################
title: "بدون زحمت، علامت های پنهان را در Word اسناد پیدا کنید" 
description: "به سرعت علامت های پنهان را با GroupDocs.Watermark for .NET شناسایی و مدیریت کنید."
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Nuget بسته به صورت رایگان"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET اطلاعات"
    link: "/watermark/net/"
    link_title: "بیشتر بدانید"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET یک راه حل جامع برای مدیریت واترمارک ها با استفاده از .NET ارائه می دهد. به راحتی واترمارک ها را از انواع قالب های سند از جمله PDF، Microsoft Word، Excel و موارد دیگر تولید، ویرایش، و حذف کنید. با استفاده از GroupDocs.Watermark for .NET واترمارک ها را با برنامه های خود پیدا کنید.

############################# Steps ############################
steps:
    enable: true
    title: "یافتن واترمارک ها در Word فایل ها با استفاده از .NET"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/)** روند یافتن واترمارک در اسناد تجاری را ساده می کند. بسته ما را در .NET برنامه های خود ادغام کنید تا مزایای آن را باز کنید.
      
      1. **Watermarker** بارگذاری کنید. شما می توانید مسیر فایل، جریان فایل یا جریان بایت را ارائه دهید.
      2. {steps.content.step_2}
      3. **جستجو** شیء **Watermarker** برای بازیابی علامت های قرار داده شده در سند استفاده کنید. شما مجموعه ای از اشیاء را نشان دهنده علامت های بالقوه برای پردازش بیشتر دریافت خواهید کرد.
      4. در نهایت، شما انعطاف پذیری را برای دستکاری نتایج جستجو در صورت نیاز دارید. می توانید واترمارک های یافت شده را حذف کنید یا خواص آنها مانند تغییر اندازه یا متن را ویرایش کنید.
   
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
        // پیدا کردن واترمارک متن در WORD

        // ایجاد واترمارکر با مسیر WORD
        using (Watermarker watermarker = new Watermarker("input.داکس"))
        {
            // علامت های آب را پیدا کنید
            PossibleWatermarkCollection possibleWatermarks = watermarker.Search();

            // از اطلاعات واترمارک های یافت شده استفاده کنید
            foreach (PossibleWatermark possibleWatermark in possibleWatermarks)
            {
                Console.WriteLine(possibleWatermark.Text);
                Console.WriteLine(possibleWatermark.Width);
                Console.WriteLine(possibleWatermark.Height);
            }
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "با GroupDocs.Watermark به طور موثر جستجو و پیدا کردن واترمارک ها"
  description: "از قدرت GroupDocs.Watermark برای جستجو و یافتن واترمارک ها در هر نوع سند با استفاده از C# در .NET استفاده کنید."
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "جستجوی واترمارک ها"
  features:
    # feature loop
    - title: "کشف واترمارک ها با جستجوی پیشرفته"
      content: "از GroupDocs.Watermark برای یافتن بدون زحمت واترمارک ها در انواع مختلف سند استفاده کنید. ابزارهای ما به شما امکان می دهد با پارامترهایی مانند محتوا، اندازه و کدورت جستجو کنید."

    # feature loop
    - title: "یافتن واترمارک ها با پارامترهای سفارشی"
      content: "معیارهای جستجوی خود را با GroupDocs.Watermark تنظیم کنید تا واترمارک ها را بر اساس ویژگی های خاص پیدا کنید و اطمینان حاصل کنید که می توانید آنها را به طور موثر مدیریت و بررسی کنید."

    # feature loop
    - title: "بازیابی و مدیریت واترمارک ها به طور موثر"
      content: "با بازیابی سریع همه واترمارک ها در یک سند، روند مدیریت اسناد خود را ساده کنید. API ما امکان شناسایی و تجزیه و تحلیل سریع واترمارک ها را فراهم می کند."
      
  code_samples:
    # code sample loop
    - title: "مثال C #: جستجو برای واترمارک ها"
      content: |
        این مثال C# نشان می دهد که چگونه واترمارک ها را در هر سند با استفاده از GroupDocs.Watermark جستجو کنید و نحوه استفاده از پارامترها برای یافتههای دقیق را نشان میدهد.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  سند را از یک منبع محلی یا شبکه ای برای پردازش بارگیری کنید
            var loadOptions = new WordProcessingLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.docx", loadOptions))
            {
                //  پارامترهای جستجوی واترمارک، مانند نوع یا دید را تعریف کنید
                Regex regex = new Regex(@"^© \d{4}$");

                //  بازیابی تمام واترمارک هایی که با معیارهای مشخص شده مطابقت دارند
                TextSearchCriteria textSearchCriteria = new TextSearchCriteria(regex);
                PossibleWatermarkCollection possibleWatermarks = watermarker.Search(textSearchCriteria);

                //  لیست علامت های یافت شده را مرور و مدیریت کنید تا تأثیر آنها را ارزیابی کنید
                Console.WriteLine("Found {0} possible watermark(s).", possibleWatermarks.Count);
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
    title: "واترمارک ها را در فرمت های پشتیبانی شده کشف کنید"
    exclude: "WORD"
    description: "به سرعت واترمارک ها را در طیف گسترده ای از فرمت های فایل پشتیبانی شده پیدا کرده و مدیریت کنید."
    items: 
        # format loop 1
        - name: "واترمارک PDF"
          format: "PDF"
          link: "/watermark/net/find//pdf/"
          description: "ادوبی Portable فرمت سند"

        # format loop 2
        - name: "واترمارک Word"
          format: "WORD"
          link: "/watermark/net/find//word/"
          description: "MS Word و اسناد آفیس باز"
          
        # format loop 3
        - name: "واترمارک Excel"
          format: "EXCEL"
          link: "/watermark/net/find//excel/"
          description: "MS Excel و صفحات گسترده آفیس باز"

        # format loop 4
        - name: "واترمارک PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/find//powerpoint/"
          description: "MS PowerPoint و ارائه های آفیس باز"

        # format loop 5
        - name: "واترمارک DOCX"
          format: "DOCX"
          link: "/watermark/net/find//docx/"
          description: "مایکروسافت Word سند XML باز"
          
        # format loop 6
        - name: "واترمارک PPTX"
          format: "PPTX"
          link: "/watermark/net/find//pptx/"
          description: "PowerPoint ارائه اکس‌ام‌ال باز"
          
        # format loop 7
        - name: "واترمارک XLSX"
          format: "XLSX"
          link: "/watermark/net/find//xlsx/"
          description: "مایکروسافت Excel صفحه گسترده XML باز"

        # format loop 8
        - name: "واترمارک DOC"
          format: "DOC"
          link: "/watermark/net/find//doc/"
          description: "سند مایکروسافت Word 97 - 2007"

        # format loop 9
        - name: "واترمارک XLS"
          format: "XLS"
          link: "/watermark/net/find//xls/"
          description: "مایکروسافت Excel کتاب کار 97-2003"

        # format loop 10
        - name: "واترمارک PPT"
          format: "PPT"
          link: "/watermark/net/find//ppt/"
          description: "PowerPoint ارائه ۹۷—۲۰۰۳"

        # format loop 11
        - name: "واترمارک RTF"
          format: "RTF"
          link: "/watermark/net/find//rtf/"
          description: "فرمت متن غنی"

---