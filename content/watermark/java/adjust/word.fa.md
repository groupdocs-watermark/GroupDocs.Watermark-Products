
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:57
draft: false
lang: fa
format: Word
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Word علامت های آب را بدون زحمت تنظیم کنید - GroupDocs.Watermark"
head_description: "با استفاده از GroupDocs.Watermark، واترمارک ها را در چندین فرمت سند به طور یکپارچه تنظیم کنید. امنیت اسناد خود را افزایش دهید"

############################# Header ############################
title: "تنظیم Word واترمارک: بدون زحمت ایمن" 
description: "با قابلیت های قدرتمند اصلاح علامت ما، اسناد خود را بدون زحمت ایمن کنید از محتوای خود با اعتماد به نفس محافظت کنید."
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
       **اصلاح علامت ها**: GroupDocs.Watermark کاربران را قادر می سازد تا واترمارک ها را در قالب های مختلف سند به طور یکپارچه تغییر دهند. با کنترل دقیق و گزینه های همه کاره، اسناد خود را با اطمینان سفارشی کنید.

############################# Steps ############################
steps:
    enable: true
    title: "واترمارک ها را در Word اسناد با Java تنظیم کنید"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** با اجرای چند مرحله آسان، تنظیم واترمارک های متن در برنامه های کاربردی خود را برای توسعه دهندگان Java آسان می کند:
      
      1. **Watermarker** بارگذاری کنید. شما می توانید فایل را برای پردازش بیشتر به عنوان جریان یا به عنوان یک مسیر در یک دیسک محلی ارائه دهید.
      2. **معیارهای جستجو** به شناسایی علامت های آب با خواص مناسب که قبلاً به یک سند اضافه شده بودند کمک می کند.
      3. **جستجو** دریافت کنید. ویژگی های واترمارک های یافت شده مانند اندازه، تراز صفحه، متن، رنگ، محتوای تصویر و غیره را تنظیم کنید راه های زیادی برای سفارشی کردن داده های شما وجود دارد.
      4. پس از اتمام فرآیند تنظیم واترمارک، شما باید سند به روز شده را ذخیره کنید. برای ذخیره نتیجه از مسیر فایل محلی، فایل یا جریان بایت استفاده کنید.
   
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

        // WORD علامت متن را تنظیم کنید

        // نشانگر واترمارک نمونه ای با سند ورودی WORD
        Watermarker watermarker = new Watermarker("input.داکس");

        // TextSearchCriteria را اولیه کنید و علامت های متن را پیدا کنید
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        
        // ویژگی های واترمارک متن را تنظیم کنید
        for (PossibleWatermark watermark : watermarks)
        {
            watermark.getFormattedTextFragments().clear();
            watermark.getFormattedTextFragments().
                add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
        }

        // سند به روز شده را ذخیره کنید
        watermarker.save("output.داکس");
        
        ```            
        
############################# More features ############################
more_features:
  enable: true
  title: "بررسی عمیق در WORD تنظیم واترمارک"
  description: "API ما Java برنامه را قادر می سازد تا در قالب های محبوب سند اضافه، ویرایش، حذف و جستجو برای واترمارک ها را فراهم کند."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "تنظیم واترمارک"
  features:
    # feature loop
    - title: "به راحتی اسناد خود را علامت گذاری کنید"
      content: "GroupDocs.Watermark علامت گذاری آب را برای Java توسعه دهندگان ساده می کند. واترمارک های متنوع را به اسناد و فایل های مختلف کسب و کار اضافه کنید. نه تنها می توانید واترمارک ها را اعمال کنید، بلکه می توانید علامت های موجود را نیز به روز کنید یا حذف کنید."

    # feature loop
    - title: "واترمارک ها را متناسب با نیازهای خود سفارشی کنید"
      content: "API ما گزینه های سفارشی سازی گسترده ای را ارائه می دهد. اندازه، چرخش، رنگ، فونت، سبک ها و موارد دیگر را به راحتی تنظیم کنید تا به علامت کامل دست یابید."

    # feature loop
    - title: "از ویژگی های سند بومی WORD استفاده کنید"
      content: "بسته به فرمت سند خاص، می توانید از قابلیت های بومی استفاده کنید. اینها ممکن است شامل پس زمینه صفحه سند، حاشیه نویسی ها، هدرها یا سایر اشیاء به عنوان ظروف واترمارک باشد."
      
  code_samples:
    # code sample loop
    - title: "PDF تنظیم علامت متن"
      content: |
        این مثال نحوه تنظیم متن مصنوعات خاص را نشان می دهد.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  بارگذاری PDF سند
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  دریافت محتوای سند
        PdfContent pdfContent = watermarker.getContent(PdfContent.class);

        //  متن واترمارک خاص را تنظیم کنید
        for (PdfArtifact artifact : pdfContent.getPages().get_Item(0).getArtifacts())
        {
            if (artifact.getText().contains("Test"))
            {
                artifact.setText("Passed");
            }
        }

        //  سند را ذخیره کنید
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
    title: "تنظیم واترمارک ها با استفاده از GroupDocs.Watermark for Java برای فرمت های محبوب"
    exclude: "WORD"
    description: "GroupDocs.Watermark از اصلاح یکپارچه واترمارک ها در قالب های مختلف پشتیبانی می کند. استراتژی علامت گذاری خود را متناسب با نیازهای خاص خود تنظیم کنید."
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