
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:20
draft: false
lang: fa
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "به روز رسانی واترمارک ها در POWERPOINT بدون زحمت"
head_description: "به طور موثر واترمارک ها را در قالب های POWERPOINT سند با استفاده از GroupDocs.Watermark for Node.js via Java به روز کنید. فرآیندهای کسب و کار خود را پالش کنید."

############################# Header ############################
title: "بدون زحمت به روز رسانی POWERPOINT واترمارک های سند" 
description: "حذف علامت بدون دردسر با GroupDocs.Watermark for Node.js via Java تجربه کنید. از اسناد کسب و کار خود با علامت های مختلف محافظت کنید. ابعاد واترمارک، تراز، زاویه چرخش و قرار دادن و موارد دیگر را سفارشی کنید."
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دریافت رایگان از NPM"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java آپی"
    link: "/watermark/nodejs-java/"
    link_title: "بیشتر بدانید"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java یک راه حل کاربر پسند برای مدیریت POWERPOINT واترمارک با استفاده از Node.js via Java ارائه می دهد. با استفاده از این ابزار، توسعه دهندگان می توانند به طور کارآمد واترمارک ها را در اسناد و فرمت های فایل مختلف از جمله PDF، مایکروسافت Word، Excel، PowerPoint، Visio، و فرمت های ایمیل به روز کنند. GroupDocs.Watermark از تمام سیستم عامل های اصلی و Node.js via Java نسخه پشتیبانی می کند.

############################# Steps ############################
steps:
    enable: true
    title: "به روز رسانی واترمارک در POWERPOINT از طریق Node.js via Java"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** توسعه‌دهندگان Node.js via Java را به یک API قوی برای به‌روزرسانی برنامه‌نویسی واترمارک‌ها در اسناد مختلف POWERPOINT مجهز می‌کند. این راهنما فرآیند را تشریح می کند:
      
      1. فرآیند را با ارائه فایل POWERPOINT خود به عنوان آرگومان برای سازنده کلاس **Watermarker** شروع کنید. بسته به درخواست شما، فایل می تواند به عنوان یک جریان یا یک مرجع به یک مکان دیسک محلی ارائه شود.
      2. متعاقباً، از شیء **SearchCriteria** برای شناسایی واترمارک‌های خاصی که نیاز به اصلاح دارند، استفاده کنید. این شیء تعیین واترمارک ها را بر اساس ویژگی های مورد نظر امکان پذیر می کند.
      3. پس از اجرای موفقیت آمیز جستجو، مجموعه ای از واترمارک های مربوطه را دریافت خواهید کرد. این واترمارک ها کنترل دانه ای را ارائه می دهند که به شما امکان می دهد ویژگی هایی مانند ابعاد، موقعیت صفحه، محتوای متن، طرح رنگ، داده های تصویر و موارد دیگر را به روز کنید.
      4. پس از تکمیل به‌روزرسانی‌های واترمارک، سند اصلاح شده را ادامه دهید. API ذخیره سازی را با استفاده از یک مسیر فایل محلی یا یک شی جریان تسهیل می کند.
   
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

        // واترمارک متنی POWERPOINT را به روز کنید

        // ارائه نمونه Watermarker برای فایل POWERPOINT
        const watermarker = new groupdocs.watermark.Watermarker("input.پی‌تی‌اکس");

        // از TextSearchCriteria برای یافتن واترمارک متن استفاده کنید
        const searchCriteria = 
            new groupdocs.watermark.TextSearchCriteria("test", false);
        const watermarks = watermarker.search(searchCriteria);
        
        // به روز رسانی واترمارک متنی
        for (const watermark of watermarks.getInnerList().toArray())
        {
            watermark.setText("passed");
        }

        // از نتیجه لذت ببرید
        watermarker.save("output.پی‌تی‌اکس");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "تسلط بر ویرایش واترمارک در PDF ثانیه با GroupDocs.Watermark"
  description: "ویژگی های جامع API را برای تنظیم و مدیریت واترمارک ها در PDF s در Node.js via Java برنامه بررسی کنید."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "ویرایش واترمارک"
  features:
    # feature loop
    - title: "بدون زحمت واترمارک ها را در PDF s ویرایش کنید"
      content: "GroupDocs.Watermark ابزارهای قدرتمندی را در Node.js via Java برای ویرایش یکپارچه واترمارک های موجود در PDF اسناد ارائه می دهد. موقعیت، شفافیت و موارد دیگر را با سهولت تنظیم کنید."

    # feature loop
    - title: "جزئیات واترمارک را برای دقیق اصلاح کنید"
      content: "کنترل جزئیات را در دست بگیرید. API ما به شما امکان می دهد ظاهر واترمارک ها را با جزئیات تنظیم کنید و تغییرات دقیق اندازه، کدورت و رنگ را در PDF s خود فعال کنید."

    # feature loop
    - title: "مدیریت واترمارک ساده"
      content: "API ما مدیریت واترمارک را ساده می کند. چه به روزرسانی و چه حذف کنید، می توانید واترمارک ها را به طور موثر مدیریت کنید و یکپارچگی اسناد را حفظ کنید و در عین حال نیازهای برندسازی خود"
      
  code_samples:
    # code sample loop
    - title: "Java مثال: ویرایش PDF واترمارک"
      content: |
        این مثال Java نحوه ویرایش یک واترمارک موجود در یک سند PDF را نشان می دهد و نحوه تنظیم خواص آن به صورت برنامه نویسی را نشان می دهد.
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  سند PDF را برای پردازش بارگیری کنید
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  علامت های خاصی را جستجو کنید که معیارهای شما را برآورده می کنند
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria("test", false);
            const watermarks = watermarker.search(searchCriteria);
  
            //  تنظیمات علامت، مانند اندازه، رنگ و موقعیت را ویرایش کنید
            for (const watermark of watermarks.getInnerList().toArray()) {
                watermark.getFormattedTextFragments().clear();
                watermark.getFormattedTextFragments().add("passed", 
                    new groupdocsWatermark.Font("Calibri", 19, groupdocsWatermark.FontStyle.Bold), 
                    groupdocsWatermark.Color.getRed(), groupdocsWatermark.Color.getAqua());
            }

            //  سند به روز شده را در یک سیستم محلی ذخیره کنید یا آن را مستقیماً پخش کنید
            watermarker.save("result.pdf");
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
    title: "به روز رسانی واترمارک ها در فرمت های دیگر فایل"
    exclude: "POWERPOINT"
    description: "به طور موثر واترمارک ها را در PDF، Word، Excel و غیره با استفاده از GroupDocs.Watermark for Node.js via Java به روز کنید. ما از تمام فرمت های تجاری محبوب پشتیبانی می کنیم."
    items: 
        # format loop 1
        - name: "واترمارک PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/update//pdf/"
          description: "ادوبی Portable فرمت سند"

        # format loop 2
        - name: "واترمارک Word"
          format: "WORD"
          link: "/watermark/nodejs-java/update//word/"
          description: "MS Word و اسناد آفیس باز"
          
        # format loop 3
        - name: "واترمارک Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/update//excel/"
          description: "MS Excel و صفحات گسترده آفیس باز"

        # format loop 4
        - name: "واترمارک PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/update//powerpoint/"
          description: "MS PowerPoint و ارائه های آفیس باز"

        # format loop 5
        - name: "واترمارک DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/update//docx/"
          description: "مایکروسافت Word سند XML باز"
          
        # format loop 6
        - name: "واترمارک PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/update//pptx/"
          description: "PowerPoint ارائه اکس‌ام‌ال باز"
          
        # format loop 7
        - name: "واترمارک XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/update//xlsx/"
          description: "مایکروسافت Excel صفحه گسترده XML باز"

        # format loop 8
        - name: "واترمارک DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/update//doc/"
          description: "سند مایکروسافت Word 97 - 2007"

        # format loop 9
        - name: "واترمارک XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/update//xls/"
          description: "مایکروسافت Excel کتاب کار 97-2003"

        # format loop 10
        - name: "واترمارک PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/update//ppt/"
          description: "PowerPoint ارائه ۹۷—۲۰۰۳"

        # format loop 11
        - name: "واترمارک RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/update//rtf/"
          description: "فرمت متن غنی"

---