---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:29
draft: false

lang: fa
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Java کتابخانه واترمارک | اضافه کردن واترمارک به اسناد"
head_description: "نرم افزار بومی Java برای اضافه کردن و دستکاری واترمارک های متن و تصویر در فایل های PDF، Word، Excel، Presentations، Visio نمودار، ایمیل و تصاویر."

############################# Header ############################
title: "واترمارک اسناد را در Java پروژه به راحتی پیاده سازی کنید"
description: "برنامه های Java خود را با قابلیت علامت گذاری فایل ها با استفاده از کتابخانه GroupDocs.Watermark ارتقا دهید. API ما علامت های قابل تنظیم را برای طیف گسترده ای از فرمت های فایل محبوب ارائه می دهد."
words:
  for: "برای"

actions:
  main: "دانلود رایگان از Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "صدور مجوز"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java/"
  title: "آماده شروع هستید؟"
  description: "ویژگی های GroupDocs.Watermark را به صورت رایگان امتحان کنید یا مجوز درخواست کنید"

release:
  title: "نسخه {0} منتشر شد"
  notes: "چیزهای جدید را ببینید"
  downloads: "دانلودها"

code:
  title: "واترمارک PDF s از طریق Java"
  more: "نمونه های بیشتر"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-watermark</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // واترمارکر نمونه ای که از مسیر PDF عبور می کند
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // گزینه های واترمارک را سفارشی کنید
    TextWatermark textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // واترمارک را به PDF سند اعمال کنید
    watermarker.add(textWatermark);

    // ذخیره سند نتیجه
    watermarker.save("result.pdf");
    watermarker.close();
      
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark در یک نگاه"
  description: "کتابخانه طراحی شده برای افزودن واترمارک با استفاده از Java فن آوری"
  features:
    # feature loop
    - title: "فایل های واترمارک از طریق Java"
      content: "از اسناد کسب و کار خود با استفاده از GroupDocs.Watermark for Java محافظت کنید. متن، تصاویر، نمودارها یا پیوست های ایمیل را به عنوان واترمارک به فرمت های مختلف فایل اضافه کنید."

    # feature loop
    - title: "سفارشی کردن واترمارک ها برای نیازهای خاص"
      content: "GroupDocs.Watermark for Java گزینه های سفارشی سازی گسترده ای را برای واترمارک ها ارائه می دهد. سبک های متن (پررنگ، ایتالیایی، فونت) و خواص تصویر (چرخش و غیره) را تنظیم کنید تا روند علامت گذاری را با اهداف خاص خود تنظیم کنید."

    # feature loop
    - title: "پشتیبانی از فرمت گسترده"
      content: "GroupDocs.Watermark for Java یکپارچه با طیف گسترده ای از فرمت های فایل ادغام می شود، از جمله: PDF، Microsoft Office (Word، Excel، PowerPoint)، تصاویر (JPEG، PNG، GIF، BMP)، Visio نمودارها و ایمیل ها. امنیت اسناد را در انواع مختلف فایل افزایش دهید."

    # feature loop
    - title: "جستجوی و مدیریت واترمارک بدون دردسر"
      content: "واترمارک های موجود را در اسناد به طور موثر مدیریت کنید. واترمارک های خاص را پیدا کنید، متن، سبک یا تصاویر آنها را تغییر دهید یا آنها را به طور کامل حذف کنید. GroupDocs.Watermark for Java گردش کار واترمارک را ساده می کند."

############################# Platforms ############################
platforms:
  enable: true
  title: "استقلال پلت فرم"
  description: "GroupDocs.Watermark for Java از سیستم عامل های مختلف و مدیران بسته پشتیبانی می کند."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "فرمت های فایل پشتیبانی شده"
  description: |
    GroupDocs.Watermark for Java پردازش طیف گسترده ای از فرمت های فایل را امکان پذیر می کند. [فهرست کامل را ببینید](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### فرمت های Microsoft Office و OpenDocument
        * **قابل حمل:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### تصاویر و گرافیک
        * **فرمت های تصویر محبوب:** BMP, JPG, JPEG, PNG
        * **تصاویر چند صفحه ای:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### دیگر
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark for Java: امکانات"
  description: "با افزودن واترمارک ها از فایل های خود محافظت کنید. پشتیبانی از فرمت های مختلف از جمله PDF، اسناد آفیس و تصاویر."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "علامت گذاری فایل ها"
      content: "واترمارک ها را از بخش های خاص یا کل اسناد برای فرمت های مختلف فایل پشتیبانی شده اضافه یا حذف کنید."

    # feature loop
    - icon: "watermark_style"
      title: "سفارشی سازی واترمارک"
      content: "ظاهر علامت خود را با گزینه هایی مانند رنگ، فونت، چرخش و موارد دیگر سفارشی کنید."

    # feature loop
    - icon: "hidden_print"
      title: "علامت چاپ پنهان برای PDF"
      content: "یک واترمارک اضافه کنید که فقط هنگام چاپ یک سند PDF ظاهر می شود."

    # feature loop
    - icon: "image_only"
      title: "علامت گذاری تصاویر انتخابی"
      content: "تمام تصاویر در یک بخش خاص، صفحه، اسلاید یا کل سند را علامت بزنید."

    # feature loop
    - icon: "image_frame"
      title: "قابهای تصویر خاص واترمارک"
      content: "واترمارک ها را به فریم های خاص در یک تصویر چند فریم اعمال کنید."

    # feature loop
    - icon: "attachments"
      title: "پیوست ها و اشکال واترمارک"
      content: "واترمارک ها را به تمام پیوست ها در Excel سند یا تمام اشکال تصویر در Presentations اضافه کنید."

    # feature loop
    - icon: "pdf_objects"
      title: "تراز علامت واترمارک در PDF"
      content: "واترمارک ها را با مناطق مختلف یک سند PDF، از جمله Bleed Box، Art Box، Crop Box و Trim Box هماهنگ کنید."

    # feature loop
    - icon: "doc_background"
      title: "واترمارک توسط تصاویر پس زمینه"
      content: "افزودن یا حذف علامت تصویر پس زمینه به صفحات گسترده یا ارائه ها."

    # feature loop
    - icon: "unreadable_characters"
      title: "حفاظت با کاراکترهای غیرقابل خواندن"
      content: "محافظت از ارائه ها با استفاده از واترمارک متن با کاراکترهای غیرقابل خواندن."

    # feature loop
    - icon: "watermark_text_search"
      title: "جستجو برای واترمارک"
      content: "لیستی از علامت های ارائه شده در فایل را با استفاده از پارامترهای مختلف از جمله عبارات منظم دریافت کنید."

    # feature loop
    - icon: "watermark_image_search"
      title: "واترمارک های تصویر مشابه را پیدا کنید"
      content: "علامت های تصویر را پیدا کنید که شبیه یک تصویر خاص به نظر می رسد."

    # feature loop
    - icon: "document_info"
      title: "استخراج اطلاعات سند"
      content: "داده های مختلف سند مانند تنظیم صفحه برای فرمت های فایل پشتیبانی شده دریافت کنید."

############################# Code samples ############################
code_samples:
  enable: true
  title: "نمونه های کد"
  description: "نمونه های کد را که نشان می دهند عملکردهای معمولی GroupDocs.Watermark for Java را بررسی کنید"
  items:
    # code sample loop
    - title: "علامت گذاری یک سند با استفاده از یک تصویر"
      content: |
        از GroupDocs.Watermark for Java برای افزایش امنیت سند با افزودن واترمارک های تصویر استفاده کنید. بیشتر بدانید: [واترمارک های تصویر](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="نحوه محافظت از فایل با علامت تصویر.">}}
        ```csharp {style=abap}
        // سند منبع را به Watermarker بارگیری کنید
        Watermarker watermarker = new Watermarker("document.pdf");
        
        // مسیر تصویر واترمارک را مشخص کنید
        ImageWatermark watermark = new ImageWatermark("watermark.jpg");

        // از فایل محافظت کنید و آن را ذخیره کنید
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "اصلاح واترمارک ها"
      content: |
        GroupDocs.Watermark for Java شما را قادر می سازد تا علامت های موجود در اسناد را مدیریت کنید. علامت های خاص را پیدا کنید و [خواص آنها را تغییر دهید](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="جستجوی و اصلاح واترمارک ها.">}}
        ```csharp {style=abap}   
        // سند منبع را بارگیری کنید
        Watermarker watermarker = new Watermarker("document.pdf");

        // واترمارک ها را برای به روز رسانی جستجو کنید
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);                               
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);                             

        // خواص مورد نظر را به روز کنید
        for (PossibleWatermark watermark : watermarks)                                                           
        {  
            watermark.setText("New Text");
        }

        // سند اصلاح شده را در یک مسیر مشخص ذخیره کنید
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
