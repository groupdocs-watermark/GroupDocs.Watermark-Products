
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:20
draft: false
lang: ru
format: Image
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Динамические водяные знаки для защиты изображений"
head_description: "Защитите свои авторские права на изображения с помощью динамических водяных знаков Node.js. Поддерживает JPG, PNG, WEBP и многое другое."

############################# Header ############################
title: "Динамические водяные знаки для защиты изображений с помощью Node.js" 
description: "Используйте наш набор инструментов Node.js для создания динамических и безопасных водяных знаков на изображениях, поддерживая такие форматы, как JPG, PNG и WEBP. Обеспечьте свои авторские права на изображения с помощью расширенных функций защиты."
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачайте бесплатно на NPM"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "Узнайте больше"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       С помощью GroupDocs.Watermark for Node.js via Java нанесение водяных знаков на изображения очень просто и легко настраивается. Этот набор инструментов поддерживает широкий спектр форматов изображений, включая традиционные растровые изображения, такие как JPG и PNG, а также новые форматы, такие как WEBP. Он позволяет разработчикам динамически добавлять водяные знаки, которые не только безопасны, но и естественным образом сочетаются с содержимым изображения, обеспечивая надежную защиту от нарушения авторских прав без ущерба для первоначальной привлекательности изображения.

############################# Steps ############################
steps:
    enable: true
    title: "Защита деловых документов: создание водяных знаков для форматов Image"
    content: |
      Повысьте безопасность своих документов с помощью **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/):** внедрите наш API в свои приложения и создавайте водяные знаки для многих поддерживаемых форматов файлов.
      
      1. **Начать создание водяных знаков.** Начните обработку документа с помощью класса **Watermarker**, предоставляющего наши основные функции. Создайте его экземпляр, передав конструктору файл Image, который должен быть защищен сгенерированными водяными знаками.
      2. **Создайте основной объект водяного знака.** Улучшите свои документы, создавая уникальные объекты **Watermark**. Помимо простых страниц, они легко интегрируются с собственными элементами, такими как вложения или заголовки, повышая уровень безопасности и профессионализма.
      3. **Уточнение атрибутов водяных знаков.** Точно настраивайте водяные знаки, регулируя размеры, выравнивание и цветовые схемы. Каждая деталь повышает целостность документа, делая ваши файлы безошибочно вашими.
      4. **Реализуйте с точностью:** используйте метод **Watermarker**, чтобы безупречно применять настроенные водяные знаки. Независимо от того, одиночный или множественный, каждый водяной знак добавляет дополнительный уровень защиты. Для дополнительной безопасности рассмотрите возможность хранения обработанных документов в отдельном безопасном месте.
   
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

        // Создать текстовый водяной знак для IMAGE

        // Передать исходный файл в экземпляр Watermarker.
        const watermarker = new groupdocs.watermark.Watermarker("input.jPEG");
        
        // Создайте текстовый водяной знак и установите его параметры.
        const  watermark = new groupdocs.watermark.TextWatermark
            ("My Watermark", groupdocs.watermark.new Font("Arial", 36));

        // Получить результат IMAGE
        watermarker.add(watermark);
        watermarker.save("output.jPEG");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Передовые методы нанесения водяных знаков"
  description: "Откройте для себя передовые методы нанесения водяных знаков с помощью нашего надежного API, разработанного для беспрепятственной интеграции в среду .NET. Идеально подходит для добавления сложных и надежных водяных знаков на самые разные типы документов, включая презентации, юридические документы и технические диаграммы."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Изысканный водяной знак"
  features:
    # feature loop
    - title: "Динамическое размещение водяных знаков"
      content: "Наш API предлагает варианты динамического размещения водяных знаков, которые адаптируют позиционирование водяных знаков в зависимости от содержимого документа. Эта функция идеально подходит для сложных макетов презентаций и технических диаграмм и обеспечивает оптимальное размещение водяных знаков без ущерба для читаемости исходной информации."

    # feature loop
    - title: "Повышенная безопасность с помощью невидимых водяных знаков"
      content: "Используйте невидимые водяные знаки, обеспечивающие надежную защиту без изменения внешнего вида документов. Эти водяные знаки предназначены для обнаружения только с помощью специальных программных инструментов, поэтому они идеально подходят для защиты конфиденциальной информации в юридических и финансовых документах."

    # feature loop
    - title: "Автоматизированные рабочие процессы нанесения водяных знаков"
      content: "Упростите процессы защиты документов с помощью автоматизированных рабочих процессов нанесения водяных знаков. Настройте правила, основанные на типе документа, степени секретности содержимого и уровнях доступа пользователей, чтобы автоматически наносить водяные знаки и обеспечивать соблюдение единых протоколов безопасности во всех документах."
      
  code_samples:
    # code sample loop
    - title: "Сгенерировать водяной знак для вложений PDF"
      content: |
        В этом примере показано, как создавать водяные знаки во всех вложениях PDF
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Загрузить документ PDF
            const loadOptions = new groupdocsWatermark.PdfLoadOptions();
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf", loadOptions);
            const pdfContent = watermarker.getContent(groupdocsWatermark.PdfContent.class);

            //  Сгенерировать текстовый водяной знак
            const watermark = new groupdocsWatermark.TextWatermark('WaterMark', new groupdocsWatermark.Font('Arial', 19));
  
            //  Добавьте водяной знак к подходящим вложениям
            for (const attachment of pdfContent.getAttachments().getInnerList().toArray()) {
                const info = attachment.getDocumentInfo();
                if (info.getFileType() !== groupdocsWatermark.FileType.Unknown && !info.isEncrypted()) {
                    const attachedWatermarker = attachment.createWatermarker();
                    attachedWatermarker.add(watermark);
                    attachment.updateContent(attachedWatermarker);
                    attachedWatermarker.close();
                }
            }

            //  Сохранить обработанное PDF
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
    title: "Внедрение удивительных водяных знаков в изображения с помощью JavaScript"
    exclude: "IMAGE"
    description: "Эффективно защищайте свои авторские права на изображения с помощью нашего API Node.js. Динамически добавляйте водяные знаки в файлы JPG, PNG и WEBP, гарантируя, что каждое изображение помечено в качестве законного владельца."
    items: 
        # format loop 1
        - name: "Водяной знак PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/generate//pdf/"
          description: "Формат документа Adobe Portable"

        # format loop 2
        - name: "Водяной знак Word"
          format: "WORD"
          link: "/watermark/nodejs-java/generate//word/"
          description: "MS Word и документы Open Office"
          
        # format loop 3
        - name: "Водяной знак Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/generate//excel/"
          description: "MS Excel и электронные таблицы Open Office"

        # format loop 4
        - name: "Изображение водяного знака"
          format: "IMAGE"
          link: "/watermark/nodejs-java/generate//image/"
          description: "Популярные форматы изображений"

        # format loop 5
        - name: "Фото водяного знака"
          format: "PHOTO"
          link: "/watermark/nodejs-java/generate//photo/"
          description: "Форматы фотографий"

        # format loop 6
        - name: "Водяной знак PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/generate//powerpoint/"
          description: "MS PowerPoint и презентации в открытом офисе"

        # format loop 7
        - name: "Водяной знак DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/generate//docx/"
          description: "Открыть XML-документ Microsoft Word"
          
        # format loop 8
        - name: "Водяной знак PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/generate//pptx/"
          description: "PowerPoint Открытая презентация XML"
          
        # format loop 9
        - name: "Водяной знак XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/generate//xlsx/"
          description: "Открытая электронная таблица XML от Майкрософт Excel"

        # format loop 10
        - name: "Водяной знак JPEG"
          format: "JPEG"
          link: "/watermark/nodejs-java/generate//jpeg/"
          description: "JPEG Изображение"

        # format loop 11
        - name: "Водяной знак PNG"
          format: "PNG"
          link: "/watermark/nodejs-java/generate//png/"
          description: "Portable Сетевая графика"

        # format loop 12
        - name: "Водяной знак TIFF"
          format: "TIFF"
          link: "/watermark/nodejs-java/generate//tiff/"
          description: "Формат файла изображения тега"

        # format loop 13
        - name: "Водяной знак WEBP"
          format: "WEBP"
          link: "/watermark/nodejs-java/generate//webp/"
          description: "Изображение в Интернете"

        # format loop 14
        - name: "Водяной знак DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/generate//doc/"
          description: "Документ Майкрософт Word 97—2007"

        # format loop 15
        - name: "Водяной знак XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/generate//xls/"
          description: "Рабочая тетрадь Майкрософт Excel 97-2003"

        # format loop 16
        - name: "Водяной знак PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/generate//ppt/"
          description: "PowerPoint Презентация 97-2003"

        # format loop 17
        - name: "Водяной знак RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/generate//rtf/"
          description: "Форматированный текстовый формат"

---