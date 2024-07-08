---
############################# Static ############################
layout: "family"
date:  2024-07-08T16:36:26
draft: false

product: "Watermark"
product_tag: "watermark"

lang: es

############################# Head ############################
head_title: "Documento Marca de agua C# Java Node.js Python | agregar marca de agua"
head_description: "Añade una marca de agua a PDF, imágenes y documentos. Solución de marcas de agua para Microsoft Office, PDF, OpenDocument, imágenes, etc."

############################# Header ############################
title: "Solución de marcas de agua para documentos"
description:  |
  Añada marcas de agua de texto e imágenes a sus documentos e imágenes.

  Busque y modifique las marcas de agua de los documentos de forma cómoda.

  Obtenga información sobre las marcas de agua que aparecen en sus documentos.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Elige tu plataforma"
  title: "Independencia de la plataforma"
  description: "La biblioteca GroupDocs.Watermark admite los siguientes sistemas operativos y marcos:"
  details_link_title: "Obtenga más información"

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
                    .NET Framework 4.5 or higher <br> .NET Core 3.0 or higher <br> .NET 5.0 or higher
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
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
                    Atom <br> Visual Studio Code <br> Cualquier otro editor de texto
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Python"
      description: GroupDocs.Watermark Python
      color: "yellow"
      tag: "python-net"
      link: "/watermark/python-net/"
      features_link: "https://docs.groupdocs.com/watermark/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Python 3.9+ and .Net 6+
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "4"
            content: |
                    IDLE <br> PyCharm <br> Visual Studio Code
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

############################# Features ###############################
features:
  enable: true
  title: "Revisión de funciones de GroupDocs.Watermark"
  description: "La biblioteca diseñada para agregar, buscar y actualizar varios tipos de marcas de agua para formatos de documentos populares."

  items:
    # items loop
    - icon: "protect"
      title: "Proteja los archivos con marcas de agua"
      content: "Añada marcas de agua de texto e imágenes a sus documentos empresariales."

    # items loop
    - icon: "search"
      title: "Búsqueda de marcas de agua existentes"
      content: "Obtenga información detallada sobre las marcas de agua colocadas anteriormente en el documento."

    # items loop
    - icon: "manipulate"
      title: "Manipule las marcas de agua del documento"
      content: "Controla el texto, el estilo, la imagen y otras funciones de marca de agua."

    # items loop
    - icon: "additional"
      title: "Diversas funciones adicionales"
      content: "Obtenga información del documento, actualice los hipervínculos o el fondo de las páginas, etc."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Proteja los documentos mediante marcas de agua"
  description: "GroupDocs.Watermark ejemplos de códigos de operaciones típicos."
  items:
    # code sample loop
    - title: "Crear una marca de agua."
      content: |
       Para añadir una marca de agua a un documento, proporcione la ruta al archivo de destino. Tiene muchas opciones entre las que elegir para obtener una marca de agua personalizada en una página específica.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Especifique el documento al que desea añadir una marca de agua
            using (Watermarker watermarker = new Watermarker("source.docx"))
            {
                // Crear objeto de marca de agua
                TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                // Definir las opciones de marca de agua
                watermark.ForegroundColor = Color.Red;
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;

                // Agregue una marca de agua y guarde el archivo procesado
                watermarker.Add(watermark);
                watermarker.Save("result.docx");
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Especifique el documento al que desea añadir una marca de agua
            Watermarker watermarker = new Watermarker("source.docx");

            // Crear objeto de marca de agua
            TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

            // Definir las opciones de marca de agua
            watermark.setForegroundColor(Color.getRed());
            watermark.setHorizontalAlignment(HorizontalAlignment.Center);
            watermark.setVerticalAlignment(VerticalAlignment.Center);

            // Agregue una marca de agua y guarde el archivo procesado
            watermarker.add(watermark);
            watermarker.save("result.docx");
            watermarker.close();
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            // Especifique el documento al que desea añadir una marca de agua
            const watermarker = new Watermarker("source.docx");

            // Crear objeto de marca de agua
            const watermark = new TextWatermark("top secret", new Font("Arial", 36));

            // Definir las opciones de marca de agua
            watermark.setForegroundColor(Color.getRed());
            watermark.setHorizontalAlignment(HorizontalAlignment.Center);
            watermark.setVerticalAlignment(VerticalAlignment.Center);

            // Agregue una marca de agua y guarde el archivo procesado
            watermarker.add(watermark);
            watermarker.save("result.docx");
            ```
        - language: "Python"
          color: "yellow"
          content: |
            ```python {style=abap}  
            def run():
                # Especifique el documento al que desea añadir una marca de agua
                with groupdocs.watermark.Watermarker("source.docx") as watermarker:
                    font = groupdocs.watermark.watermarks.Font("Arial", 36.0)

                    # Crear objeto de marca de agua
                    watermark = groupdocs.watermark.watermarks.TextWatermark("top secret", font)

                    # Definir las opciones de marca de agua
                    watermark.foreground_color = groupdocs.watermark.watermarks.Color.red;
                    watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
                    watermark.vertical_alignment = groupdocs.watermark.common.VerticalAlignment.CENTER

                    # Agregue una marca de agua y guarde el archivo procesado
                    watermarker.add(watermark)
                    watermarker.save("result.docx")
            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "Compatible con más de 50 formatos de archivo"
  description: "GroupDocs.Watermark proporciona marcas de agua para los formatos populares de documentos y archivos."

############################# Metrics ###############################
metrics:
  enable: true
  title: "Datos estadísticos de nuestra biblioteca"
  description: "Sumérjase en las métricas clave y revele información sobre nuestros logros, impacto y crecimiento."

  items:
    # items loop
    - number: "50+"
      title: "Formatos compatibles"
      content: "La biblioteca puede procesar más de 50 de los formatos de archivo más populares."

    # items loop
    - number: "500k"
      title: "NuGet descargas"
      content: "GroupDocs.Watermark for .NET es una biblioteca popular con más de 500 000 descargas en NuGet."

    # items loop
    - number: "15k"
      title: "Descargas de Maven"
      content: "Con más de 15 000 descargas en Maven, GroupDocs.Watermark es una opción popular entre Java desarrolladores."

    # items loop
    - number: "140+"
      title: "Clientes satisfechos"
      content: "Los desarrolladores individuales y las principales empresas de todo el mundo prefieren nuestras bibliotecas para crear soluciones innovadoras."


############################# Customers ###############################
customers:
  enable: true
  title: "Nuestros clientes satisfechos"
  description: "GroupDocs bibliotecas son empleadas por marcas reconocidas y distinguidas de todo el mundo."

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
  title: "¿Estás listo para empezar?"
  description: "Prueba GroupDocs.Watermark funciones gratis en tu plataforma"

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
  title: "Preguntas frecuentes"
  description: "Consulta nuestras preguntas frecuentes"

  items:
    # items loop
    - question: "¿GroupDocs.Watermark necesita bibliotecas externas para manipular documentos?"
      answer: "GroupDocs.Watermark funciona de forma independiente, sin necesidad de software de terceros como Adobe Acrobat, Microsoft Office, etc."

    # items loop
    - question: "¿Puedo probar GroupDocs.Watermark funciones antes de comprar?"
      answer: "¡Sí, GroupDocs.Watermark ofrece una prueba gratuita! Instálala y pruébala, pero ten en cuenta que las versiones de prueba añaden «insignias de prueba» a tus documentos y solo se procesan las 3 primeras páginas. ¿Quieres disfrutar de la experiencia completa? Obtenga una licencia temporal gratuita de 30 días para disfrutar de todas las funciones. Consulta los detalles en [licencia temporal](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "¿Qué tipos de licencia se proporcionan?"
      answer: "¿Necesitas una licencia GroupDocs.Watermark? ¡Tenemos opciones! Elija entre las licencias en función de muchas opciones. Número de desarrolladores de tu equipo. Ubicaciones de implementación, como oficinas individuales o lugares de trabajo remotos. ¿La distribución para clientes finales necesita compartir el SDK/API con los clientes? Como alternativa, existe una licencia de uso mensual: paga solo por lo que usas con los planes con contador. Sumérgete más y encuentra el [precio perfecto](https://purchase.groupdocs.com/pricing/watermark/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Watermark API de bajo código"
  description: "Agregue marcas de agua a los archivos mediante su aplicación mediante nuestra API REST basada en la nube."
  
  items:
    # items loop
    - title: "GroupDocs.Watermark Cloud for cURL"
      content: "Usa la API cURL REST ful para añadir marcas de agua a PDF, Word, Excel, PowerPoint, JPEG y otros formatos de archivo populares."
      icon: "groupdocs_watermark-for-curl"
      link: "https://products.groupdocs.cloud/watermark/curl"

    # items loop
    - title: "GroupDocs.Watermark Cloud for .NET"
      content: "Potencie sus .NET aplicaciones con funciones de marca de agua de documentos de Cloud SDK para .NET. Proteja los documentos empresariales por su cuenta."
      icon: "groupdocs_watermark-for-net"
      link: "https://products.groupdocs.cloud/watermark/net"

    # items loop
    - title: "GroupDocs.Watermark Cloud for Java"
      content: "El SDK GroupDocs.Watermark diseñado para Java ofrece nuevas posibilidades para sus Java aplicaciones y archivos empresariales."
      icon: "groupdocs_watermark-for-java"
      link: "https://products.groupdocs.cloud/watermark/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Watermark Aplicaciones web"
  description: "GroupDocs otorga acceso a la aplicación web para añadir marcas de agua a sus documentos. Puedes añadir marcas de agua a más de 50 formatos de archivo populares en tu navegador favorito DE FORMA GRATUITA."

  items:
    # items loop
    - title: "GroupDocs.Watermark Total"
      content: "Herramienta en línea para añadir marcas de agua a los documentos desde cualquier dispositivo."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/watermark/total"

    # items loop
    - title: "GroupDocs.Watermark DOCX"
      content: "Watermark MS Word DOCX en línea."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/watermark/docx"

    # items loop
    - title: "GroupDocs.Watermark PDF"
      content: "Proteja PDF documentos en línea."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/watermark/pdf"


      


---