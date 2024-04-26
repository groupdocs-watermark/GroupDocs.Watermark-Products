---
############################# Static ############################
layout: "landing"
date: 2024-04-26T21:39:09
draft: false

lang: uk
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
head_title: "Node.js Бібліотека водяних знаків | водяні знаки для документів"
head_description: "Рішення Node.js захищає ділові документи за допомогою текстових і зображених водяних знаків. Підтримуються популярні формати, такі як PDF, Word, Excel, PowerPoint."

############################# Header ############################
title: "Доступ до технології водяних знаків у Node.js за допомогою Java рішень"
description: "Захистіть свою інтелектуальну власність та запобігайте несанкціонованому копіюванню за допомогою цього рішення Node.js. Це дозволяє користувачам легко додавати водяні знаки до ділових документів у різних форматах, включаючи PDF, Word, Excel, PowerPoint, зображення тощо."
words:
  for: "для"

actions:
  main: "Використовуйте NPM для безкоштовного завантаження"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.watermark"
  alt: "Ліцензування"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
  title: "Готові розпочати роботу?"
  description: "Спробуйте GroupDocs.Watermark функцій безкоштовно або попросіть ліцензію"

release:
  title: "Випущена версія {0}"
  notes: "Подивіться, що нового"
  downloads: "Завантаження"
  link: "https://releases.groupdocs.com/watermark/nodejs-java/"

code:
  title: "Додайте водяний знак до PDF за допомогою TypeScript"
  more: "Більше прикладів"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.watermarker"
  content: |
    ```javascript {style=abap}

    // Принциповувати водяний маркер, що проходить шлях PDF
    let loadOptions = new PdfLoadOptions();
    let watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Налаштування параметрів водяного знака
    let textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Застосувати водяний знак до документа PDF
    watermarker.add(textWatermark);

    // Зберегти документ результату
    watermarker.save("result.pdf");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark з першого погляду"
  description: "Node.js Бібліотека TypeScript для водяних знаків"
  features:
    # feature loop
    - title: "Водяний знак файлу Node.js"
      content: "Захистіть свої ділові документи за допомогою GroupDocs.Watermark for Node.js via Java. Додайте текст, зображення, діаграми або вкладення електронної пошти як водяні знаки до різних форматів файлів."

    # feature loop
    - title: "Налаштуйте водяні знаки для ваших потреб"
      content: "GroupDocs.Watermark for Node.js via Java надає широкі можливості налаштування водяних знаків. Точне налаштування стилів тексту (жирний, курсив, шрифт) та властивостей зображення (обертання тощо) дозволяють налаштувати обробку документів."

    # feature loop
    - title: "Комплексна підтримка формату"
      content: "GroupDocs.Watermark for Node.js via Java легко інтегрується з широким спектром форматів файлів, включаючи: PDF, MS Office, як-от Word, Excel, PowerPoint, зображення, такі як JPEG, PNG, GIF, BMP, Visio, Visio діаграми, електронні листи тощо. Розширюйте можливості обробки документів для досягнення бізнес-цілей."

    # feature loop
    - title: "Потужний пошук та оновлення водяних знаків"
      content: "Отримуйте та оновлюйте наявні водяні знаки у документах з водяними знаками. Змініть текст, стиль, вміст зображення або видаліть їх повністю. GroupDocs.Watermark for Node.js via Java забезпечує широкий спектр обробки водяних знаків."

############################# Platforms ############################
platforms:
  enable: true
  title: "Незалежність платформи"
  description: "GroupDocs.Watermark for Node.js via Java легко інтегрується з різними операційними системами та менеджерами пакетів."
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
  title: "Підтримувані формати файлів"
  description: |
    GroupDocs.Watermark for Node.js via Java дає вам можливість обробляти різноманітні формати файлів. [Ознайомтеся з повним списком](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office & OpenDocument формати
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### Зображення та графіка
        * **Популярні формати зображень:** BMP, JPG, JPEG, PNG
        * **Багатосторінкові зображення:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### Інше
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark for Node.js via Java: Набір функцій"
  description: "Забезпечуйте надійну безпеку документів за допомогою програмних водяних знаків. Підтримує різні формати файлів, включаючи: PDF, DOCX, XLSX, PPTX та формати зображень (PNG, JPG тощо)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Точний контроль водяних знаків"
      content: "Точно маніпулюйте водяними знаками, додаючи або видаляючи їх із певних розділів, цілих документів або окремих вкладень та фігур у різних форматах файлів."

    # feature loop
    - icon: "watermark_style"
      title: "Налаштування зовнішнього вигляду водяного знака"
      content: "Здійснюйте чіткий контроль над естетикою водяних знаків, змінюючи атрибути, такі як колір, шрифт, непрозорість, обертання та позиціонування всередині документа."

    # feature loop
    - icon: "hidden_print"
      title: "Друк PDF Водяні знаки"
      content: "Розгорніть прихований водяний знак, який залишається невидимим під час звичайного перегляду документів, але стає очевидним лише під час процесу друку, що стримано підвищує безпеку документів."

    # feature loop
    - icon: "image_only"
      title: "Конкретний водяний знак зображення"
      content: "Конкретні зображення водяного знака в документі за допомогою нашого рішення. Виберіть, щоб вбудовувати водяні знаки у визначений розділ (наприклад, сторінку, слайд) або в усьому документі."

    # feature loop
    - icon: "image_frame"
      title: "Багатокадровий водяний знак зображень"
      content: "Нанесіть водяні знаки вибірково до певних кадрів у форматі багатокадрового зображення, забезпечуючи детальний контроль над розміщенням водяних знаків."

    # feature loop
    - icon: "attachments"
      title: "Комплексний захист контенту"
      content: "Розширте захист на різні елементи документа, як-от вкладення в Excel документах та фігури зображень у презентаціях, забезпечуючи додатковий рівень безпеки."

    # feature loop
    - icon: "pdf_objects"
      title: "Розширені водяні маркування в PDF"
      content: "Позначте водяним знаком різні області довжиною PDF с, включаючи Bleed Box, Art Box, Crop Box, Trim Box тощо."

    # feature loop
    - icon: "doc_background"
      title: "Фонове зображення водяний знак"
      content: "Керуйте водяними знаками на фонових зображеннях електронних таблиць та презентацій, пропонуючи додаткові параметри налаштування для візуальних заходів безпеки."

    # feature loop
    - icon: "unreadable_characters"
      title: "Текстовий водяний знак з нечитаними символами"
      content: "Використовуйте нечитані символи у текстових водяних знаках, вбудованих у презентації, підвищуючи безпеку, роблячи несанкціоноване вилучення водяних знаків значно складнішим."

    # feature loop
    - icon: "watermark_text_search"
      title: "Розширений пошук водяних знаків"
      content: "Використовуйте комплексні можливості пошуку, щоб знайти водяні знаки в документах на основі конкретних параметрів або шляхом поєднання різних критеріїв, що забезпечує ефективний пошук та управління."

    # feature loop
    - icon: "watermark_image_search"
      title: "Подібне виявлення водяного знака зображення"
      content: "Знайдіть подібні зображення водяних знаків у документах, які візуально нагадують вихідне зображення."

    # feature loop
    - icon: "document_info"
      title: "Програмне вилучення інформації про документ"
      content: "Програмно витягуйте цінні метадані, включаючи деталі налаштування сторінки та іншу інформацію про документ для підтримуваних форматів файлів."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Зразки коду"
  description: "Пориньте в приклади коду, що демонструють загальні GroupDocs.Watermark for Node.js via Java функціональні можливості"
  items:
    # code sample loop
    - title: "Встановіть водяний знак документа із зображенням"
      content: |
        Використовуйте GroupDocs.Watermark for Node.js via Java для підвищення безпеки документів, додаючи водяні знаки зображення. Дізнайтеся більше: [Водяні знаки зображення](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Як захистити файл водяним знаком зображення.">}}
        ```javascript {style=abap}
        // Завантажте вихідний документ у Watermarker
        let watermarker = new Watermarker("document.pdf");
        
        // Вкажіть шлях до зображення водяного знака
        let watermark = new ImageWatermark("watermark.jpg");

        // Захистіть файл і збережіть його
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Пошук і зміна існуючих водяних знаків"
      content: |
        GroupDocs.Watermark for Node.js via Java дає вам змогу керувати водяними знаками документів. Виділіть водяні знаки, змініть їх властивості. Дізнайтеся, як: [Змінити водяні знаки](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Пошук і модифікація водяних знаків.">}}
        ```javascript {style=abap}   
        // Завантажити вихідний документ
        let watermarker = new Watermarker("document.pdf");

        // Пошук водяних знаків для оновлення
        let searchCriteria = new TextSearchCriteria("test", false);                               
        let watermarks = watermarker.search(searchCriteria); 

        // Оновлення бажаних властивостей
        watermarks.forEach((watermark)
        {  
            watermark.setText("New Text");
        }

        // Збереження зміненого документа у вказаний шлях
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
