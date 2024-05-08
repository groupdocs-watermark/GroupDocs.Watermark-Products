
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:19
draft: false
lang: fa
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Excel حذف علامت با C# .NET API "
head_description: "از C# .NET API ما برای حذف و مدیریت کارآمد واترمارک ها در Excel اسناد استفاده کنید و از وضوح داده ها و یکپارچگی برگه اطمینان حاصل کنید."

############################# Header ############################
title: "C# .NET برای Excel عملیات واترمارک" 
description: "با حذف یکپارچه یا ویرایش واترمارک ها، با ابزارهایی که برای دقت و سهولت استفاده طراحی شده اند، گردش کار Excel سند خود را در محیط .NET بهبود دهید."
subtitle: "GroupDocs.Watermark for .NET C# آپی" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود رایگان Nuget بسته"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET C# کتابخانه"
    link: "/watermark/net/"
    link_title: "بیشتر بدانید"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       کتابخانه GroupDocs.Watermark for .NET C# ابزارهای قوی برای مدیریت واترمارک ها در Excel فایل فراهم می کند. از حذف علائم ناخواسته گرفته تا ویرایش علائم موجود، کنترل جامع واترمارک را تسهیل می کند، ایده آل برای کسب و کارهایی که پاکیزگی و حرفه ای بودن اسناد را او

############################# Steps ############################
steps:
    enable: true
    title: "حذف واترمارک از اسناد Excel با استفاده از .NET"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/)** کار حذف واترمارک از اسناد تجاری را ساده می‌کند. با ادغام کتابخانه ما به برنامه .NET خود قدرت دهید و این مراحل ساده را دنبال کنید:
      
      1. با نمونه سازی کلاس اصلی، **Watermarker**، با سند Excel شروع کنید. API ما از پردازش اسناد ارائه شده به عنوان یک جریان یا یک مسیر محلی پشتیبانی می کند.
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
        // علامت متنی را از سند Excel حذف کنید

        // ارائه نمونه Watermarker برای سند منبع Excel
        using (Watermarker watermarker = new Watermarker("input.اکس‌اس‌لکس"))
        {
            // واترمارک های انتخاب شده را از سند حذف کنید
            TextFormattingSearchCriteria criteria = new TextFormattingSearchCriteria();
            criteria.ForegroundColorRange = new ColorRange();
            criteria.FontBold = true;
            PossibleWatermarkCollection watermarks = watermarker.Search(criteria);
            watermarks.Clear();

            // فایل را در مسیر ارائه شده ذخیره کنید
            watermarker.Save("output.اکس‌اس‌لکس");
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
    title: "ساده سازی Excel حذف علامت در .NET"
    exclude: "EXCEL"
    description: "یاد بگیرید که چگونه از GroupDocs.Watermark for .NET C# API برای حذف موثر علامت های آب از Excel ورق استفاده کنید و از گزارش های مالی و تجزیه و تحلیل داده ها بکر و قابل ارائه اطمینان حاصل کنید."
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