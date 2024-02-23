---
############################# Static ############################
layout: "autogen-child"
draft: false
path: "watermark/net/remove/text/vtx/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VDW VSS VST
############################# Head ############################
head_title: "Удалить водяной знак из VTX в C#, ASP.NET, VB.NET"
head_description: ".NET для поиска и удаления водяных знаков из документа VTX с помощью интеллектуального поиска в приложениях C#, ASP.NET, VB.NET и .NET Core с использованием API-интерфейсов GroupDocs.Watermark для .NET."
############################# Header ############################
title: "Удалить водяной знак из VTX в C# .NET"
description: "Используйте интеллектуальный поиск, чтобы найти и удалить водяной знак из документа VTX с форматированием текста из приложений C#, ASP.NET, VB.NET и .NET Core. Определите критерий поиска для поиска и удаления водяных знаков на основе определенного имени шрифта, цвета, размера и других соответствующих свойств."
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
    title_left: "Удалить водяной знак из файла VTX в .NET"
    content_left: |
        [GroupDocs.Watermark](/ru/watermark/net/) позволяет разработчикам .NET легко находить и удалять водяные знаки с форматированием текста из своих приложений, выполняя несколько простых шагов.
        * Создайте **Watermarker** с входным документом VTX.
        * Инициализируйте **TextFormattingSearchCriteria**, чтобы найти текстовые водяные знаки.
        * Инициализировать определенные критерии поиска, чтобы найти и удалить водяные знаки.
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
        // Поиск и удаление водяных знаков с форматированием текста из документа VTX в приложениях C#, ASP.NET, VB.NET и .NET Core
        // Создание водяного маркера с входным документом VTX
        using (Watermarker watermarker = new Watermarker(input.vtx));
          {
            // Инициализируем TextFormattingSearchCriteria для определения водяных знаков для поиска
            TextFormattingSearchCriteria criteria = new TextFormattingSearchCriteria();
            criteria.ForegroundColorRange = new ColorRange();
            criteria.ForegroundColorRange.MinHue = -5;
            criteria.ForegroundColorRange.MaxHue = 10;
            criteria.ForegroundColorRange.MinBrightness = 0.01f;
            criteria.ForegroundColorRange.MaxBrightness = 0.99f;
            criteria.BackgroundColorRange = new ColorRange();
            criteria.BackgroundColorRange.IsEmpty = true;
            criteria.FontName = "Arial";
            criteria.MinFontSize = 19;
            criteria.MaxFontSize = 42;
            criteria.FontBold = true;
            PossibleWatermarkCollection watermarks = watermarker.Search(criteria);
            watermarks.Clear();
            // Сохраняем измененный документ
            watermarker.Save(output.vtx);
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
