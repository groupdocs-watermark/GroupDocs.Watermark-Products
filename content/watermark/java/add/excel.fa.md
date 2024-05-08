
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:17
draft: false
lang: fa
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "تولید واترمارک در Excel صفحه گسترده برای Java"
head_description: "به راحتی تولید واترمارک های متن و تصویر را در Excel با Java پیاده سازی کنید تا از صفحات گسترده داده Excel خود محافظت کنید"

############################# Header ############################
title: "خودکار کردن Excel علامت گذاری با Java کد" 
description: "با استفاده از Java، واترمارک های متن یا تصویر سفارشی را در صفحات گسترده Excel پیاده سازی کنید. این راهنما دستورالعمل های گام به گام برای افزایش امنیت اسناد و برندسازی را ارائه می دهد که متناسب با انواع نیازهای حرفه ای است."
subtitle: "GroupDocs.Watermark for Java آپی" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود رایگان Maven"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java کتابخانه"
    link: "/watermark/java/"
    link_title: "بیشتر بدانید"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java مدیریت جامع واترمارک را در صفحات گسترده Excel ارائه می دهد و توسعه دهندگان را قادر می سازد تا به راحتی واترمارک ها را تولید، تنظیم و پاک کنند. این برنامه از تمام فرمت های محبوب Excel فایل پشتیبانی می کند و امکان جاسازی هر دو علامت متن و تصویر را فراهم می کند که می توانند از نظر فونت، رنگ، اندازه و موقعیت سفارشی شوند. GroupDocs.Watermark همچنین شامل ویژگی هایی برای جستجوی واترمارک است که اطمینان حاصل می کند که واترمارک های شما دست نخورده و ضد دستکاری هستند. ایده آل برای برنامه های کاربردی که نیاز به بهبود امنیت سند در محیط Java دارند.

############################# Steps ############################
steps:
    enable: true
    title: "افزودن واترمارک به سند Excel از طریق Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** افزودن واترمارک از انواع مختلف به فرمت‌های فایل تجاری محبوب را برای توسعه‌دهندگان Java آسان می‌کند. کتابخانه ما را با چند مرحله آسان که در زیر ذکر شده است به اسناد درخواستی و واترمارک خود اضافه کنید.
      
      1. کلاس اصلی API ما **Watermarker** است. قبل از پردازش سند باید آن را نمونه برداری کنید. فراموش نکنید که فایل Excel را به عنوان یک مسیر یا یک شی جریان به سازنده ارسال کنید.
      2. مرحله بعدی ساخت یک شی **Watermark** از نوع دلخواه است. می‌توان آن را نه تنها در یک صفحه سند خاص، بلکه در بخش‌های سند بومی مانند پیوست‌ها یا سرصفحه‌ها قرار داد.
      3. ویژگی های واترمارک مانند ارتفاع و عرض، تراز صفحه (بالا، چپ، مرکزی و غیره)، خانواده فونت و رنگ و بسیاری موارد دیگر را تنظیم کنید.
      4. برای افزودن واترمارک جدید، روش **Watermarker** را فراخوانی کنید. شما می توانید به تعداد مورد نیاز واترمارک اضافه کنید. توصیه می شود سند پردازش شده را در مکان دیگری ذخیره کنید.
   
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

        // اضافه کردن واترمارک متنی به EXCEL

        // فایل را برای واترمارک شدن به Watermarker منتقل کنید
        Watermarker watermarker = new Watermarker("input.اکس‌اس‌لکس");
        
        // ایجاد واترمارک متنی و تنظیم خواص
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        watermark.setForegroundColor(Color.getRed());

        // ذخیره فایل واترمارک شده
        watermarker.add(watermark);
        watermarker.save("output.اکس‌اس‌لکس");
        
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
    title: "Java تکنیک برای Excel علامت گذاری"
    exclude: "EXCEL"
    description: "با استفاده از GroupDocs.Watermark for Java، به راحتی واترمارک های متنی یا تصویری را روی صفحات گسترده Excel اعمال کنید و امنیت اسناد و برندسازی را به عنوان بخشی از گردش کار کسب و کار خود به طور قابل توجهی افزایش می دهد."
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