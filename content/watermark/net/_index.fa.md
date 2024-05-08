---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:29
draft: false

lang: fa
product: "Watermark"
product_tag: "watermark"
platform: "Net"
platform_tag: "net"

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
head_title: "C# .NET نرم افزار واترمارک سند | اضافه کردن واترمارک"
head_description: "کتابخانه C# .NET برای افزودن، جستجو و حذف واترمارک ها در اسناد: PDF، Word، Excel، ارائه ها، Visio نمودارها، ایمیل و فرمت های فایل تصویری."

############################# Header ############################
title: "اسناد واترمارک به راحتی در برنامه های C# .NET شما"
description: "راه حل های C# خود را با یک API واترمارک اسناد انعطاف پذیر که اضافه کردن واترمارک های قابل تنظیم به تمام فرمت های محبوب سند را فراهم می کند، تقویت کنید."
words:
  for: "برای"

actions:
  main: "دانلود رایگان NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Watermark"
  alt: "صدور مجوز"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/net/"
  title: "آماده شروع هستید؟"
  description: "ویژگی های GroupDocs.Watermark را به صورت رایگان امتحان کنید یا مجوز درخواست کنید"

release:
  title: "نسخه {0} منتشر شد"
  notes: "چیزهای جدید را ببینید"
  downloads: "دانلودها"

code:
  title: "علامت گذاری PDF فایل ها در C #"
  more: "نمونه های بیشتر"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
  install: "dotnet add package GroupDocs.Watermark"
  content: |
    ```csharp {style=abap}   
    // واترمارکر نمونه ای که از مسیر PDF عبور می کند
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    using (Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions))
    {
        // گزینه های واترمارک را سفارشی کنید
        TextWatermark textWatermark = 
            new TextWatermark("Approved", new Font("Arial", 8));
        
        // واترمارک را به PDF سند اعمال کنید
        watermarker.Add(textWatermark);

        // ذخیره سند نتیجه
        watermarker.Save("result.pdf");
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark در یک نگاه"
  description: "API برای قرار دادن واترمارک بر روی اسناد از طریق .NET"
  features:
    # feature loop
    - title: "علامت فایل های C#"
      content: "با استفاده از GroupDocs.Watermark واترمارک ها را به فایل های کسب و کار خود اضافه کنید. از متن، تصاویر، نمودارها یا پیوست های ایمیل استفاده کنید."

    # feature loop
    - title: "واترمارک ها را با اهداف خود سفارشی کنید"
      content: "نرم افزار GroupDocs.Watermark for .NET اجازه می دهد تا واترمارک ها را به روش های مختلف سفارشی کنید. سبک های متن مانند پررنگ، ایتالیک، انواع فونت همراه با خواص تصویر مانند چرخش و غیره روند علامت گذاری را غنی می کنند."

    # feature loop
    - title: "تمام فرمت های فایل محبوب پشتیبانی می شوند"
      content: "بسیاری از فرمت های فایل و سند توسط راه حل GroupDocs.Watermark پشتیبانی می شوند. PDF، Microsoft Office Word، Excel، PowerPoint، تصاویری مانند JPEG، PNG، GIF، BMP، Visio، ایمیل ها و غیره می توانند با واترمارک های ما محافظت شوند."

    # feature loop
    - title: "جستجو و به روز رسانی واترمارک ها"
      content: "علامت هایی که قبلاً در یک سند ارائه شده اند ممکن است دوباره پیدا شوند و پردازش شوند. متن، سبک، تصاویر را تغییر دهید یا علامت های آشکار شده را بدون تلاش اضافی حذف کنید."

############################# Platforms ############################
platforms:
  enable: true
  title: "استقلال پلت فرم"
  description: "GroupDocs.Watermark for .NET از سیستم عامل ها، چارچوب ها و مدیران بسته ذکر شده در زیر پشتیبانی می کند"
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "فرمت های فایل پشتیبانی شده"
  description: |
    GroupDocs.Watermark for .NET پردازش [فرمت های فایل](https://docs.groupdocs.com/watermark/net/supported-document-formats/) زیر را فراهم می کند .
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
  title: "GroupDocs.Watermark ویژگی ها"
  description: "محافظت از PDF، دفتر، تصاویر و سایر فرمت ها با واترمارک"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "علامت گذاری اسناد"
      content: "واترمارک ها را از یک بخش خاص یا کل سند با فرمت های مختلف فایل اضافه یا حذف کنید."

    # feature loop
    - icon: "watermark_style"
      title: "واترمارک خود را سبک کنید"
      content: "خصوصیات مختلف واترمارک مانند رنگ، فونت، چرخش و غیره را سفارشی کنید"

    # feature loop
    - icon: "hidden_print"
      title: "PDF علامت چاپ پنهان"
      content: "واترمارک پنهان را به PDF اختصاص دهید که فقط هنگام چاپ سند ظاهر می شود."

    # feature loop
    - icon: "image_only"
      title: "علامت گذاری فقط تصاویر در اسناد"
      content: "تمام تصاویر را در یک بخش خاص، صفحه، اسلاید یا سند علامت گذاری کنید."

    # feature loop
    - icon: "image_frame"
      title: "پردازش فریم های تصویر انتخاب شده"
      content: "واترمارک را فقط به فریم های خاص یک تصویر چند فریم اختصاص دهید."

    # feature loop
    - icon: "attachments"
      title: "پیوست ها و اشکال"
      content: "واترمارک را برای همه پیوست ها در یک سند Excel و تمام اشکال تصویر در اسلایدها تنظیم کنید."

    # feature loop
    - icon: "pdf_objects"
      title: "PDF اشیاء"
      content: "واترمارک را با جعبه Bleed، جعبه هنر، جعبه برش یا جعبه برش در PDF سند تنظیم کنید."

    # feature loop
    - icon: "doc_background"
      title: "سوابق اسناد"
      content: "واترمارک را قرار دهید یا آن را از تصاویر پس زمینه صفحه گسترده یا اسلایدها حذف کنید."

    # feature loop
    - icon: "unreadable_characters"
      title: "حفاظت از شخصیت های غیر قابل خواندن"
      content: "محافظت از واترمارک متن با استفاده از کاراکترهای غیرقابل خواندن در ارائه ها."

    # feature loop
    - icon: "watermark_text_search"
      title: "جستجو واترمارک در اسناد"
      content: "واترمارک ها را بر اساس پارامترهای خاص یا با ترکیب معیارهای متعدد جستجو کنید."

    # feature loop
    - icon: "watermark_image_search"
      title: "جستجوی واترمارک های تصویر مشابه"
      content: "به دنبال واترمارک های تصویری باشید که شبیه یک تصویر خاص هستند."

    # feature loop
    - icon: "document_info"
      title: "دریافت اطلاعات سند"
      content: "به صورت برنامه ریزی راه اندازی صفحه و سایر اطلاعات را برای فرمت های پشتیبانی شده استخراج کنید."

############################# Code samples ############################
code_samples:
  enable: true
  title: "نمونه های کد"
  description: "برخی از موارد استفاده از عملیات معمولی GroupDocs.Watermark for .NET"
  items:
    # code sample loop
    - title: "واترمارک با افزودن یک تصویر به یک سند."
      content: |
        برای محافظت از هر سند می توانید از [واترمارک های تصویر](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/) استفاده کنید:
        {{< landing/code title="نحوه محافظت از فایل با علامت تصویر.">}}
        ```csharp {style=abap}
        // سند منبع را به Watermarker بارگیری کنید
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // مسیر تصویر واترمارک را مشخص کنید
            using (ImageWatermark watermark = new ImageWatermark("watermark.jpg"))
            {
                // از فایل محافظت کنید و آن را ذخیره کنید
                watermarker.Add(watermark);

                watermarker.Save("result.pdf");
            }
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "علامت های موجود را جستجو و اصلاح کنید."
      content: |
        GroupDocs.Watermark قادر به [اصلاح واترمارک](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/) است که قبلاً در یک سند ارائه شده اند. موارد مورد نظر را جستجو کنید و خواص آنها را به روز کنید.
        {{< landing/code title="جستجوی و اصلاح واترمارک ها.">}}
        ```csharp {style=abap}   
        // سند منبع را بارگیری کنید
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // واترمارک ها را برای به روز رسانی جستجو کنید
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                // خواص مورد نظر را به روز کنید
                watermark.Text = "New Text";
            }

            // سند اصلاح شده را در یک مسیر مشخص ذخیره کنید
            watermarker.Save("document.pdf");
        }
        ```
        {{< /landing/code >}}

---
