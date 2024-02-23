---
############################# Static ############################
layout: "autogen-child"
draft: false
path: "watermark/java/search/image/xltx/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST
############################# Head ############################
head_title: "Поиск водяных знаков изображения из XLTX в Java"
head_description: "Библиотека Java для поиска водяных знаков изображений в документе XLTX с использованием функций интеллектуального поиска в приложениях Java и J2SE с использованием API-интерфейсов GroupDocs.Watermark для Java."
############################# Header ############################
title: "Поиск водяных знаков изображения из XLTX в Java"
description: "Используйте интеллектуальный поиск, чтобы найти все возможные водяные знаки изображения из файла XLTX в приложениях Java и J2SE. Определите критерии поиска, чтобы найти все совпадающие водяные знаки изображения на всех или определенных страницах исходного документа."
############################# SubMenu ############################
submenu:
    enable: false
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark для Java API"
    content: |
        GroupDocs.Watermark for Java — это комплексное решение для управления водяными знаками для приложений Java. Разработчики могут быстро выполнять такие операции с водяными знаками, как; добавлять, редактировать, искать и удалять различные типы водяных знаков в документах всех популярных форматов файлов. Он поддерживает работу с текстовыми и графическими водяными знаками в различных документах, включая PDF, Microsoft Word, Excel, PowerPoint, Visio, электронную почту и форматы изображений.
        API-интерфейсы GroupDocs.Watermark хорошо поддерживаются во всех основных операционных системах и версиях Java, включая J2SE 7.0 (1.7), J2SE 8.0 (1.8) и Java 10.
############################# Steps ############################
steps:
    enable: true
    title_left: "Поиск водяных знаков из XLTX в Java"
    content_left: |
        [GroupDocs.Watermark](/ru/watermark/java/) позволяет разработчикам Java легко выполнять интеллектуальный поиск водяных знаков изображений в своих документах, выполняя несколько простых шагов.
        * Создайте **Watermarker** с входным документом XLTX.
        * Инициализируйте **ImageSearchCriteria** для поиска водяных знаков.
        * Установите максимально допустимую разницу между изображениями.
        * Отображение возможных совпадающих водяных знаков.
    title_right: "Системные Требования"
    content_right: |
        Перед выполнением приведенного ниже примера кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: NetBeans, IntelliJ IDEA, Eclipse
        * Фреймворки: Java 7 (1.7) и выше
        * Загрузите последнюю версию GroupDocs.Watermark для Java с [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
    code: |
        ```cs
        // поиск возможных водяных знаков IMAGE в документе XLTX с использованием Java.
        // Создание водяного знака с входным документом XLTX
        Watermarker watermarker = new Watermarker(input.xltx);
        // Инициализируем ImageSearchCriteria для запуска поиска водяных знаков
        ImageSearchCriteria imageSearchCriteria = new ImageDctHashSearchCriteria(watermark.jpeg);
        // Установить максимально допустимую разницу между образцом изображения и возможным водяным знаком
        imageSearchCriteria.setMaxDifference(0.9);
        PossibleWatermarkCollection possibleWatermarks = watermarker.search(imageSearchCriteria);
        System.out.println("Found " + possibleWatermarks.getCount() + " possible watermark(s).");
        watermarker.close();        
        ```        
demos:
    enable: false
about_formats:
    enable: false
more_formats:
    enable: true
back_to_top:
    enable: true
---
