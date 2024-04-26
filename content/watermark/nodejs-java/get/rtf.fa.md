
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:39:08
draft: false
lang: fa
format: Rtf
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "استخراج واترمارک RTF اسناد کارآمد"
head_description: "با استفاده از GroupDocs.Watermark for Node.js via Java به طور موثر واترمارک ها را از اسناد استخراج کنید."

############################# Header ############################
title: "بازیابی علامت اسناد RTF ساده" 
description: "با استفاده از رویکرد ساده GroupDocs.Watermark for Node.js via Java واترمارک ها را بدون زحمت بازیابی کنید."
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
    title: "درباره GroupDocs.Watermark for Node.js via Java بیشتر بدانید"
    link: "/watermark/nodejs-java/"
    link_title: "بیشتر بدانید"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java قابلیت های استخراج واترمارک کارآمد را برای مدیریت واترمارک ها در Node.js via Java ارائه می دهد. روند بازیابی علامت را در فرمت های مختلف فایل ساده کنید.

############################# Steps ############################
steps:
    enable: true
    title: "دریافت واترمارک ها از Rtf فایل با استفاده از GroupDocs.Watermark"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** یک راه حل جامع برای قرار دادن واترمارک ها در قالب های محبوب سند تجاری ارائه می دهد. با ادغام کتابخانه ما در Node.js via Java برنامه های خود، می توانید آنها را به قابلیت های جستجوی واترمارک قدرتمند مجهز کنید.
      
      1. **Watermarker** را نمونه سازی کنید و مسیر فایل Rtf را ارائه دهید. همچنین می توانید از فایل ذخیره شده به عنوان جریان بایت استفاده کنید. این عمل اساساً سند هدف را برای تجزیه و تحلیل جامع واترمارک بارگذاری می کند.
      2. **SearchCriteria** را ایجاد کنید. شما می توانید یک تصویر را برای پیدا کردن علامت های تصویر مشابه مشخص کنید. متناوباً، برای واترمارک های متنی، محتوای متن، خواص فونت، ویژگی های رنگ و سایر پارامترهای مربوطه را برای اصلاح معیارهای جستجو و دستیابی به نتایج دقیق تر تعریف کنید.
      3. **Get** (یا یک کنوانسیون نامگذاری مشابه) شیء **Watermarker** را فراخوانی کنید تا فرآیند دریافت واترمارک در سند بارگذاری شده شروع شود. این تابع مجموعه ای از اشیاء را که نشان دهنده علامت های بالقوه هستند برمی گرداند و پردازش بیشتر را بر اساس نیازهای خاص شما تسهیل می کند.
      4. مجموعه نتیجه واترمارک ها به شما امکان می دهد واترمارک های شناسایی شده در سند را کنترل کنید. می توانید واترمارک های ناخواسته را حذف کنید یا خصوصیات آنها را به صورت پویا تغییر دهید، مانند تنظیم اندازه، موقعیت یا محتوای متن آنها، متناسب با نیازهای خود.
   
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

        // دریافت واترمارک های تصویر قرار داده شده در RTF

        // ایجاد شی Watermarker با مسیر منبع
        const watermarker = new groupdocs.watermark.Watermarker("input.rtf");
        
        // واترمارک ها را با هش تصویر مشابه دریافت کنید
        const imageSearchCriteria = 
            new groupdocs.watermark.ImageDctHashSearchCriteria("watermark.jpg");
        imageSearchCriteria.setMaxDifference(0.9);
        const possibleWatermarks = watermarker.search(imageSearchCriteria);

        // واترمارک ها را همانطور که می خواهید پردازش کنید
        console.log(`Found ${possibleWatermarks.getCount()} possible watermark(s).`);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "از Node.js برای جستجوی علامت با GroupDocs.Watermark استفاده کنید"
  description: "قابلیت های جستجوی واترمارک پویا و کارآمد را در برنامه های Node.js خود با استفاده از GroupDocs.Watermark در پلت فرم Node.js via Java پیاده سازی کنید."
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "جستجوی واترمارک Node.js"
  features:
    # feature loop
    - title: "API Node.js برای جستجوی واترمارک انعطاف پذیر"
      content: "از انعطاف پذیری Node.js با GroupDocs.Watermark استفاده کنید تا واترمارک ها را در چندین فرمت سند جستجو کنید. جستجو ها را به راحتی متناسب با نیازهای خاص مانند اندازه، نوع یا محتوا پیکربندی کنید."

    # feature loop
    - title: "شناسایی علامت گذاری پیشرفته با Node.js"
      content: "پردازش سند خود را با شناسایی دقیق واترمارک ها با استفاده از Node.js بهبود دهید. از API GroupDocs.Watermark برای شناسایی واترمارک ها حتی در ساختارهای پیچیده سند استفاده کنید."

    # feature loop
    - title: "راه حل های جستجوی علامت گذاری شده"
      content: "راه حل های امنیتی اسناد خود را با Node.js مقیاس دهید. GroupDocs.Watermark امکان پردازش کارآمد دسته های بزرگ سند را فراهم می کند و آن را برای برنامه های کاربردی در سطح سازمانی ایده آل می کند."
      
  code_samples:
    # code sample loop
    - title: "Node.js مثال: جستجو و بازیابی علامت های آب"
      content: |
        این مثال Node.js نحوه استفاده از GroupDocs.Watermark برای جستجو و بازیابی واترمارک ها را نشان می دهد و عملیات جستجوی کارآمد و مقیاس پذیر را نشان می دهد.
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            const files = ["source.docx", "source.xlsx", "source.pptx", "source.vsdx"];
            for (const file of files) {
                //  محیط Node.js را تنظیم کنید و اسناد لازم را بارگیری کنید
                const settings = new groupdocsWatermark.WatermarkerSettings();
                settings.setSearchableObjects(new groupdocsWatermark.SearchableObjects());
                settings.getSearchableObjects().setWordProcessingSearchableObjects(
                    groupdocsWatermark.WordProcessingSearchableObjects.Hyperlinks | 
                    groupdocsWatermark.WordProcessingSearchableObjects.Text
                );
                settings.getSearchableObjects().setSpreadsheetSearchableObjects(
                    groupdocsWatermark.SpreadsheetSearchableObjects.HeadersFooters
                );
                settings.getSearchableObjects().setPresentationSearchableObjects(
                    groupdocsWatermark.PresentationSearchableObjects.SlidesBackgrounds |
                    groupdocsWatermark.PresentationSearchableObjects.Shapes
                );
                settings.getSearchableObjects().setDiagramSearchableObjects(groupdocsWatermark.DiagramSearchableObjects.None);
                settings.getSearchableObjects().setPdfSearchableObjects(groupdocsWatermark.PdfSearchableObjects.All);

                //  جستجوی خود را برای شناسایی واترمارک ها بر اساس معیارهای مختلف پیکربندی کنید
                const watermarker = new groupdocsWatermark.Watermarker(file, settings);

                //  جستجوی علامت گذاری را اجرا کنید و داده ها را در مورد واترمارک های شناسایی شده جمع آوری کنید
                const watermarks = watermarker.search();

                //  نتایج را برای اصلاح یا حذف علامت های آب طبق نیاز کسب و کار پردازش کنید
                console.log(`In ${documentPath} found ${watermarks.getCount()} possible watermark(s).`);
                watermarker.close();
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
    title: "استخراج علامت های آب به طور موثر"
    exclude: "RTF"
    description: "با GroupDocs.Watermark for Node.js via Java به طور موثر واترمارک ها را از فرمت های مختلف فایل استخراج کنید."
    items: 
        # format loop 1
        - name: "واترمارک PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/get//pdf/"
          description: "ادوبی Portable فرمت سند"

        # format loop 2
        - name: "واترمارک Word"
          format: "WORD"
          link: "/watermark/nodejs-java/get//word/"
          description: "MS Word و اسناد آفیس باز"
          
        # format loop 3
        - name: "واترمارک Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/get//excel/"
          description: "MS Excel و صفحات گسترده آفیس باز"

        # format loop 4
        - name: "واترمارک PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/get//powerpoint/"
          description: "MS PowerPoint و ارائه های آفیس باز"

        # format loop 5
        - name: "واترمارک DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/get//docx/"
          description: "مایکروسافت Word سند XML باز"
          
        # format loop 6
        - name: "واترمارک PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/get//pptx/"
          description: "PowerPoint ارائه اکس‌ام‌ال باز"
          
        # format loop 7
        - name: "واترمارک XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/get//xlsx/"
          description: "مایکروسافت Excel صفحه گسترده XML باز"

        # format loop 8
        - name: "واترمارک DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/get//doc/"
          description: "سند مایکروسافت Word 97 - 2007"

        # format loop 9
        - name: "واترمارک XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/get//xls/"
          description: "مایکروسافت Excel کتاب کار 97-2003"

        # format loop 10
        - name: "واترمارک PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/get//ppt/"
          description: "PowerPoint ارائه ۹۷—۲۰۰۳"

        # format loop 11
        - name: "واترمارک RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/get//rtf/"
          description: "فرمت متن غنی"

---