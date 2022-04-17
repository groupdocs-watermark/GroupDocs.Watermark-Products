---
############################# Static ############################
layout: "autogen-child"
draft: false
path: "watermark/net/search/text/ppsm/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST
############################# Head ############################
head_title: "Поиск водяных знаков из PPSM в C#, ASP.NET, VB.NET"
head_description: ".NET для поиска водяных знаков в документе PPSM с использованием функций интеллектуального поиска в приложениях C#, ASP.NET, VB.NET и .NET Core с использованием API-интерфейсов GroupDocs.Watermark для .NET."
############################# Header ############################
title: "Поиск водяных знаков из PPSM в C# .NET"
description: "Используйте интеллектуальный поиск, чтобы найти все возможные водяные знаки из файла PPSM в приложениях C#, ASP.NET, VB.NET и .NET Core. Определите критерии поиска на основе текста, регулярных выражений (RegEx), изображений, гиперссылок, символов и различных объектов поиска, чтобы найти водяные знаки на всех или определенных страницах исходного документа."
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
    title_left: "Поиск водяных знаков из PPSM в .NET"
    content_left: |
        [GroupDocs.Watermark](/ru/watermark/net/) упрощает разработчикам .NET интеллектуальный поиск водяных знаков в своих приложениях, выполняя несколько простых шагов.
        * Создайте экземпляр **Watermarker** с входным документом PPSM.
        * Инициализируйте **PossibleWatermarkCollection** для поиска водяных знаков.
        * Определены критерии поиска возможных водяных знаков.
    title_right: "Системные Требования"
    content_right: |
        Перед выполнением приведенного ниже примера кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Visual Studio, Xamarin, MonoDevelop
        * Фреймворки: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Watermark для .NET из [NuGet](https://www.nuget.org/packages/GroupDocs.Watermark).
    code: |
        ```cs
        // поиск возможных водяных знаков в документе PPSM с использованием C#, ASP.NET, VB.NET и .NET Core.
        // Создаем водяной маркер с входным документом PPSM
        using (Watermarker watermarker = new Watermarker(input.ppsm));
          {
            // Инициализируем PossibleWatermarkCollection, чтобы начать поиск водяных знаков
            PossibleWatermarkCollection possibleWatermarks = watermarker.Search();
            foreach (PossibleWatermark possibleWatermark in possibleWatermarks)
            {
                if (possibleWatermark.ImageData != null)
                {
                    Console.WriteLine(possibleWatermark.ImageData.Length);
                }
                // Определены критерии поиска для поиска возможных водяных знаков
                Console.WriteLine(possibleWatermark.Text);
                Console.WriteLine(possibleWatermark.X);
                Console.WriteLine(possibleWatermark.Y);
                Console.WriteLine(possibleWatermark.RotateAngle);
                Console.WriteLine(possibleWatermark.Width);
                Console.WriteLine(possibleWatermark.Height);
            }
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
