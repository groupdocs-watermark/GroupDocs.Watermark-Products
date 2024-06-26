---
############################# Static ############################
layout: "landing"
date: 2024-06-26T08:41:24
draft: false

lang: fa
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

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
    # supported_platforms loop
    - title: "Python"
      tag: "python-net"

############################# Head ############################
head_title: "Python کتابخانه واترمارک | واترمارک های سند"
head_description: "Python از اسناد تجاری با واترمارک های متنی و تصویری محافظت می کند. فرمت های فایل مانند PDF، Word، Excel و PowerPoint پشتیبانی می شوند."

############################# Header ############################
title: "به فناوری واترمارکینگ Python via .NET دسترسی پیدا کنید"
description: "با این راه حل Python از داده های خود محافظت کنید و از کپی غیرمجاز جلوگیری کنید. به راحتی واترمارک ها را به اسناد تجاری در قالب های مختلف از جمله PDF، Word، Excel، PowerPoint، تصاویر و غیره اضافه کنید."
words:
  for: "برای"

actions:
  main: "PyPi را به صورت رایگان دانلود کنید"
  main_link: "https://pypi.org/project/groupdocs-watermark-net/"
  alt: "صدور مجوز"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
  title: "آماده شروع هستید؟"
  description: "ویژگی های GroupDocs.Watermark را به صورت رایگان امتحان کنید یا مجوز درخواست کنید"

release:
  title: "نسخه {0} منتشر شد"
  notes: "چیزهای جدید را ببینید"
  downloads: "دانلودها"
  link: "https://releases.groupdocs.com/watermark/python-net/"

code:
  title: "اضافه کردن واترمارک به PDF با استفاده از Python"
  more: "نمونه های بیشتر"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
  install: "pip install groupdocs-watermark-net"
  content: |
    ```python {style=abap}

    import groupdocs.watermark as gw
    import groupdocs.watermark.watermarks as gww
    import groupdocs.watermark.options.pdf as gwop
    import groupdocs.watermark.common as gwc

    # واترمارکر نمونه ای که از مسیر PDF عبور می کند
    pdf_lo = gwop.PdfLoadOptions()
    with gw.Watermarker("source.pdf", pdf_lo) as watermarker:
        options = gwop.PdfArtifactWatermarkOptions()

        # گزینه های واترمارک را سفارشی کنید
        text_watermark = 
            gww.TextWatermark("Approved", gww.Font("Arial", 8.0))
        text_watermark.horizontal_alignment = 
            gwc.HorizontalAlignment.RIGHT

        # واترمارک را به PDF سند اعمال کنید
        watermarker.add(text_watermark, options)

        # ذخیره سند نتیجه
        watermarker.save("result.pdf")

    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark در یک نگاه"
  description: "کتابخانه Python برای واترمارکینگ"
  features:
    # feature loop
    - title: "Python واترمارک کردن سند"
      content: "اطلاعات حساس خود را با GroupDocs.Watermark for Python via .NET ایمن کنید. متن یا تصاویر را در قالب های مختلف فایل به عنوان واترمارک قرار دهید."

    # feature loop
    - title: "واترمارک ها را سفارشی کنید"
      content: "بسیاری از گزینه های سفارشی سازی در GroupDocs.Watermark for Python via .NET موجود است. سبک‌های متن (پررنگ، مورب، فونت) یا ویژگی‌های تصویر مانند اندازه یا چرخش را برای تنظیم واترمارک سند تنظیم کنید."

    # feature loop
    - title: "پشتیبانی از فرمت های فایل محبوب"
      content: "GroupDocs.Watermark for Python via .NET از طیف وسیعی از فرمت‌های فایل، از جمله PDF، اسناد MS Office مانند Word، Excel، PowerPoint و تصاویری مانند JPEG، PNG، GIF، BMP، نمودارهای Visio، ایمیل‌ها و غیره پشتیبانی می‌کند. پردازش اسناد را برای پاسخگویی به کسب و کار افزایش دهید. اهداف"

    # feature loop
    - title: "جستجو و به روز رسانی واترمارک"
      content: "واترمارک هایی که در اسناد قرار داده شده اند را بازیابی و به روز کنید. سبک متن، محتوای تصویر را تغییر دهید یا آنها را به طور کامل حذف کنید. GroupDocs.Watermark for Python via .NET طیف وسیعی از قابلیت‌های پردازش واترمارک را ارائه می‌دهد."

############################# Platforms ############################
platforms:
  enable: true
  title: "استقلال پلت فرم"
  description: "GroupDocs.Watermark for Python via .NET به طور یکپارچه با سیستم عامل های مختلف و مدیران بسته ادغام می شود."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "فرمت های فایل پشتیبانی شده"
  description: |
    GroupDocs.Watermark for Python via .NET به شما این امکان را می‌دهد که طیف متنوعی از قالب‌های فایل را پردازش کنید. [لیست کامل را کاوش کنید](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "ویژگی های GroupDocs.Watermark for Python via .NET"
  description: "تقویت امنیت اسناد از طریق واترمارکینگ برنامه‌ای. فرمت های مختلف فایل از جمله PDF، DOCX، XLSX، PPTX و فرمت های تصویر (PNG، JPG و غیره) را پردازش کنید."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "کنترل واترمارکینگ دقیق"
      content: "با افزودن یا حذف آنها از بخش‌های خاص، کل اسناد، یا پیوست‌ها و شکل‌های جداگانه در قالب‌های فایل مختلف، واترمارک‌ها را دقیقاً مدیریت کنید."

    # feature loop
    - icon: "watermark_style"
      title: "ظاهر واترمارک را سفارشی کنید"
      content: "با اصلاح ویژگی‌هایی مانند رنگ، فونت، کدورت، چرخش و موقعیت‌یابی در سند، کنترل دقیقی بر زیبایی‌شناسی واترمارک اعمال کنید."

    # feature loop
    - icon: "hidden_print"
      title: "چاپ PDF Watermarking"
      content: "واترمارک های مخفی را به اسناد معمولی اضافه کنید که فقط در طول فرآیند چاپ قابل مشاهده هستند و امنیت اسناد را به طور محتاطانه ای افزایش می دهند."

    # feature loop
    - icon: "image_only"
      title: "واترمارکینگ تصویر خاص"
      content: "با استفاده از راه حل ما، تصاویر خاص را در یک سند واترمارک کنید. واترمارک ها را در یک بخش مشخص شده (به عنوان مثال، صفحه، اسلاید) یا در کل سند جاسازی کنید."

    # feature loop
    - icon: "image_frame"
      title: "واترمارک تصویر چند لایه"
      content: "واترمارک ها را دقیقاً به فریم های خاص در قالب تصویر چند فریمی اضافه کنید و به کنترل دانه ای بر روی قرار دادن واترمارک دست یابید."

    # feature loop
    - icon: "attachments"
      title: "حفاظت جامع از محتوا"
      content: "حفاظت را به عناصر مختلف سند مانند پیوست‌ها در اسناد اکسل و شکل‌های تصویر در ارائه‌ها گسترش دهید و یک لایه امنیتی اضافی را فراهم کنید."

    # feature loop
    - icon: "pdf_objects"
      title: "Watermarking پیشرفته PDF"
      content: "قسمت های مختلف فایل های PDF، از جمله Bleed Box، Art Box، Crop Box، Trim Box و غیره را واترمارک کنید."

    # feature loop
    - icon: "doc_background"
      title: "واترمارکینگ تصویر پس زمینه"
      content: "واترمارک ها را در تصاویر پس زمینه صفحات گسترده و ارائه ها مدیریت کنید و گزینه های سفارشی سازی اضافی را برای اقدامات امنیتی بصری ارائه دهید."

    # feature loop
    - icon: "unreadable_characters"
      title: "واترمارک متنی با کاراکترهای ناخوانا"
      content: "از کاراکترهای غیرقابل خواندن در واترمارک های متنی که در ارائه ها تعبیه شده اند، استفاده کنید و با چالش برانگیزتر کردن استخراج واترمارک غیرمجاز، امنیت را تقویت کنید."

    # feature loop
    - icon: "watermark_text_search"
      title: "جستجوی واترمارک پیشرفته"
      content: "از ویژگی های جستجوی جامع برای تعیین موقعیت واترمارک در اسناد بر اساس پارامترهای خاص یا با ترکیب معیارهای مختلف استفاده کنید."

    # feature loop
    - icon: "watermark_image_search"
      title: "تشخیص واترمارک تصویر مشابه"
      content: "تصاویر واترمارک مشابه را در اسنادی که از نظر بصری شبیه تصویر منبع هستند پیدا کنید."

    # feature loop
    - icon: "document_info"
      title: "تجزیه و تحلیل اطلاعات اسناد"
      content: "برای تجزیه و تحلیل بیشتر، داده های اسناد ضروری مانند تنظیم صفحه را استخراج کنید."

############################# Code samples ############################
code_samples:
  enable: true
  title: "نمونه های کد"
  description: "نمونه‌های کدی را کاوش کنید که عملکردهای رایج GroupDocs.Watermark for Python via .NET را نشان می‌دهد."
  items:
    # code sample loop
    - title: "یک سند را با یک تصویر واترمارک کنید"
      content: |
        از GroupDocs.Watermark for Python via .NET برای محافظت از اسناد با افزودن واترمارک تصویر استفاده کنید. [بیشتر بیاموزید](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="نحوه محافظت از فایل با علامت تصویر.">}}
        ```python {style=abap}

        # سند منبع را به Watermarker بارگیری کنید
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # مسیر تصویر واترمارک را مشخص کنید
            watermark = groupdocs.watermark.watermarks.ImageWatermark("watermark.jpg")
            watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwgroupdocs.watermark.common.VerticalAlignment.CENTER

            # از فایل محافظت کنید و آن را ذخیره کنید
            watermarker.add(watermark)
            watermarker.save("result.pdf")
       
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "جستجو و اصلاح واترمارک های موجود"
      content: |
        GroupDocs.Watermark for Python via .NET به شما امکان مدیریت واترمارک سند را می‌دهد. واترمارک ها را انتخاب کنید و ویژگی های آنها را تغییر دهید. [چگونه را کشف کنید](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/).
        {{< landing/code title="جستجوی و اصلاح واترمارک ها.">}}
        ```python {style=abap}

        # سند منبع را بارگیری کنید
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # واترمارک ها را برای به روز رسانی جستجو کنید
            search_criteria = groupdocs.watermark.search.searchcriteria.TextSearchCriteria("annotation", False)
            watermarks = watermarker.search(search_criteria)
            
            # خواص مورد نظر را به روز کنید
            for watermark in watermarks:
                watermark.text = "passed"

            # سند اصلاح شده را در یک مسیر مشخص ذخیره کنید
            watermarker.save("result.pdf")


        ```
        {{< /landing/code >}}

---
