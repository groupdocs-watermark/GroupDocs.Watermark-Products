---
############################# Static ############################
layout: "autogen-child"
draft: false
path: "watermark/net/search/image/xlsb/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST
############################# Head ############################
head_title: "Поиск водяных знаков изображения из XLSB в C# ASP.NET VB.NET"
head_description: ".NET для поиска водяных знаков изображений в документе XLSB с использованием функций интеллектуального поиска в приложениях C#, ASP.NET, VB.NET и .NET Core с использованием API-интерфейсов GroupDocs.Watermark для .NET."
############################# Header ############################
title: "Поиск водяных знаков изображения из XLSB в C#"
description: "Используйте интеллектуальный поиск, чтобы найти все возможные водяные знаки изображения из файла XLSB в приложениях C#, ASP.NET, VB.NET и .NET Core. Определите критерии поиска, чтобы найти все совпадающие водяные знаки изображения со всех или определенных страниц исходного документа."
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
    title_left: "Поиск водяных знаков из XLSB в .NET"
    content_left: |
        [GroupDocs.Watermark](/ru/watermark/net/) упрощает разработчикам .NET интеллектуальный поиск водяных знаков изображений в своих документах, выполняя несколько простых шагов.
        * Создайте экземпляр **Watermarker** с входным документом XLSB.
        * Инициализируйте **ImageSearchCriteria** для поиска водяных знаков.
        * Установите максимально допустимую разницу между изображениями.
        * Отображение возможных совпадающих водяных знаков.
    title_right: "Системные Требования"
    content_right: |
        Перед выполнением приведенного ниже примера кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Visual Studio, Xamarin, MonoDevelop
        * Фреймворки: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Watermark для .NET из [NuGet](https://www.nuget.org/packages/GroupDocs.Watermark).
    code: |
        ```cs
        // поиск возможных водяных знаков IMAGE в документе XLSB с использованием C#, ASP.NET, VB.NET и .NET Core.
        // Создание водяного маркера с входным документом XLSB
        using (Watermarker watermarker = new Watermarker(input.xlsb));
          {
            // Инициализируем ImageSearchCriteria для запуска поиска водяных знаков
            ImageSearchCriteria imageSearchCriteria = new ImageDctHashSearchCriteria(watermark.jpeg);
            // Установить максимально допустимую разницу между образцом изображения и возможным водяным знаком
            imageSearchCriteria.MaxDifference = 0.9;
            PossibleWatermarkCollection possibleWatermarks = watermarker.Search(imageSearchCriteria);
            Console.WriteLine("Found {0} possible watermark(s).", possibleWatermarks.Count);
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
