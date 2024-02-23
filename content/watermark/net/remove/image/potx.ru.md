---
############################# Static ############################
layout: "autogen-child"
draft: false
path: "watermark/net/remove/image/potx/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST
############################# Head ############################
head_title: "Удалить водяной знак изображения из POTX в C# .NET"
head_description: ".NET для поиска и удаления водяных знаков изображения из документа POTX с помощью интеллектуального поиска в приложениях C#, ASP.NET, VB.NET и .NET Core с использованием API-интерфейсов GroupDocs.Watermark для .NET."
############################# Header ############################
title: "Удалить водяной знак изображения из POTX в C#"
description: "Используйте интеллектуальный поиск, чтобы найти и удалить водяной знак изображения из документа POTX в приложениях C#, ASP.NET, VB.NET и .NET Core. Определите критерий поиска для поиска и удаления указанных водяных знаков из документа."
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
    title_left: "Удалить водяной знак из файла POTX в .NET"
    content_left: |
        [GroupDocs.Watermark](/ru/watermark/net/) позволяет разработчикам .NET легко находить и удалять водяные знаки с форматированием текста из своих приложений, выполняя несколько простых шагов.
        * Создайте экземпляр **Watermarker** с входным документом POTX.
        * Инициализируйте **SearchCriteria**, чтобы найти водяные знаки изображения.
        * Удалить определенный водяной знак из документа.
        * Сохраните измененный документ.
    title_right: "Системные Требования"
    content_right: |
        Перед выполнением приведенного ниже примера кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Visual Studio, Xamarin, MonoDevelop
        * Фреймворки: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Watermark для .NET из [NuGet](https://www.nuget.org/packages/GroupDocs.Watermark).
    code: |
        ```cs
        // Поиск и удаление водяного знака изображения из документа POTX в приложениях C#, ASP.NET, VB.NET и .NET Core
        // Создаем водяной маркер с входным документом POTX
        using (Watermarker watermarker = new Watermarker(input.potx));
          {
            // Инициализируем SearchCriteria для соответствия конкретному изображению
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria(logo.png);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            // Удалить указанный водяной знак из документа
            possibleWatermarks.Remove(possibleWatermarks[0]);
            // Сохраняем измененный документ
            watermarker.Save(output.potx);
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
