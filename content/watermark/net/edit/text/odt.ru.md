---
############################# Static ############################
layout: "autogen-child"
draft: false
path: "watermark/net/edit/text/odt/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST
############################# Head ############################
head_title: "Редактировать текстовый водяной знак в ODT в C#, ASP.NET, VB.NET"
head_description: ".NET для редактирования найденного текстового водяного знака в файле ODT в приложениях C#, ASP.NET, VB.NET и .NET Core с использованием API-интерфейсов GroupDocs.Watermark для .NET."
############################# Header ############################
title: "Редактировать текстовый водяной знак в ODT в C# .NET"
description: "Найдите и измените найденный текстовый водяной знак в документе ODT с форматированием в приложениях C#, ASP.NET, VB.NET и .NET Core. Управляйте размером водяного знака, типом шрифта, углом поворота и положением водяного знака на страницах документа, как вам может понадобиться."
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
    title_left: "Редактировать текстовый водяной знак в файле ODT в .NET"
    content_left: |
        [GroupDocs.Watermark](/ru/watermark/net/) позволяет разработчикам .NET легко редактировать текстовые водяные знаки в своих приложениях, выполняя несколько простых шагов.
        * Создайте экземпляр **Watermarker* с входным документом ODT.
        * Инициализируйте **TextSearchCriteria**, чтобы найти текстовые водяные знаки.
        * Редактировать текст найденных водяных знаков
        * Редактировать и устанавливать свойства водяного знака (стиль шрифта, цвет и т. д.).
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
        // Поиск и замена текстового водяного знака форматированием в ODT в приложениях C#, ASP.NET, VB.NET и .NET Core
        // Создаем водяной маркер с входным ODT-документом
        using (Watermarker watermarker = new Watermarker(input.odt));
          {
            // Инициализируем TextSearchCriteria для поиска текстовых водяных знаков
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
                {
                    try
                        {
                            // Редактируем текст и устанавливаем свойства водяного знака
                            watermark.FormattedTextFragments.Clear();
                            watermark.FormattedTextFragments.Add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
                        }
                    catch (Exception e)
                    {
                        // Найденный объект может не поддерживать редактирование текста
                        // Передаваемые аргументы могут иметь недопустимое значение
                        // Обрабатываем такие случаи здесь
                    }
                }
            // Сохраняем документ с водяным знаком
            watermarker.Save(output.odt);
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
