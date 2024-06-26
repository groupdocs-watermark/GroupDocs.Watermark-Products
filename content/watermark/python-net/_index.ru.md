---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:49
draft: false

lang: ru
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

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
    # supported_platforms loop
    - title: "Python"
      tag: "python-net"

############################# Head ############################
head_title: "Python Библиотека водяных знаков | Водяные знаки документов"
head_description: "Python защищает деловые документы текстовыми и графическими водяными знаками. Поддерживаются такие форматы файлов, как PDF, Word, Excel и PowerPoint."

############################# Header ############################
title: "Доступ к технологии создания водяных знаков Python via .NET"
description: "Защитите свои данные и предотвратите несанкционированное копирование с помощью этого решения Python. Легко добавляйте водяные знаки в деловые документы в различных форматах, включая PDF, Word, Excel, PowerPoint, изображения и т. д."
words:
  for: "для"

actions:
  main: "PyPi скачать бесплатно"
  main_link: "https://pypi.org/project/groupdocs-watermark-net/"
  alt: "Лицензирование"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Watermark бесплатно или запросите лицензию"

release:
  title: "Выпущена версия {0}"
  notes: "Узнайте, что нового"
  downloads: "Загрузки"
  link: "https://releases.groupdocs.com/watermark/python-net/"

code:
  title: "Добавьте водяной знак в PDF с помощью Python"
  more: "Больше примеров"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
  install: "pip install groupdocs-watermark-net"
  content: |
    ```python {style=abap}

    import groupdocs.watermark as gw
    import groupdocs.watermark.watermarks as gww
    import groupdocs.watermark.options.pdf as gwop
    import groupdocs.watermark.common as gwc

    # Создайте экземпляр Watermarker, передающий путь PDF
    pdf_lo = gwop.PdfLoadOptions()
    with gw.Watermarker("source.pdf", pdf_lo) as watermarker:
        options = gwop.PdfArtifactWatermarkOptions()

        # Настройте параметры водяных знаков
        text_watermark = 
            gww.TextWatermark("Approved", gww.Font("Arial", 8.0))
        text_watermark.horizontal_alignment = 
            gwc.HorizontalAlignment.RIGHT

        # Применить водяной знак к документу PDF
        watermarker.add(text_watermark, options)

        # Сохранить документ с результатами
        watermarker.save("result.pdf")

    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark с первого взгляда"
  description: "Python Библиотека для водяных знаков"
  features:
    # feature loop
    - title: "Python Водяной знак документа"
      content: "Защитите свои конфиденциальные данные с помощью GroupDocs.Watermark for Python via .NET. Помещайте текст или изображения в файлы различных форматов в виде водяных знаков."

    # feature loop
    - title: "Настройте водяные знаки"
      content: "В GroupDocs.Watermark for Python via .NET доступно множество вариантов настройки. Настройте стили текста (жирный, курсив, шрифт) или свойства изображения, такие как размер или поворот, чтобы настроить водяные знаки в документе."

    # feature loop
    - title: "Поддержка популярных форматов файлов"
      content: "GroupDocs.Watermark for Python via .NET поддерживает широкий спектр форматов файлов, включая PDF, документы MS Office, такие как Word, Excel, PowerPoint, а также изображения, такие как JPEG, PNG, GIF, BMP, диаграммы Visio, электронные письма и т. д. Улучшите обработку документов для удовлетворения потребностей бизнеса. цели."

    # feature loop
    - title: "Поиск и обновление водяных знаков"
      content: "Извлекайте и обновляйте водяные знаки, размещенные в документах. Измените стиль текста, содержимое изображения или полностью удалите их. GroupDocs.Watermark for Python via .NET предлагает широкий спектр возможностей обработки водяных знаков."

############################# Platforms ############################
platforms:
  enable: true
  title: "Независимость платформы"
  description: "GroupDocs.Watermark for Python via .NET легко интегрируется с различными операционными системами и менеджерами пакетов."
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
    GroupDocs.Watermark for Python via .NET позволяет вам обрабатывать файлы самых разных форматов. [Изучите полный список](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "Функции GroupDocs.Watermark for Python via .NET"
  description: "Повысьте безопасность документов с помощью программных водяных знаков. Обрабатывайте файлы различных форматов, включая PDF, DOCX, XLSX, PPTX и форматы изображений (PNG, JPG и т. д.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Точный контроль водяных знаков"
      content: "Точно управляйте водяными знаками, добавляя или удаляя их из определенных разделов, целых документов или отдельных вложений и фигур в файлах разных форматов."

    # feature loop
    - icon: "watermark_style"
      title: "Настройте внешний вид водяного знака"
      content: "Осуществляйте детальный контроль над внешним видом водяных знаков, изменяя такие атрибуты, как цвет, шрифт, непрозрачность, поворот и расположение в документе."

    # feature loop
    - icon: "hidden_print"
      title: "Печать PDF с водяными знаками"
      content: "Добавляйте в обычные документы скрытые водяные знаки, которые становятся видимыми только во время процесса печати, незаметно повышая безопасность документа."

    # feature loop
    - icon: "image_only"
      title: "Водяные знаки конкретного изображения"
      content: "Добавляйте водяные знаки на определенные изображения в документе с помощью нашего решения. Встраивайте водяные знаки в определенный раздел (например, страницу, слайд) или по всему документу."

    # feature loop
    - icon: "image_frame"
      title: "Многослойные водяные знаки изображений"
      content: "Добавляйте водяные знаки точно к определенным кадрам в формате многокадрового изображения, обеспечивая детальный контроль над размещением водяных знаков."

    # feature loop
    - icon: "attachments"
      title: "Комплексная защита контента"
      content: "Расширьте защиту различных элементов документа, таких как вложения в документах Excel и фигуры изображений в презентациях, обеспечивая дополнительный уровень безопасности."

    # feature loop
    - icon: "pdf_objects"
      title: "Расширенные возможности создания водяных знаков в PDF-файлах"
      content: "Добавляйте водяные знаки в различные области PDF-файлов, включая рамку за обрез, рамку обрезки, рамку обрезки и т. д."

    # feature loop
    - icon: "doc_background"
      title: "Водяные знаки фонового изображения"
      content: "Управляйте водяными знаками на фоновых изображениях электронных таблиц и презентаций, предлагая дополнительные возможности настройки мер визуальной безопасности."

    # feature loop
    - icon: "unreadable_characters"
      title: "Текстовый водяной знак с нечитаемыми символами"
      content: "Используйте нечитаемые символы в текстовых водяных знаках, встроенных в презентации, что повышает безопасность, значительно усложняя несанкционированное извлечение водяных знаков."

    # feature loop
    - icon: "watermark_text_search"
      title: "Расширенный поиск водяных знаков"
      content: "Используйте комплексные функции поиска, чтобы находить водяные знаки в документах на основе определенных параметров или путем сочетания различных критериев."

    # feature loop
    - icon: "watermark_image_search"
      title: "Обнаружение водяных знаков похожего изображения"
      content: "Найдите похожие изображения водяных знаков в документах, которые визуально напоминают исходное изображение."

    # feature loop
    - icon: "document_info"
      title: "Анализируйте информацию о документе"
      content: "Извлеките важные данные документа, такие как настройки страницы, для дальнейшего анализа."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Образцы кода"
  description: "Изучите примеры кода, демонстрирующие общие функции GroupDocs.Watermark for Python via .NET."
  items:
    # code sample loop
    - title: "Водяной знак на документе с изображением"
      content: |
        Используйте GroupDocs.Watermark for Python via .NET для защиты документов путем добавления водяных знаков изображений. [Подробнее](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Как защитить файл водяным знаком изображения.">}}
        ```python {style=abap}

        # Загрузить исходный документ в Watermarker
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Укажите путь к изображению водяного знака
            watermark = groupdocs.watermark.watermarks.ImageWatermark("watermark.jpg")
            watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwgroupdocs.watermark.common.VerticalAlignment.CENTER

            # Защитите файл и сохраните его
            watermarker.add(watermark)
            watermarker.save("result.pdf")
       
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Найдите и измените существующие водяные знаки"
      content: |
        GroupDocs.Watermark for Python via .NET позволяет вам управлять водяными знаками документов. Выберите водяные знаки и измените их свойства. [Узнайте, как](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Поиск и модификация водяных знаков.">}}
        ```python {style=abap}

        # Загрузить исходный документ
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Поиск водяных знаков, подлежащих обновлению
            search_criteria = groupdocs.watermark.search.searchcriteria.TextSearchCriteria("annotation", False)
            watermarks = watermarker.search(search_criteria)
            
            # Обновите нужные свойства
            for watermark in watermarks:
                watermark.text = "passed"

            # Сохранить измененный документ по указанному пути
            watermarker.save("result.pdf")


        ```
        {{< /landing/code >}}

---
