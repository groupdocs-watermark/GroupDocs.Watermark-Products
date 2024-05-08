---
############################# Static ############################
layout: "family"
date:  2024-05-08T17:25:28
draft: false

product: "Watermark"
product_tag: "watermark"

lang: ru

############################# Head ############################
head_title: "Водяной знак документа C# Java Node.js | добавить водяной знак"
head_description: "Добавьте водяной знак к PDF, изображениям и документам. Решение для нанесения водяных знаков на Microsoft Office, PDF, OpenDocument, изображения и т. д."

############################# Header ############################
title: "Решение для водяных знаков для документов"
description:  |
  Добавьте текстовые и графические водяные знаки к документам и изображениям.

  Ищите и изменяйте водяные знаки документов удобным способом.

  Получите информацию о водяных знаках, представленных в ваших документах.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Выберите свою платформу"
  title: "Независимость платформы"
  description: "Библиотека GroupDocs.Watermark поддерживает следующие операционные системы и фреймворки:"
  details_link_title: "Узнайте больше"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Watermark .NET 
      color: "blue"
      tag: "net"
      link: "/watermark/net/"
      features_link: "https://docs.groupdocs.com/watermark/net/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    .NET Framework 4.6.2 or higher <br> .NET Core 2.0 or higher <br> .NET 6.0 or higher
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Watermark Java
      color: "red"
      tag: "java"
      link: "/watermark/java/"
      features_link: "https://docs.groupdocs.com/watermark/java/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    Java 8 or higher <br> Kotlin
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Watermark Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/watermark/nodejs-java/"
      features_link: "https://docs.groupdocs.com/watermark/"
      features:
          # features loop
          - rows: "4"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Любой другой текстовый редактор
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

############################# Features ###############################
features:
  enable: true
  title: "Обзор характеристик GroupDocs.Watermark"
  description: "Библиотека, предназначенная для добавления, поиска и обновления различных типов водяных знаков для популярных форматов документов."

  items:
    # items loop
    - icon: "protect"
      title: "Защитите файлы водяными знаками"
      content: "Добавляйте текстовые и графические водяные знаки к своим деловым документам."

    # items loop
    - icon: "search"
      title: "Поиск существующих водяных знаков"
      content: "Получите подробную информацию о водяных знаках, размещенных в документе ранее."

    # items loop
    - icon: "manipulate"
      title: "Манипулирование водяными знаками документов"
      content: "Управляйте текстом, стилем, изображением и другими функциями водяных знаков."

    # items loop
    - icon: "additional"
      title: "Различные дополнительные функции"
      content: "Получите информацию о документе, обновите гиперссылки или фон страниц и т. д."

############################# Code Samples ###############################
code_samples:
  enable: true
  title: "Защита документов водяными знаками"
  description: "GroupDocs.Watermark примеры типичных операционных кодов."

  items:
    # items loop
    - title: "Создание водяного знака."
      content: "Чтобы добавить водяной знак к документу, укажите путь к целевому файлу. Вы можете выбрать множество вариантов размещения индивидуального водяного знака на определенной странице."
      samples:
          # samples loop
          - language: "C#"
            color: "blue"
            content: |
                    <code class="language-csharp" data-lang="csharp">
                        // Укажите документ, на который будет нанесен водяной знак

                        using (Watermarker watermarker = new Watermarker("source.docx"))
                        {
                          // Создать объект водяного знака
                          TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                          // Настройка параметров водяных знаков
                          watermark.ForegroundColor = Color.Red;
                          watermark.HorizontalAlignment = HorizontalAlignment.Center;
                          watermark.VerticalAlignment = VerticalAlignment.Center;

                          // Добавьте водяной знак и сохраните обработанный файл
                          watermarker.Add(watermark);
                          watermarker.Save("result.docx");
                        }                    
                    </code>

          # samples loop
          - language: "Java"
            color: "red"
            content: |
                    <code class="language-java" data-lang="java">
                        // Укажите документ, на который будет нанесен водяной знак

                        Watermarker watermarker = new Watermarker("source.docx");

                        // Создать объект водяного знака
                        TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // Настройка параметров водяных знаков
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // Добавьте водяной знак и сохраните обработанный файл
                        watermarker.add(watermark);
                        watermarker.save("result.docx");
                        watermarker.close();

                    </code>

          # samples loop
          - language: "TypeScript"
            color: "green"
            content: |
                    <code class="language-java" data-lang="javascript">
                        // Укажите документ, на который будет нанесен водяной знак

                        const watermarker = new Watermarker("source.docx");
    
                        // Создать объект водяного знака
                        const watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // Настройка параметров водяных знаков
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // Добавьте водяной знак и сохраните обработанный файл
                        watermarker.add(watermark);
                        watermarker.save("result.docx");                        

                    </code>

############################# Supported Formats ###############################
formats:
  enable: true
  title: "Поддерживается более 50 форматов файлов"
  description: "GroupDocs.Watermark предоставляет водяные знаки для популярных форматов документов и файлов."

############################# Metrics ###############################
metrics:
  enable: true
  title: "Статистические данные нашей библиотеки"
  description: "Погрузитесь в ключевые показатели и узнайте о наших достижениях, влиянии и росте."

  items:
    # items loop
    - number: "50+"
      title: "Поддерживаемые форматы"
      content: "Библиотека способна обрабатывать более 50 самых популярных форматов файлов."

    # items loop
    - number: "800k"
      title: "NuGet загрузок"
      content: "GroupDocs.Watermark for .NET — популярная библиотека, которую загрузили более 800 000 раз на NuGet."

    # items loop
    - number: "15k"
      title: "Загрузки Maven"
      content: "GroupDocs.Watermark скачан на Maven более 15 000 раз, поэтому GroupDocs.Watermark является популярным выбором для Java разработчиков."

    # items loop
    - number: "140+"
      title: "Счастливые клиенты"
      content: "Отдельные разработчики и ведущие компании по всему миру отдают предпочтение нашим библиотекам для создания инновационных решений."


############################# Customers ###############################
customers:
  enable: true
  title: "Наши довольные клиенты"
  description: "GroupDocs библиотек используют всемирно известные и авторитетные бренды по всему миру."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Watermark бесплатно на своей платформе"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/watermark/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/watermark/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/watermark/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "Часто задаваемые вопросы"
  description: "Ознакомьтесь с нашими часто задаваемыми вопросами"

  items:
    # items loop
    - question: "Требуются ли GroupDocs.Watermark внешние библиотеки для работы с документами?"
      answer: "GroupDocs.Watermark работает независимо, нет необходимости в стороннем программном обеспечении, таком как Adobe Acrobat, Microsoft Office и т. д."

    # items loop
    - question: "Могу ли я протестировать функции GroupDocs.Watermark перед покупкой?"
      answer: "Да, GroupDocs.Watermark предлагает бесплатную пробную версию! Установите его и попробуйте, но имейте в виду: в пробных версиях к вашим документам добавляются «пробные значки», обрабатываются только первые 3 страницы. Хотите получить полный опыт? Получите бесплатную 30-дневную временную лицензию для полной функциональности. Подробнее см. в разделе [временная лицензия](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Какие типы лицензий предоставляются?"
      answer: "Нужна лицензия GroupDocs.Watermark? У нас есть варианты! Выбирайте из множества лицензий. Количество разработчиков в вашей команде. Места развертывания, такие как отдельный офис или удаленные рабочие места. Нужно ли конечным пользователям предоставлять клиентам SDK/API? Кроме того, существует лицензия на ежемесячное использование: платите только за то, что используете в тарифных планах с оплатой. Погрузитесь глубже и найдите идеальную [цену](https://purchase.groupdocs.com/pricing/watermark/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Watermark API с низким кодом"
  description: "Добавляйте водяные знаки к файлам с помощью нашего облачного API REST."
  
  items:
    # items loop
    - title: "GroupDocs.Watermark Cloud for cURL"
      content: "Используйте полный API cURL REST для нанесения водяных знаков PDF, Word, Excel, PowerPoint, JPEG и других популярных форматов файлов."
      icon: "groupdocs_watermark-for-curl"
      link: "https://products.groupdocs.cloud/watermark/curl"

    # items loop
    - title: "GroupDocs.Watermark Cloud for .NET"
      content: "Предоставьте своим .NET приложениям возможность нанесения водяных знаков на документы с помощью Cloud SDK для .NET. Защитите деловые документы самостоятельно."
      icon: "groupdocs_watermark-for-net"
      link: "https://products.groupdocs.cloud/watermark/net"

    # items loop
    - title: "GroupDocs.Watermark Cloud for Java"
      content: "GroupDocs.Watermark SDK, разработанный для Java, предоставляет новые возможности для ваших Java приложений и бизнес-файлов."
      icon: "groupdocs_watermark-for-java"
      link: "https://products.groupdocs.cloud/watermark/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Watermark Веб-приложения"
  description: "GroupDocs предоставляет доступ к веб-приложению для добавления водяных знаков в ваши документы. Более 50 популярных форматов файлов можно БЕСПЛАТНО добавить водяные знаки в вашем любимом браузере."

  items:
    # items loop
    - title: "GroupDocs.Watermark Total"
      content: "Онлайн-инструмент для добавления водяных знаков к документам с любого устройства."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/watermark/total"

    # items loop
    - title: "GroupDocs.Watermark DOCX"
      content: "Водяной знак MS Word DOCX в режиме онлайн."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/watermark/docx"

    # items loop
    - title: "GroupDocs.Watermark PDF"
      content: "Защитите PDF документов в режиме онлайн."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/watermark/pdf"


      


---