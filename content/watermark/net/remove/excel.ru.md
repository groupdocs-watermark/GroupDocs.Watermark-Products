
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:19
draft: false
lang: ru
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Excel Удаление водяных знаков с помощью API C# .NET "
head_description: "Используйте наш API C# .NET для эффективного удаления водяных знаков в документах Excel и управления ими, обеспечивая четкость данных и целостность листов."

############################# Header ############################
title: "C# .NET для операций с водяными знаками Excel" 
description: "Усовершенствуйте рабочие процессы с документами Excel в средах .NET, легко удаляя или редактируя водяные знаки с помощью инструментов, разработанных для обеспечения точности и простоты использования."
subtitle: "GroupDocs.Watermark for .NET C# API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Бесплатная загрузка пакета Nuget"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "Библиотека GroupDocs.Watermark for .NET C#"
    link: "/watermark/net/"
    link_title: "Узнайте больше"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       Библиотека GroupDocs.Watermark for .NET C# предоставляет надежные инструменты для управления водяными знаками в файлах Excel. От удаления ненужных знаков до редактирования существующих — она обеспечивает комплексный контроль водяных знаков, что идеально подходит для компаний, которые уделяют первостепенное внимание чистоте документов и профессионализму.

############################# Steps ############################
steps:
    enable: true
    title: "Удаление водяных знаков из документов Excel с помощью .NET"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/)** упрощает задачу удаления водяных знаков из деловых документов. Расширьте возможности своего приложения .NET, интегрировав нашу библиотеку, и выполните следующие простые шаги:
      
      1. Начните с создания экземпляра основного класса **Watermarker** с документом Excel. Наш API поддерживает обработку документов, предоставляемых в виде потока или локального пути.
      2. Используйте **SearchCriteria**, чтобы сузить набор водяных знаков, подлежащих обработке. Вы можете использовать различные параметры, такие как изображения, текст или функции форматирования. Чем конкретнее вы укажите параметры поиска, тем более точные результаты вы получите.
      3. Обработать список водяных знаков документа, полученный в результате поиска, и удалить их из документа.
      4. После удаления водяных знаков сохраните полученный документ как локальный файл или байтовый поток.
   
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
        // Удалить текстовый водяной знак из документа Excel

        // Предоставьте экземпляр Watermarker для исходного документа документа Excel.
        using (Watermarker watermarker = new Watermarker("input.xslx"))
        {
            // Удалить выбранные водяные знаки из документа
            TextFormattingSearchCriteria criteria = new TextFormattingSearchCriteria();
            criteria.ForegroundColorRange = new ColorRange();
            criteria.FontBold = true;
            PossibleWatermarkCollection watermarks = watermarker.Search(criteria);
            watermarks.Clear();

            // Сохранить файл по указанному пути
            watermarker.Save("output.xslx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Упростите удаление водяных знаков с помощью API C# .NET"
  description: "Откройте для себя мощные возможности удаления водяных знаков в нашем API C# .NET, разработанном для беспрепятственной интеграции с вашими приложениями .NET. Эффективно удаляйте или очищайте водяные знаки из PDF и офисных документов, сохраняя исходное качество файлов."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "Удалить водяной знак"
  features:
    # feature loop
    - title: "Точное удаление водяных знаков"
      content: "Наш API .NET предоставляет точные инструменты для чистого удаления водяных знаков из любого документа. Эта функция, разработанная специально для разработчиков, гарантирует, что удаление водяных знаков не ухудшит качество или макет документа."

    # feature loop
    - title: "Автоматическое массовое удаление водяных знаков"
      content: "Автоматизируйте процесс удаления водяных знаков из больших наборов документов с помощью нашего API .NET. Идеально подходит для компаний, обрабатывающих большие объемы документов, и позволяет повысить эффективность и безопасность документов."

    # feature loop
    - title: "Расширенные функции редактирования водяных знаков"
      content: "Используйте расширенные функции для выборочного редактирования или изменения водяных знаков. Наш API поддерживает детальные настройки, чтобы ваши документы выглядели профессионально и при этом сохраняли конфиденциальную информацию."
      
  code_samples:
    # code sample loop
    - title: "Удалить текстовый водяной знак в электронных таблицах"
      content: |
        Как удалить текстовые водяные знаки с помощью специального форматирования в документах Excel.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Загрузить рабочую книгу Excel
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  Получите контент и найдите подходящий водяной знак
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();
                foreach (SpreadsheetWorksheet section in content.Worksheets)
                {
                    for (int i = section.Shapes.Count - 1; i >= 0; i--)
                    {
                        foreach (FormattedTextFragment fragment in section.Shapes[i].FormattedTextFragments)
                        {
                            if (fragment.ForegroundColor.Equals(Color.Red) && fragment.Font.FamilyName == "Arial")
                            {
                                //  Удалить текстовый водяной знак
                                section.Shapes.RemoveAt(i);
                                break;
                            }
                        }
                    }
                }

                //  Сохранить обработанное XLSX
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
    title: "Упрощение процесса удаления водяных знаков Excel в .NET"
    exclude: "EXCEL"
    description: "Узнайте, как использовать API GroupDocs.Watermark for .NET C# для эффективного удаления водяных знаков с Excel листов, обеспечивая безупречную и презентабельную финансовую отчетность и анализ данных."
    items: 
        # format loop 1
        - name: "Водяной знак PDF"
          format: "PDF"
          link: "/watermark/net/remove//pdf/"
          description: "Формат документа Adobe Portable"

        # format loop 2
        - name: "Водяной знак Word"
          format: "WORD"
          link: "/watermark/net/remove//word/"
          description: "MS Word и документы Open Office"
          
        # format loop 3
        - name: "Водяной знак Excel"
          format: "EXCEL"
          link: "/watermark/net/remove//excel/"
          description: "MS Excel и электронные таблицы Open Office"

        # format loop 4
        - name: "Водяной знак PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/remove//powerpoint/"
          description: "MS PowerPoint и презентации в открытом офисе"

        # format loop 5
        - name: "Водяной знак DOCX"
          format: "DOCX"
          link: "/watermark/net/remove//docx/"
          description: "Открыть XML-документ Microsoft Word"
          
        # format loop 6
        - name: "Водяной знак PPTX"
          format: "PPTX"
          link: "/watermark/net/remove//pptx/"
          description: "PowerPoint Открытая презентация XML"
          
        # format loop 7
        - name: "Водяной знак XLSX"
          format: "XLSX"
          link: "/watermark/net/remove//xlsx/"
          description: "Открытая электронная таблица XML от Майкрософт Excel"

        # format loop 8
        - name: "Водяной знак DOC"
          format: "DOC"
          link: "/watermark/net/remove//doc/"
          description: "Документ Майкрософт Word 97—2007"

        # format loop 9
        - name: "Водяной знак XLS"
          format: "XLS"
          link: "/watermark/net/remove//xls/"
          description: "Рабочая тетрадь Майкрософт Excel 97-2003"

        # format loop 10
        - name: "Водяной знак PPT"
          format: "PPT"
          link: "/watermark/net/remove//ppt/"
          description: "PowerPoint Презентация 97-2003"

        # format loop 11
        - name: "Водяной знак RTF"
          format: "RTF"
          link: "/watermark/net/remove//rtf/"
          description: "Форматированный текстовый формат"

---