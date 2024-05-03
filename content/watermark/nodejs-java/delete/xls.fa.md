
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:18
draft: false
lang: fa
format: Xls
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "حذف دقیق علامت های واترن در XLS صفحات گسترده"
head_description: "GroupDocs.Watermark کنترل دقیق بر حذف واترمارک های خاص را ارائه می دهد."

############################# Header ############################
title: "XLS واترمارک خاص هدف" 
description: "علامت های ناخواسته را به طور انتخابی حذف کنید و در حالی که علامت های مورد نظر را با GroupDocs.Watermark حفظ کنید."
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود در NPM به صورت رایگان"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "بیشتر بدانید"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark توسعه دهندگان را با توانایی هدف قرار دادن و حذف علامت های خاص در اسناد فراهم می کند. این کنترل دانه ای ویرایش دقیق سند را تضمین می کند و به شما امکان می دهد واترمارک های قدیمی یا بی ربط را در عین حال حفظ اطلاعات مهم حذف کنید. GroupDocs.Watermark به طور یکپارچه با محیط .NET ادغام می شود و حذف واترمارک را برای فرمت های مختلف فایل ساده می کند.

############################# Steps ############################
steps:
    enable: true
    title: "حذف بدون زحمت واترمارک ها از Xls توسط Node.js via Java"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/nodejs-java/)** فرآیند حذف واترمارک از اسناد تجاری را ساده می‌کند. برنامه Node.js via Java خود را با ادغام یکپارچه کتابخانه ما و دنبال کردن این مراحل ساده ارتقا دهید:
      
      1. فرآیند را با نمونه سازی کلاس اصلی، **Watermarker** با سند Xls آغاز کنید. API همه کاره ما به صورت یکپارچه اسناد را پردازش می کند، چه به صورت جریان یا یک مسیر محلی ارائه شود.
      2. از **SearchCriteria** برای تعیین دقیق واترمارک هایی که باید پرداخته شوند، استفاده کنید. از پارامترهای مختلف مانند تصاویر، متن یا ویژگی های قالب بندی برای اصلاح جستجوی خود استفاده کنید. هرچه معیارهای شما دقیق تر باشد، نتایج شما دقیق تر است.
      3. فرآیند حذف را در فهرست واترمارک های سند بازیابی شده از طریق جستجوی خود اجرا کنید. بدون زحمت آنها را از سند حذف کنید.
      4. پس از حذف موفقیت آمیز واترمارک ها، سند حاصل را به صورت ایمن به عنوان یک فایل محلی یا یک جریان بایت ذخیره کنید و یکپارچگی آن را حفظ کنید.
   
    code:
      platform: "net"
      copy_title: "کپی کردن"
      install:
        command: "npm i @groupdocs/groupdocs.watermark"
        copy_tip: "برای کپی کلیک کنید"
        copy_done: "کپی شده"
      links:
        #  loop
        - title: "نمونه های بیشتر"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
        #  loop
        - title: "مستندات"
          link: "https://docs.groupdocs.com/watermark/nodejs-java/"
          
      content: |
        ```javascript {style=abap}

        // واترمارک تصویر را در سند XLS حذف کنید

        // دریافت Watermarker مسیر XLS به عنوان آرگومان
        const watermarker = new groupdocs.watermark.Watermarker("input.xls");
        
        // واترمارک های تصویر را با معیارهای جستجو پاک کنید
        const searchCriteria = 
            new groupdocs.watermark.ImageDctHashSearchCriteria("logo.png");
        const watermarks = watermarker.search(searchCriteria);
        watermarks.clear();

        // فایل پردازش شده را ذخیره کنید
        watermarker.save("output.xls");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Node.js via Java API برای حذف علامت | GroupDocs.Watermark"
  description: "API Node.js via Java ما را یکپارچه کنید تا علامت های آب را بدون زحمت از اسناد حذف کنید، وضوح و زیبایی شناسی اسناد را افزایش دهید. این API متناسب با محیط Node.js via Java است، برای برنامه هایی که نیاز به پردازش و ارائه اسناد پاک بدون علامت دارند مناسب است."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "حذف علامت"
  features:
    # feature loop
    - title: "حذف واترمارک ساده برای Node.js via Java"
      content: "API ما ابزارهای ساده حذف واترمارک را ارائه می دهد که به طور خاص برای Node.js via Java برنامه طراحی شده اند و توسعه دهندگان را قادر می سازد تا خوانایی سند و ظاهر حرفه ای را بدون کدگذاری پیچیده افزایش دهند."

    # feature loop
    - title: "Node.js via Java پاک کردن واترمارک دسته ای"
      content: "با ویژگی پردازش دسته ای ما از توانایی پاک کردن واترمارک ها از چندین سند در یک زمان استفاده کنید. این به ویژه برای برنامه هایی مفید است که نیاز به مدیریت سریع و کارآمد جریان های اسناد بزرگ دارند."

    # feature loop
    - title: "ویرایش واترمارک انعطاف پذیر از طریق Node.js via Java"
      content: "با استفاده از ابزارهای ویرایش انعطاف پذیر ما، واترمارک ها را تنظیم، اصلاح یا کاملاً حذف کنید. این ویژگی به Node.js via Java توسعه دهندگان اجازه می دهد تا پردازش اسناد را متناسب با نیازهای تجاری خاص یا درخواست های مشتری تنظیم کنند و نتایج بهینه را تضمین کنند."
      
  code_samples:
    # code sample loop
    - title: "واترمارک هدر صفحه گسترده را حذف کنید"
      content: |
        این مثال نحوه حذف واترمارک هایی را که در XLSX هدر قرار داده شده اند نشان می دهد
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  بارگذاری کتاب صفحه گسترده
            const loadOptions = new groupdocsWatermark.SpreadsheetLoadOptions();
            const watermarker = new groupdocsWatermark.Watermarker("source.xlsx", loadOptions);

            //  لیست بخش های هدر را دریافت کنید
            const content = watermarker.getContent(groupdocsWatermark.SpreadsheetContent.class);
            const sections = content.getWorksheets().get_Item(0).getHeadersFooters()
                .getByOfficeHeaderFooterType(groupdocsWatermark.OfficeHeaderFooterType.HeaderPrimary).getSections();
  
            //  واترمارک ها را از هدر حذف کنید
            for (const section of sections.getInnerList().toArray()) {
                section.setScript(null);
                section.setImage(null);
            }

            //  ذخیره کتاب کار پاک شده
            watermarker.save("result.xlsx");
            watermarker.close();

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "آماده شروع هستید؟"
  description: "ویژگی های GroupDocs.Watermark را به صورت رایگان امتحان کنید یا مجوز درخواست کنید"
  items:
    #  loop
    - title: "NPM دانلود"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      color: "red"
        #  loop
    - title: "صدور مجوز"
      link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "حذف دقیق در سراسر فرمت ها"
    exclude: "XLS"
    description: "واترمارک های خاص را در انواع مختلف سند با GroupDocs.Watermark هدف قرار دهید."
    items: 
        # format loop 1
        - name: "واترمارک PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/delete//pdf/"
          description: "ادوبی Portable فرمت سند"

        # format loop 2
        - name: "واترمارک Word"
          format: "WORD"
          link: "/watermark/nodejs-java/delete//word/"
          description: "MS Word و اسناد آفیس باز"
          
        # format loop 3
        - name: "واترمارک Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/delete//excel/"
          description: "MS Excel و صفحات گسترده آفیس باز"

        # format loop 4
        - name: "واترمارک PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/delete//powerpoint/"
          description: "MS PowerPoint و ارائه های آفیس باز"

        # format loop 5
        - name: "واترمارک DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/delete//docx/"
          description: "مایکروسافت Word سند XML باز"
          
        # format loop 6
        - name: "واترمارک PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/delete//pptx/"
          description: "PowerPoint ارائه اکس‌ام‌ال باز"
          
        # format loop 7
        - name: "واترمارک XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/delete//xlsx/"
          description: "مایکروسافت Excel صفحه گسترده XML باز"

        # format loop 8
        - name: "واترمارک DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/delete//doc/"
          description: "سند مایکروسافت Word 97 - 2007"

        # format loop 9
        - name: "واترمارک XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/delete//xls/"
          description: "مایکروسافت Excel کتاب کار 97-2003"

        # format loop 10
        - name: "واترمارک PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/delete//ppt/"
          description: "PowerPoint ارائه ۹۷—۲۰۰۳"

        # format loop 11
        - name: "واترمارک RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/delete//rtf/"
          description: "فرمت متن غنی"

---