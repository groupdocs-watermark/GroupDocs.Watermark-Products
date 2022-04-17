---
############################# Static ############################
layout: "autogen-child"
draft: false
path: "watermark/java/search/text/xltm/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST
############################# Head ############################
head_title: "Поиск водяных знаков от XLTM в Java"
head_description: "Библиотека Java для поиска водяных знаков в документе XLTM с использованием функций интеллектуального поиска в приложениях Java с использованием API-интерфейсов GroupDocs.Watermark для Java."
############################# Header ############################
title: "Поиск водяных знаков от XLTM в Java"
description: "Используйте интеллектуальный поиск, чтобы найти все возможные водяные знаки из файла XLTM в приложениях Java и J2SE. Определите критерии поиска на основе текста, регулярных выражений (RegEx), изображений, гиперссылок, символов и различных объектов поиска, чтобы найти водяные знаки на всех или определенных страницах исходного документа."
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
    title_left: "Поиск водяных знаков от XLTM в Java"
    content_left: |
        [GroupDocs.Watermark](/ru/watermark/java/) позволяет разработчикам Java легко выполнять интеллектуальный поиск водяных знаков в своих приложениях, выполняя несколько простых шагов.
        * Создайте экземпляр **Watermarker** с входным документом XLTM.
        * Инициализируйте **PossibleWatermarkCollection** для поиска водяных знаков.
        * Определены критерии поиска возможных водяных знаков.
    title_right: "Системные Требования"
    content_right: |
        Перед выполнением приведенного ниже примера кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: NetBeans, IntelliJ IDEA, Eclipse
        * Фреймворки: Java 7 (1.7) и выше
        * Загрузите последнюю версию GroupDocs.Watermark для Java с [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
    code: |
        ```cs
        // поиск возможных водяных знаков в документе XLTM с использованием Java.
        // Создание водяного знака с входным документом XLTM
        Watermarker watermarker = new Watermarker(input.xltm));
        // Инициализируем PossibleWatermarkCollection, чтобы начать поиск водяных знаков
        PossibleWatermarkCollection possibleWatermarks = watermarker.search();
        for (PossibleWatermark possibleWatermark : possibleWatermarks)
        {
            if (possibleWatermark.getImageData() != null)
            {
                System.out.println(possibleWatermark.getImageData().length);
            }
            // Определены критерии поиска для поиска возможных водяных знаков
            System.out.println(possibleWatermark.getText());
            System.out.println(possibleWatermark.getX());
            System.out.println(possibleWatermark.getY());
            System.out.println(possibleWatermark.getRotateAngle());
            System.out.println(possibleWatermark.getWidth());
            System.out.println(possibleWatermark.getHeight());
        }
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
