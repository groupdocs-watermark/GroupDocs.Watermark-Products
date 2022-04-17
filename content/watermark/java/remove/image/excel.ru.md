---
############################# Static ############################
layout: "autogen-child"
draft: false
path: "watermark/java/remove/image/excel/"
otherformats: PDF WORD IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST
############################# Head ############################
head_title: "Удалить водяной знак изображения из EXCEL в Java"
head_description: "Библиотека Java для поиска и удаления водяного знака изображения из документа EXCEL с помощью интеллектуального поиска в приложениях Java и J2SE с использованием API-интерфейсов GroupDocs.Watermark для Java."
############################# Header ############################
title: "Удалить водяной знак изображения из EXCEL в Java"
description: "Используйте интеллектуальный поиск, чтобы найти и удалить водяной знак изображения из документа EXCEL из приложений Java и J2SE. Определите критерий поиска для поиска и удаления указанных водяных знаков из документа."
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
    title_left: "Удалить водяной знак из файла EXCEL в Java"
    content_left: |
        [GroupDocs.Watermark](/ru/watermark/java/) позволяет разработчикам Java легко находить и удалять водяные знаки с форматированием текста из своих приложений, выполняя несколько простых шагов.
        * Создайте экземпляр **Watermarker** с входным документом EXCEL.
        * Инициализируйте **PossibleWatermarkCollection**, чтобы найти водяные знаки изображения.
        * Удалить указанные водяные знаки из документа.
        * Сохраните измененный документ.
    title_right: "Системные Требования"
    content_right: |
        Перед выполнением приведенного ниже примера кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: NetBeans, IntelliJ IDEA, Eclipse
        * Фреймворки: Java 7 (1.7) и выше
        * Загрузите последнюю версию GroupDocs.Watermark для Java с [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
    code: |
        ```cs
        // Поиск и удаление водяного знака изображения из документа EXCEL в приложениях Java
        // Создание водяного знака с входным документом EXCEL
        Watermarker watermarker = new Watermarker(input.excel);
        PossibleWatermarkCollection possibleWatermarks = watermarker.search();
        // Удалить водяной знак из указанной позиции индекса в документе
        possibleWatermarks.removeAt(0);
        // Удалить указанный возможный водяной знак из документа
        possibleWatermarks.remove(possibleWatermarks.get_Item(0);
        // Сохраняем измененный документ
        watermarker.save(output.excel);
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
