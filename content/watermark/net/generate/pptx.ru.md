
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:38
draft: false
lang: ru
format: Pptx
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Встраивайте водяные знаки в PPTX с помощью C#"
head_description: "Защитите свои PPTX презентации с помощью .NET водяных знаков, нанесенных на C#, и защитите интеллектуальную собственность."

############################# Header ############################
title: "Расширенные водяные знаки в C# для PPTX" 
description: "Внедрите .NET C# для создания надежных водяных знаков в PPTX файлах, что идеально подходит для повышения безопасности корпоративных и образовательных презентаций."
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
       GroupDocs.Watermark for .NET предоставляет комплексное решение на языке C# на .NET для нанесения водяных знаков на файлы PPTX, подходящее для профессионалов, которым требуется защита презентационных материалов. Этот API поддерживает интеграцию настраиваемых водяных знаков, которые могут включать текст, логотипы или другую графику. Он предлагает такие функции, как регулировка прозрачности, размера и позиционирования, благодаря чему водяные знаки могут быть одновременно эффективными и незаметными. GroupDocs.Watermark идеально подходит для компаний, преподавателей и всех, кто предоставляет конфиденциальную или конфиденциальную информацию. Она обеспечивает не только безопасность ваших презентаций, но и их эстетическое качество. Этот инструмент, совместимый с версиями .NET 5 и выше, обеспечивает надежную поддержку современных сред Microsoft Office.

############################# Steps ############################
steps:
    enable: true
    title: "Легко создавайте водяные знаки для документов Pptx"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/):** Расширенная библиотека водяных знаков для приложений .NET. Расширьте возможности своего решения и защитите документы водяными знаками вовремя.
      
      1. **Основной класс: Watermarker.** Основной класс нашего API — **Watermarker**. Вам необходимо создать его экземпляр перед обработкой документа. Не забудьте передать файл Pptx конструктору как путь или объект потока.
      2. **Создание водяного знака.** Следующим шагом является создание объекта водяного знака нужного типа. Его можно разместить не только на конкретной странице документа, но и в его собственных частях, таких как изображения или заголовки.
      3. **Точная настройка внешнего вида.** Установите такие свойства водяного знака, как высота и ширина, сверху, слева, выравнивание по центру, шрифты и цвета и т. д.
      4. **Применение и сохранение.** Используйте метод **Watermarker**, чтобы добавить новый водяной знак. Не стесняйтесь добавлять столько водяных знаков, сколько вам нужно. Вы можете сохранить документ с водяным знаком в любом месте.
   
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
        // Создать водяной знак изображения в файле PPTX

        // Укажите путь к исходному файлу конструктору Watermarker.
        using (Watermarker watermarker = new Watermarker("input.pptx"))
        {
            // Создать экземпляр водяного знака изображения с помощью файла изображения
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // Сохранить результат PPTX с водяным знаком
            watermarker.Save("output.pptx");
        }
        
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "Улучшите свою игру с водяными знаками"
  description: "Откройте для себя расширенные возможности создания водяных знаков с помощью нашего API GroupDocs.Watermark для .NET. Этот мощный инструмент позволяет точно настраивать и наносить водяные знаки на различные типы документов, обеспечивая максимальную безопасность и соблюдение авторских прав при минимальном нарушении визуального восприятия."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Комплексные решения по нанесению водяных знаков"
  features:
    # feature loop
    - title: "Сложные варианты укладки плитки"
      content: "С помощью наших опций для нанесения водяных знаков на все документы можно легко наносить водяные знаки на все документы. Эта функция позволяет водяным знакам покрывать всю область документа, предотвращая их удаление и обеспечивая полную защиту документов без ущерба для дизайна или удобочитаемости."

    # feature loop
    - title: "Яркая настройка цвета"
      content: "Добавьте ярких красок своим водяным знакам! Наш API позволяет настраивать полный спектр цветов, позволяя наносить водяные знаки, идеально соответствующие вашему корпоративному бренду или стилю документа. Повысьте визуальную привлекательность, сохранив при этом надежные функции безопасности."

    # feature loop
    - title: "Расширенные настройки безопасности"
      content: "Поднимите безопасность документов на новый уровень с помощью расширенных настроек водяных знаков. Настройте многослойные водяные знаки, включающие как видимые, так и невидимые элементы, для защиты от несанкционированного копирования и обеспечения доступа к важной информации только предполагаемым получателям."
      
  code_samples:
    # code sample loop
    - title: "Сгенерировать водяной знак PowerPoint"
      content: |
        В этом примере показано, как добавить водяной знак к фоновым изображениям PPTX
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Загрузить презентацию PPTX
            var loadOptions = new PresentationLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pptx", loadOptions))
            {
                //  Настройка свойств водяного знака
                TextWatermark watermark = new TextWatermark("Protected image", new Font("Arial", 8));
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermark.RotateAngle = 45;
                watermark.SizingType = SizingType.ScaleToParentDimensions;
                watermark.ScaleFactor = 1;

                //  Фон слайдов с водяными знаками
                PresentationContent content = watermarker.GetContent<PresentationContent>();
                foreach (PresentationSlide slide in content.Slides)
                {
                    if (slide.ImageFillFormat.BackgroundImage != null)
                    {
                        slide.ImageFillFormat.BackgroundImage.Add(watermark);
                    }
                }

                //  Сохранить обработанную презентацию
                watermarker.save("result.pptx");
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
    title: "Решения C# Watermark для PPTX файлов"
    exclude: "PPTX"
    description: "Используйте .NET C# для нанесения дискретных водяных знаков в PPTX файлах, защищая презентации от несанкционированного распространения."
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