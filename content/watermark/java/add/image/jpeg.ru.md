---
############################# Static ############################
layout: "autogen-child"
draft: false
path: "watermark/java/add/image/jpeg/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST
############################# Head ############################
head_title: "Добавить водяной знак изображения в JPEG в Java"
head_description: "Библиотека Java для добавления водяного знака изображения в файл JPEG в приложениях Java и J2SE с использованием API-интерфейсов GroupDocs.Watermark для Java."
############################# Header ############################
title: "Добавить водяной знак изображения в JPEG в Java"
description: "Добавление водяного знака изображения в файл JPEG в приложениях Java и J2SE. Добавляйте в документы водяные знаки изображений BMP, PNG, GIF и JPEG. Также управляйте размером водяного знака, выравниванием, углом поворота и положением водяного знака на страницах документа, как вам может понадобиться."
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
    title_left: "Добавить водяной знак изображения в файл JPEG в Java"
    content_left: |
        [GroupDocs.Watermark](/ru/watermark/java/) позволяет разработчикам Java легко добавлять водяные знаки изображений (BMP, PNG, GIF или JPEG) в свои приложения, выполняя несколько простых шагов.
        * Создайте экземпляр **Watermarker** с входным документом JPEG.
        * Используйте путь водяного знака изображения в качестве параметра конструктора класса **ImageWatermark**.
        * Установите свойства водяного знака (размер, выравнивание, цвет и т. д.).
        * Добавьте водяной знак к водяному знаку и сгенерируйте выходной документ.
    title_right: "Системные Требования"
    content_right: |
        Перед выполнением приведенного ниже примера кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: NetBeans, IntelliJ IDEA, Eclipse
        * Фреймворки: Java 7 (1.7) и выше
        * Загрузите последнюю версию GroupDocs.Watermark для Java с [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
    code: |
        ```cs
        // Добавляем водяной знак изображения в JPEG в Java-приложениях
        // Создание водяного маркера с входным документом JPEG
        Watermarker watermarker = new Watermarker(input.jpeg);
        // Использовать путь к водяному знаку изображения в качестве параметра конструктора класса ImageWatermark
        ImageWatermark watermark = new ImageWatermark(watermark.png);
        // Установка свойств водяного знака (ширина, высота, выравнивание)
        watermark.Width = 140;
        watermark.Height = 140;
        watermark.HorizontalAlignment = HorizontalAlignment.Center;
        watermark.VerticalAlignment = VerticalAlignment.Center;
        // Добавляем водяной знак к водяному знаку и генерируем выходной документ
        watermarker.add(watermark);
        watermarker.save(output.jpeg);
        watermark.close();
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
