---
############################# Static ############################
layout: "landing"
date: 2024-04-29T14:27:12
draft: false

lang: es
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

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
head_title: "Java Biblioteca de marcas de agua | añadir marcas de agua a los documentos"
head_description: "Software nativo Java para agregar y manipular marcas de agua de texto e imágenes en archivos PDF, Word, Excel, presentaciones, Visio diagramas, correo electrónico e imágenes."

############################# Header ############################
title: "Implemente fácilmente la marca de agua de documentos en Java proyectos"
description: "Mejore sus Java aplicaciones con la posibilidad de añadir marcas de agua a los archivos mediante la biblioteca GroupDocs.Watermark. Nuestra API ofrece marcas de agua personalizables para una amplia gama de formatos de archivo populares."
words:
  for: "por"

actions:
  main: "Descarga gratuita desde Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "Licencias"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java/"
  title: "¿Estás listo para empezar?"
  description: "Pruebe GroupDocs.Watermark funciones de forma gratuita o solicite una licencia"

release:
  title: "Publicada la versión {0}"
  notes: "Vea qué hay de nuevo"
  downloads: "Descargas"

code:
  title: "Marca de agua PDF s a través de Java"
  more: "Más ejemplos"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-watermark</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Instanciar Watermarker que pase por la ruta PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Personalice las opciones de marca de agua
    TextWatermark textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Aplicar marca de agua al documento PDF
    watermarker.add(textWatermark);

    // Guardar documento de resultados
    watermarker.save("result.pdf");
    watermarker.close();
      
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark de un vistazo"
  description: "Biblioteca diseñada para agregar marcas de agua mediante tecnologías Java"
  features:
    # feature loop
    - title: "Archivos de marcas de agua mediante Java"
      content: "Proteja sus documentos empresariales con GroupDocs.Watermark for Java. Agregue texto, imágenes, diagramas o archivos adjuntos de correo electrónico como marcas de agua a varios formatos de archivo."

    # feature loop
    - title: "Personalice las marcas de agua para necesidades específicas"
      content: "GroupDocs.Watermark for Java ofrece amplias opciones de personalización para las marcas de agua. Ajusta los estilos del texto (negrita, cursiva, fuente) y las propiedades de la imagen (rotación, etc.) para adaptar el proceso de creación de marcas de agua a tus objetivos específicos."

    # feature loop
    - title: "Soporte de formato amplio"
      content: "GroupDocs.Watermark for Java se integra perfectamente con una amplia gama de formatos de archivo, incluidos: PDF, Microsoft Office (Word, Excel, PowerPoint), imágenes (JPEG, PNG, GIF, BMP), Visio diagramas y correos electrónicos. Mejore la seguridad de los documentos en diversos tipos de archivos."

    # feature loop
    - title: "Búsqueda y gestión de marcas de agua sin esfuerzo"
      content: "Gestione de forma eficiente las marcas de agua existentes en los documentos. Localice marcas de agua específicas, modifique su texto, estilo o imágenes, o elimínelas por completo. GroupDocs.Watermark for Java simplifica el flujo de trabajo de las marcas de agua."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independencia de la plataforma"
  description: "GroupDocs.Watermark for Java admite varios sistemas operativos y gestores de paquetes."
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de archivo compatibles"
  description: |
    GroupDocs.Watermark for Java permite procesar una amplia gama de formatos de archivo. [Ver la lista completa](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formatos Microsoft Office y OpenDocument
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### Imágenes y gráficos
        * **Formatos de imagen populares:** BMP, JPG, JPEG, PNG
        * **Imágenes de varias páginas:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### Otros
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark for Java: Características"
  description: "Proteja sus archivos añadiendo marcas de agua. Admite varios formatos, incluidos PDF, documentos de Office e imágenes."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Marcas de agua de archivos"
      content: "Agregue o elimine marcas de agua de secciones específicas o documentos completos para varios formatos de archivo compatibles."

    # feature loop
    - icon: "watermark_style"
      title: "Personalización de marcas de agua"
      content: "Personaliza la apariencia de tu marca de agua con opciones como el color, la fuente, la rotación y más."

    # feature loop
    - icon: "hidden_print"
      title: "Marca de agua de impresión oculta para PDF"
      content: "Agregue una marca de agua que solo aparezca al imprimir un documento PDF."

    # feature loop
    - icon: "image_only"
      title: "Marca de agua selectiva de imágenes"
      content: "Añade marcas de agua a todas las imágenes de una sección, página, diapositiva o documento completo en concreto."

    # feature loop
    - icon: "image_frame"
      title: "Añadir marcas de agua a marcos de imagen específicos"
      content: "Aplica marcas de agua a marcos específicos dentro de una imagen con varios marcos."

    # feature loop
    - icon: "attachments"
      title: "Marcar archivos adjuntos y formas"
      content: "Agregue marcas de agua a todos los archivos adjuntos de Excel documentos o a todas las formas de imagen en Presentations."

    # feature loop
    - icon: "pdf_objects"
      title: "Alineación de marcas de agua en PDF"
      content: "Alinee las marcas de agua con diferentes áreas de un documento PDF, incluidas Bleed Box, Art Box, Crop Box y Trim Box."

    # feature loop
    - icon: "doc_background"
      title: "Marca de agua por imágenes de fondo"
      content: "Agregue o elimine la marca de agua de la imagen de fondo a las hojas de cálculo o presentaciones."

    # feature loop
    - icon: "unreadable_characters"
      title: "Protección con caracteres ilegibles"
      content: "Proteja las presentaciones con marcas de agua de texto con caracteres ilegibles."

    # feature loop
    - icon: "watermark_text_search"
      title: "Búsqueda de marcas de agua"
      content: "Obtenga la lista de las marcas de agua presentadas en el archivo, utilizando varios parámetros, incluidas las expresiones regulares."

    # feature loop
    - icon: "watermark_image_search"
      title: "Encuentra marcas de agua de imágenes similares"
      content: "Localice las marcas de agua de la imagen que se parezcan a una imagen específica."

    # feature loop
    - icon: "document_info"
      title: "Extraer información del documento"
      content: "Obtenga varios datos de documentos, como la configuración de página para los formatos de archivo compatibles."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ejemplos de código"
  description: "Explore ejemplos de código que ilustran las funcionalidades típicas de GroupDocs.Watermark for Java"
  items:
    # code sample loop
    - title: "Añadir una marca de agua a un documento con una imagen"
      content: |
        Utilice GroupDocs.Watermark for Java para mejorar la seguridad de los documentos añadiendo marcas de agua a las imágenes. Más información: [Marcas de agua de imagen](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Cómo proteger un archivo con una marca de agua de imagen.">}}
        ```csharp {style=abap}
        // Cargar el documento fuente en Watermarker
        Watermarker watermarker = new Watermarker("document.pdf");
        
        // Especificar la ruta a una imagen con marca de agua
        ImageWatermark watermark = new ImageWatermark("watermark.jpg");

        // Proteja el archivo y guárdelo
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Modificar marcas de agua"
      content: |
        GroupDocs.Watermark for Java le permite gestionar las marcas de agua existentes en los documentos. Localice marcas de agua específicas y [modifique sus propiedades](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Búsqueda y modificación de marcas de agua.">}}
        ```csharp {style=abap}   
        // Cargar documento fuente
        Watermarker watermarker = new Watermarker("document.pdf");

        // Busca marcas de agua para actualizarlas
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);                               
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);                             

        // Actualizar las propiedades deseadas
        for (PossibleWatermark watermark : watermarks)                                                           
        {  
            watermark.setText("New Text");
        }

        // Guardar el documento modificado en una ruta especificada
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
