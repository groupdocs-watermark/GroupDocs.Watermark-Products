
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:16
draft: false
lang: ru
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Редактирование водяных знаков в файлах Excel"
head_description: "С помощью GroupDocs.Watermark for Python via .NET вы можете настраивать параметры водяного знака для защиты и персонализации ваших документов."

############################# Header ############################
title: "Обновите водяные знаки в таблицах Excel с помощью Python" 
description: "Обеспечьте безопасность ваших электронных таблиц Excel с нашими гибкими инструментами редактирования водяных знаков для Python."
subtitle: "GroupDocs.Watermark for Python via .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Получите бесплатно на PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET Библиотека"
    link: "/watermark/python-net/"
    link_title: "Узнайте больше"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Быстро редактируйте водяные знаки Excel:** GroupDocs.Watermark for Python via .NET предоставляет разработчикам Python все инструменты, необходимые для управления водяными знаками с минимальными усилиями, улучшая рабочий процесс и безопасность ваших документов.

############################# Steps ############################
steps:
    enable: true
    title: "Измените водяные знаки в документах Excel с Python"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** помогает разработчикам Python обновлять водяные знаки в различных файлах Excel. Вот как вы можете использовать его в своём проекте:
      
      1. Сначала откройте ваш файл Excel, передав его в конструктор **Watermarker**. Вы можете использовать путь к файлу, байтовый поток или поток файла.
      2. Затем найдите водяные знаки, которые хотите изменить, с помощью **SearchCriteria**, который позволяет искать текст или свойства водяного знака.
      3. Как только водяной знак найден, вы можете изменить такие детали, как текст, шрифт, размер, положение, цвет и многое другое. Это даст вам полный контроль над внешним видом водяного знака.
      4. После внесения изменений сохраните документ. Вы можете записать результат в поток или по пути к файлу.
   
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
        # Обновите текст водяного знака в EXCEL
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Создайте Watermarker с использованием файла EXCEL
        with gw.Watermarker("input.xslx") as watermarker:

            # Настройте TextSearchCriteria для поиска текста водяного знака
            search_criteria = gwss.TextSearchCriteria("test", False)

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # Измените текст водяного знака
                        watermark.text = "passed"
                    except Exception as e:
                        pass
            
            watermarker.save("output.xslx")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Откройте для себя дополнительные способы обновления водяных знаков"
  description: "С нашей библиотекой приложения Python могут добавлять, находить, редактировать или удалять водяные знаки в различных типах файлов."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Редактирование водяных знаков"
  features:
    # feature loop
    - title: "Добавляйте водяные знаки в свои файлы"
      content: "Используйте GroupDocs.Watermark for Python via .NET для добавления и управления водяными знаками в ваших документах. Ищите, обновляйте или удаляйте водяные знаки по мере необходимости с помощью простого API."

    # feature loop
    - title: "Настройте водяные знаки под ваши нужды"
      content: "Настраивайте параметры водяного знака, такие как шрифт, размер, ориентация и цвет, с помощью нашего гибкого API, чтобы получить именно тот результат, который вы хотите."

    # feature loop
    - title: "Используйте специфические функции формата"
      content: "В зависимости от формата файла вы можете использовать нативные функции, такие как заголовки, нижние колонтитулы, аннотации или фоны в качестве областей для водяных знаков."
      
  code_samples:
    # code sample loop
    - title: "Редактирование текстового водяного знака в Excel"
      content: |
        Этот код показывает, как изменить текст водяного знака в электронных таблицах Excel.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # Откройте файл XLSX
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # Прочитайте данные электронной таблицы
        with gw.Watermarker("source.xlsx") as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,3]

            # Измените текст водяного знака
            watermarks = watermarker.search(search_criteria)
            for watermark in watermarks:
                try:
                    watermark.formatted_text_fragments.clear()
                    watermark.formatted_text_fragments.add(
                       "passed", 
                        gww.Font("Calibri", 19.0, gww.FontStyle.bold), 
                        gww.Color.red, 
                        gww.Color.aqua
                    )
                except Exception as e:
                    pass
        
            # Сохраните результат
            watermarker.save("output.xlsx")
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
    title: "Обновите водяные знаки в других форматах"
    exclude: "EXCEL"
    description: "Легко настраивайте параметры водяного знака для различных форматов файлов с помощью GroupDocs.Watermark for Python via .NET."
    items: 
        # format loop 1
        - name: "Водяной знак PDF"
          format: "PDF"
          link: "/watermark/python-net/edit//pdf/"
          description: "Формат документа Adobe Portable"

        # format loop 2
        - name: "Водяной знак Word"
          format: "WORD"
          link: "/watermark/python-net/edit//word/"
          description: "MS Word и документы Open Office"
          
        # format loop 3
        - name: "Водяной знак Excel"
          format: "EXCEL"
          link: "/watermark/python-net/edit//excel/"
          description: "MS Excel и электронные таблицы Open Office"

        # format loop 4
        - name: "Водяной знак PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/edit//powerpoint/"
          description: "MS PowerPoint и презентации в открытом офисе"

        # format loop 5
        - name: "Водяной знак DOCX"
          format: "DOCX"
          link: "/watermark/python-net/edit//docx/"
          description: "Открыть XML-документ Microsoft Word"
          
        # format loop 6
        - name: "Водяной знак PPTX"
          format: "PPTX"
          link: "/watermark/python-net/edit//pptx/"
          description: "PowerPoint Открытая презентация XML"
          
        # format loop 7
        - name: "Водяной знак XLSX"
          format: "XLSX"
          link: "/watermark/python-net/edit//xlsx/"
          description: "Открытая электронная таблица XML от Майкрософт Excel"

        # format loop 8
        - name: "Водяной знак DOC"
          format: "DOC"
          link: "/watermark/python-net/edit//doc/"
          description: "Документ Майкрософт Word 97—2007"

        # format loop 9
        - name: "Водяной знак XLS"
          format: "XLS"
          link: "/watermark/python-net/edit//xls/"
          description: "Рабочая тетрадь Майкрософт Excel 97-2003"

        # format loop 10
        - name: "Водяной знак PPT"
          format: "PPT"
          link: "/watermark/python-net/edit//ppt/"
          description: "PowerPoint Презентация 97-2003"

        # format loop 11
        - name: "Водяной знак RTF"
          format: "RTF"
          link: "/watermark/python-net/edit//rtf/"
          description: "Форматированный текстовый формат"

---