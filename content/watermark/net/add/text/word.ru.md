---
############################# Static ############################
layout: "autogen-child"
draft: false
path: "watermark/net/add/text/word/"
otherformats: PDF EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST
############################# Head ############################
head_title: "Добавить текстовый водяной знак в WORD в C#, ASP.NET, VB.NET"
head_description: ".NET для добавления текстового водяного знака в файл WORD в приложениях C#, ASP.NET, VB.NET и .NET Core с использованием API-интерфейсов GroupDocs.Watermark для .NET."
############################# Header ############################
title: "Добавить текстовый водяной знак в WORD в C# .NET"
description: "Добавление текстового водяного знака в файл WORD в приложениях C#, ASP.NET, VB.NET и .NET Core. Управляйте размером водяного знака, типом шрифта, углом поворота и положением водяного знака на страницах документа, как вам может понадобиться."
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
    title_left: "Добавить текстовый водяной знак в файл WORD в .NET"
    content_left: |
        [GroupDocs.Watermark](/ru/watermark/net/) позволяет разработчикам .NET легко добавлять текстовые водяные знаки в свои приложения, выполняя несколько простых шагов.
        * Создание экземпляра **Watermarker** с входным документом WORD.
        * Инициализируйте **Font**, который будет использоваться для водяного знака.
        * Создайте объект **TextWatermark**.
        * Установите свойства водяного знака (выравнивание, цвет и т. д.).
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
        // Добавляем текстовый водяной знак в WORD в приложениях C#, ASP.NET, VB.NET и .NET Core
        // Создание водяного маркера с входным документом WORD
        using (Watermarker watermarker = new Watermarker(input.word));
          {
            // Инициализируем шрифт, который будет использоваться для водяного знака
            Font font = new Font("Arial", 19, FontStyle.Bold | FontStyle.Italic);
            // Создаем объект TextWatermark
            TextWatermark watermark = new TextWatermark("my watermark", font);
            // Установить свойства водяного знака
            watermark.ForegroundColor = Color.Red;
            watermark.BackgroundColor = Color.Blue;
            watermark.TextAlignment = TextAlignment.Right;
            watermark.Opacity = 0.5;
            // Добавляем водяной знак и сохраняем изображение с водяным знаком
            watermarker.Add(watermark);
            watermarker.Save(output.word);
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
