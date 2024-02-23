---
############################# Static ############################
layout: "autogen-child"
draft: false
path: "watermark/java/add/text/vssx/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSDM VSSM VSTM VTX VDW VSS VST
############################# Head ############################
head_title: "Добавить текстовый водяной знак в VSSX в Java"
head_description: "Библиотека Java для добавления текстового водяного знака в файл VSSX в приложениях Java и J2SE с использованием API GroupDocs.Watermark для Java"
############################# Header ############################
title: "Добавить текстовый водяной знак в VSSX в Java"
description: "Добавление текстового водяного знака в файл VSSX в приложениях Java и J2SE. Управляйте размером водяного знака, типом шрифта, углом поворота и положением водяного знака на страницах документа, как вам может понадобиться."
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
    title_left: "Добавить текстовый водяной знак в файл VSSX в Java"
    content_left: |
        [GroupDocs.Watermark] (/ru/watermark/java/) позволяет разработчикам Java легко добавлять текстовые водяные знаки в свои приложения, выполняя несколько простых шагов.
        * Создайте экземпляр **Watermarker** с входным документом VSSX.
        * Инициализируйте **TextWatermarker** с текстом водяного знака, размером и стилем шрифта.
        * Установите свойства водяного знака (выравнивание, цвет и т. д.).
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
        // Добавляем текстовый водяной знак в VSSX в Java
        // Создаем водяной маркер с входным документом VSSX
        (Watermarker watermarker = new Watermarker(input.vssx));
        // Создаем TextWatermarker с текстом водяного знака, размером и стилем шрифта
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        // Установить свойства водяного знака
        watermark.setForegroundColor(Color.getRed());
        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
        watermark.setVerticalAlignment(VerticalAlignment.Center);
        // Добавляем водяной знак и сохраняем изображение с водяным знаком
        watermarker.add(watermark);
        watermarker.save(output.vssx);
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
