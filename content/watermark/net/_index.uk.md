---
############################# Static ############################
layout: "landing"
date: 2024-04-26T21:39:08
draft: false

lang: uk
product: "Watermark"
product_tag: "watermark"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "C# .NET Програмне забезпечення для водяних знаків документа | додати водяний знак"
head_description: "C# .NET Бібліотека для додавання, пошуку та видалення водяних знаків у документах: PDF, Word, Excel, презентації, Visio діаграми, електронні листи та формати файлів зображень."

############################# Header ############################
title: "Документи водяних знаків легко у ваших програмах C # .NET"
description: "Розширюйте можливості C# за допомогою гнучкого API водяного маркування документів, який забезпечує додавання настроюваних водяних знаків до всіх популярних форматів документів."
words:
  for: "для"

actions:
  main: "Безкоштовно NuGet Завантажити"
  main_link: "https://www.nuget.org/packages/GroupDocs.Watermark"
  alt: "Ліцензування"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/net/"
  title: "Готові розпочати роботу?"
  description: "Спробуйте GroupDocs.Watermark функцій безкоштовно або попросіть ліцензію"

release:
  title: "Випущена версія {0}"
  notes: "Подивіться, що нового"
  downloads: "Завантаження"

code:
  title: "Водяний знак PDF файлів у C#"
  more: "Більше прикладів"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
  install: "dotnet add package GroupDocs.Watermark"
  content: |
    ```csharp {style=abap}   
    // Принциповувати водяний маркер, що проходить шлях PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    using (Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions))
    {
        // Налаштування параметрів водяного знака
        TextWatermark textWatermark = 
            new TextWatermark("Approved", new Font("Arial", 8));
        
        // Застосувати водяний знак до документа PDF
        watermarker.Add(textWatermark);

        // Зберегти документ результату
        watermarker.Save("result.pdf");
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark з першого погляду"
  description: "API для розміщення водяних знаків на документи через .NET"
  features:
    # feature loop
    - title: "C # файли водяний знак"
      content: "Додайте водяні знаки до своїх бізнес-файлів за допомогою GroupDocs.Watermark. Використовуйте текст, зображення, діаграми або вкладення електронної пошти."

    # feature loop
    - title: "Налаштуйте водяні знаки відповідно до своїх цілей"
      content: "GroupDocs.Watermark for .NET програмне забезпечення дозволяє налаштовувати водяні знаки різними способами. Стилі тексту, такі як жирний, курсив, типи шрифтів, а також властивості зображення, такі як обертання тощо, збагачують процес водяного маркування."

    # feature loop
    - title: "Підтримуються всі популярні формати файлів"
      content: "Багато форматів файлів і документів підтримуються рішенням GroupDocs.Watermark. PDF, Microsoft Office Word, Excel, PowerPoint, зображення на кшталт JPEG, PNG, GIF, BMP, Visio діаграми, електронні листи тощо можуть бути захищені нашими водяними знаками."

    # feature loop
    - title: "Пошук і оновлення водяних знаків"
      content: "Водяні знаки, які вже представлені в документі, можуть бути знайдені та оброблені знову. Змінюйте текст, стиль, зображення або видаліть відкриті водяні знаки без додаткових зусиль."

############################# Platforms ############################
platforms:
  enable: true
  title: "Незалежність платформи"
  description: "GroupDocs.Watermark for .NET підтримує операційні системи, фреймворки та менеджери пакетів, перераховані нижче"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Підтримувані формати файлів"
  description: |
    GroupDocs.Watermark for .NET забезпечує обробку наступних [форматів файлів](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office & OpenDocument формати
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### Зображення та графіка
        * **Популярні формати зображень:** BMP, JPG, JPEG, PNG
        * **Багатосторінкові зображення:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### Інше
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark особливості"
  description: "Захист PDF, Office, зображень та інших форматів водяним знаком"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Водяний знак документів"
      content: "Додайте або видаліть водяні знаки з певного розділу або цілого документа різних форматів файлів."

    # feature loop
    - icon: "watermark_style"
      title: "Стилізуйте водяний знак"
      content: "Налаштуйте різні властивості водяного знака, такі як колір, шрифт, обертання тощо."

    # feature loop
    - icon: "hidden_print"
      title: "PDF прихований друкарський водяний знак"
      content: "Виділіть прихований водяний знак до PDF, який відображається лише під час друку документа."

    # feature loop
    - icon: "image_only"
      title: "Водяний знак лише зображення в документах"
      content: "Встановіть водяний знак усіх зображень у певному розділі, сторінці, слайді чи документі."

    # feature loop
    - icon: "image_frame"
      title: "Обробка вибраних кадрів зображень"
      content: "Призначте водяний знак лише окремим кадрам багаторамкового зображення."

    # feature loop
    - icon: "attachments"
      title: "Навісне обладнання та форми"
      content: "Встановіть водяний знак для всіх вкладень у документі Excel та всіх фігур зображень у слайдах."

    # feature loop
    - icon: "pdf_objects"
      title: "PDF об'єктів"
      content: "Вирівняти водяний знак за рамкою обрізки, картинною скринькою, рамкою обрізки або полем обрізки у документі PDF."

    # feature loop
    - icon: "doc_background"
      title: "Передумови документів"
      content: "Розмістіть водяний знак або видаліть його з фонових зображень електронної таблиці або слайдів."

    # feature loop
    - icon: "unreadable_characters"
      title: "Захист нечитабельних символів"
      content: "Захистіть текстовий водяний знак за допомогою нечитаних символів у презентаціях."

    # feature loop
    - icon: "watermark_text_search"
      title: "Пошук водяних знаків у документах"
      content: "Шукайте водяні знаки на основі конкретних параметрів або комбінуючи кілька критеріїв."

    # feature loop
    - icon: "watermark_image_search"
      title: "Пошук схожих зображень водяних знаків"
      content: "Шукайте водяні знаки зображення, які нагадують конкретне зображення."

    # feature loop
    - icon: "document_info"
      title: "Отримати інформацію про документ"
      content: "Програмно витягніть налаштування сторінки та іншу інформацію для підтримуваних форматів."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Зразки коду"
  description: "Деякі випадки використання типових GroupDocs.Watermark for .NET операцій"
  items:
    # code sample loop
    - title: "Водяний знак шляхом додавання зображення до документа."
      content: |
        Для захисту будь-якого документа ви можете використовувати [водяні знаки зображення](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/):
        {{< landing/code title="Як захистити файл водяним знаком зображення.">}}
        ```csharp {style=abap}
        // Завантажте вихідний документ у Watermarker
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Вкажіть шлях до зображення водяного знака
            using (ImageWatermark watermark = new ImageWatermark("watermark.jpg"))
            {
                // Захистіть файл і збережіть його
                watermarker.Add(watermark);

                watermarker.Save("result.pdf");
            }
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Пошук і зміна існуючих водяних знаків."
      content: |
        GroupDocs.Watermark може [змінювати водяні знаки](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/), які вже представлені в документі. Шукайте потрібні елементи та оновлюйте їх властивості.
        {{< landing/code title="Пошук і модифікація водяних знаків.">}}
        ```csharp {style=abap}   
        // Завантажити вихідний документ
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Пошук водяних знаків для оновлення
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                // Оновлення бажаних властивостей
                watermark.Text = "New Text";
            }

            // Збереження зміненого документа у вказаний шлях
            watermarker.Save("document.pdf");
        }
        ```
        {{< /landing/code >}}

---
