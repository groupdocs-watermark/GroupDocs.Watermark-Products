---
############################# Static ############################
layout: "autogen-child"
draft: false
path: "watermark/java/edit/image/vsd/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST
############################# Head ############################
head_title: "Редактировать водяной знак изображения в VSD в Java"
head_description: "Библиотека Java для редактирования водяного знака найденного изображения в файле VSD в приложениях Java и J2SE с использованием API-интерфейсов GroupDocs.Watermark для Java."
############################# Header ############################
title: "Редактировать водяной знак изображения в VSD в Java"
description: "Найдите и измените водяной знак найденного изображения в документе VSD в приложениях Java и J2SE. Добавляйте в документы водяные знаки изображений BMP, PNG, GIF и JPEG. Также управляйте размером водяного знака, типом шрифта, углом поворота и положением водяного знака на страницах документа, как вам может понадобиться."
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
    title_left: "Редактировать водяные знаки изображения в файле VSD в Java"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/) makes it easy for Java developers to edit image (BMP, PNG, GIF or JPEG) watermarks in their applications by implementing a few easy steps.
        * Создайте экземпляр **Watermarker** с входным документом VSD.
        * Инициализируйте **SearchCriteria**, чтобы найти водяные знаки изображения.
        * Заменить найденный водяной знак.
        * Сохраните новый документ с водяным знаком.
    title_right: "Системные Требования"
    content_right: |
        Перед выполнением приведенного ниже примера кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: NetBeans, IntelliJ IDEA, Eclipse
        * Фреймворки: Java 7 (1.7) и выше
        * Загрузите последнюю версию GroupDocs.Watermark для Java с [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
    code: |
        ```cs
        // Поиск и замена водяного знака изображения в VSD в приложениях Java
        // Создание водяного маркера с входным документом VSD
        Watermarker watermarker = new Watermarker(input.vsd);
        // Инициализируем SearchCriteria для соответствия конкретному изображению
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria(logo.png);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        for (PossibleWatermark watermark : watermarks)
        {
                try
                {
                    // Заменяем найденное изображение
                    watermark.setImageData(imageData);
                }
                catch (Exception e)
                {
                    // Найденный объект может не поддерживать редактирование текста
                    // Передаваемые аргументы могут иметь недопустимое значение
                    // Обрабатываем такие случаи здесь
                }
        }
        // Сохраняем документ с водяным знаком
        watermarker.save(output.vsd);
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
