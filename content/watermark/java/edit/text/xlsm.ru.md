---
############################# Static ############################
layout: "autogen-child"
draft: false
path: "watermark/java/edit/text/xlsm/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST
############################# Head ############################
head_title: "Редактировать текстовый водяной знак в XLSM на Java"
head_description: "Библиотека Java для редактирования найденного текстового водяного знака в файле XLSM в приложениях Java с использованием API GroupDocs.Watermark для Java."
############################# Header ############################
title: "Редактировать текстовый водяной знак в XLSM на Java"
description: "Поиск и изменение найденного текстового водяного знака в документе XLSM с форматированием в приложениях Java и J2SE. Управляйте размером водяного знака, типом шрифта, углом поворота и положением водяного знака на страницах документа, как вам может понадобиться."
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
    title_left: "Редактировать текстовый водяной знак в файле XLSM в Java"
    content_left: |
        [GroupDocs.Watermark](/ru/watermark/java/) позволяет разработчикам Java легко редактировать текстовые водяные знаки в своих приложениях, выполняя несколько простых шагов.
        * Создайте экземпляр **Watermarker** с входным документом XLSM.
        * Инициализируйте **TextSearchCriteria** для поиска текстовых водяных знаков.
        * Редактировать текст найденных водяных знаков.
        * Установите свойства водяного знака (стиль шрифта, цвет и т. д.).
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
        // Поиск и обновление текстового водяного знака с форматированием в XLSM в приложениях Java
        // Создаем водяной маркер с входным документом XLSM
        Watermarker watermarker = new Watermarker(input.xlsm));
        // Инициализируем TextSearchCriteria для поиска текстовых водяных знаков
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        for (PossibleWatermark watermark : watermarks)
        {
            try
            {
                // Редактируем текст и устанавливаем свойства водяного знака
                watermark.getFormattedTextFragments().clear();
                watermark.getFormattedTextFragments().add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
            }
            catch (Exception e)
            {
                // Найденный объект может не поддерживать редактирование текста
                // Передаваемые аргументы могут иметь недопустимое значение
                // Обрабатываем такие случаи здесь
            }
        }
        // Сохраняем документ с водяным знаком
        watermarker.save(output.xlsm);
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
