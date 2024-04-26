
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:58
draft: false
lang: ru
format: Word
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Редактирование водяных знаков в Word документах"
head_description: "Уточните размещение водяных знаков и обеспечьте безопасность документов с помощью GroupDocs.Watermark for .NET. Легко адаптируйте водяные знаки Word к своим решениям."

############################# Header ############################
title: "Улучшите Word Водяные знаки: .NET Уверенность" 
description: "Обеспечьте подлинность Word документов и целостность бренда с помощью GroupDocs.Watermark for .NET. С уверенностью редактируйте водяные знаки с помощью нашего решения."
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачайте бесплатно на Nuget"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "Узнайте больше"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Повышение безопасности документов Word:** GroupDocs.Watermark for .NET позволяет разработчикам с легкостью повышать безопасность документов. С уверенностью редактируйте водяные знаки в соответствии со своими конкретными требованиями.

############################# Steps ############################
steps:
    enable: true
    title: "Редактируйте водяные знаки в Word документах с помощью .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** позволяет разработчикам .NET легко редактировать водяные знаки в различных Word документах. Вот упрощенное руководство по использованию нашего API в вашем приложении:
      
      1. **Watermarker**. Файл можно указать в виде потока байтов, потока файлов или пути к локальному диску.
      2. **SearchCriteria** для идентификации водяных знаков с соответствующими свойствами, ранее добавленными в документ.
      3. После поиска вы получите список соответствующих водяных знаков. Затем вы можете настроить их свойства, такие как размер, выравнивание страницы, текст, цвет, содержимое изображения и многое другое. Это дает вам полный контроль над данными.
      4. После завершения редактирования водяных знаков сохраните обновленный документ. Для хранения конечного результата можно использовать локальный путь к файлу или поток.
   
    code:
      platform: "net"
      copy_title: "Копировать"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "нажмите, чтобы скопировать"
        copy_done: "скопировал"
      links:
        #  loop
        - title: "Больше примеров"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "Документация"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // Отредактируйте текстовый водяной знак WORD

        // Сделайте водяной маркер, содержащий файл WORD
        using (Watermarker watermarker = new Watermarker("input.docx"))
        {
            // Создайте критерии TextSearchCriteria и получите текстовые водяные знаки
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                 // Редактирование текстового водяного знака
                 watermark.FormattedTextFragments.Clear();
                 watermark.FormattedTextFragments.Add("passed", 
                    new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
            }

            // Сохраните документ
            watermarker.Save("output.docx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Подробнее о модификации водяных знаков"
  description: "Расширьте возможности своих .NET приложений с помощью нашей библиотеки и добавляйте, редактируйте, удаляйте или ищите водяные знаки в различных форматах файлов."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Изменить водяной знак"
  features:
    # feature loop
    - title: "Файлы водяных знаков для вашего бизнеса"
      content: "Используйте GroupDocs.Watermark for .NET для нанесения водяных знаков на файлы и документы. Добавляйте водяные знаки и управляйте ими без дополнительных усилий, внедряя наш API в свои приложения. Ищите, редактируйте и удаляйте ранее добавленные водяные знаки."

    # feature loop
    - title: "Точная настройка водяных знаков в соответствии с вашими требованиями"
      content: "Наш API предлагает полный набор опций настройки. Легко изменяйте такие параметры, как размер, ориентацию, цветовую схему, семейство шрифтов и многое другое, чтобы создать идеальный водяной знак."

    # feature loop
    - title: "Используйте функции, специфичные для документов"
      content: "В зависимости от используемого формата файла вы можете использовать встроенные функции. Сюда могут входить фон документа, аннотации, заголовки или другие элементы, служащие контейнерами для водяных знаков."
      
  code_samples:
    # code sample loop
    - title: "Excel редактирование текста водяного знака"
      content: |
        В этом примере показано, как редактировать текст определенных водяных знаков на листах Excel
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Загрузить электронную таблицу XLSX
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  Загрузить содержимое электронной таблицы
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();

                //  Редактирование внутреннего текста водяного знака
                foreach (SpreadsheetShape shape in content.Worksheets[0].Shapes)
                {
                    if (shape.Text == "GroupDocs 2016")
                    {
                        shape.Text = "GroupDocs 2017";
                    }
                }

                //  Сохранить результат вывода
                watermarker.save("result.xlsx");
            }

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Watermark бесплатно или запросите лицензию"
  items:
    #  loop
    - title: "Nuget скачать"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "Лицензирование"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Повысьте безопасность других форматов"
    exclude: "WORD"
    description: "GroupDocs.Watermark for .NET предлагает эффективные решения для повышения безопасности документов в различных форматах."
    items: 
        # format loop 1
        - name: "Водяной знак PDF"
          format: "PDF"
          link: "/watermark/net/edit//pdf/"
          description: "Формат документа Adobe Portable"

        # format loop 2
        - name: "Водяной знак Word"
          format: "WORD"
          link: "/watermark/net/edit//word/"
          description: "MS Word и документы Open Office"
          
        # format loop 3
        - name: "Водяной знак Excel"
          format: "EXCEL"
          link: "/watermark/net/edit//excel/"
          description: "MS Excel и электронные таблицы Open Office"

        # format loop 4
        - name: "Водяной знак PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/edit//powerpoint/"
          description: "MS PowerPoint и презентации в открытом офисе"

        # format loop 5
        - name: "Водяной знак DOCX"
          format: "DOCX"
          link: "/watermark/net/edit//docx/"
          description: "Открыть XML-документ Microsoft Word"
          
        # format loop 6
        - name: "Водяной знак PPTX"
          format: "PPTX"
          link: "/watermark/net/edit//pptx/"
          description: "PowerPoint Открытая презентация XML"
          
        # format loop 7
        - name: "Водяной знак XLSX"
          format: "XLSX"
          link: "/watermark/net/edit//xlsx/"
          description: "Открытая электронная таблица XML от Майкрософт Excel"

        # format loop 8
        - name: "Водяной знак DOC"
          format: "DOC"
          link: "/watermark/net/edit//doc/"
          description: "Документ Майкрософт Word 97—2007"

        # format loop 9
        - name: "Водяной знак XLS"
          format: "XLS"
          link: "/watermark/net/edit//xls/"
          description: "Рабочая тетрадь Майкрософт Excel 97-2003"

        # format loop 10
        - name: "Водяной знак PPT"
          format: "PPT"
          link: "/watermark/net/edit//ppt/"
          description: "PowerPoint Презентация 97-2003"

        # format loop 11
        - name: "Водяной знак RTF"
          format: "RTF"
          link: "/watermark/net/edit//rtf/"
          description: "Форматированный текстовый формат"

---