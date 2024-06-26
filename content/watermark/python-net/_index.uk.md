---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:49
draft: false

lang: uk
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

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
    # supported_platforms loop
    - title: "Python"
      tag: "python-net"

############################# Head ############################
head_title: "Python Бібліотека водяних знаків | Водяні знаки документа"
head_description: "Python захищає ділові документи текстовими та графічними водяними знаками. Підтримуються такі формати файлів, як PDF, Word, Excel і PowerPoint."

############################# Header ############################
title: "Доступ до технології водяних знаків Python via .NET"
description: "Захистіть свої дані та запобігайте несанкціонованому копіюванню за допомогою цього рішення Python. Легко додавайте водяні знаки до ділових документів у різних форматах, включаючи PDF, Word, Excel, PowerPoint, зображення тощо."
words:
  for: "для"

actions:
  main: "PyPi завантажити безкоштовно"
  main_link: "https://pypi.org/project/groupdocs-watermark-net/"
  alt: "Ліцензування"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
  title: "Готові розпочати роботу?"
  description: "Спробуйте GroupDocs.Watermark функцій безкоштовно або попросіть ліцензію"

release:
  title: "Випущена версія {0}"
  notes: "Подивіться, що нового"
  downloads: "Завантаження"
  link: "https://releases.groupdocs.com/watermark/python-net/"

code:
  title: "Додайте водяний знак до PDF за допомогою Python"
  more: "Більше прикладів"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
  install: "pip install groupdocs-watermark-net"
  content: |
    ```python {style=abap}

    import groupdocs.watermark as gw
    import groupdocs.watermark.watermarks as gww
    import groupdocs.watermark.options.pdf as gwop
    import groupdocs.watermark.common as gwc

    # Принциповувати водяний маркер, що проходить шлях PDF
    pdf_lo = gwop.PdfLoadOptions()
    with gw.Watermarker("source.pdf", pdf_lo) as watermarker:
        options = gwop.PdfArtifactWatermarkOptions()

        # Налаштування параметрів водяного знака
        text_watermark = 
            gww.TextWatermark("Approved", gww.Font("Arial", 8.0))
        text_watermark.horizontal_alignment = 
            gwc.HorizontalAlignment.RIGHT

        # Застосувати водяний знак до документа PDF
        watermarker.add(text_watermark, options)

        # Зберегти документ результату
        watermarker.save("result.pdf")

    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark з першого погляду"
  description: "Python бібліотека водяних знаків"
  features:
    # feature loop
    - title: "Водяні знаки документа Python"
      content: "Захистіть свої конфіденційні дані за допомогою GroupDocs.Watermark for Python via .NET. Розмістіть текст або зображення на файлах різних форматів як водяні знаки."

    # feature loop
    - title: "Налаштувати водяні знаки"
      content: "У GroupDocs.Watermark for Python via .NET доступно багато параметрів налаштування. Налаштуйте стилі тексту (жирний, курсив, шрифт) або властивості зображення, як-от розмір або поворот, щоб налаштувати водяні знаки документа."

    # feature loop
    - title: "Підтримка популярних форматів файлів"
      content: "GroupDocs.Watermark for Python via .NET підтримує широкий спектр форматів файлів, зокрема PDF, документи MS Office, як-от Word, Excel, PowerPoint, а також зображення, як-от JPEG, PNG, GIF, BMP, діаграми Visio, електронні листи тощо. Покращуйте обробку документів для задоволення потреб бізнесу цілі."

    # feature loop
    - title: "Пошук і оновлення водяних знаків"
      content: "Отримувати та оновлювати водяні знаки, розміщені в документах. Змініть стиль тексту, вміст зображення або повністю видаліть їх. GroupDocs.Watermark for Python via .NET пропонує широкий спектр можливостей обробки водяних знаків."

############################# Platforms ############################
platforms:
  enable: true
  title: "Незалежність платформи"
  description: "GroupDocs.Watermark for Python via .NET легко інтегрується з різними операційними системами та менеджерами пакетів."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Підтримувані формати файлів"
  description: |
    GroupDocs.Watermark for Python via .NET дає змогу обробляти різноманітні формати файлів. [Ознайомтеся з повним списком](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "Функції GroupDocs.Watermark for Python via .NET"
  description: "Підвищте безпеку документів за допомогою програмних водяних знаків. Обробляйте різноманітні формати файлів, включаючи PDF, DOCX, XLSX, PPTX і формати зображень (PNG, JPG тощо)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Точний контроль водяних знаків"
      content: "Точне керування водяними знаками, додаючи або видаляючи їх із певних розділів, цілих документів або окремих вкладень і фігур у різних форматах файлів."

    # feature loop
    - icon: "watermark_style"
      title: "Налаштувати вигляд водяного знака"
      content: "Здійснюйте точний контроль над естетикою водяних знаків, змінюючи такі атрибути, як колір, шрифт, непрозорість, обертання та розташування в документі."

    # feature loop
    - icon: "hidden_print"
      title: "Друк PDF із водяними знаками"
      content: "Додайте приховані водяні знаки в звичайні документи, які стають видимими лише під час процесу друку, непомітно підвищуючи безпеку документа."

    # feature loop
    - icon: "image_only"
      title: "Водяні знаки спеціального зображення"
      content: "Водяний знак на певних зображеннях у документі за допомогою нашого рішення. Вставте водяні знаки у визначений розділ (наприклад, на сторінку, слайд) або по всьому документу."

    # feature loop
    - icon: "image_frame"
      title: "Багатошарові зображення водяних знаків"
      content: "Додайте водяні знаки точно до певних кадрів у форматі багатокадрового зображення, досягаючи детального контролю над розміщенням водяних знаків."

    # feature loop
    - icon: "attachments"
      title: "Комплексний захист вмісту"
      content: "Поширте захист на різні елементи документа, як-от вкладення в документах Excel і форми зображень у презентаціях, забезпечуючи додатковий рівень безпеки."

    # feature loop
    - icon: "pdf_objects"
      title: "Розширені водяні знаки PDF"
      content: "Водяні знаки на різних ділянках PDF-файлів, у тому числі на Bleed Box, Art Box, Crop Box, Trim Box тощо."

    # feature loop
    - icon: "doc_background"
      title: "Водяний знак фонового зображення"
      content: "Керуйте водяними знаками на фонових зображеннях електронних таблиць і презентацій, пропонуючи додаткові параметри налаштування для візуальних заходів безпеки."

    # feature loop
    - icon: "unreadable_characters"
      title: "Текстовий водяний знак із нечитабельними символами"
      content: "Використовуйте нечитабельні символи в текстових водяних знаках, вбудованих у презентації, підвищуючи безпеку, значно ускладнюючи несанкціоноване вилучення водяних знаків."

    # feature loop
    - icon: "watermark_text_search"
      title: "Розширений пошук водяних знаків"
      content: "Використовуйте комплексні функції пошуку, щоб знаходити водяні знаки в документах на основі певних параметрів або комбінуючи різні критерії."

    # feature loop
    - icon: "watermark_image_search"
      title: "Виявлення водяного знака подібного зображення"
      content: "Знайдіть схожі зображення водяних знаків у документах, які візуально нагадують вихідне зображення."

    # feature loop
    - icon: "document_info"
      title: "Аналізуйте інформацію документа"
      content: "Витягніть важливі дані документа, наприклад налаштування сторінки, для подальшого аналізу."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Зразки коду"
  description: "Перегляньте приклади коду, що демонструють поширені функції GroupDocs.Watermark for Python via .NET."
  items:
    # code sample loop
    - title: "Водяний знак на документ із зображенням"
      content: |
        Використовуйте GroupDocs.Watermark for Python via .NET, щоб захистити документи, додавши водяні знаки на зображення. [Докладніше](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Як захистити файл водяним знаком зображення.">}}
        ```python {style=abap}

        # Завантажте вихідний документ у Watermarker
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Вкажіть шлях до зображення водяного знака
            watermark = groupdocs.watermark.watermarks.ImageWatermark("watermark.jpg")
            watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwgroupdocs.watermark.common.VerticalAlignment.CENTER

            # Захистіть файл і збережіть його
            watermarker.add(watermark)
            watermarker.save("result.pdf")
       
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Пошук і зміна існуючих водяних знаків"
      content: |
        GroupDocs.Watermark for Python via .NET дає вам змогу керувати водяними знаками документів. Виберіть водяні знаки та змініть їхні властивості. [Дізнайтеся, як](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Пошук і модифікація водяних знаків.">}}
        ```python {style=abap}

        # Завантажити вихідний документ
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Пошук водяних знаків для оновлення
            search_criteria = groupdocs.watermark.search.searchcriteria.TextSearchCriteria("annotation", False)
            watermarks = watermarker.search(search_criteria)
            
            # Оновлення бажаних властивостей
            for watermark in watermarks:
                watermark.text = "passed"

            # Збереження зміненого документа у вказаний шлях
            watermarker.save("result.pdf")


        ```
        {{< /landing/code >}}

---
