---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:29
draft: false

lang: ru
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
head_title: "Библиотека водяных знаков Node.js | водяные знаки документов"
head_description: "Решение Node.js защищает деловые документы с помощью текстовых и графических водяных знаков. Поддерживаются популярные форматы, такие как PDF, Word, Excel, PowerPoint."

############################# Header ############################
title: "Доступ к технологии водяных знаков в Node.js с помощью решений Java"
description: "Защитите свою интеллектуальную собственность и предотвратите несанкционированное копирование с помощью этого решения Node.js. Оно позволяет пользователям легко добавлять водяные знаки в деловые документы различных форматов, включая PDF, Word, Excel, PowerPoint, изображения и т. д."
words:
  for: "для"

actions:
  main: "Используйте NPM для бесплатной загрузки"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.watermark"
  alt: "Лицензирование"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Watermark бесплатно или запросите лицензию"

release:
  title: "Выпущена версия {0}"
  notes: "Узнайте, что нового"
  downloads: "Загрузки"
  link: "https://releases.groupdocs.com/watermark/nodejs-java/"

code:
  title: "Добавьте водяной знак в PDF с помощью TypeScript"
  more: "Больше примеров"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.watermark"
  content: |
    ```javascript {style=abap}

    // Создайте экземпляр Watermarker, передающий путь PDF
    let loadOptions = new PdfLoadOptions();
    let watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Настройте параметры водяных знаков
    let textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Применить водяной знак к документу PDF
    watermarker.add(textWatermark);

    // Сохранить документ с результатами
    watermarker.save("result.pdf");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark с первого взгляда"
  description: "Библиотека TypeScript Node.js для водяных знаков"
  features:
    # feature loop
    - title: "Нанесение водяных знаков на файл Node.js"
      content: "Защитите свои деловые документы с помощью GroupDocs.Watermark for Node.js via Java. Добавляйте текст, изображения, диаграммы или вложения электронной почты в качестве водяных знаков к файлам различных форматов."

    # feature loop
    - title: "Настройте водяные знаки в соответствии со своими потребностями"
      content: "GroupDocs.Watermark for Node.js via Java предоставляет широкие возможности настройки водяных знаков. Точная настройка стилей текста (полужирный шрифт, курсив, шрифт) и свойств изображения (поворот и т. д.) позволяет настроить обработку документов."

    # feature loop
    - title: "Комплексная поддержка форматов"
      content: "GroupDocs.Watermark for Node.js via Java легко интегрируется с широким спектром форматов файлов, включая PDF, MS Office, например Word, Excel, PowerPoint, изображения, такие как JPEG, PNG, GIF, BMP, Visio, диаграммы, электронные письма и т. д. Упрощают обработку документов для достижения бизнес-целей."

    # feature loop
    - title: "Мощный поиск и обновление водяных знаков"
      content: "Получите и обновите существующие водяные знаки в документах с водяными знаками. Измените текст, стиль, содержимое изображений или полностью удалите их. GroupDocs.Watermark for Node.js via Java предоставляет широкий спектр возможностей обработки водяных знаков."

############################# Platforms ############################
platforms:
  enable: true
  title: "Независимость платформы"
  description: "GroupDocs.Watermark for Node.js via Java легко интегрируется с различными операционными системами и менеджерами пакетов."
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
  title: "Поддерживаемые форматы файлов"
  description: |
    GroupDocs.Watermark for Node.js via Java позволяет обрабатывать файлы самых разных форматов. [Ознакомьтесь с полным списком](https://docs.groupdocs.com/watermark/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### форматы Microsoft Office и OpenDocument
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### Изображения и графика
        * **Популярные форматы изображений:** BMP, JPG, JPEG, PNG
        * **Многостраничные изображения:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### Другой
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark for Node.js via Java: набор функций"
  description: "Обеспечьте надежную защиту документов с помощью программных водяных знаков. Поддерживает различные форматы файлов, включая: PDF, DOCX, XLSX, PPTX и форматы изображений (PNG, JPG и т. д.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Точное управление водяными знаками"
      content: "Точно управляйте водяными знаками, добавляя или удаляя их из определенных разделов, целых документов или отдельных вложений и фигур в разных форматах файлов."

    # feature loop
    - icon: "watermark_style"
      title: "Настройка внешнего вида водяных знаков"
      content: "Тщательно контролируйте эстетику водяных знаков, изменяя такие атрибуты, как цвет, шрифт, непрозрачность, поворот и положение в документе."

    # feature loop
    - icon: "hidden_print"
      title: "Распечатать PDF Водяные знаки"
      content: "Установите скрытый водяной знак, который остается невидимым при обычном просмотре документов, но становится заметным только в процессе печати, тем самым незаметно повышая безопасность документов."

    # feature loop
    - icon: "image_only"
      title: "Водяные знаки для конкретных изображений"
      content: "Используйте наше решение для нанесения водяных знаков на определенные изображения в документе. Выберите встраивание водяных знаков в определенный раздел (например, страницу, слайд) или во весь документ."

    # feature loop
    - icon: "image_frame"
      title: "Нанесение водяных знаков на многокадровые изображения"
      content: "Выборочно наносите водяные знаки на определенные кадры в формате многокадрового изображения, обеспечивая детальный контроль над размещением водяных знаков."

    # feature loop
    - icon: "attachments"
      title: "Комплексная защита контента"
      content: "Расширьте защиту различных элементов документов, таких как вложения в Excel документах и формы изображений в презентациях, обеспечив дополнительный уровень безопасности."

    # feature loop
    - icon: "pdf_objects"
      title: "Расширенные водяные знаки в PDF"
      content: "Нанесите водяные знаки на различные области PDF s, включая Bleed Box, Art Box, Crop Box, Trim Box и т. д."

    # feature loop
    - icon: "doc_background"
      title: "Водяные знаки на фоновом изображении"
      content: "Управляйте водяными знаками на фоновых изображениях электронных таблиц и презентаций, предлагая дополнительные возможности настройки визуальных мер безопасности."

    # feature loop
    - icon: "unreadable_characters"
      title: "Текстовый водяной знак с нечитаемыми символами"
      content: "Используйте нечитаемые символы в текстовых водяных знаках, встроенных в презентации, чтобы повысить безопасность, значительно усложняя несанкционированное извлечение водяных знаков."

    # feature loop
    - icon: "watermark_text_search"
      title: "Расширенный поиск водяных знаков"
      content: "Используйте комплексные возможности поиска для поиска водяных знаков в документах на основе определенных параметров или комбинирования различных критериев, что обеспечивает эффективный поиск и управление ими."

    # feature loop
    - icon: "watermark_image_search"
      title: "Обнаружение водяных знаков на похожих изображениях"
      content: "Найдите похожие изображения водяных знаков в документах, визуально напоминающих исходное изображение."

    # feature loop
    - icon: "document_info"
      title: "Программное извлечение информации из документов"
      content: "Извлекайте ценные метаданные программно, включая сведения о настройках страницы и другую информацию о документах для поддерживаемых форматов файлов."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Образцы кода"
  description: "Ознакомьтесь с примерами кода, демонстрирующими распространенные функции GroupDocs.Watermark for Node.js via Java"
  items:
    # code sample loop
    - title: "Нанесение водяных знаков на документ с помощью изображения"
      content: |
        Используйте GroupDocs.Watermark for Node.js via Java для повышения безопасности документов, добавляя водяные знаки изображений. Подробнее: [Водяные знаки на изображениях](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Как защитить файл водяным знаком изображения.">}}
        ```javascript {style=abap}
        // Загрузить исходный документ в Watermarker
        let watermarker = new Watermarker("document.pdf");
        
        // Укажите путь к изображению водяного знака
        let watermark = new ImageWatermark("watermark.jpg");

        // Защитите файл и сохраните его
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Поиск и изменение существующих водяных знаков"
      content: |
        GroupDocs.Watermark for Node.js via Java позволяет управлять водяными знаками документов. Выберите водяные знаки, измените их свойства. Узнайте, как: [Изменить водяные знаки](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Поиск и модификация водяных знаков.">}}
        ```javascript {style=abap}   
        // Загрузить исходный документ
        let watermarker = new Watermarker("document.pdf");

        // Поиск водяных знаков, подлежащих обновлению
        let searchCriteria = new TextSearchCriteria("test", false);                               
        let watermarks = watermarker.search(searchCriteria); 

        // Обновите нужные свойства
        watermarks.forEach((watermark)
        {  
            watermark.setText("New Text");
        }

        // Сохранить измененный документ по указанному пути
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
