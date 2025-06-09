
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:16
draft: false
lang: uk
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Редагуйте водяні знаки у файлах Powerpoint"
head_description: "Використовуйте GroupDocs.Watermark for Python via .NET для швидкої зміни вмісту водяних знаків у презентаціях Powerpoint та захисту ваших документів."

############################# Header ############################
title: "Точне редагування водяних знаків Powerpoint у Python" 
description: "Отримайте повний контроль над макетом і видимістю водяних знаків у ваших презентаціях за допомогою GroupDocs.Watermark for Python via .NET."
subtitle: "GroupDocs.Watermark for Python via .NET Бібліотека" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Безкоштовне завантаження з PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET API"
    link: "/watermark/python-net/"
    link_title: "Дізнатися більше"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Контролюйте макет водяних знаків у файлах Powerpoint:** Завдяки GroupDocs.Watermark for Python via .NET ви можете розмістити водяні знаки точно там, де це потрібно, і легко захистити свої презентації.

############################# Steps ############################
steps:
    enable: true
    title: "Змінюйте водяні знаки у документах Powerpoint за допомогою Python"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** допомагає розробникам Python оновлювати водяні знаки у різних файлах Powerpoint. Ось як ви можете використовувати його у своєму проекті:
      
      1. Спочатку відкрийте файл Powerpoint, передавши його конструктору **Watermarker**. Ви можете використовувати шлях до файлу, байтовий потік або потік файлу.
      2. Потім знайдіть водяні знаки, які потрібно змінити, використовуючи **SearchCriteria**, що дозволяє шукати текст або властивості водяного знака.
      3. Після знаходження ви можете змінити такі деталі, як текст, шрифт, розмір, положення, колір та інше. Це дає вам повний контроль над зовнішнім виглядом водяного знака.
      4. Після внесення змін збережіть документ. Ви можете записати результат у потік або за допомогою шляху до файлу.
   
    code:
      platform: "python-net"
      copy_title: "Копіювати"
      install:
        command: |
        command: "pip install groupdocs-watermark-net"
        copy_tip: "натисніть, щоб скопіювати"
        copy_done: "скопійовано"
      links:
        #  loop
        - title: "Більше прикладів"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
        #  loop
        - title: "Документація"
          link: "https://docs.groupdocs.com/watermark/python-net/"
          
      content: |
        ```python {style=abap}
        # Оновіть текст водяного знака у POWERPOINT
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Створіть Watermarker за допомогою файлу POWERPOINT
        with gw.Watermarker("input.pptx") as watermarker:

            # Налаштуйте TextSearchCriteria для пошуку тексту водяного знака
            search_criteria = gwss.TextSearchCriteria("test", False)

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # Змініть текст водяного знака
                        watermark.text = "passed"
                    except Exception as e:
                        pass
            
            watermarker.save("output.pptx")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Відкрийте більше можливостей для оновлення водяних знаків"
  description: "З нашою бібліотекою програми Python можуть додавати, знаходити, редагувати або видаляти водяні знаки у багатьох типах файлів."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Редагування водяних знаків"
  features:
    # feature loop
    - title: "Водяні знаки ваших файлів без проблем"
      content: "Використовуйте GroupDocs.Watermark for Python via .NET для додавання та управління водяними знаками у ваших документах. Шукайте, оновлюйте або видаляйте водяні знаки за потреби, використовуючи простий API."

    # feature loop
    - title: "Налаштуйте водяні знаки відповідно до ваших потреб"
      content: "Коригуйте налаштування водяних знаків, такі як шрифт, розмір, орієнтація та колір, використовуючи наш гнучкий API, щоб отримати точний результат, який ви хочете."

    # feature loop
    - title: "Використовуйте особливості, специфічні для форматів"
      content: "В залежності від формату файлу, ви можете використовувати рідні функції, такі як заголовки, колонтитули, анотації або фонові області як зони для водяних знаків."
      
  code_samples:
    # code sample loop
    - title: "Редагування текстового водяного знака в Excel"
      content: |
        Цей код демонструє, як змінити текст водяного знака в таблицях Excel.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # Відкрийте файл XLSX
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # Прочитайте дані таблиці
        with gw.Watermarker("source.xlsx") as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,3]

            # Змініть текст водяного знака
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
        
            # Збережіть результат
            watermarker.save("output.xlsx")
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Готові розпочати роботу?"
  description: "Спробуйте GroupDocs.Watermark функцій безкоштовно або попросіть ліцензію"
  items:
    #  loop
    - title: "PyPi завантажити"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      color: "red"
        #  loop
    - title: "Ліцензування"
      link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Редагуйте водяні знаки в інших типах файлів"
    exclude: "POWERPOINT"
    description: "Використовуйте GroupDocs.Watermark for Python via .NET для роботи з водяними знаками у різних форматах документів."
    items: 
        # format loop 1
        - name: "Водяний знак PDF"
          format: "PDF"
          link: "/watermark/python-net/edit//pdf/"
          description: "Adobe Portable Формат документа"

        # format loop 2
        - name: "Водяний знак Word"
          format: "WORD"
          link: "/watermark/python-net/edit//word/"
          description: "MS Word та документи Відкритого офісу"
          
        # format loop 3
        - name: "Водяний знак Excel"
          format: "EXCEL"
          link: "/watermark/python-net/edit//excel/"
          description: "MS Excel та електронні таблиці Open Office"

        # format loop 4
        - name: "Водяний знак PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/edit//powerpoint/"
          description: "MS PowerPoint та презентації з відкритим офісом"

        # format loop 5
        - name: "Водяний знак DOCX"
          format: "DOCX"
          link: "/watermark/python-net/edit//docx/"
          description: "Майкрософт Word Відкритий документ XML"
          
        # format loop 6
        - name: "Водяний знак PPTX"
          format: "PPTX"
          link: "/watermark/python-net/edit//pptx/"
          description: "PowerPoint Відкрита презентація XML"
          
        # format loop 7
        - name: "Водяний знак XLSX"
          format: "XLSX"
          link: "/watermark/python-net/edit//xlsx/"
          description: "Microsoft Excel Відкрита таблиця XML"

        # format loop 8
        - name: "Водяний знак DOC"
          format: "DOC"
          link: "/watermark/python-net/edit//doc/"
          description: "Майкрософт Word 97 - Документ 2007 року"

        # format loop 9
        - name: "Водяний знак XLS"
          format: "XLS"
          link: "/watermark/python-net/edit//xls/"
          description: "Майкрософт Excel Книга 97-2003"

        # format loop 10
        - name: "Водяний знак PPT"
          format: "PPT"
          link: "/watermark/python-net/edit//ppt/"
          description: "PowerPoint Презентація 97-2003"

        # format loop 11
        - name: "Водяний знак RTF"
          format: "RTF"
          link: "/watermark/python-net/edit//rtf/"
          description: "Формат багатого тексту"

---