
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: ru
format: Image
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Добавляйте водяные знаки на изображения с Python"
head_description: "Узнайте, как добавлять водяные знаки на изображения в Python. Защитите ваши фотографии без потери качества."

############################# Header ############################
title: "Быстрое добавление водяных знаков на изображения с Python" 
description: "Наш инструмент Python позволяет быстро добавлять водяные знаки на изображения. Поддерживаются различные форматы, от фотографий до цифрового искусства."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачайте PyPi бесплатно"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "Узнайте больше"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET помогает добавлять водяные знаки к изображениям на Python. Он поддерживает JPEG, PNG, BMP, TIFF и другие форматы. Вы можете изменить прозрачность, размер и положение водяного знака в соответствии с вашими потребностями. Используйте его для защиты ваших изображений или добавления брендинга, сохраняя оригинальное качество.

############################# Steps ############################
steps:
    enable: true
    title: "Добавление водяных знаков: Python Водяное знаку для Image"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** это библиотека, которая позволяет быстро добавлять водяные знаки к различным типам бизнес-файлов. Следуйте этим шагам, чтобы быстро добавить водяные знаки к вашим документам на Python:
      
      1. **Начните с водяных знаков:** Начните с создания экземпляра класса **Watermarker**. Передайте ваш файл Image (в виде пути или потока) в конструктор, чтобы открыть его для добавления водяного знака.
      2. **Создайте свой водяной знак:** Создайте объект **Watermark** с вашим текстом и настройками. Вы можете добавлять водяные знаки на любую страницу или даже к элементам документа, таким как заголовки или вложения.
      3. **Настройте водяной знак:** Измените размер, положение, шрифт, цвет и выравнивание водяного знака в соответствии с вашими потребностями. Это поможет вашему водяному знаку выглядеть оптимально в документе.
      4. **Примените и сохраните:** Используйте метод **Watermarker**, чтобы добавить ваш(и) водяной знак(и) в документ. Сохраните результат, лучше в новый файл для безопасности.
   
    code:
      platform: "python-net"
      copy_title: "Копировать"
      install:
        command: |
        command: "pip install groupdocs-watermark-net"
        copy_tip: "нажмите, чтобы скопировать"
        copy_done: "скопировал"
      links:
        #  loop
        - title: "Больше примеров"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
        #  loop
        - title: "Документация"
          link: "https://docs.groupdocs.com/watermark/python-net/"
          
      content: |
        ```python {style=abap}
        # Добавьте текстовый водяной знак в файл IMAGE
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # Выберите файл, который вы хотите заверить водяным знаком
        with gw.Watermarker("input.jpeg") as watermarker:

            # Создайте объект текстового водяного знака
            font = gww.Font("Arial", 36.0)
            watermark = gww.TextWatermark("top secret", font)
            watermark.foreground_color = gww.Color.red
            watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
            watermark.opacity = 0.4

            watermarker.add(watermark)

            # Сохраните обновленный файл IMAGE
            watermarker.save("output.jpeg")
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Изучите больше возможностей добавления водяных знаков"
  description: "Используйте наш API Python для добавления, просмотра, преобразования и управления водяными знаками в документах, слайдах, диаграммах и многом другом. GroupDocs.Watermark for Python via .NET помогает защитить ваши файлы и добавить информацию о авторских правах без усилий."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Добавить водяной знак"
  features:
    # feature loop
    - title: "Легкое добавление водяных знаков"
      content: "GroupDocs.Watermark позволяет разработчикам Python быстро добавлять текстовые, графические или динамические водяные знаки в бизнес-документы. Защищайте свои файлы и сохраняйте брендинг с минимальными усилиями."

    # feature loop
    - title: "Полная настраиваемость водяных знаков"
      content: "Изменяйте размер водяного знака, угол поворота, прозрачность, цвет и шрифт с помощью GroupDocs.Watermark. Настройте ваш водяной знак так, чтобы он идеально вписывался в документ и отражал важный контент."

    # feature loop
    - title: "Используйте функции документа для добавления водяных знаков"
      content: "Используйте встроенные функции документа, такие как аннотации PDF, фоны Word или заголовки Excel для добавления водяных знаков. GroupDocs.Watermark работает со структурами документа для эффективного и ненавязчивого добавления водяных знаков."
      
  code_samples:
    # code sample loop
    - title: "Добавьте изображение водяного знака в DOCX"
      content: |
        Этот пример показывает, как применить эффекты изображения к водяным знаком в форме.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.wordprocessing as gwow

        # Откройте документ Word
        load_options = gwow.WordProcessingLoadOptions()
        with gw.Watermarker("source.docx", load_options) as watermarker:

            # Настройте параметры водяного знака
            with gww.ImageWatermark("logo.png") as watermark:

                effects = gwow.WordProcessingImageEffects()
                effects.brightness = 0.7
                effects.contrast = 0.6
                effects.chroma_key = gww.Color.red

                options = gwow.WordProcessingWatermarkSectionOptions()
                options.Effects = effects;

                # Создайте водяной знак
                watermarker.add(watermark, options)

                # Сохраните документ с водяным знаком
                watermarker.save("result.docx")
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Watermark бесплатно или запросите лицензию"
  items:
    #  loop
    - title: "PyPi скачать"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      color: "red"
        #  loop
    - title: "Лицензирование"
      link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Добавьте водяные знаки на изображения с Python"
    exclude: "IMAGE"
    description: "Защитите ваши изображения с помощью нашего набора инструментов Python. Быстро и просто добавляйте водяные знаки к множеству форматов изображений."
    items: 
        # format loop 1
        - name: "Водяной знак PDF"
          format: "PDF"
          link: "/watermark/python-net/add//pdf/"
          description: "Формат документа Adobe Portable"

        # format loop 2
        - name: "Водяной знак Word"
          format: "WORD"
          link: "/watermark/python-net/add//word/"
          description: "MS Word и документы Open Office"
          
        # format loop 3
        - name: "Водяной знак Excel"
          format: "EXCEL"
          link: "/watermark/python-net/add//excel/"
          description: "MS Excel и электронные таблицы Open Office"

        # format loop 4
        - name: "Изображение водяного знака"
          format: "IMAGE"
          link: "/watermark/python-net/add//image/"
          description: "Популярные форматы изображений"

        # format loop 5
        - name: "Фото водяного знака"
          format: "PHOTO"
          link: "/watermark/python-net/add//photo/"
          description: "Форматы фотографий"

        # format loop 6
        - name: "Водяной знак PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/add//powerpoint/"
          description: "MS PowerPoint и презентации в открытом офисе"

        # format loop 7
        - name: "Водяной знак DOCX"
          format: "DOCX"
          link: "/watermark/python-net/add//docx/"
          description: "Открыть XML-документ Microsoft Word"
          
        # format loop 8
        - name: "Водяной знак PPTX"
          format: "PPTX"
          link: "/watermark/python-net/add//pptx/"
          description: "PowerPoint Открытая презентация XML"
          
        # format loop 9
        - name: "Водяной знак XLSX"
          format: "XLSX"
          link: "/watermark/python-net/add//xlsx/"
          description: "Открытая электронная таблица XML от Майкрософт Excel"

        # format loop 10
        - name: "Водяной знак JPEG"
          format: "JPEG"
          link: "/watermark/python-net/add//jpeg/"
          description: "JPEG Изображение"

        # format loop 11
        - name: "Водяной знак PNG"
          format: "PNG"
          link: "/watermark/python-net/add//png/"
          description: "Portable Сетевая графика"

        # format loop 12
        - name: "Водяной знак TIFF"
          format: "TIFF"
          link: "/watermark/python-net/add//tiff/"
          description: "Формат файла изображения тега"

        # format loop 13
        - name: "Водяной знак WEBP"
          format: "WEBP"
          link: "/watermark/python-net/add//webp/"
          description: "Изображение в Интернете"

        # format loop 14
        - name: "Водяной знак DOC"
          format: "DOC"
          link: "/watermark/python-net/add//doc/"
          description: "Документ Майкрософт Word 97—2007"

        # format loop 15
        - name: "Водяной знак XLS"
          format: "XLS"
          link: "/watermark/python-net/add//xls/"
          description: "Рабочая тетрадь Майкрософт Excel 97-2003"

        # format loop 16
        - name: "Водяной знак PPT"
          format: "PPT"
          link: "/watermark/python-net/add//ppt/"
          description: "PowerPoint Презентация 97-2003"

        # format loop 17
        - name: "Водяной знак RTF"
          format: "RTF"
          link: "/watermark/python-net/add//rtf/"
          description: "Форматированный текстовый формат"

---