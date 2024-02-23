---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "API Java для добавления поиска, удаления водяных знаков в PDF, Word, Excel, изображения"
head_description: "API водяных знаков документов Java — создание, поиск и удаление водяных знаков из документов: форматы PDF, Word, Excel, презентации, Visio, электронная почта и файлы изображений."

############################# Header ############################
title: "Java API для управления водяными знаками"
description: "Разрабатывайте Java-приложения для выполнения операций добавления водяных знаков к изображениям и тексту с помощью интеллектуального поиска и надежной защиты."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Watermark for Java"
        image: "/border/groupdocs-watermark-java.svg"
        product: "GroupDocs.Watermark"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Обзор"

            # button loop
            - link: "#features"
              text: "Функции"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/watermark"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/watermark/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/watermark"
        link_learn: "https://docs.groupdocs.com/watermark/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Обзор ############################
overview:
    enable: true
    content: |
      GroupDocs.Watermark для Java позволяет создавать бизнес-приложения, позволяющие вашим конечным пользователям применять новые водяные знаки, искать и удалять существующие водяные знаки в файлах поддерживаемых форматов. Вы можете программно назначать цифровые водяные знаки множеству форматов файлов и использовать его мощные возможности интеллектуального поиска. GroupDocs.Watermark для Java предоставляет различные встроенные меры безопасности, которые можно использовать для предотвращения неправомерного использования цифровых документов, содержащих конфиденциальную информацию или содержимое интеллектуальной собственности.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          Ниже приводится обзор GroupDocs.Watermark для Java:

        правильно:
          enable: true
          icon: "fab fa-html5"
          title: "Обзор"
          content: |
            * Добавить и удалить водяной знак
            * Поиск и замена водяного знака
            * Поиск по форматированию
            * Поиск по сравнению изображений
            * Работа с верхними и нижними колонтитулами
            * Работа с фоновыми изображениями
            * Работа с вложениями
            * Растеризовать страницы
            * Применить ограничения редактирования
      
      ## TAB TWO ##
      tab_two:
        description: |
          Поддерживаемые [форматы документов и тип водяного знака](https://docs.groupdocs.com/watermark/java/supported-document-formats/) для каждого формата перечислены ниже:

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
                * **Visio:** VSD, VDX, VSS, VSSX, VSX, VST, VSTX, VTX, VSDX, VDW, VSTM, VSSM, VSDM

            # table loop
            - title: "Добавление водяного знака"
              content: |
                * **PDF**: XObject, артефакт, аннотация
                * **Слово**: Форма
                * **Excel**: форма, верхний и нижний колонтитулы
                * **PowerPoint**: Форма
                * **Visio**: Форма
                * **Растровое изображение**: текст, изображение
                * **Многостраничный Tiff**: текст, изображение
                * **Анимированный Gif**: текст, изображение

        right:
          enable: true
          table:
            # table loop
            - title: "PDF и графические документы"
              content: |
                * **Переносимый формат документа**: PDF
                * **Открыть документ**: ODT
                * **Электронная почта**: EML, MSG, EMLX, OFT
                * **Изображения**: PNG, BMP, GIF, JPG, JPEG, JP2, TIF, TIFF, WebP

            # table loop
            - title: "Удаление водяного знака"
              content: |
                * **PDF**: XObject, артефакт, аннотация, обычный текст
                * **Word**: Фигура, обычный текст
                * **Excel**: форма, верхний и нижний колонтитулы, фоновое изображение, текст и формулы в ячейках
                * **PowerPoint**: Форма
                * **Visio**: форма, комментарии к диаграмме
                * **Электронная почта**: прикрепленные и встроенные изображения, фрагменты темы и основного текста

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Watermark for Java поддерживает следующие Операционные системы, Фреймворки и менеджеры пакетов:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Операционные системы"
              content: |
                * Рабочий стол Microsoft Windows
                * Сервер Microsoft Windows
                * линукс
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Поддерживаемые платформы"
              content: |
                * Java 7 (1.7) и выше

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Среды разработки"
              content: |
                * NetBeans
                * IntelliJ ИДЕЯ
                * Затмение
            # table loop
            - icon: "fas fa-tools"
              title: "Инструмент автоматизации сборки"
              content: |
                * Мавен

############################# Функции ############################
features:
    enable: true
    title: "GroupDocs.Watermark for Java Функции"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Извлеките все документы различных форматов из папки и нанесите или удалите водяные знаки"

      # feature loop
      - icon: "fas fa-eye"
        content: "Использование или удаление водяного знака из определенного раздела или всего документа"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Добавление водяного знака к выбранным кадрам мультикадрового изображения"

      # feature loop
      - icon: "fas fa-code"
        content: "Примените скрытый водяной знак к PDF, чтобы он отображался при печати документа"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Используйте водяной знак для вложений в документе Excel и всех фигурах изображений в слайдах"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Поместите водяной знак или удалите его из фоновых изображений слайдов или листа Excel"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Установите водяной знак для поддерживаемых файлов во вложениях электронной почты или PDF-файла"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Добавить или удалить водяной знак как XObject, артефакты и аннотации в PDF-файлах"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Удалить водяной знак, соответствующий тексту с определенным форматированием"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Найдите водяные знаки изображения, напоминающие определенное изображение"

      # feature loop
      - icon: "fas fa-columns"
        content: "Определите текстовый водяной знак, даже если между буквами есть нечитаемые символы"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Ищите водяные знаки на основе определенных параметров или путем назначения нескольких критериев"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Укажите форматирование шрифта, чтобы найти совпадающий текстовый водяной знак"

      # feature loop
      - icon: "fas fa-print"
        content: "Получить размеры страницы, слайда, ячейки для абсолютного размера и положения водяного знака"

      # feature loop
      - icon: "fas fa-lock"
        content: "Добавить водяной знак к фигурам изображения в документе Word и ограничить редактирование водяных знаков"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Защитный текстовый водяной знак в презентациях с использованием нечитаемых символов"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Защита водяных знаков PDF-документа путем растрирования отдельной страницы или всего документа"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Изменить форматирование текста при замене текущего текстового водяного знака"

      # feature loop
      - icon: "fas fa-heading"
        content: "Выравнивание водяного знака по окну за обрез, художественному окну, окну обрезки или окну обрезки в файле PDF"

    больше_функций:
      # more_feature_loop
      - title: "Используйте водяные знаки"
        content: |
          GroupDocs.Watermark для Java позволяет работать с многочисленными видами водяных знаков. Чтобы добавить водяной знак любого типа, достаточно всего нескольких строк кода. В следующем примере показано, как добавить водяной знак изображения в документ Word с помощью Java:
          
          ```java
          Document doc = Document.load(Common.mapSourceFilePath("D://test.docx"));
          Font font = new Font("Times New Roman", 12);
          TextWatermark watermark = new TextWatermark("Test watermark", font);

          // Установить тип размера
          watermark.setSizingType(SizingType.ScaleToParentDimensions);

          // Установить масштаб водяного знака
          watermark.setScaleFactor(0.5);

          doc.addWatermark(watermark);
          doc.save(Common.mapOutputFilePath("D://test.docx"));
          doc.close();
          ```
      # more_feature_loop
      - title: "Добавляйте водяные знаки в файлы разных форматов за один раз"
        content: "С помощью API GroupDocs.Watermark для Java вы можете добавлять или удалять водяные знаки всех документов, присутствующих в определенной папке, в пакетном режиме. Не имеет значения, если документы имеют разный формат, GroupDocs.Watermark для Java точно применит водяной знак ко всем файлам.."

      # more_feature_loop
      - title: "Назначьте надежную защиту своим водяным знакам"
        content: "С помощью минимального кода вы можете назначить надежную защиту своим водяным знакам и затруднить для любого стороннего инструмента изменение или удаление назначенного вам водяного знака из файла PDF. Это связано с тем, что GroupDocs.Watermark для Java позволяет конвертировать все страницы PDF-файла в растровые изображения. Такой подход делает ваши цифровые водяные знаки безопасными, сохраняя при этом их качество близким к оригинальному."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Watermark предлагает API для просмотра документов для других популярных сред разработки."

    solution:
        # solution loop
        - img_alt: "GroupDocs.Watermark for .NET"
          image: "/border/groupdocs-watermark-net.svg"
          product: "GroupDocs.Watermark"
          platform: ".NET"
          link: "/watermark/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---