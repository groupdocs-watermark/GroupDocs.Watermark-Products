---
############################# Static ############################
layout: "family"
date:  2024-05-08T17:25:28
draft: false

product: "Watermark"
product_tag: "watermark"

lang: fa

############################# Head ############################
head_title: "واترمارک سند C# Java Node.js | اضافه کردن واترمارک"
head_description: "واترمارک را به PDF، تصاویر و اسناد اضافه کنید. راه حل علامت گذاری برای Microsoft Office، PDF، OpenDocument، تصاویر و غیره"

############################# Header ############################
title: "راه حل علامت اسناد"
description:  |
  علامت های متن و تصویر را برای اسناد و تصاویر خود اضافه کنید.

  علامت های سند را به روشی راحت جستجو و اصلاح کنید.

  در مورد واترمارک هایی که در اسناد شما ارائه شده است اطلاعات کسب کنید.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "پلت فرم خود را انتخاب کنید"
  title: "استقلال پلت فرم"
  description: "کتابخانه GroupDocs.Watermark از سیستم عامل ها و چارچوبهای زیر پشتیبانی می کند:"
  details_link_title: "بیشتر بدانید"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Watermark .NET 
      color: "blue"
      tag: "net"
      link: "/watermark/net/"
      features_link: "https://docs.groupdocs.com/watermark/net/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    .NET Framework 4.5 or higher <br> .NET Core 3.0 or higher <br> .NET 5.0 or higher
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Watermark Java
      color: "red"
      tag: "java"
      link: "/watermark/java/"
      features_link: "https://docs.groupdocs.com/watermark/java/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    Java 8 or higher <br> Kotlin
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Watermark Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/watermark/nodejs-java/"
      features_link: "https://docs.groupdocs.com/watermark/"
      features:
          # features loop
          - rows: "4"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> هر ویرایشگر متن دیگر
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

############################# Features ###############################
features:
  enable: true
  title: "بررسی ویژگی های GroupDocs.Watermark"
  description: "این کتابخانه برای اضافه کردن، جستجو و به روز رسانی انواع واترمارک برای فرمت های محبوب سند طراحی شده است."

  items:
    # items loop
    - icon: "protect"
      title: "محافظت از فایل ها با واترمارک ها"
      content: "واترمارک های متن و تصویر را به اسناد کسب و کار خود اضافه کنید."

    # items loop
    - icon: "search"
      title: "علامت های موجود را جستجو کنید"
      content: "اطلاعات دقیق در مورد واترمارک هایی که قبلاً در سند قرار داده شده اند دریافت کنید."

    # items loop
    - icon: "manipulate"
      title: "دستکاری واترمارک های سند"
      content: "کنترل متن، سبک، تصویر و سایر ویژگی های واترمارک."

    # items loop
    - icon: "additional"
      title: "ویژگی های مختلف اضافی"
      content: "اطلاعات سند را دریافت کنید، لینک های هیپر-لینک یا پس زمینه صفحات و غیره را به روز کنید"

############################# Code Samples ###############################
code_samples:
  enable: true
  title: "محافظت از اسناد توسط واترمارک"
  description: "GroupDocs.Watermark نمونه کد عملیات معمولی."

  items:
    # items loop
    - title: "ایجاد یک واترمارک"
      content: "برای افزودن یک واترمارک به یک سند، مسیر فایل هدف را ارائه دهید. برای دریافت واترمارک سفارشی در یک صفحه خاص، گزینه های زیادی برای انتخاب دارید."
      samples:
          # samples loop
          - language: "C#"
            color: "blue"
            content: |
                    <code class="language-csharp" data-lang="csharp">
                        // سندی را که باید علامت گذاری شود مشخص کنید

                        using (Watermarker watermarker = new Watermarker("source.docx"))
                        {
                          // ایجاد شی واترمارک
                          TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                          // گزینه های واترمارک را تنظیم کنید
                          watermark.ForegroundColor = Color.Red;
                          watermark.HorizontalAlignment = HorizontalAlignment.Center;
                          watermark.VerticalAlignment = VerticalAlignment.Center;

                          // اضافه کردن واترمارک و ذخیره فایل پردازش شده
                          watermarker.Add(watermark);
                          watermarker.Save("result.docx");
                        }                    
                    </code>

          # samples loop
          - language: "Java"
            color: "red"
            content: |
                    <code class="language-java" data-lang="java">
                        // سندی را که باید علامت گذاری شود مشخص کنید

                        Watermarker watermarker = new Watermarker("source.docx");

                        // ایجاد شی واترمارک
                        TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // گزینه های واترمارک را تنظیم کنید
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // اضافه کردن واترمارک و ذخیره فایل پردازش شده
                        watermarker.add(watermark);
                        watermarker.save("result.docx");
                        watermarker.close();

                    </code>

          # samples loop
          - language: "TypeScript"
            color: "green"
            content: |
                    <code class="language-java" data-lang="javascript">
                        // سندی را که باید علامت گذاری شود مشخص کنید

                        const watermarker = new Watermarker("source.docx");
    
                        // ایجاد شی واترمارک
                        const watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // گزینه های واترمارک را تنظیم کنید
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // اضافه کردن واترمارک و ذخیره فایل پردازش شده
                        watermarker.add(watermark);
                        watermarker.save("result.docx");                        

                    </code>

############################# Supported Formats ###############################
formats:
  enable: true
  title: "50+ فرمت فایل پشتیبانی می شود"
  description: "GroupDocs.Watermark علامت گذاری برای فرمت های محبوب سند و فایل فراهم می کند."

############################# Metrics ###############################
metrics:
  enable: true
  title: "دادههای آماری کتابخانه ما"
  description: "عمیق به معیارهای کلیدی بپردازید و بینش را در مورد دستاوردها، تأثیر و رشد ما آشکار کنید."

  items:
    # items loop
    - number: "50+"
      title: "فرمت های پشتیبانی شده"
      content: "کتابخانه قادر به پردازش بیش از 50 فرمت فایل محبوب است."

    # items loop
    - number: "500k"
      title: "NuGet دانلود"
      content: "GroupDocs.Watermark برای .NET یک کتابخانه محبوب با بیش از 500,000 دانلود در NuGet است."

    # items loop
    - number: "15k"
      title: "دانلود های Maven"
      content: "با بیش از 15K دانلود در Maven، GroupDocs.Watermark یک انتخاب محبوب برای Java توسعه دهندگان است."

    # items loop
    - number: "140+"
      title: "مشتریان خوشحال"
      content: "توسعه دهندگان فردی و شرکت های برتر در سراسر جهان کتابخانه های ما را برای ساخت راه حل های نوآورانه ترجیح می دهند"


############################# Customers ###############################
customers:
  enable: true
  title: "مشتریان خوشحال ما"
  description: "GroupDocs کتابخانه توسط مارک های مشهور و برجسته جهانی در سراسر جهان استخدام می شوند."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "آماده شروع هستید؟"
  description: "GroupDocs.Watermark ویژگی را به صورت رایگان در پلتفرم خود امتحان کنید"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/watermark/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/watermark/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/watermark/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "سوالات متداول"
  description: "سوالات متداول ما را بررسی کنید"

  items:
    # items loop
    - question: "آیا کتابخانه های خارجی توسط GroupDocs.Watermark برای دستکاری اسناد مورد نیاز هستند؟"
      answer: "GroupDocs.Watermark به طور مستقل کار می کند، بدون نیاز به نرم افزارهای شخص ثالث مانند Adobe Acrobat، Microsoft Office و غیره."

    # items loop
    - question: "آیا می توانم ویژگی های GroupDocs.Watermark را قبل از خرید آزمایش کنم؟"
      answer: "بله، GroupDocs.Watermark یک دوره آزمایشی رایگان ارائه می دهد! آن را نصب کنید و آن را امتحان کنید، اما به خاطر داشته باشید: نسخه های آزمایشی «نشان های آزمایشی» را به اسناد شما اضافه می کنند، فقط 3 صفحه اول پردازش می شوند. آیا می خواهید تجربه کامل داشته باشید؟ مجوز موقت 30 روزه رایگان برای عملکرد کامل دریافت کنید. جزئیات را در زیر [مجوز موقت](https://purchase.groupdocs.com/temporary-license/) مشاهده کنید."

    # items loop
    - question: "چه نوع مجوز ارائه شده است؟"
      answer: "به مجوز GroupDocs.Watermark نیاز دارید؟ ما گزينه هاي داريم از بین مجوزها بر اساس بسیاری از گزینه ها انتخاب کنید. تعداد توسعه دهندگان در تیم شما مکان های استقرار مانند دفتر واحد یا محل کار از راه دور. آیا توزیع مشتری نهایی نیاز به اشتراک گذاری SDK/API با مشتریان دارد؟ متناوباً، مجوز برای استفاده ماهانه وجود دارد: فقط برای آنچه در برنامه های اندازه گیری شده استفاده می کنید پرداخت کنید. عمیق تر غواصی کنید و [قیمت](https://purchase.groupdocs.com/pricing/watermark/net/) کامل  را پیدا کنید."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Watermark API های کد پایین"
  description: "با استفاده از REST API مبتنی بر ابر ما، واترمارک ها را توسط برنامه خود به فایل ها اضافه کنید."
  
  items:
    # items loop
    - title: "GroupDocs.Watermark Cloud for cURL"
      content: "از API cURL REST ful برای علامت گذاری PDF، Word، Excel، PowerPoint، JPEG و سایر فرمت های فایل محبوب استفاده کنید."
      icon: "groupdocs_watermark-for-curl"
      link: "https://products.groupdocs.cloud/watermark/curl"

    # items loop
    - title: "GroupDocs.Watermark Cloud for .NET"
      content: ".NET برنامه های خود را با ویژگی های واترمارک اسناد توسط Cloud SDK برای .NET تقویت کنید. اسناد کسب و کار را به تنهایی محافظت کنید."
      icon: "groupdocs_watermark-for-net"
      link: "https://products.groupdocs.cloud/watermark/net"

    # items loop
    - title: "GroupDocs.Watermark Cloud for Java"
      content: "GroupDocs.Watermark SDK طراحی شده برای Java امکانات جدیدی را برای Java برنامه ها و فایل های تجاری شما فراهم می کند."
      icon: "groupdocs_watermark-for-java"
      link: "https://products.groupdocs.cloud/watermark/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Watermark برنامه های وب"
  description: "GroupDocs دسترسی به برنامه وب را برای افزودن واترمارک به اسناد شما فراهم می کند. بیش از 50 فرمت فایل محبوب را می توان به صورت رایگان در مرورگر مورد علاقه خود علامت گذاری کرد."

  items:
    # items loop
    - title: "GroupDocs.Watermark Total"
      content: "ابزار آنلاین برای اضافه کردن واترمارک به اسناد از هر دستگاهی."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/watermark/total"

    # items loop
    - title: "GroupDocs.Watermark DOCX"
      content: "واترمارک MS Word DOCX آنلاین."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/watermark/docx"

    # items loop
    - title: "GroupDocs.Watermark PDF"
      content: "از PDF اسناد آنلاین محافظت کنید."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/watermark/pdf"


      


---