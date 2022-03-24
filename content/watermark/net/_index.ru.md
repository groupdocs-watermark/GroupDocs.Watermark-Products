---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET API для добавления поиска и удаления водяных знаков в изображения Word Excel PDF"
head_description: "C# .NET API для добавления, поиска и удаления графических и текстовых водяных знаков из документов: PDF, Word, Excel, презентации, Visio, электронная почта и форматы файлов изображений."

############################# Header ############################
title: ".NET API для управления водяными знаками"
description: "Создавайте приложения .NET для работы с текстовыми и графическими водяными знаками с функциями интеллектуального поиска и надежной защиты."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Watermark for .NET"
        image: "/border/groupdocs-watermark-net.svg"
        product: "GroupDocs.Watermark"
        platform: ".NET"

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
            - link: "https://purchase.groupdocs.com/pricing/watermark/net"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/watermark"
        link_learn: "https://docs.groupdocs.com/watermark/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Обзор ############################
overview:
    enable: true
    content: |
      GroupDocs.Watermark для .NET позволяет создавать готовые к продаже бизнес-приложения на C#, ASP.NET и других технологиях, связанных с .NET, которые позволяют вашим конечным пользователям добавлять новые водяные знаки, искать и удалять существующие водяные знаки в поддерживаемых форматах файлов. . Используя GroupDocs.Watermark для .NET, вы можете программно применять цифровые водяные знаки к множеству форматов файлов и препятствовать несанкционированному использованию интеллектуальной собственности, а также надежно маркировать документы конфиденциального характера с помощью различных встроенных мер безопасности, предлагаемых этим API.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Ниже приведен обзор GroupDocs.Watermark для .NET:
      
        right:
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
          Поддерживаемые [форматы документов и тип водяного знака](https://docs.groupdocs.com/watermark/net/supported-document-formats/) для каждого формата перечислены ниже:

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
                * **Portable Document Format**: PDF
                * **Open Document**: ODT
                * **Email**: EML, MSG, EMLX, OFT
                * **Images**: PNG, BMP, GIF, JPG, JPEG, JP2, TIF, TIFF, WebP

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
          GroupDocs.Watermark for .NET поддерживает следующие Операционные системы, Frameworks & Менеджер пакетовs:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Операционные системы"
              content: |
                * Рабочий стол Windows
                * Windows-сервер
                * Windows Azure
                * линукс

            # table loop
            - icon: "fas fa-code"
              title: "Поддерживаемые платформы"
              content: |
                * .NET Framework 2.0 или выше
                * Монофреймворк 1.2 или выше
                * .NET Стандарт 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Менеджер пакетов"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Среды разработки"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * МоноДевелопмент

############################# Функции ############################
features:
    enable: true
    title: "GroupDocs.Watermark for .NET Функции"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Добавление или удаление водяных знаков из определенного раздела или всего документа различных форматов файлов"

      # feature loop
      - icon: "fas fa-eye"
        content: "Прикрепите водяной знак ко всем изображениям в определенном разделе, странице, слайде или документе"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Назначить водяной знак только определенным кадрам многокадрового изображения"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Выделить скрытый водяной знак для PDF, который появляется только при печати документа"

      # feature loop
      - icon: "fas fa-code"
        content: "Установите водяной знак на все вложения в документе Excel и на все формы изображений в слайдах"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Поместите водяной знак или удалите его с фоновых изображений электронной таблицы или слайдов"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Используйте водяной знак для поддерживаемых файлов во всех вложениях электронного письма или документа PDF"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Применение или удаление водяных знаков в качестве объектов XObject, артефактов и аннотаций в документах PDF"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Удалите водяной знак, содержащий текст с определенным форматированием"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Ищите водяные знаки изображения, которые напоминают определенное изображение"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Определите текстовый водяной знак, даже если между буквами есть нечитаемые символы"

      # feature loop
      - icon: "fas fa-columns"
        content: "Поиск водяных знаков по определенным параметрам или по нескольким критериям"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Укажите форматирование шрифта для поиска соответствующего текстового водяного знака"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Программное извлечение параметров страницы и другой информации для поддерживаемых форматов"

      # feature loop
      - icon: "fas fa-print"
        content: "Добавляйте водяные знаки к изображениям внутри любых верхних и нижних колонтитулов в поддерживаемых форматах документов"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Добавьте водяной знак к фигурам изображения в документе Word и заблокируйте водяные знаки, чтобы ограничить редактирование"

      # feature loop
      - icon: "fas fa-lock"
        content: "Защита текстового водяного знака с помощью нечитаемых символов в презентациях"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Растеризация отдельной страницы или всего PDF-документа для защиты добавленных водяных знаков"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Изменить форматирование текста при замене существующего текстового водяного знака"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Выровнять водяной знак по окну выпуска за обрез, художественному окну, окну обрезки или окну обрезки в документе PDF"

      # feature loop
      - icon: "fas fa-heading"
        content: "Редактирование свойств фигуры в документах Microsoft Visio"

    больше_функций:
      # more_feature_loop
      - title: "Добавление водяного знакаs"
        content: |
          GroupDocs.Watermark для .NET поддерживает несколько типов водяных знаков. Добавление водяных знаков любого типа — это всего лишь несколько строк кода. В следующем примере показано применение водяного знака изображения к документу Word с помощью C#:

          ```cs
          // Загрузите документ
          using (FileStream stream = File.Open("document.docx", FileMode.Open, FileAccess.ReadWrite))
          {
            using (Watermarker watermarker = new(Watermarker(stream))
            {
                // Использовать путь к изображению в качестве параметра конструктора
                using (ImageWatermark watermark = new ImageWatermark("logo.png"))
                {
                    watermark.HorizontalAlignment = HorizontalAlignment.Center;
                    watermark.VerticalAlignment = VerticalAlignment.Center;
                    watermarker.Add(watermark);
                }
                // Сохраните полученный документ
                watermarker.Save("document_watermarked.docx");
                }
          }
          ```
      # more_feature_loop
      - title: "Применить водяной знак to Files of Different Formats in a Go"
        content: "API GroupDocs.Watermark позволяет применить водяной знак или удалить водяной знак для всех файлов в определенной папке за один раз. Файлы могут быть даже разного формата, но водяной знак будет применен ко всем им точно."

      # more_feature_loop
      - title: "Надежная защита для водяных знаков"
        content: "С помощью всего одной строки кода вы можете затруднить удаление водяного знака из PDF-файлов любым инструментом. Это достигается за счет преобразования всех страниц PDF-документа в растровые изображения с сохранением исходного качества.."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Watermark предлагает API для просмотра документов для других популярных сред разработки."

    solution:
        # solution loop
        - img_alt: "GroupDocs.Watermark for Java"
          image: "/border/groupdocs-watermark-java.svg"
          product: "GroupDocs.Watermark"
          platform: "Java"
          link: "/watermark/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---