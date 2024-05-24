---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:29
draft: false

lang: uk
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
head_title: "Java Бібліотека водяних знаків | додавання водяних знаків до документів"
head_description: "Внутрішнє Java програмне забезпечення для додавання та маніпулювання текстовими водяними знаками та зображеннями у файлах PDF, Word, Excel, Презентацій, Visio діаграм, електронних листів та зображень."

############################# Header ############################
title: "Легко впроваджуйте водяний знак документів у Java проектах"
description: "Покращуйте свої Java програми за допомогою можливості додавати водяні знаки файлів за допомогою бібліотеки GroupDocs.Watermark. Наш API пропонує настроювані водяні знаки для широкого спектру популярних форматів файлів."
words:
  for: "для"

actions:
  main: "Безкоштовно завантажити з Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "Ліцензування"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java/"
  title: "Готові розпочати роботу?"
  description: "Спробуйте GroupDocs.Watermark функцій безкоштовно або попросіть ліцензію"

release:
  title: "Випущена версія {0}"
  notes: "Подивіться, що нового"
  downloads: "Завантаження"

code:
  title: "Водяний знак PDF с через Java"
  more: "Більше прикладів"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-watermark</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Принциповувати водяний маркер, що проходить шлях PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Налаштування параметрів водяного знака
    TextWatermark textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Застосувати водяний знак до документа PDF
    watermarker.add(textWatermark);

    // Зберегти документ результату
    watermarker.save("result.pdf");
    watermarker.close();
      
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark з першого погляду"
  description: "Бібліотека, призначена для додавання водяних знаків за допомогою Java технологій"
  features:
    # feature loop
    - title: "Файли водяних знаків через Java"
      content: "Захистіть свої ділові документи за допомогою GroupDocs.Watermark for Java. Додайте текст, зображення, діаграми або вкладення електронної пошти як водяні знаки до різних форматів файлів."

    # feature loop
    - title: "Налаштуйте водяні знаки для конкретних потреб"
      content: "GroupDocs.Watermark for Java пропонує широкі можливості налаштування водяних знаків. Налаштуйте стилі тексту (жирний, курсив, шрифт) та властивості зображення (обертання тощо), щоб адаптувати процес водяних знаків до ваших конкретних цілей."

    # feature loop
    - title: "Підтримка широкого формату"
      content: "GroupDocs.Watermark for Java легко інтегрується з широким спектром форматів файлів, включаючи: PDF, Microsoft Office (Word, Excel, PowerPoint), зображення (JPEG, PNG, GIF, BMP), Visio діаграми та електронні листи. Підвищення безпеки документів у різних типах файлів."

    # feature loop
    - title: "Легкий пошук і управління водяними знаками"
      content: "Ефективно керуйте існуючими водяними знаками в документах. Знайдіть певні водяні знаки, змініть їх текст, стиль або зображення або видаліть їх повністю. GroupDocs.Watermark for Java спрощує процес водяних знаків."

############################# Platforms ############################
platforms:
  enable: true
  title: "Незалежність платформи"
  description: "GroupDocs.Watermark for Java підтримує різні операційні системи та менеджери пакетів."
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
  title: "Підтримувані формати файлів"
  description: |
    GroupDocs.Watermark for Java дозволяє обробляти широкий спектр форматів файлів. [Дивіться повний список](https://docs.groupdocs.com/watermark/java/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Java: Особливості"
  description: "Захистіть свої файли, додавши водяні знаки. Підтримує різні формати, включаючи PDF, документи Office та зображення."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Файли водяний знак"
      content: "Додайте або видаляйте водяні знаки з певних розділів або цілих документів для різних підтримуваних форматів файлів."

    # feature loop
    - icon: "watermark_style"
      title: "Налаштування водяних знаків"
      content: "Налаштуйте зовнішній вигляд водяного знака за допомогою таких параметрів, як колір, шрифт, обертання тощо."

    # feature loop
    - icon: "hidden_print"
      title: "Прихований друкарський водяний знак для PDF"
      content: "Додайте водяний знак, який з'являється лише під час друку документа PDF."

    # feature loop
    - icon: "image_only"
      title: "Вибірковий водяний знак зображення"
      content: "Встановіть водяним знаком усі зображення в певному розділі, сторінці, слайді або в цілому документі."

    # feature loop
    - icon: "image_frame"
      title: "Водяні маркування конкретних кадрів зображень"
      content: "Застосовуйте водяні знаки до певних кадрів у багаторамковому зображенні."

    # feature loop
    - icon: "attachments"
      title: "Вкладення та форми для водяних знаків"
      content: "Додайте водяні знаки до всіх вкладень у документах Excel або до всіх форм зображень у презентаціях."

    # feature loop
    - icon: "pdf_objects"
      title: "Вирівнювання водяних знаків у PDF"
      content: "Вирівнюйте водяні знаки за різними ділянками документа PDF, включаючи поле для розпуску, графічне поле, поле для обрізання та поле обрізки."

    # feature loop
    - icon: "doc_background"
      title: "Водяний знак за фоновим зображенням"
      content: "Додайте або видаліть водяний знак фонового зображення до електронних таблиць або презентацій."

    # feature loop
    - icon: "unreadable_characters"
      title: "Захист нечитабельними символами"
      content: "Захистіть презентації за допомогою текстового водяного знака з нечитабельними символами."

    # feature loop
    - icon: "watermark_text_search"
      title: "Пошук водяних знаків"
      content: "Отримати список водяних знаків, представлених у файлі, використовуючи різні параметри, включаючи регулярні вирази."

    # feature loop
    - icon: "watermark_image_search"
      title: "Знайти схожі зображення водяні знаки"
      content: "Знайдіть водяні знаки зображення, схожі на конкретне зображення."

    # feature loop
    - icon: "document_info"
      title: "Витягніть інформацію про документ"
      content: "Отримайте різні дані документа, як-от налаштування сторінки для підтримуваних форматів файлів."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Зразки коду"
  description: "Вивчіть приклади коду, що ілюструють типові GroupDocs.Watermark for Java функціональні можливості"
  items:
    # code sample loop
    - title: "Встановіть водяний знак документа за допомогою зображення"
      content: |
        Використовуйте GroupDocs.Watermark for Java для підвищення безпеки документів, додаючи водяні знаки зображення. Дізнайтеся більше: [Водяні знаки зображення](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Як захистити файл водяним знаком зображення.">}}
        ```java {style=abap}
        // Завантажте вихідний документ у Watermarker
        Watermarker watermarker = new Watermarker("document.pdf");
        
        // Вкажіть шлях до зображення водяного знака
        ImageWatermark watermark = new ImageWatermark("watermark.jpg");

        // Захистіть файл і збережіть його
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Змінити водяні знаки"
      content: |
        GroupDocs.Watermark for Java дає вам змогу керувати наявними водяними знаками в документах. Знайдіть конкретні водяні знаки та [змініть їх властивості](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Пошук і модифікація водяних знаків.">}}
        ```java {style=abap}   
        // Завантажити вихідний документ
        Watermarker watermarker = new Watermarker("document.pdf");

        // Пошук водяних знаків для оновлення
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);                               
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);                             

        // Оновлення бажаних властивостей
        for (PossibleWatermark watermark : watermarks)                                                           
        {  
            watermark.setText("New Text");
        }

        // Збереження зміненого документа у вказаний шлях
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
