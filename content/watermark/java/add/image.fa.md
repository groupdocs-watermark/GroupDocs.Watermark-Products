
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:56
draft: false
lang: fa
format: Image
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "تولید علامت های موثر برای تصاویر با Java"
head_description: "از Java برای ایجاد علامت های پیشرفته برای تصاویر استفاده کنید. از اسناد خود محافظت کنید و کپی رایت را به طور موثر اعلام"

############################# Header ############################
title: "تصاویر علامت گذاری یکپارچه در Java" 
description: "علامت های پویا را در فایل های تصویری خود با استفاده از Java پیاده سازی کنید. این ابزار امکان تنظیم دقیق موقعیت یابی، مقیاس پذیری و شفافیت را برای افزایش امنیت و شناخت برند فراهم می کند."
subtitle: "GroupDocs.Watermark for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود در Maven به صورت رایگان"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java"
    link: "/watermark/java/"
    link_title: "بیشتر بدانید"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java GroupDocs.Watermark for Java توسعه دهندگان را قادر می سازد تا به طور موثر واترمارک ها را بر روی فایل های تصویری تولید و مدیریت کنند. با پشتیبانی از طیف گسترده ای از فرمت های تصویر، کاربران می توانند هر دو علامت های متنی و گرافیکی را که از نظر موقعیت، مقیاس و شفافیت کاملاً قابل تنظیم هستند پیاده سازی کنند. این قابلیت برای برنامه های کاربردی در رسانه های دیجیتال، تبلیغات و توزیع محتوای آنلاین بسیار مهم است، جایی که برندسازی و یکپارچگی کپی رایت از اهمیت بالایی برخوردار است. علاوه بر این، GroupDocs.Watermark شامل ویژگی هایی برای جستجو و حذف علامت های موجود است و ابزاری همه کاره برای مدیریت و امنیت تصویر فراهم می کند.

############################# Steps ############################
steps:
    enable: true
    title: "افزودن واترمارک به Image سند از طریق Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** افزودن واترمارک های مختلف به فرمت های محبوب فایل تجاری را برای توسعه دهندگان Java آسان می کند. کتابخانه ما را در چند مرحله آسان به برنامه و اسناد واترمارک خود اضافه کنید، همانطور که در زیر ذکر شده است.
      
      1. **Watermarker** است. شما باید قبل از پردازش سند آن را نمونه سازی کنید. فراموش نکنید که فایل Image را به عنوان یک مسیر یا یک شیء جریان به سازنده منتقل کنید.
      2. **Watermark** از نوع دلخواه است. این را می توان نه تنها در یک صفحه سند خاص بلکه در قسمت های اسناد بومی مانند پیوست ها یا هدر قرار داد.
      3. ویژگی های واترمارک مانند ارتفاع و عرض، تراز صفحه (بالا، چپ، مرکزی و غیره)، خانواده فونت و رنگ و بسیاری دیگر را تنظیم کنید.
      4. **Watermarker** را فراخوانی کنید. شما می توانید هر تعداد واترمارک را که نیاز دارید اضافه کنید. توصیه می شود سند پردازش شده را در مکان دیگری ذخیره کنید.
   
    code:
      platform: "net"
      copy_title: "کپی کردن"
      install:
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-watermark</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "برای کپی کلیک کنید"
        copy_done: "کپی شده"
      links:
        #  loop
        - title: "نمونه های بیشتر"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
        #  loop
        - title: "مستندات"
          link: "https://docs.groupdocs.com/watermark/java/"
          
      content: |
        ```java {style=abap}

        // افزودن واترمارک متن به IMAGE

        // پرونده را برای علامت گذاری به Watermarker منتقل کنید
        Watermarker watermarker = new Watermarker("input.جی پی جی پی");
        
        // ایجاد علامت متن و تنظیم خواص
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        watermark.setForegroundColor(Color.getRed());

        // ذخیره فایل علامت گذاری شده
        watermarker.add(watermark);
        watermarker.save("output.جی پی جی پی");
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "واترمارک های خود را به راحتی تقویت کنید"
  description: "از قدرت GroupDocs.Watermark برای تولید، ترکیب و اضافه کردن واترمارک در چندین قالب سند استفاده کنید. این API نه تنها امنیت اسناد را افزایش می دهد بلکه از مالکیت معنوی شما نیز با جاسازی واترمارک های قابل تنظیم که هم همه کاره و هم قوی هستند محافظت می کند."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "افزودن واترمارک"
  features:
    # feature loop
    - title: "گزینه های واترمارک همه کاره."
      content: "طیف گسترده ای از گزینه های علامت گذاری را با GroupDocs.Watermark کشف کنید. از تنظیم کدورت و چرخش گرفته تا اندازه مقیاس بندی متناسب، API ما به شما امکان می دهد واترمارک ها را دقیقاً با نیازهای خود سفارشی کنید و اطمینان حاصل کنید که آنها به طور یکپارچه با اسناد شما ترکیب می شوند و در عین حال یکپارچگی محتوا را حفظ می کنند."

    # feature loop
    - title: "سبک واترمارک پیشرفته."
      content: "GroupDocs.Watermark به شما امکان می دهد تا واترمارک های خود را با فونت ها، رنگ ها و سایه های مختلف سبک کنید و آنها را متمایز کرده و حذف آنها سخت تر می شود. جذابیت زیبایی شناختی اسناد و تصاویر محافظت شده خود را با علامت های شیک که نشان دهنده هویت و حرفه ای بودن نام تجاری شما است، افزایش دهید."

    # feature loop
    - title: "کاشی کاری و موقعیت یابی واترمارک"
      content: "با GroupDocs.Watermark، جلوه های کاشی کاری را برای پوشش کل سند خود پیاده سازی کنید و حفاظت کامل را تضمین کنید. واترمارک ها را دقیقاً در جایی که به آنها نیاز دارید - در مرکز، گوشه یا مکان های سفارشی قرار دهید. گزینه های موقعیت یابی انعطاف پذیر ما به محافظت از اسناد شما در برابر استفاده غیر مجاز و تکرار کمک می کند."
      
  code_samples:
    # code sample loop
    - title: "PDF علامت حاشیه نویسی"
      content: |
        این مثال نحوه افزودن حاشیه نویسی واترمارک به یک سند PDF را نشان می دهد
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  بارگذاری سند به عنوان PDF
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  ایجاد واترمارک بر اساس حاشیه نویسی PDF
        PdfAnnotationWatermarkOptions options = new PdfAnnotationWatermarkOptions();
        TextWatermark textWatermark = new TextWatermark("Annotation watermark", new Font("Arial", 8));

        //  تنظیمات علامت گذاری را تنظیم کنید
        textWatermark.setHorizontalAlignment(HorizontalAlignment.Left);
        textWatermark.setVerticalAlignment(VerticalAlignment.Top);

        //  افزودن علامت متن به سند نتیجه
        watermarker.add(textWatermark, options);
        watermarker.save("result.pdf");

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "آماده شروع هستید؟"
  description: "ویژگی های GroupDocs.Watermark را به صورت رایگان امتحان کنید یا مجوز درخواست کنید"
  items:
    #  loop
    - title: "Maven دانلود"
      link: "https://releases.groupdocs.com/watermark/java/"
      color: "red"
        #  loop
    - title: "صدور مجوز"
      link: "https://purchase.groupdocs.com/pricing/watermark/java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "تصاویر امنیتی را با علامت گذاری واترمارک در Java ساده کنید"
    exclude: "IMAGE"
    description: "کیت ابزار Java ما امکان تولید واترمارک های شخصی برای هر قالب تصویری را فراهم می کند و امنیت و برندسازی را افزایش می دهد. واترمارک های متناسب اطمینان حاصل می کنند که تصاویر شما در رسانه های مختلف شناخته شده و محافظت می شود."
    items: 
        # format loop 1
        - name: "واترمارک PDF"
          format: "PDF"
          link: "/watermark/java/add//pdf/"
          description: "ادوبی Portable فرمت سند"

        # format loop 2
        - name: "واترمارک Word"
          format: "WORD"
          link: "/watermark/java/add//word/"
          description: "MS Word و اسناد آفیس باز"
          
        # format loop 3
        - name: "واترمارک Excel"
          format: "EXCEL"
          link: "/watermark/java/add//excel/"
          description: "MS Excel و صفحات گسترده آفیس باز"

        # format loop 4
        - name: "تصویر واترمارک"
          format: "IMAGE"
          link: "/watermark/java/add//image/"
          description: "فرمت های تصویر محبوب"

        # format loop 5
        - name: "عکس واترمارک"
          format: "PHOTO"
          link: "/watermark/java/add//photo/"
          description: "فرمت های عکس"

        # format loop 6
        - name: "واترمارک PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/add//powerpoint/"
          description: "MS PowerPoint و ارائه های آفیس باز"

        # format loop 7
        - name: "واترمارک DOCX"
          format: "DOCX"
          link: "/watermark/java/add//docx/"
          description: "مایکروسافت Word سند XML باز"
          
        # format loop 8
        - name: "واترمارک PPTX"
          format: "PPTX"
          link: "/watermark/java/add//pptx/"
          description: "PowerPoint ارائه اکس‌ام‌ال باز"
          
        # format loop 9
        - name: "واترمارک XLSX"
          format: "XLSX"
          link: "/watermark/java/add//xlsx/"
          description: "مایکروسافت Excel صفحه گسترده XML باز"

        # format loop 10
        - name: "واترمارک JPEG"
          format: "JPEG"
          link: "/watermark/java/add//jpeg/"
          description: "JPEG تصویر"

        # format loop 11
        - name: "واترمارک PNG"
          format: "PNG"
          link: "/watermark/java/add//png/"
          description: "Portable گرافیک شبکه"

        # format loop 12
        - name: "واترمارک TIFF"
          format: "TIFF"
          link: "/watermark/java/add//tiff/"
          description: "برچسب فرمت فایل تصویر"

        # format loop 13
        - name: "واترمارک WEBP"
          format: "WEBP"
          link: "/watermark/java/add//webp/"
          description: "تصویر WEB"

        # format loop 14
        - name: "واترمارک DOC"
          format: "DOC"
          link: "/watermark/java/add//doc/"
          description: "سند مایکروسافت Word 97 - 2007"

        # format loop 15
        - name: "واترمارک XLS"
          format: "XLS"
          link: "/watermark/java/add//xls/"
          description: "مایکروسافت Excel کتاب کار 97-2003"

        # format loop 16
        - name: "واترمارک PPT"
          format: "PPT"
          link: "/watermark/java/add//ppt/"
          description: "PowerPoint ارائه ۹۷—۲۰۰۳"

        # format loop 17
        - name: "واترمارک RTF"
          format: "RTF"
          link: "/watermark/java/add//rtf/"
          description: "فرمت متن غنی"

---