---
############################# Static ############################
layout: "autogen-child"
draft: false
path: "watermark/net/add/image/pot/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST
############################# Head ############################
head_title: "Добавить водяной знак изображения в POT в C#, ASP.NET, VB.NET"
head_description: ".NET для добавления водяного знака изображения в файл POT в приложениях C#, ASP.NET, VB.NET и .NET Core с использованием API-интерфейсов GroupDocs.Watermark для .NET."
############################# Header ############################
title: "Добавить водяной знак изображения в POT в C# .NET"
description: "Добавление водяного знака изображения в файл POT в приложениях C#, ASP.NET, VB.NET и .NET Core. Добавляйте в документы водяные знаки изображений BMP, PNG, GIF и JPEG. Также управляйте размером водяного знака, выравниванием, углом поворота и положением водяного знака на страницах документа, как вам может понадобиться."
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
    title_left: "Добавить водяной знак изображения в файл POT в .NET"
    content_left: |
        [GroupDocs.Watermark](/ru/watermark/net/) позволяет разработчикам .NET легко добавлять водяные знаки изображений (BMP, PNG, GIF или JPEG) в свои приложения, выполняя несколько простых шагов.
        * Создайте экземпляр **Watermarker** с входным документом POT.
        * Используйте путь водяного знака изображения в качестве параметра конструктора класса **ImageWatermark**.
        * Установите свойства водяного знака (размер, выравнивание, цвет и т. д.).
        * Добавьте водяной знак к водяному знаку и сгенерируйте выходной документ.
    title_right: "Системные Требования"
    content_right: |
        Перед выполнением приведенного ниже примера кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Visual Studio, Xamarin, MonoDevelop
        * Фреймворки: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Watermark для .NET из [NuGet](https://www.nuget.org/packages/GroupDocs.Watermark).
    code: |
        ```cs
        // Добавляем водяной знак изображения в POT в приложениях C#, ASP.NET, VB.NET и .NET Core
        // Создание водяного маркера с входным документом POT
        using (Watermarker watermarker = new Watermarker(input.pot));
          {
            // Использовать путь к водяному знаку изображения в качестве параметра конструктора класса ImageWatermark
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                // Установка свойств водяного знака (ширина, высота, выравнивание)
                watermark.Width = 140;
                watermark.Height = 140;
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                // Добавляем водяной знак к водяному знаку и генерируем выходной документ
                watermarker.Add(watermark);
                watermarker.Save(output.pot);
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
