
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:19
draft: false
lang: fa
format: Word
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C# .NET API برای حذف علامت Word"
head_description: "با استفاده از C# .NET API ما برای ارائه سند بی عیب و نقص، واترمارک ها را از Word اسناد به طور موثر پاک کنید، حذف یا ویرایش کنید."

############################# Header ############################
title: "Word پاک کننده واترمارک برای C# .NET" 
description: "از GroupDocs.Watermark for .NET C# API برای حذف واترمارک ها از Word اسناد استفاده کنید که برای حفظ یکپارچگی و پاکیزگی اسناد حقوقی و شرکتی مناسب است."
subtitle: "GroupDocs.Watermark for .NET C# آپی" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود در Nuget به صورت رایگان"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET C# کتابخانه"
    link: "/watermark/net/"
    link_title: "بیشتر بدانید"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       با کتابخانه GroupDocs.Watermark for .NET C# .NET، توسعه دهندگان می توانند به راحتی واترمارک ها را در فایل های مایکروسافت Word مدیریت و حذف کنند. این ابزار از طیف گسترده ای از عملیات واترمارک، از جمله تشخیص، اصلاح و حذف علامت های متن و تصویر پشتیبانی می کند و ضمن حفظ طرح و قالب بندی، اطمینان حاصل می کند که اسناد عاری از علائم ناخواسته هستند.

############################# Steps ############################
steps:
    enable: true
    title: "حذف واترمارک از اسناد Word با استفاده از .NET"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/)** کار حذف واترمارک از اسناد تجاری را ساده می‌کند. با ادغام کتابخانه ما به برنامه .NET خود قدرت دهید و این مراحل ساده را دنبال کنید:
      
      1. با نمونه سازی کلاس اصلی، **Watermarker**، با سند Word شروع کنید. API ما از پردازش اسناد ارائه شده به عنوان یک جریان یا یک مسیر محلی پشتیبانی می کند.
      2. از **SearchCriteria** برای محدود کردن مجموعه واترمارک های مورد پردازش استفاده کنید. می توانید از پارامترهای مختلفی مانند تصاویر، متن یا ویژگی های قالب بندی استفاده کنید. هرچه پارامترهای جستجوی شما مشخص تر باشد، نتایج دقیق تری به دست می آورید.
      3. فهرست واترمارک های سند به دست آمده به عنوان یک نتیجه جستجو را پردازش کنید و آنها را از سند حذف کنید.
      4. پس از حذف واترمارک ها، سند حاصل را به عنوان یک فایل محلی یا یک جریان بایت ذخیره کنید.
   
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
        // علامت متنی را از سند Word حذف کنید

        // ارائه نمونه Watermarker برای سند منبع Word
        using (Watermarker watermarker = new Watermarker("input.داکس"))
        {
            // واترمارک های انتخاب شده را از سند حذف کنید
            TextFormattingSearchCriteria criteria = new TextFormattingSearchCriteria();
            criteria.ForegroundColorRange = new ColorRange();
            criteria.FontBold = true;
            PossibleWatermarkCollection watermarks = watermarker.Search(criteria);
            watermarks.Clear();

            // فایل را در مسیر ارائه شده ذخیره کنید
            watermarker.Save("output.داکس");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "حذف علامت واترمارک را با C# .NET API ساده کنید"
  description: "قابلیت های قدرتمند حذف واترمارک API C# .NET ما را کشف کنید که برای ادغام یکپارچه با برنامه های .NET شما طراحی شده است. در حالی که کیفیت اصلی فایل حفظ می شود، علامت های آب را از PDF s و اسناد اداری به طور موثر حذف یا پاک کنید."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "حذف علامت"
  features:
    # feature loop
    - title: "ترخیص واترمارک دقیق"
      content: ".NET API ما ابزارهای دقیقی را برای حذف واترمارک ها از هر سندی فراهم می کند. این ویژگی که برای توسعه دهندگان طراحی شده است، تضمین می کند که حذف واترمارک ها کیفیت یا طرح سند را به خطر نمی اندازد."

    # feature loop
    - title: "حذف علامت فله اتوماتیک"
      content: "فرآیند حذف واترمارک ها از مجموعه های اسناد بزرگ را با .NET API خودکارسازی کنید. ایده آل برای کسب و کارهایی که حجم زیادی از اسناد را مدیریت می کنند و هم کارایی و هم امنیت اسناد را بهبود می بخشند."

    # feature loop
    - title: "ویژگی های پیشرفته ویرایش واترمارک"
      content: "از ویژگی های پیشرفته برای ویرایش انتخابی یا اصلاح واترمارک ها استفاده کنید. API ما از تنظیمات دقیق پشتیبانی می کند تا اطمینان حاصل شود که اسناد شما در عین حال اطلاعات حساس از ظاهر حرفه ای حفظ می کنند."
      
  code_samples:
    # code sample loop
    - title: "علامت متن صفحات گسترده را حذف کنید"
      content: |
        نحوه حذف علامت های متنی با قالب بندی خاص در Excel اسناد.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  بارگیری کتاب کار Excel
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  محتوا را دریافت کنید و علامت مناسب را پیدا کنید
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();
                foreach (SpreadsheetWorksheet section in content.Worksheets)
                {
                    for (int i = section.Shapes.Count - 1; i >= 0; i--)
                    {
                        foreach (FormattedTextFragment fragment in section.Shapes[i].FormattedTextFragments)
                        {
                            if (fragment.ForegroundColor.Equals(Color.Red) && fragment.Font.FamilyName == "Arial")
                            {
                                //  حذف علامت متن
                                section.Shapes.RemoveAt(i);
                                break;
                            }
                        }
                    }
                }

                //  ذخیره پردازش شده XLSX
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
    title: "مدیریت Word واترمارک با .NET"
    exclude: "WORD"
    description: "ویژگی های قدرتمند مدیریت واترمارک در Word اسناد را با استفاده از API C# .NET که برای افزایش امنیت سند و ارائه بدون به خطر انداختن کیفیت طراحی شده است، کشف کنید."
    items: 
        # format loop 1
        - name: "واترمارک PDF"
          format: "PDF"
          link: "/watermark/net/remove//pdf/"
          description: "ادوبی Portable فرمت سند"

        # format loop 2
        - name: "واترمارک Word"
          format: "WORD"
          link: "/watermark/net/remove//word/"
          description: "MS Word و اسناد آفیس باز"
          
        # format loop 3
        - name: "واترمارک Excel"
          format: "EXCEL"
          link: "/watermark/net/remove//excel/"
          description: "MS Excel و صفحات گسترده آفیس باز"

        # format loop 4
        - name: "واترمارک PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/remove//powerpoint/"
          description: "MS PowerPoint و ارائه های آفیس باز"

        # format loop 5
        - name: "واترمارک DOCX"
          format: "DOCX"
          link: "/watermark/net/remove//docx/"
          description: "مایکروسافت Word سند XML باز"
          
        # format loop 6
        - name: "واترمارک PPTX"
          format: "PPTX"
          link: "/watermark/net/remove//pptx/"
          description: "PowerPoint ارائه اکس‌ام‌ال باز"
          
        # format loop 7
        - name: "واترمارک XLSX"
          format: "XLSX"
          link: "/watermark/net/remove//xlsx/"
          description: "مایکروسافت Excel صفحه گسترده XML باز"

        # format loop 8
        - name: "واترمارک DOC"
          format: "DOC"
          link: "/watermark/net/remove//doc/"
          description: "سند مایکروسافت Word 97 - 2007"

        # format loop 9
        - name: "واترمارک XLS"
          format: "XLS"
          link: "/watermark/net/remove//xls/"
          description: "مایکروسافت Excel کتاب کار 97-2003"

        # format loop 10
        - name: "واترمارک PPT"
          format: "PPT"
          link: "/watermark/net/remove//ppt/"
          description: "PowerPoint ارائه ۹۷—۲۰۰۳"

        # format loop 11
        - name: "واترمارک RTF"
          format: "RTF"
          link: "/watermark/net/remove//rtf/"
          description: "فرمت متن غنی"

---