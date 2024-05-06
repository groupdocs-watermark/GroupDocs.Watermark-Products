
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:31
draft: false
lang: ru
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Обновить водяные знаки для электронных таблиц Excel"
head_description: "Обновите водяные знаки в электронных таблицах различных форматов, используя GroupDocs.Watermark for Node.js via Java. Обогатите свои Node.js via Java приложения."

############################# Header ############################
title: "Революционизируйте использование водяных знаков в электронных таблицах с помощью Node.js via Java" 
description: "Ощутите всю мощь GroupDocs.Watermark for Node.js via Java. Защитите свои деловые документы различными водяными знаками. Обновите размер водяного знака, выравнивание, угол поворота, положение и т. д."
subtitle: "GroupDocs.Watermark for Node.js via Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачать бесплатно NPM"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "библиотека GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "Узнайте больше"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java — это комплексное решение для управления водяными знаками в среде Node.js via Java. С помощью этого инструмента разработчики могут легко выполнять такие операции, как добавление, редактирование, поиск и удаление водяных знаков из документов в различных форматах файлов, включая PDF, Microsoft Word, Excel, PowerPoint, Visio, электронную почту и графические форматы. GroupDocs.Watermark поддерживает все основные операционные системы и версии Node.js.

############################# Steps ############################
steps:
    enable: true
    title: "Обновите водяные знаки в EXCEL через Node.js via Java"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** предоставляет разработчикам Node.js via Java надежный API для программного обновления водяных знаков в различных документах EXCEL. В этом руководстве описан процесс:
      
      1. Начните процесс, предоставив файл EXCEL в качестве аргумента конструктору класса **Watermarker**. В зависимости от ваших требований файл может быть предоставлен либо в виде потока, либо в виде ссылки на местоположение на локальном диске.
      2. Впоследствии используйте объект **SearchCriteria**, чтобы определить конкретные водяные знаки, требующие изменения. Этот объект позволяет точно определять водяные знаки на основе желаемых свойств.
      3. После успешного выполнения поиска вы получите коллекцию соответствующих водяных знаков. Эти водяные знаки обеспечивают детальный контроль, позволяя обновлять такие свойства, как размеры, расположение страницы, текстовое содержимое, цветовую схему, данные изображения и многое другое.
      4. После завершения обновления водяных знаков сохраните измененный документ. API упрощает хранение, используя либо локальный путь к файлу, либо объект потока.
   
    code:
      platform: "net"
      copy_title: "Копировать"
      install:
        command: "npm i @groupdocs/groupdocs.watermark"
        copy_tip: "нажмите, чтобы скопировать"
        copy_done: "скопировал"
      links:
        #  loop
        - title: "Больше примеров"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
        #  loop
        - title: "Документация"
          link: "https://docs.groupdocs.com/watermark/nodejs-java/"
          
      content: |
        ```javascript {style=abap}

        // Обновить текстовый водяной знак EXCEL

        // Предоставьте экземпляр Watermarker для файла EXCEL.
        const watermarker = new groupdocs.watermark.Watermarker("input.xslx");

        // Используйте TextSearchCriteria для поиска текстовых водяных знаков.
        const searchCriteria = 
            new groupdocs.watermark.TextSearchCriteria("test", false);
        const watermarks = watermarker.search(searchCriteria);
        
        // Обновить текстовый водяной знак
        for (const watermark of watermarks.getInnerList().toArray())
        {
            watermark.setText("passed");
        }

        // Наслаждайтесь результатом
        watermarker.save("output.xslx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Освоение редактирования водяных знаков за PDF с помощью GroupDocs.Watermark"
  description: "Изучите комплексные функции API для настройки водяных знаков и управления ими в PDF s в Node.js via Java приложениях."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Изменить водяной знак"
  features:
    # feature loop
    - title: "Без труда редактируйте водяные знаки за PDF s"
      content: "GroupDocs.Watermark предлагает надежные инструменты в Node.js via Java для удобного редактирования существующих водяных знаков в PDF документах. С легкостью настраивайте положение, прозрачность и многое другое."

    # feature loop
    - title: "Уточните детали водяных знаков для обеспечения точности"
      content: "Возьмите детали под свой контроль. Наш API позволяет точно настроить внешний вид водяных знаков, точно изменяя размер, непрозрачность и цвет ваших PDF s."

    # feature loop
    - title: "Упрощенное управление водяными знаками"
      content: "Наш API упрощает управление водяными знаками. Независимо от того, обновляете ли вы или удаляете водяные знаки, вы можете эффективно управлять водяными знаками, сохраняя целостность документов и удовлетворяя потребности в брендинге."
      
  code_samples:
    # code sample loop
    - title: "Java Пример: отредактируйте водяной знак PDF"
      content: |
        В этом примере Java показано, как редактировать существующий водяной знак в документе PDF и как программно настроить его свойства.
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Загрузите документ PDF для обработки
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  Найдите конкретные водяные знаки, соответствующие вашим критериям
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria("test", false);
            const watermarks = watermarker.search(searchCriteria);
  
            //  Отредактируйте настройки водяного знака, такие как размер, цвет и положение
            for (const watermark of watermarks.getInnerList().toArray()) {
                watermark.getFormattedTextFragments().clear();
                watermark.getFormattedTextFragments().add("passed", 
                    new groupdocsWatermark.Font("Calibri", 19, groupdocsWatermark.FontStyle.Bold), 
                    groupdocsWatermark.Color.getRed(), groupdocsWatermark.Color.getAqua());
            }

            //  Сохраните обновленный документ в локальной системе или передайте его напрямую
            watermarker.save("result.pdf");
            watermarker.close();

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Watermark бесплатно или запросите лицензию"
  items:
    #  loop
    - title: "NPM скачать"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      color: "red"
        #  loop
    - title: "Лицензирование"
      link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Обновление водяных знаков в поддерживаемых форматах файлов"
    exclude: "EXCEL"
    description: "Эффективно обновляйте водяные знаки в PDF, Word, Excel и других системах с помощью GroupDocs.Watermark for Node.js via Java. Документы с водяными знаками могут обогатить ваши бизнес-процессы."
    items: 
        # format loop 1
        - name: "Водяной знак PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/update//pdf/"
          description: "Формат документа Adobe Portable"

        # format loop 2
        - name: "Водяной знак Word"
          format: "WORD"
          link: "/watermark/nodejs-java/update//word/"
          description: "MS Word и документы Open Office"
          
        # format loop 3
        - name: "Водяной знак Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/update//excel/"
          description: "MS Excel и электронные таблицы Open Office"

        # format loop 4
        - name: "Водяной знак PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/update//powerpoint/"
          description: "MS PowerPoint и презентации в открытом офисе"

        # format loop 5
        - name: "Водяной знак DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/update//docx/"
          description: "Открыть XML-документ Microsoft Word"
          
        # format loop 6
        - name: "Водяной знак PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/update//pptx/"
          description: "PowerPoint Открытая презентация XML"
          
        # format loop 7
        - name: "Водяной знак XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/update//xlsx/"
          description: "Открытая электронная таблица XML от Майкрософт Excel"

        # format loop 8
        - name: "Водяной знак DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/update//doc/"
          description: "Документ Майкрософт Word 97—2007"

        # format loop 9
        - name: "Водяной знак XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/update//xls/"
          description: "Рабочая тетрадь Майкрософт Excel 97-2003"

        # format loop 10
        - name: "Водяной знак PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/update//ppt/"
          description: "PowerPoint Презентация 97-2003"

        # format loop 11
        - name: "Водяной знак RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/update//rtf/"
          description: "Форматированный текстовый формат"

---