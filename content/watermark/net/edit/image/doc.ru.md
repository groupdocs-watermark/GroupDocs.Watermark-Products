---
############################# Static ############################
layout: "autogen-child"
draft: false
path: "watermark/net/edit/image/doc/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST
############################# Head ############################
head_title: "Редактировать водяной знак изображения в DOC в C#, ASP.NET, VB.NET"
head_description: ".NET для редактирования водяного знака найденного изображения в файле DOC в приложениях C#, ASP.NET, VB.NET и .NET Core с использованием API-интерфейсов GroupDocs.Watermark для .NET."
############################# Header ############################
title: "Редактировать водяной знак изображения в DOC на С# .NET"
description: "Найдите и измените водяной знак найденного изображения в документе DOC в приложениях C#, ASP.NET, VB.NET и .NET Core. Добавляйте в документы водяные знаки изображений BMP, PNG, GIF и JPEG. Также управляйте размером водяного знака, типом шрифта, углом поворота и положением водяного знака на страницах документа, как вам может понадобиться."
############################# SubMenu ############################
submenu:
    enable: false
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark для .NET API"
    content: |
        GroupDocs.Watermark для .NET — это комплексное решение для управления водяными знаками для приложений .NET. Разработчики могут быстро выполнять такие операции с водяными знаками, как; добавлять, редактировать, искать и удалять различные типы водяных знаков в документах всех популярных форматов файлов. Он поддерживает работу с текстовыми и графическими водяными знаками в различных документах, включая PDF, Microsoft Word, Excel, PowerPoint, Visio, электронную почту и форматы изображений.
        API-интерфейсы GroupDocs.Watermark хорошо поддерживаются на всех основных операционных системах и платформах, включая .NET Framework, .NET Standard, .NET Core, Mono и Xamarin.
############################# Steps ############################
steps:
    enable: true
    title_left: "Редактировать водяной знак изображения в файле DOC в .NET"
    content_left: |
        [GroupDocs.Watermark](/ru/watermark/net/) позволяет разработчикам .NET легко редактировать водяные знаки изображений (BMP, PNG, GIF или JPEG) в своих приложениях, выполняя несколько простых шагов.
        * Создайте экземпляр **Watermarker** с входным документом DOC.
        * Инициализируйте **SearchCriteria**, чтобы найти водяные знаки изображения.
        * Заменить найденный водяной знак.
        * Сохраните новый документ с водяным знаком.
    title_right: "Системные Требования"
    content_right: |
        Перед выполнением приведенного ниже примера кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Visual Studio, Xamarin, MonoDevelop
        * Фреймворки: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Watermark для .NET из [NuGet](https://www.nuget.org/packages/GroupDocs.Watermark).
    code: |
        ```cs
        // Поиск и замена водяного знака изображения в DOC в приложениях C#, ASP.NET, VB.NET и .NET Core
        // Создаем водяной маркер с входным документом DOC
        using (Watermarker watermarker = new Watermarker(input.doc));
          {
            // Инициализируем SearchCriteria для соответствия конкретному изображению
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria(logo.png);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
                {
                    try
                        {
                            // Заменяем найденное изображение
                            watermark.ImageData = imageData;
                        }
                    catch (Exception e)
                    {
                        // Найденный объект может не поддерживать редактирование текста
                        // Передаваемые аргументы могут иметь недопустимое значение
                        // Обрабатываем такие случаи здесь
                    }
                }
            // Сохраняем документ с водяным знаком
            watermarker.Save(output.doc);
          }
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