
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:26
draft: false
lang: fa
format: Webp
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "واترمارک ها را در WEBP با Node.js جاسازی کنید"
head_description: "از Node.js برای اعمال علامت های پیشرفته روی تصاویر WEBP استفاده کنید و حفاظت و کپی رایت را افزایش دهید."

############################# Header ############################
title: "ایجاد واترمارک برای WEBP تصاویر از طریق Node.js" 
description: "Node.js را برای تولید علامت های سفارشی و ایمن برای فایل WEBP پیاده سازی کنید، ایده آل برای سازندگان محتوای دیجیتال که به دنبال محافظت از تصاویر خود هستند."
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
       GroupDocs.Watermark for Node.js via Java توسعه دهندگان Node.js را به ابزارهایی برای اضافه کردن، مدیریت و سفارشی سازی واترمارک ها در تصاویر WEBP مجهز می کند. این API امکان ادغام علامت های شفاف یا مات را فراهم می کند که به طور یکپارچه با تصویر ترکیب می شوند و اطمینان حاصل می کند که یکپارچگی آثار هنری در عین حال محافظت در برابر استفاده غیرمجاز حفظ می شود. اندازه، کدورت و موقعیت واترمارک را تنظیم کنید تا برند خود را برجسته کند یا دارایی های دیجیتال خود را به طور مخفیانه ایمن کنید. مناسب برای عکاسان، طراحان گرافیک و هر حرفه ای که با رسانه های دیجیتال سروکار دارند، GroupDocs.Watermark امنیت تصاویر WEBP را از طریق یک رابط Node.js انعطاف پذیر و قدرتمند افزایش می دهد.

############################# Steps ############################
steps:
    enable: true
    title: "محافظت از اسناد تجاری: واترمارک های Webp ایجاد کنید"
    content: |
      تقویت امنیت سند با **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/):** - یک راه حل قدرتمند برای تولید واترمارک برای Node.js via Java.
      
      1. **در برنامه های کاربردی Node.js via Java خود، واترمارک ایمن را ساده کنید:** کلاس **Watermarker** به عنوان جزء اصلی API GroupDocs.Watermark عمل می کند. این کتابخانه تولید واترمارک فرمت‌های مختلف سند، از جمله Webp را ساده می‌کند. برای شروع، قبل از پردازش سند خود یک نمونه Watermarker ایجاد کنید. مسیر فایل Webp یا یک شی جریان را در حین مقداردهی اولیه به سازنده ارائه دهید.
      2. ** ایجاد واترمارک برای حفاظت پیشرفته:** واترمارک هایی را تقویت کنید که کاملاً با نیازهای امنیتی شما هماهنگ باشد. یک شی **Watermark** بسازید که نوع مورد نظر را مشخص کنید. برخلاف قرار دادن صفحات سنتی، می‌توانید واترمارک‌ها را در عناصر سند بومی مانند سرصفحه‌ها یا پیوست‌ها جاسازی کنید، امنیت سند را تقویت کرده و یک لمس حرفه‌ای به آن اضافه کنید.
      3. ** تنظیم دقیق ظاهر واترمارک برای تاثیر بهینه:** جنبه های بصری واترمارک های خود را کنترل کنید. ویژگی‌هایی مانند ارتفاع، عرض، تراز (بالا، چپ، مرکز، و غیره)، خانواده‌های فونت و رنگ‌ها را برای دستیابی به یک نتیجه بصری مؤثر و ثابت که مشروعیت سند را تقویت می‌کند، سفارشی کنید.
      4. **برنامه واترمارک و ذخیره سازی ایمن**: واترمارک های خود را با استفاده از روش **Watermarker** ترکیب کنید. این کتابخانه به شما امکان می دهد در صورت لزوم برای محافظت بیشتر، چندین واترمارک اضافه کنید. توصیه می شود برای حفظ فایل اصلی و محافظت از اسناد واترمارک شده خود، سند اصلاح شده Webp را در مکانی جداگانه و امن ذخیره کنید.
   
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

        // ایجاد واترمارک تصویر برای WEBP

        // فایل منبع انتقال Watermarker را نمونه‌سازی کنید
        const watermarker = new groupdocs.watermark.Watermarker("input.webp");
        
        // ایجاد واترمارک با ارائه فایل تصویر
        const watermark = new groupdocs.watermark.ImageWatermark("watermark.png");

        // نتیجه WEBP را دریافت کنید
        watermarker.add(watermark);
        watermarker.save("output.webp");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ادغام علامت تصفیه شده"
  description: "GroupDocs.Watermark API ما برای .NET توسعه دهندگان راه حل های تصفیه شده را برای ادغام واترمارک ها به طور یکپارچه در هر سند ارائه می دهد. این ابزار برای ایجاد واترمارک های پیچیده و غیرقابل توجه طراحی شده است که حفاظت از کپی رایت را ضمن حفظ زیبایی شناسی سند تضمین می کند."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "ادغام واترمارک دقیق"
  features:
    # feature loop
    - title: "اثرات واترمارک گرادیان"
      content: "واترمارک های گرادیان را پیاده سازی کنید که به راحتی در اسناد شما ترکیب می شوند. این ویژگی امکان گرادینتهای خطی یا شعاعی را فراهم می کند و ظاهری مدرن به ویژگی های امنیتی اضافه می کند که هم حفاظت و هم تعامل بصری را بدون غلبه بر محتوا افزایش می دهد."

    # feature loop
    - title: "علامت های الگو برای امنیت اضافی"
      content: "از علامت گذاری مبتنی بر الگوی برای اضافه کردن یک لایه امنیتی اضافی استفاده کنید. API ما از الگوهای مختلفی پشتیبانی می کند که می توانند به طور پیچیده طراحی و در سراسر سند تکرار شوند و علامت واترمارک را در برابر دستکاری و حذف مقاوم تر می کند."

    # feature loop
    - title: "واترمارک مخصوص سند"
      content: "واترمارک ها را به طور منحصر به فرد برای انواع مختلف سند تنظیم کنید. خواه قراردادهای قانونی، برنامه های تجاری یا گزارش های علمی باشد، واترمارک ها را متناسب با هدف سند و دسترسی به خواننده سفارشی کنید و از یکپارچه سازی و امنیت مطلوب اطمینان حاصل کنید."
      
  code_samples:
    # code sample loop
    - title: "تولید PDF واترمارک تصویر"
      content: |
        تولید علامت های تصویر برای تمام تصاویر ارائه شده در یک سند PDF
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  بارگذاری سند به عنوان PDF
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  ایجاد واترمارک بر اساس حاشیه نویسی PDF
            const imageWatermark = new groupdocsWatermark.ImageWatermark("watermark.jpg");
            imageWatermark.setHorizontalAlignment(groupdocsWatermark.HorizontalAlignment.Center);
            imageWatermark.setVerticalAlignment(groupdocsWatermark.VerticalAlignment.Center);
            imageWatermark.setRotateAngle(-45);
            imageWatermark.setSizingType(groupdocsWatermark.SizingType.ScaleToParentDimensions);
            imageWatermark.setScaleFactor(1);
  
            //  تنظیمات علامت گذاری را تنظیم کنید
            const images = watermarker.getImages();
            for (let i = 0; i < images.getCount(); i++) {
                if (images.get_Item(i).getWidth() > 100 && images.get_Item(i).getHeight() > 100) {
                    images.get_Item(i).add(imageWatermark);
                }
            }

            //  افزودن علامت متن به سند نتیجه
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
    title: "WEBP فایل ها را با علامت های Node.js ایمن کنید"
    exclude: "WEBP"
    description: "Node.js را برای قرار دادن علامت های قابل تنظیم و قوی در WEBP تصاویر نصب کنید و اطمینان حاصل کنید که کپی رایت و دید نام تجاری محافظت می شود."
    items: 
        # format loop 1
        - name: "واترمارک PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/generate//pdf/"
          description: "ادوبی Portable فرمت سند"

        # format loop 2
        - name: "واترمارک Word"
          format: "WORD"
          link: "/watermark/nodejs-java/generate//word/"
          description: "MS Word و اسناد آفیس باز"
          
        # format loop 3
        - name: "واترمارک Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/generate//excel/"
          description: "MS Excel و صفحات گسترده آفیس باز"

        # format loop 4
        - name: "تصویر واترمارک"
          format: "IMAGE"
          link: "/watermark/nodejs-java/generate//image/"
          description: "فرمت های تصویر محبوب"

        # format loop 5
        - name: "عکس واترمارک"
          format: "PHOTO"
          link: "/watermark/nodejs-java/generate//photo/"
          description: "فرمت های عکس"

        # format loop 6
        - name: "واترمارک PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/generate//powerpoint/"
          description: "MS PowerPoint و ارائه های آفیس باز"

        # format loop 7
        - name: "واترمارک DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/generate//docx/"
          description: "مایکروسافت Word سند XML باز"
          
        # format loop 8
        - name: "واترمارک PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/generate//pptx/"
          description: "PowerPoint ارائه اکس‌ام‌ال باز"
          
        # format loop 9
        - name: "واترمارک XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/generate//xlsx/"
          description: "مایکروسافت Excel صفحه گسترده XML باز"

        # format loop 10
        - name: "واترمارک JPEG"
          format: "JPEG"
          link: "/watermark/nodejs-java/generate//jpeg/"
          description: "JPEG تصویر"

        # format loop 11
        - name: "واترمارک PNG"
          format: "PNG"
          link: "/watermark/nodejs-java/generate//png/"
          description: "Portable گرافیک شبکه"

        # format loop 12
        - name: "واترمارک TIFF"
          format: "TIFF"
          link: "/watermark/nodejs-java/generate//tiff/"
          description: "برچسب فرمت فایل تصویر"

        # format loop 13
        - name: "واترمارک WEBP"
          format: "WEBP"
          link: "/watermark/nodejs-java/generate//webp/"
          description: "تصویر WEB"

        # format loop 14
        - name: "واترمارک DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/generate//doc/"
          description: "سند مایکروسافت Word 97 - 2007"

        # format loop 15
        - name: "واترمارک XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/generate//xls/"
          description: "مایکروسافت Excel کتاب کار 97-2003"

        # format loop 16
        - name: "واترمارک PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/generate//ppt/"
          description: "PowerPoint ارائه ۹۷—۲۰۰۳"

        # format loop 17
        - name: "واترمارک RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/generate//rtf/"
          description: "فرمت متن غنی"

---