
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:58
draft: false
lang: ru
format: Photo
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Быстро и легко наносите водяные знаки на ваши фотографии"
head_description: "Быстро защитите свои фотографии и защитите их авторские права с помощью .NET водяных знаков C#. Начните защищать свою работу уже сегодня."

############################# Header ############################
title: "Быстрое и простое нанесение водяных знаков на фотографии с помощью .NET" 
description: "Наша мощная библиотека C# позволяет быстро наносить водяные знаки на ваши фотографии, защищая авторские права и повышая узнаваемость бренда без ущерба для качества изображения."
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачайте бесплатно на Nuget"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "Узнайте больше"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET предлагает мощное решение для служб фотографов, стремящихся защитить свои авторские права и фирменный стиль. Этот API позволяет быстро добавлять текстовые или графические водяные знаки к фотографиям в различных форматах, включая JPEG, PNG и RAW. Настройте водяные знаки так, чтобы их прозрачность, размер и положение идеально сочетались с фотографией, сохраняя эстетическое качество, отстаивая свои законные права и предотвращая несанкционированное использование.

############################# Steps ############################
steps:
    enable: true
    title: "Улучшите свои документы: создайте водяные знаки для Photo с помощью .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** — библиотека, которая упрощает добавление водяных знаков в различные форматы бизнес-файлов для .NET разработчиков. Интегрируйте нашу библиотеку в свое приложение и легко наносите водяные знаки на документы, выполнив следующие действия:
      
      1. **Начните свой путь к созданию водяных знаков:** Начните с знакомства с классом **Watermarker**, краеугольным камнем нашего API. Чтобы начать процесс, обязательно создайте его экземпляр до начала обработки документа. Не упускайте из виду важность предоставления конструктору файла Photo, будь то путь или объект потока.
      2. **Создание специальных водяных знаков:** Перейдите к следующему этапу, создав объект **Watermark**, соответствующий вашим спецификациям. Этот универсальный инструмент не ограничивается определенными страницами документов; его также можно легко интегрировать в исходные элементы документа, такие как вложения или заголовки.
      3. **Точная настройка атрибутов водяных знаков:** Усовершенствуйте интерфейс водяных знаков, настроив такие свойства, как высота, ширина, выравнивание страницы, семейство шрифтов и цвет. Такой уровень настройки гарантирует, что водяные знаки идеально сочетаются с документами.
      4. **Нанесение водяных знаков:** Используйте метод **Watermarker**, чтобы легко наносить собственные водяные знаки на документы. Независимо от того, нужно ли вам добавить один или несколько водяных знаков, этот процесс обеспечивает гибкость. Для дополнительной безопасности рассмотрите возможность хранения обработанных документов в отдельном месте.
   
    code:
      platform: "net"
      copy_title: "Копировать"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "нажмите, чтобы скопировать"
        copy_done: "скопировал"
      links:
        #  loop
        - title: "Больше примеров"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "Документация"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // Сгенерировать текстовый водяной знак в файле PHOTO

        // Укажите файл для нанесения водяного знака
        using (Watermarker watermarker = new Watermarker("input.png"))
        {
            // Создать экземпляр текстового водяного знака
            Font font = new Font("Arial", 19, FontStyle.Bold | FontStyle.Italic);
            TextWatermark watermark = new TextWatermark("my watermark", font);
            watermark.ForegroundColor = Color.Red;
            watermark.BackgroundColor = Color.Blue;
            watermarker.Add(watermark);

            // Сохранить результат PHOTO
            watermarker.Save("output.png");
        }
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Глубокое погружение в добавление водяных знаков"
  description: "Используйте наш мощный API для визуализации, отображения, преобразования и управления документами, слайдами, диаграммами и другими типами документов в приложениях .NET. GroupDocs.Watermark легко интегрирует возможности водяных знаков для повышения безопасности документов и защиты авторских прав."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Добавить водяной знак"
  features:
    # feature loop
    - title: "Легко наносите водяные знаки на ваши документы."
      content: "GroupDocs.Watermark позволяет разработчикам .NET легко интегрировать водяные знаки в свои приложения. Без труда добавляйте текстовые, графические или динамические водяные знаки в популярные деловые документы и файлы, гарантируя безопасность контента и одинаковую фирменную символику на всех платформах."

    # feature loop
    - title: "Настройте водяные знаки в соответствии со своими потребностями."
      content: "Настройте водяные знаки в соответствии со своими конкретными требованиями с помощью расширенных функций, поддерживаемых GroupDocs.Watermark. Отрегулируйте размер, угол поворота, прозрачность, цвет и шрифт, чтобы водяной знак не только выглядел идеально, но и повысил безопасность документов без потери важной информации."

    # feature loop
    - title: "Используйте встроенные функции документов для нанесения водяных знаков"
      content: "Используйте неотъемлемые особенности форматов документов для создания сложных водяных знаков. Будь то использование оригинальных аннотаций PDF, фона MS Word или верхних и нижних колонтитулов Excel, GroupDocs.Watermark глубоко интегрируется со структурами документов, позволяя наносить водяные знаки одновременно эффективно и минимально инвазивно."
      
  code_samples:
    # code sample loop
    - title: "Сгенерировать водяной знак изображения для DOCX"
      content: |
        В этом примере показано, как применять эффекты изображения к водяным знакам фигуры.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Загрузить документ Word
            var loadOptions = new WordProcessingLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.docx", loadOptions))
            {
                //  Настройка параметров водяных знаков
                using (ImageWatermark watermark = new ImageWatermark("logo.png"))
                {
                    WordProcessingImageEffects effects = new WordProcessingImageEffects();
                    effects.Brightness = 0.7;
                    effects.Contrast = 0.6;
                    effects.ChromaKey = Color.Red;
                    effects.BorderLineFormat.Enabled = true;
                    effects.BorderLineFormat.Weight = 1;

                    WordProcessingWatermarkSectionOptions options = new WordProcessingWatermarkSectionOptions();
                    options.Effects = effects;

                    //  Сгенерировать водяной знак
                    watermarker.Add(watermark, options);
                }

                //  Сохранить обновленный документ
                watermarker.save("result.docx");
            }

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Watermark бесплатно или запросите лицензию"
  items:
    #  loop
    - title: "Nuget скачать"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "Лицензирование"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Защитите свои фотографии с помощью эффективных водяных знаков C#"
    exclude: "PHOTO"
    description: "Защитите и стилизуйте свой фотографический контент с помощью настраиваемых водяных знаков с помощью нашего API .NET C#, разработанного для беспрепятственной интеграции и сохранения качества изображения."
    items: 
        # format loop 1
        - name: "Водяной знак PDF"
          format: "PDF"
          link: "/watermark/net/generate//pdf/"
          description: "Формат документа Adobe Portable"

        # format loop 2
        - name: "Водяной знак Word"
          format: "WORD"
          link: "/watermark/net/generate//word/"
          description: "MS Word и документы Open Office"
          
        # format loop 3
        - name: "Водяной знак Excel"
          format: "EXCEL"
          link: "/watermark/net/generate//excel/"
          description: "MS Excel и электронные таблицы Open Office"

        # format loop 4
        - name: "Изображение водяного знака"
          format: "IMAGE"
          link: "/watermark/net/generate//image/"
          description: "Популярные форматы изображений"

        # format loop 5
        - name: "Фото водяного знака"
          format: "PHOTO"
          link: "/watermark/net/generate//photo/"
          description: "Форматы фотографий"

        # format loop 6
        - name: "Водяной знак PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/generate//powerpoint/"
          description: "MS PowerPoint и презентации в открытом офисе"

        # format loop 7
        - name: "Водяной знак DOCX"
          format: "DOCX"
          link: "/watermark/net/generate//docx/"
          description: "Открыть XML-документ Microsoft Word"
          
        # format loop 8
        - name: "Водяной знак PPTX"
          format: "PPTX"
          link: "/watermark/net/generate//pptx/"
          description: "PowerPoint Открытая презентация XML"
          
        # format loop 9
        - name: "Водяной знак XLSX"
          format: "XLSX"
          link: "/watermark/net/generate//xlsx/"
          description: "Открытая электронная таблица XML от Майкрософт Excel"

        # format loop 10
        - name: "Водяной знак JPEG"
          format: "JPEG"
          link: "/watermark/net/generate//jpeg/"
          description: "JPEG Изображение"

        # format loop 11
        - name: "Водяной знак PNG"
          format: "PNG"
          link: "/watermark/net/generate//png/"
          description: "Portable Сетевая графика"

        # format loop 12
        - name: "Водяной знак TIFF"
          format: "TIFF"
          link: "/watermark/net/generate//tiff/"
          description: "Формат файла изображения тега"

        # format loop 13
        - name: "Водяной знак WEBP"
          format: "WEBP"
          link: "/watermark/net/generate//webp/"
          description: "Изображение в Интернете"

        # format loop 14
        - name: "Водяной знак DOC"
          format: "DOC"
          link: "/watermark/net/generate//doc/"
          description: "Документ Майкрософт Word 97—2007"

        # format loop 15
        - name: "Водяной знак XLS"
          format: "XLS"
          link: "/watermark/net/generate//xls/"
          description: "Рабочая тетрадь Майкрософт Excel 97-2003"

        # format loop 16
        - name: "Водяной знак PPT"
          format: "PPT"
          link: "/watermark/net/generate//ppt/"
          description: "PowerPoint Презентация 97-2003"

        # format loop 17
        - name: "Водяной знак RTF"
          format: "RTF"
          link: "/watermark/net/generate//rtf/"
          description: "Форматированный текстовый формат"

---