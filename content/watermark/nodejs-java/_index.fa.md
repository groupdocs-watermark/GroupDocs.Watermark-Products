---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:29
draft: false

lang: fa
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js کتابخانه واترمارک | واترمارک های سند"
head_description: "راه حل Node.js از اسناد تجاری با واترمارک های متن و تصویر محافظت می کند. فرمت های محبوب مانند PDF، Word، Excel، PowerPoint پشتیبانی می شوند."

############################# Header ############################
title: "دسترسی به فناوری واترمارک در Node.js از طریق Java راه حل"
description: "با این راه حل Node.js از مالکیت معنوی خود محافظت کنید و از کپی کردن غیر مجاز جلوگیری کنید. این امکان را به کاربران می دهد تا به راحتی واترمارک ها را به اسناد تجاری در فرمت های مختلف اضافه کنند، از جمله PDF، Word، Excel، PowerPoint، تصاویر و غیره."
words:
  for: "برای"

actions:
  main: "برای دانلود رایگان از NPM استفاده کنید"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.watermark"
  alt: "صدور مجوز"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
  title: "آماده شروع هستید؟"
  description: "ویژگی های GroupDocs.Watermark را به صورت رایگان امتحان کنید یا مجوز درخواست کنید"

release:
  title: "نسخه {0} منتشر شد"
  notes: "چیزهای جدید را ببینید"
  downloads: "دانلودها"
  link: "https://releases.groupdocs.com/watermark/nodejs-java/"

code:
  title: "اضافه کردن واترمارک به PDF با TypeScript"
  more: "نمونه های بیشتر"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.watermarker"
  content: |
    ```javascript {style=abap}

    // واترمارکر نمونه ای که از مسیر PDF عبور می کند
    let loadOptions = new PdfLoadOptions();
    let watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // گزینه های واترمارک را سفارشی کنید
    let textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // واترمارک را به PDF سند اعمال کنید
    watermarker.add(textWatermark);

    // ذخیره سند نتیجه
    watermarker.save("result.pdf");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark در یک نگاه"
  description: "کتابخانه تایپ اسکریپت Node.js برای علامت گذاری آب"
  features:
    # feature loop
    - title: "علامت گذاری فایل Node.js"
      content: "از اسناد کسب و کار خود با GroupDocs.Watermark for Node.js via Java محافظت کنید. متن، تصاویر، نمودارها یا پیوست های ایمیل را به عنوان واترمارک به فرمت های مختلف فایل اضافه کنید."

    # feature loop
    - title: "واترمارک ها را برای نیازهای خود سفارشی کنید"
      content: "GroupDocs.Watermark for Node.js via Java گزینه های سفارشی سازی گسترده ای را برای واترمارک ها فراهم می کند. سبک های متن با تنظیم دقیق (پررنگ، ایتالیک، فونت) و خواص تصویر (چرخش و غیره) امکان سفارشی سازی پردازش اسناد را فراهم می کند."

    # feature loop
    - title: "پشتیبانی از فرمت جامع"
      content: "GroupDocs.Watermark for Node.js via Java یکپارچه با طیف گسترده ای از فرمت های فایل ادغام می شود، از جمله: PDF، MS Office مانند Word، Excel، PowerPoint، تصاویری مانند JPEG، PNG، GIF، BMP، Visio نمودارها، ایمیل ها و غیره پردازش اسناد را برای دستیابی به اهداف کسب و کار تقویت می کند."

    # feature loop
    - title: "جستجوی و به روز رسانی قدرتمند علامت"
      content: "واترمارک های موجود را در اسناد واترمارک دریافت و به روز کنید. متن، سبک، محتوای تصویر را اصلاح کنید یا آنها را به طور کامل حذف کنید. GroupDocs.Watermark for Node.js via Java طیف گسترده ای از پردازش واترمارک ها را فراهم می کند."

############################# Platforms ############################
platforms:
  enable: true
  title: "استقلال پلت فرم"
  description: "GroupDocs.Watermark for Node.js via Java به راحتی با سیستم عامل های مختلف و مدیران بسته ادغام می شود."
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
    GroupDocs.Watermark for Node.js via Java شما را قادر می سازد تا طیف متنوعی از فرمت های فایل را پردازش کنید. [لیست کامل را بررسی کنید](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Node.js via Java: مجموعه ویژگی"
  description: "امنیت مستحکم اسناد را از طریق علامت گذاری برنامه نویسی تقویت کنید. پشتیبانی از فرمت های مختلف فایل از جمله: PDF، DOCX، XLSX، PPTX و فرمت های تصویر (PNG، JPG و غیره)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "کنترل دقیق علامت گذاری"
      content: "واترمارک ها را با اضافه کردن یا حذف آنها از بخش های خاص، اسناد کامل یا پیوست ها و اشکال جداگانه در فرمت های مختلف فایل دستکاری کنید."

    # feature loop
    - icon: "watermark_style"
      title: "سفارشی سازی ظاهر واترمارک"
      content: "با تغییر ویژگی هایی مانند رنگ، فونت، کدورت، چرخش و موقعیت در سند، کنترل دقیق بر زیبایی علامت واترمارک اعمال کنید."

    # feature loop
    - icon: "hidden_print"
      title: "چاپ PDF علامت گذاری"
      content: "یک علامت مخفی را نصب کنید که در طول مشاهده منظم سند نامرئی باقی می ماند اما فقط در طول فرآیند چاپ آشکار می شود و امنیت سند را به طور محتاطانه افزایش می دهد."

    # feature loop
    - icon: "image_only"
      title: "واترمارک تصویر خاص"
      content: "تصاویر خاص را در یک سند با استفاده از راه حل ما علامت گذاری کنید. انتخاب کنید که واترمارک ها را در یک بخش تعیین شده (به عنوان مثال، صفحه، اسلاید) یا در کل سند جاسازی کنید."

    # feature loop
    - icon: "image_frame"
      title: "علامت گذاری تصاویر چند فریمی"
      content: "واترمارک ها را به صورت انتخابی به فریم های خاص در یک فرمت تصویر چند فریم اعمال کنید و از کنترل دانه ای بر روی قرار دادن واترمارک اطمینان حاصل کنید"

    # feature loop
    - icon: "attachments"
      title: "حفاظت جامع از محتوا"
      content: "حفاظت را به عناصر مختلف سند مانند پیوست ها در Excel اسناد و اشکال تصویر در Presentations گسترش دهید و یک لایه امنیتی اضافی را فراهم کنید."

    # feature loop
    - icon: "pdf_objects"
      title: "علامت گذاری پیشرفته در PDF"
      content: "مناطق مختلف PDF ثانیه را علامت گذاری کنید، از جمله Bleed Box، Art Box، Crop Box، Trim Box و غیره"

    # feature loop
    - icon: "doc_background"
      title: "واترمارک تصویر پس زمینه"
      content: "واترمارک ها را در تصاویر پس زمینه صفحات گسترده و ارائه ها مدیریت کنید و گزینه های سفارشی سازی اضافی را برای اقدامات امنیتی بصری ارائه دهید."

    # feature loop
    - icon: "unreadable_characters"
      title: "واترمارک متن با کاراکترهای غیرقابل خواندن"
      content: "از کاراکترهای غیرقابل خواندن در علامت های متن تعبیه شده در Presentations استفاده کنید و امنیت را با استخراج علامت غیرمجاز به طور قابل توجهی چالش برانگیزتر کنید."

    # feature loop
    - icon: "watermark_text_search"
      title: "جستجوی پیشرفته علامت"
      content: "از قابلیت های جستجوی جامع برای یافتن علامت های آب در اسناد بر اساس پارامترهای خاص یا با ترکیب معیارهای مختلف استفاده کنید، بازیابی و مدیریت کارآمد را امکان پذیر کنید."

    # feature loop
    - icon: "watermark_image_search"
      title: "تشخیص واترمارک تصویر مشابه"
      content: "تصاویر واترمارک مشابه را در اسنادی پیدا کنید که از نظر بصری شبیه تصویر منبع هستند"

    # feature loop
    - icon: "document_info"
      title: "استخراج اطلاعات سند برنامه ریزی شده"
      content: "فراداده های ارزشمند را به صورت برنامه نویسی استخراج کنید، از جمله جزئیات راه اندازی صفحه و سایر اطلاعات سند برای فرمت های فایل پشتیبانی شده."

############################# Code samples ############################
code_samples:
  enable: true
  title: "نمونه های کد"
  description: "به نمونه های کدی که قابلیت های مشترک GroupDocs.Watermark for Node.js via Java را نشان می دهند، بپردازید"
  items:
    # code sample loop
    - title: "علامت گذاری یک سند با یک تصویر"
      content: |
        از GroupDocs.Watermark for Node.js via Java برای افزایش امنیت سند با افزودن واترمارک های تصویر استفاده کنید. بیشتر بدانید: [واترمارک های تصویر](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="نحوه محافظت از فایل با علامت تصویر.">}}
        ```javascript {style=abap}
        // سند منبع را به Watermarker بارگیری کنید
        let watermarker = new Watermarker("document.pdf");
        
        // مسیر تصویر واترمارک را مشخص کنید
        let watermark = new ImageWatermark("watermark.jpg");

        // از فایل محافظت کنید و آن را ذخیره کنید
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "جستجو و اصلاح واترمارک های موجود"
      content: |
        GroupDocs.Watermark for Node.js via Java شما را قادر می سازد تا واترمارک های سند را مدیریت کنید. واترمارک ها را انتخاب کنید، خواص آنها را تغییر دهید. نحوه انجام این کار را کشف کنید: [اصلاح علامت های آب](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="جستجوی و اصلاح واترمارک ها.">}}
        ```javascript {style=abap}   
        // سند منبع را بارگیری کنید
        let watermarker = new Watermarker("document.pdf");

        // واترمارک ها را برای به روز رسانی جستجو کنید
        let searchCriteria = new TextSearchCriteria("test", false);                               
        let watermarks = watermarker.search(searchCriteria); 

        // خواص مورد نظر را به روز کنید
        watermarks.forEach((watermark)
        {  
            watermark.setText("New Text");
        }

        // سند اصلاح شده را در یک مسیر مشخص ذخیره کنید
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
