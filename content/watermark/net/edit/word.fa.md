
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:58
draft: false
lang: fa
format: Word
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "ویرایش واترمارک ها در Word اسناد"
head_description: "جایگذاری واترمارک را اصلاح کنید و امنیت سند را با GroupDocs.Watermark for .NET اطمینان حاصل کنید. Word واترمارک ها را بدون زحمت در راه حل های خود تنظیم کنید."

############################# Header ############################
title: "افزایش Word علامت های آب: .NET اعتماد به نفس" 
description: "اطمینان حاصل کنید که Word اسناد صحت و یکپارچگی برند با GroupDocs.Watermark for .NET. واترمارک ها را با اطمینان با استفاده از راه حل ما ویرایش کنید."
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
       **افزایش Word امنیت اسناد:** GroupDocs.Watermark for .NET توسعه دهندگان را قادر می سازد تا امنیت اسناد را با سهولت افزایش دهند. واترمارک های خود را ویرایش کنید تا با اطمینان نیازهای خاص خود را برآورده کنید.

############################# Steps ############################
steps:
    enable: true
    title: "ویرایش واترمارک ها در Word اسناد با استفاده از .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** توسعه دهندگان .NET را قادر می سازد تا بدون زحمت واترمارک ها را در Word اسناد مختلف ویرایش کنند. در اینجا یک راهنمای ساده برای استفاده از API ما در برنامه شما آورده شده است:
      
      1. **Watermarker** شروع کنید. شما می توانید فایل را به عنوان جریان بایت، جریان فایل یا مسیر دیسک محلی ارائه دهید.
      2. **معیارهای جستجو** برای شناسایی واترمارک ها با خواص مربوطه که قبلاً به سند اضافه شده است استفاده کنید.
      3. پس از جستجو، لیستی از واترمارک های مربوطه را دریافت خواهید کرد. سپس می توانید خواص آنها مانند اندازه، تراز صفحه، متن، رنگ، محتوای تصویر و موارد دیگر را سفارشی کنید. این به شما کنترل گسترده ای بر داده های خود می دهد.
      4. پس از اتمام ویرایش واترمارک ها، سند به روز شده را ذخیره کنید. شما می توانید از یک مسیر فایل محلی یا یک جریان برای ذخیره نتیجه نهایی استفاده کنید.
   
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
        // ویرایش WORD علامت متن

        // واترمارکر را برای ارائه فایل WORD ایجاد کنید
        using (Watermarker watermarker = new Watermarker("input.داکس"))
        {
            // معیارهای TextSearchCriteria را بسازید و علامت های متن را دریافت کنید
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                 // ویرایش علامت متن
                 watermark.FormattedTextFragments.Clear();
                 watermark.FormattedTextFragments.Add("passed", 
                    new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
            }

            // سند را ذخیره کنید
            watermarker.Save("output.داکس");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "درباره اصلاح واترمارک ها بیشتر بدانید"
  description: ".NET برنامه های خود را با کتابخانه ما توانمند کنید و واترمارک ها را در قالب های مختلف فایل اضافه، ویرایش، حذف یا جستجو کنید."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "ویرایش واترمارک"
  features:
    # feature loop
    - title: "فایل های واترمارک برای کسب و کار شما"
      content: "از GroupDocs.Watermark for .NET برای علامت گذاری فایل ها و اسناد استفاده کنید. بدون تلاش اضافی برای پیاده سازی API ما در برنامه های خود، واترمارک ها را اضافه و مدیریت کنید. علامت های اضافه شده قبلی را جستجو، ویرایش و حذف کنید."

    # feature loop
    - title: "تنظیم دقیق واترمارک ها برای نیازهای شما"
      content: "API ما مجموعه ای جامع از گزینه های سفارشی سازی را ارائه می دهد. برای ایجاد علامت ایده آل، جنبه هایی مانند اندازه، جهت گیری، طرح رنگ، خانواده فونت و موارد دیگر را بدون زحمت تغییر دهید."

    # feature loop
    - title: "از ویژگی های خاص سند استفاده کنید"
      content: "بسته به قالب پرونده ای که استفاده می کنید، می توانید ویژگی های داخلی را بگنجانید. اینها ممکن است شامل پس زمینه سند، حاشیه نویسی، هدر یا سایر عناصر باشد که به عنوان ظروف واترمارک عمل کنند."
      
  code_samples:
    # code sample loop
    - title: "Excel ویرایش متن واترمارک"
      content: |
        این مثال نحوه ویرایش متن برای واترمارک های خاص در Excel برگه ها را نشان می دهد
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  بارگیری صفحه گسترده XLSX
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  محتوای صفحه گسترده را بارگیری کنید
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();

                //  ویرایش متن داخلی واترمارک
                foreach (SpreadsheetShape shape in content.Worksheets[0].Shapes)
                {
                    if (shape.Text == "GroupDocs 2016")
                    {
                        shape.Text = "GroupDocs 2017";
                    }
                }

                //  ذخیره نتیجه خروجی
                watermarker.save("result.xlsx");
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
    title: "امنیت فرمت های دیگر را افزایش دهید"
    exclude: "WORD"
    description: "GroupDocs.Watermark for .NET راه حل های کارآمد را برای افزایش امنیت اسناد در فرمت های مختلف ارائه می دهد."
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