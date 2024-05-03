
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:06
draft: false
lang: fa
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "ویرایش واترمارک ها در Powerpoint اسناد"
head_description: "ویرایش علامت Powerpoint را ساده کنید و اسناد خود را با GroupDocs.Watermark for .NET Library محافظت کنید. به کنترل دقیق و تطبیق پذیری دست یابید."

############################# Header ############################
title: "ویرایش Powerpoint جایگذاری علامت های آب: .NET دقت" 
description: "با GroupDocs.Watermark for .NET راه حل، کنترل دقیق بر روی قرار دادن علامت واترمارک و امنیت اسناد را به دست آورید. Powerpoint واترمارک ها را دقیقاً ویرایش کنید."
subtitle: "GroupDocs.Watermark for .NET کتابخانه" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود در Nuget"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET آپی"
    link: "/watermark/net/"
    link_title: "بیشتر بدانید"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **ویرایش Powerpoint قرار دادن علامت های آب:** با GroupDocs.Watermark for .NET توسعه دهندگان کنترل دقیق بر روی قرار دادن علامت واترمارک و امنیت اسناد را به دست آورید. گردش کار خود را ساده کنید و از اصالت بدون زحمت اطمینان حاصل کنید

############################# Steps ############################
steps:
    enable: true
    title: "ویرایش واترمارک در اسناد Powerpoint با استفاده از .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** به توسعه دهندگان .NET اجازه می‌دهد بدون زحمت واترمارک‌ها را در اسناد مختلف Powerpoint ویرایش کنند. در اینجا یک راهنمای ساده برای نحوه استفاده از API ما در برنامه خود آورده شده است:
      
      1. با ارسال فایل Powerpoint خود به عنوان پارامتر به سازنده کلاس **Watermarker** شروع کنید. می توانید فایل را به صورت جریان بایت، جریان فایل یا مسیر دیسک محلی ارائه دهید.
      2. سپس، واترمارک های خاصی را که نیاز به ویرایش دارند پیدا کنید. از **SearchCriteria** برای شناسایی واترمارک ها با ویژگی های مربوطه که قبلاً به سند اضافه شده است استفاده کنید.
      3. پس از جستجو، فهرستی از واترمارک های مربوطه را دریافت خواهید کرد. سپس می‌توانید ویژگی‌های آن‌ها مانند اندازه، تراز صفحه، متن، رنگ، محتوای تصویر و موارد دیگر را سفارشی کنید. این به شما کنترل گسترده ای بر روی داده های خود می دهد.
      4. پس از تکمیل ویرایش واترمارک ها، سند به روز شده را ذخیره کنید. می توانید از یک مسیر فایل محلی یا یک جریان برای ذخیره نتیجه نهایی استفاده کنید.
   
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
        // واترمارک متنی POWERPOINT را ویرایش کنید

        // Watermarker را به ارائه فایل POWERPOINT تبدیل کنید
        using (Watermarker watermarker = new Watermarker("input.پی‌تی‌اکس"))
        {
            // TextSearchCriteria را بسازید و واترمارک متنی را دریافت کنید
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                 // واترمارک متن را ویرایش کنید
                 watermark.FormattedTextFragments.Clear();
                 watermark.FormattedTextFragments.Add("passed", 
                    new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
            }

            // سند را ذخیره کنید
            watermarker.Save("output.پی‌تی‌اکس");
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
    title: "تصفیه واترمارک ها در فرمت های دیگر"
    exclude: "POWERPOINT"
    description: "واترمارک ها را در قالب های مختلف سند با GroupDocs.Watermark for .NET ویرایش کنید."
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