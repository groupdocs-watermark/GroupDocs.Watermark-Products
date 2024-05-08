
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:21
draft: false
lang: fa
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "تنظیم واترمارک ها در DOCX اسناد - GroupDocs.Watermark"
head_description: "با استفاده از GroupDocs.Watermark، واترمارک ها را به طور موثر در قالب های مختلف سند ویرایش کنید. اصالت سند را افزایش دهید."

############################# Header ############################
title: "تنظیم DOCX علامت های آب: سفارشی سازی بدون درز" 
description: "اسناد خود را به صورت یکپارچه با ابزار ویرایش واترمارک کارآمد ما سفارشی کنید. تصویر برند خود را بدون زحمت ارتقا دهید."
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
    title: "GroupDocs.Watermark for Java آپی"
    link: "/watermark/java/"
    link_title: "بیشتر بدانید"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **ویرایش علامت ها**: اسناد خود را با ابزارهای ویرایش قدرتمند ما به صورت یکپارچه سفارشی کنید. خواه تنظیم مکان یا تغییر محتوا باشد، بدون زحمت به جلوه های واترمارک دلخواه خود دست یابید.

############################# Steps ############################
steps:
    enable: true
    title: "تنظیم واترمارک سند Docx با استفاده از Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** به توسعه دهندگان Java اجازه می دهد تا به راحتی واترمارک را در بسیاری از اسناد با استفاده از برنامه های خود تنظیم کنند. در اینجا یک راهنمای سریع وجود دارد:
      
      1. ابتدا باید فایل Docx را به عنوان پارامتر سازنده کلاس **Watermarker** ارسال کنید. جریان بایت یا فایل یا یک مسیر دیسک محلی را ارائه دهید.
      2. در مرحله دوم، واترمارک هایی که باید تنظیم شوند را پیدا کنید. از **SearchCriteria** برای شناسایی واترمارک ها با ویژگی های خاصی که قبلاً به سند اضافه شده است استفاده کنید.
      3. پس از جستجو، لیستی از واترمارک های مربوطه را دریافت خواهید کرد. سپس می‌توانید ویژگی‌های آن‌ها، از جمله اندازه، تراز صفحه، متن، رنگ، محتوای تصویر و موارد دیگر را تنظیم کنید. این درجه بالایی از سفارشی سازی داده های شما را ارائه می دهد.
      4. پس از اتمام تنظیم واترمارک ها، سند به روز شده را ذخیره کنید. می توانید از یک مسیر فایل محلی یا استریم برای ذخیره نتیجه استفاده کنید.
   
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
        // واترمارک تصویر DOCX را تنظیم کنید

        // نمونه سازی Watermarker با DOCX
        Watermarker watermarker = new Watermarker("input.docx");
        
        // برای مطابقت با یک تصویر خاص، SearchCriteria را مقداردهی اولیه کنید
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);

        for (PossibleWatermark watermark : watermarks)
        {
            // تصویر پیدا شده را جایگزین کنید
            watermark.setImageData(imageData);
        }

        // فایل تنظیم شده را ذخیره کنید
        watermarker.save("output.docx");
        
        ```
        
############################# More features ############################
more_features:
  enable: true
  title: "مدیریت پیشرفته DOCX علامت واترمارک برای Java برنامه"
  description: "API GroupDocs.Watermark به توسعه دهندگان این امکان را می دهد تا قابلیت واترمارک را به طور یکپارچه در Java برنامه های خود ادغام کنند. از افزودن، ویرایش، حذف و جستجوی واترمارک ها در طیف گسترده ای از فرمت های سند پشتیبانی می کند."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "تنظیم واترمارک"
  features:
    # feature loop
    - title: "ادغام علامت بدون دردسر"
      content: "GroupDocs.Watermark روند افزودن واترمارک های متنوع به اسناد و فایل های مختلف کسب و کار در Java برنامه ها را ساده می کند. توسعه دهندگان نه تنها می توانند واترمارک ها را اعمال کنند، بلکه موارد موجود را به صورت برنامه نویسی به روز یا حذف کنند."

    # feature loop
    - title: "سفارشی سازی علامت گرانول"
      content: "API گزینه های سفارشی سازی گسترده ای را برای واترمارک ها فراهم می کند. توسعه دهندگان می توانند به راحتی اندازه، چرخش، رنگ، فونت، سبک ها و سایر خواص را برای دستیابی به جلوه بصری مورد نظر تنظیم کنند."

    # feature loop
    - title: "استفاده از DOCX ویژگی های اسناد بومی"
      content: "بسته به قالب سند هدف، توسعه دهندگان می توانند از قابلیت های بومی برای قرار دادن واترمارک استفاده کنند. این قابلیت ها ممکن است شامل پس زمینه صفحه سند، حاشیه نویسی ها، هدرها یا سایر اشیاء به عنوان ظروف واترمارک باشد."
      
  code_samples:
    # code sample loop
    - title: "تنظیم علامت تصویر در صفحات گسترده"
      content: |
        این مثال ها نحوه تنظیم تصویر اشکال خاص در یک برگه Excel را نشان می دهد.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  بارگذاری سند به عنوان صفحه گسترده
        SpreadsheetLoadOptions loadOptions = new SpreadsheetLoadOptions();
        Watermarker watermarker = new Watermarker("source.xlsx", loadOptions);

        //  بایت های واترمارک جدید را دریافت کنید
        File file = new File("new_watermark.png");
        byte[] imageBytes = new byte[(int) file.length()];
        FileInputStream inputStream = new FileInputStream(file);
        inputStream.read(imageBytes);
        inputStream.close();

        //  محتوای واترمارک خاص را تنظیم کنید
        for (SpreadsheetShape shape : content.getWorksheets().get_Item(0).getShapes())
        {
            if (shape.getImage() != null)
            {
                shape.setImage(new SpreadsheetWatermarkableImage(imageBytes));
            }
        }

        //  ذخیره سند نتیجه
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
    title: "واترمارک ها را در بسیاری از فرمت ها با استفاده از GroupDocs.Watermark for Java اصلاح کنید"
    exclude: "DOCX"
    description: "به طور یکپارچه واترمارک ها را در چندین قالب سند ویرایش کنید ضمن اطمینان از حفاظت و اصالت، اسناد خود را بدون زحمت سفارشی کنید."
    items: 
        # format loop 1
        - name: "واترمارک PDF"
          format: "PDF"
          link: "/watermark/java/adjust//pdf/"
          description: "ادوبی Portable فرمت سند"

        # format loop 2
        - name: "واترمارک Word"
          format: "WORD"
          link: "/watermark/java/adjust//word/"
          description: "MS Word و اسناد آفیس باز"
          
        # format loop 3
        - name: "واترمارک Excel"
          format: "EXCEL"
          link: "/watermark/java/adjust//excel/"
          description: "MS Excel و صفحات گسترده آفیس باز"

        # format loop 4
        - name: "واترمارک PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/adjust//powerpoint/"
          description: "MS PowerPoint و ارائه های آفیس باز"

        # format loop 5
        - name: "واترمارک DOCX"
          format: "DOCX"
          link: "/watermark/java/adjust//docx/"
          description: "مایکروسافت Word سند XML باز"
          
        # format loop 6
        - name: "واترمارک PPTX"
          format: "PPTX"
          link: "/watermark/java/adjust//pptx/"
          description: "PowerPoint ارائه اکس‌ام‌ال باز"
          
        # format loop 7
        - name: "واترمارک XLSX"
          format: "XLSX"
          link: "/watermark/java/adjust//xlsx/"
          description: "مایکروسافت Excel صفحه گسترده XML باز"

        # format loop 8
        - name: "واترمارک DOC"
          format: "DOC"
          link: "/watermark/java/adjust//doc/"
          description: "سند مایکروسافت Word 97 - 2007"

        # format loop 9
        - name: "واترمارک XLS"
          format: "XLS"
          link: "/watermark/java/adjust//xls/"
          description: "مایکروسافت Excel کتاب کار 97-2003"

        # format loop 10
        - name: "واترمارک PPT"
          format: "PPT"
          link: "/watermark/java/adjust//ppt/"
          description: "PowerPoint ارائه ۹۷—۲۰۰۳"

        # format loop 11
        - name: "واترمارک RTF"
          format: "RTF"
          link: "/watermark/java/adjust//rtf/"
          description: "فرمت متن غنی"

---