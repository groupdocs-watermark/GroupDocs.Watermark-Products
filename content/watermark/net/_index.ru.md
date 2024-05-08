---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:29
draft: false

lang: ru
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
head_title: "C# .NET Программное обеспечение для водяных знаков для документов | добавить водяной знак"
head_description: "Библиотека C# .NET для добавления, поиска и удаления водяных знаков в документах: PDF, Word, Excel, презентации, Visio диаграммы, форматы файлов электронной почты и изображений."

############################# Header ############################
title: "Легко наносите водяные знаки на документы в приложениях на C# .NET"
description: "Расширьте возможности своих решений на C# с помощью гибкого API водяных знаков для документов, который позволяет добавлять настраиваемые водяные знаки во все популярные форматы документов."
words:
  for: "для"

actions:
  main: "Бесплатно NuGet Скачать"
  main_link: "https://www.nuget.org/packages/GroupDocs.Watermark"
  alt: "Лицензирование"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/net/"
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Watermark бесплатно или запросите лицензию"

release:
  title: "Выпущена версия {0}"
  notes: "Узнайте, что нового"
  downloads: "Загрузки"

code:
  title: "Файлы водяных знаков PDF в C#"
  more: "Больше примеров"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
  install: "dotnet add package GroupDocs.Watermark"
  content: |
    ```csharp {style=abap}   
    // Создайте экземпляр Watermarker, передающий путь PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    using (Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions))
    {
        // Настройте параметры водяных знаков
        TextWatermark textWatermark = 
            new TextWatermark("Approved", new Font("Arial", 8));
        
        // Применить водяной знак к документу PDF
        watermarker.Add(textWatermark);

        // Сохранить документ с результатами
        watermarker.Save("result.pdf");
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark с первого взгляда"
  description: "API для нанесения водяных знаков на документы через .NET"
  features:
    # feature loop
    - title: "Водяной знак файлов C#"
      content: "Добавьте водяные знаки в свои бизнес-файлы, используя GroupDocs.Watermark. Используйте текст, изображения, диаграммы или вложения электронной почты."

    # feature loop
    - title: "Настройте водяные знаки в соответствии со своими целями"
      content: "Программное обеспечение GroupDocs.Watermark for .NET позволяет настраивать водяные знаки различными способами. Стили текста, такие как полужирный шрифт, курсив, типы шрифтов, а также такие свойства изображения, как поворот и т. д., обогащают процесс нанесения водяных знаков."

    # feature loop
    - title: "Поддерживаются все популярные форматы файлов"
      content: "Решение GroupDocs.Watermark поддерживает множество форматов файлов и документов. PDF, Microsoft Office Word, Excel, PowerPoint, изображения, такие как диаграммы JPEG, PNG, GIF, BMP, Visio, электронные письма и т. д., можно защитить нашими водяными знаками."

    # feature loop
    - title: "Поиск и обновление водяных знаков"
      content: "Водяные знаки, которые уже представлены в документе, можно найти и снова обработать. Измените текст, стиль, изображения или удалите обнаруженные водяные знаки без дополнительных усилий."

############################# Platforms ############################
platforms:
  enable: true
  title: "Независимость платформы"
  description: "GroupDocs.Watermark for .NET поддерживает операционные системы, фреймворки и менеджеры пакетов, перечисленные ниже"
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
  title: "Поддерживаемые форматы файлов"
  description: |
    GroupDocs.Watermark for .NET обеспечивает обработку следующих [форматов файлов](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "Характеристики GroupDocs.Watermark"
  description: "Защитите PDF, Office, изображения и другие форматы водяным знаком"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Водяные знаки документов"
      content: "Добавьте или удалите водяные знаки из определенного раздела или всего документа различных форматов файлов."

    # feature loop
    - icon: "watermark_style"
      title: "Придайте своему водяному знаку стиль"
      content: "Настройте различные свойства водяных знаков, такие как цвет, шрифт, поворот и т. д."

    # feature loop
    - icon: "hidden_print"
      title: "PDF скрытый водяной знак для печати"
      content: "Присвойте скрытому водяному знаку PDF, который появляется только при печати документа."

    # feature loop
    - icon: "image_only"
      title: "Изображения в документах только водяными знаками"
      content: "Нанесите водяной знак на все изображения в определенном разделе, странице, слайде или документе."

    # feature loop
    - icon: "image_frame"
      title: "Обработать выбранные кадры изображения"
      content: "Присваивайте водяной знак только определенным кадрам многорамочного изображения."

    # feature loop
    - icon: "attachments"
      title: "Насадки и формы"
      content: "Установите водяной знак на все вложения в документе Excel и на все фигуры изображений на слайдах."

    # feature loop
    - icon: "pdf_objects"
      title: "PDF объектов"
      content: "Совместите водяной знак с коробкой Bleed Box, Art Box, Crop Box или Trim Box в документе PDF."

    # feature loop
    - icon: "doc_background"
      title: "Справочная информация о документах"
      content: "Поместите водяной знак или удалите его с фоновых изображений электронной таблицы или слайдов."

    # feature loop
    - icon: "unreadable_characters"
      title: "Защита от нечитаемых символов"
      content: "Защитите текстовый водяной знак с помощью нечитаемых символов в презентациях."

    # feature loop
    - icon: "watermark_text_search"
      title: "Поиск водяных знаков в документах"
      content: "Ищите водяные знаки на основе определенных параметров или комбинируя несколько критериев."

    # feature loop
    - icon: "watermark_image_search"
      title: "Искать похожие водяные знаки на изображениях"
      content: "Ищите водяные знаки на изображении, напоминающие конкретное изображение."

    # feature loop
    - icon: "document_info"
      title: "Получите информацию о документе"
      content: "Программно извлекайте настройки страницы и другую информацию о поддерживаемых форматах."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Образцы кода"
  description: "Некоторые варианты использования типичных операций GroupDocs.Watermark for .NET"
  items:
    # code sample loop
    - title: "Нанесите водяной знак, добавив изображение в документ."
      content: |
        Для защиты любого документа вы можете использовать [водяные знаки изображений](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/):
        {{< landing/code title="Как защитить файл водяным знаком изображения.">}}
        ```csharp {style=abap}
        // Загрузить исходный документ в Watermarker
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Укажите путь к изображению водяного знака
            using (ImageWatermark watermark = new ImageWatermark("watermark.jpg"))
            {
                // Защитите файл и сохраните его
                watermarker.Add(watermark);

                watermarker.Save("result.pdf");
            }
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Найдите и измените существующие водяные знаки."
      content: |
        GroupDocs.Watermark может [изменять водяные знаки](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/), которые уже представлены в документе. Найдите нужные элементы и обновите их свойства.
        {{< landing/code title="Поиск и модификация водяных знаков.">}}
        ```csharp {style=abap}   
        // Загрузить исходный документ
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Поиск водяных знаков, подлежащих обновлению
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                // Обновите нужные свойства
                watermark.Text = "New Text";
            }

            // Сохранить измененный документ по указанному пути
            watermarker.Save("document.pdf");
        }
        ```
        {{< /landing/code >}}

---
