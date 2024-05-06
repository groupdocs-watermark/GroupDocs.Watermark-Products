---
############################# Static ############################
layout: "landing"
date: 2024-05-06T23:13:47
draft: false

lang: ru
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
head_title: "Java Библиотека водяных знаков | добавление водяных знаков к документам"
head_description: "Встроенное программное обеспечение Java для добавления и обработки текстовых и графических водяных знаков в PDF, Word, Excel, презентациях, Visio диаграммах, электронных письмах и файлах изображений."

############################# Header ############################
title: "Легко внедряйте водяные знаки на документы в Java проектах"
description: "Усовершенствуйте свои приложения Java, предоставив возможность нанесения водяных знаков на файлы с помощью библиотеки GroupDocs.Watermark. Наш API предлагает настраиваемые водяные знаки для широкого спектра популярных форматов файлов."
words:
  for: "для"

actions:
  main: "Бесплатная загрузка с Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "Лицензирование"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java/"
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Watermark бесплатно или запросите лицензию"

release:
  title: "Выпущена версия {0}"
  notes: "Узнайте, что нового"
  downloads: "Загрузки"

code:
  title: "Водяной знак PDF s через Java"
  more: "Больше примеров"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-watermark</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Создайте экземпляр Watermarker, передающий путь PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Настройте параметры водяных знаков
    TextWatermark textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Применить водяной знак к документу PDF
    watermarker.add(textWatermark);

    // Сохранить документ с результатами
    watermarker.save("result.pdf");
    watermarker.close();
      
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark с первого взгляда"
  description: "Библиотека, предназначенная для добавления водяных знаков с использованием технологий Java"
  features:
    # feature loop
    - title: "Файлы водяных знаков через Java"
      content: "Защитите свои деловые документы с помощью GroupDocs.Watermark for Java. Добавляйте текст, изображения, диаграммы или вложения электронной почты в качестве водяных знаков к файлам различных форматов."

    # feature loop
    - title: "Настройка водяных знаков в соответствии с конкретными потребностями"
      content: "GroupDocs.Watermark for Java предлагает широкие возможности настройки водяных знаков. Настройте стили текста (полужирный шрифт, курсив, шрифт) и свойства изображения (поворот и т. д.), чтобы настроить процесс нанесения водяных знаков в соответствии с вашими конкретными целями."

    # feature loop
    - title: "Поддержка широкого формата"
      content: "GroupDocs.Watermark for Java легко интегрируется с широким спектром форматов файлов, включая: PDF, Microsoft Office (Word, Excel, PowerPoint), изображения (JPEG, PNG, GIF, BMP), Visio диаграммы и электронные письма. Повысьте безопасность документов различных типов файлов."

    # feature loop
    - title: "Простой поиск и управление водяными знаками"
      content: "Эффективно управляйте существующими водяными знаками в документах. Найдите определенные водяные знаки, измените их текст, стиль или изображения или полностью удалите их. GroupDocs.Watermark for Java упрощает рабочий процесс создания водяных знаков."

############################# Platforms ############################
platforms:
  enable: true
  title: "Независимость платформы"
  description: "GroupDocs.Watermark for Java поддерживает различные операционные системы и менеджеры пакетов."
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
  title: "Поддерживаемые форматы файлов"
  description: |
    GroupDocs.Watermark for Java позволяет обрабатывать широкий спектр форматов файлов. [См. полный список](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Java: Характеристики"
  description: "Защитите свои файлы, добавив водяные знаки. Поддерживает различные форматы, включая PDF, офисные документы и изображения."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Водяные знаки файлов"
      content: "Добавляйте или удаляйте водяные знаки из определенных разделов или целых документов для различных поддерживаемых форматов файлов."

    # feature loop
    - icon: "watermark_style"
      title: "Настройка водяных знаков"
      content: "Настройте внешний вид водяного знака с помощью таких параметров, как цвет, шрифт, поворот и многое другое."

    # feature loop
    - icon: "hidden_print"
      title: "Скрытый водяной знак для печати для PDF"
      content: "Добавьте водяной знак, который появляется только при печати документа PDF."

    # feature loop
    - icon: "image_only"
      title: "Выборочные водяные маркировки изображений"
      content: "Наносите водяные знаки на все изображения в определенном разделе, странице, слайде или во всем документе."

    # feature loop
    - icon: "image_frame"
      title: "Нанесение водяных знаков на определенные рамки изображений"
      content: "Применяйте водяные знаки к определенным кадрам многорамочного изображения."

    # feature loop
    - icon: "attachments"
      title: "Насадки и формы для нанесения водяных знаков"
      content: "Добавьте водяные знаки ко всем вложениям в Excel документах или ко всем фигурам изображений в презентациях."

    # feature loop
    - icon: "pdf_objects"
      title: "Выравнивание водяных знаков в PDF"
      content: "Совместите водяные знаки с различными областями документа PDF, включая Bleed Box, Art Box, Crop Box и Trim Box."

    # feature loop
    - icon: "doc_background"
      title: "Водяной знак на фоновых изображениях"
      content: "Добавьте или удалите водяной знак фонового изображения в электронных таблицах или презентациях."

    # feature loop
    - icon: "unreadable_characters"
      title: "Защита нечитаемыми символами"
      content: "Защитите презентации с помощью текстовых водяных знаков с нечитаемыми символами."

    # feature loop
    - icon: "watermark_text_search"
      title: "Поиск водяных знаков"
      content: "Получите список водяных знаков, представленных в файле, используя различные параметры, включая регулярные выражения."

    # feature loop
    - icon: "watermark_image_search"
      title: "Найдите похожие водяные знаки на изображениях"
      content: "Найдите водяные знаки на изображении, похожие на конкретное изображение."

    # feature loop
    - icon: "document_info"
      title: "Извлечь информацию о документе"
      content: "Получите различные данные документа, например настройку страницы для поддерживаемых форматов файлов."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Образцы кода"
  description: "Изучите примеры кода, иллюстрирующие типичные функции GroupDocs.Watermark for Java"
  items:
    # code sample loop
    - title: "Нанесение водяных знаков на документ с помощью изображения"
      content: |
        Используйте GroupDocs.Watermark for Java для повышения безопасности документов, добавляя водяные знаки изображений. Подробнее: [Водяные знаки на изображениях](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Как защитить файл водяным знаком изображения.">}}
        ```csharp {style=abap}
        // Загрузить исходный документ в Watermarker
        Watermarker watermarker = new Watermarker("document.pdf");
        
        // Укажите путь к изображению водяного знака
        ImageWatermark watermark = new ImageWatermark("watermark.jpg");

        // Защитите файл и сохраните его
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Изменить водяные знаки"
      content: |
        GroupDocs.Watermark for Java позволяет управлять существующими водяными знаками в документах. Найдите определенные водяные знаки и [измените их свойства](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Поиск и модификация водяных знаков.">}}
        ```csharp {style=abap}   
        // Загрузить исходный документ
        Watermarker watermarker = new Watermarker("document.pdf");

        // Поиск водяных знаков, подлежащих обновлению
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);                               
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);                             

        // Обновите нужные свойства
        for (PossibleWatermark watermark : watermarks)                                                           
        {  
            watermark.setText("New Text");
        }

        // Сохранить измененный документ по указанному пути
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
