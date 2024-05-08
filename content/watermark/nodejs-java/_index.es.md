---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:29
draft: false

lang: es
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Biblioteca de marcas de agua de Node.js | marcas de agua de documentos"
head_description: "La solución Node.js protege los documentos empresariales con marcas de agua de texto e imágenes. Se admiten los formatos más populares, como PDF, Word, Excel y PowerPoint."

############################# Header ############################
title: "Acceso a la tecnología de marcas de agua en Node.js a través de soluciones Java"
description: "Proteja su propiedad intelectual y evite las copias no autorizadas con esta solución Node.js. Permite a los usuarios añadir fácilmente marcas de agua a los documentos empresariales en varios formatos, incluidos PDF, Word, Excel, PowerPoint, imágenes, etc."
words:
  for: "por"

actions:
  main: "Usa NPM para descargar gratis"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.watermark"
  alt: "Licencias"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
  title: "¿Estás listo para empezar?"
  description: "Pruebe GroupDocs.Watermark funciones de forma gratuita o solicite una licencia"

release:
  title: "Publicada la versión {0}"
  notes: "Vea qué hay de nuevo"
  downloads: "Descargas"
  link: "https://releases.groupdocs.com/watermark/nodejs-java/"

code:
  title: "Agregue una marca de agua a PDF con TypeScript"
  more: "Más ejemplos"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.watermarker"
  content: |
    ```javascript {style=abap}

    // Instanciar Watermarker que pase por la ruta PDF
    let loadOptions = new PdfLoadOptions();
    let watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Personalice las opciones de marca de agua
    let textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Aplicar marca de agua al documento PDF
    watermarker.add(textWatermark);

    // Guardar documento de resultados
    watermarker.save("result.pdf");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark de un vistazo"
  description: "Biblioteca TypeScript de Node.js para marcas de agua"
  features:
    # feature loop
    - title: "Marcación de agua del archivo Node.js"
      content: "Proteja sus documentos empresariales con GroupDocs.Watermark for Node.js via Java. Añada texto, imágenes, diagramas o archivos adjuntos de correo electrónico como marcas de agua a varios formatos de archivo."

    # feature loop
    - title: "Personalice las marcas de agua según sus necesidades"
      content: "GroupDocs.Watermark for Node.js via Java ofrece amplias opciones de personalización para las marcas de agua. Los estilos de texto (negrita, cursiva, fuente) y las propiedades de la imagen (rotación, etc.) permiten personalizar el procesamiento de los documentos."

    # feature loop
    - title: "Soporte integral de formatos"
      content: "GroupDocs.Watermark for Node.js via Java se integra perfectamente con una amplia gama de formatos de archivo, que incluyen: PDF, MS Office, como Word, Excel, PowerPoint, imágenes como JPEG, PNG, GIF, BMP, Visio diagramas, correos electrónicos, etc. Permita el procesamiento de documentos para alcanzar los objetivos empresariales."

    # feature loop
    - title: "Potente búsqueda y actualización de marcas de agua"
      content: "Obtenga y actualice las marcas de agua existentes en los documentos con marca de agua. Modifique el texto, el estilo o el contenido de la imagen o elimínelos por completo. GroupDocs.Watermark for Node.js via Java ofrece una amplia gama de procesamiento de marcas de agua."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independencia de la plataforma"
  description: "GroupDocs.Watermark for Node.js via Java se integra fácilmente con varios sistemas operativos y gestores de paquetes."
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
  title: "Formatos de archivo compatibles"
  description: |
    GroupDocs.Watermark for Node.js via Java le permite procesar una amplia gama de formatos de archivo. [Explore la lista completa](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Node.js via Java: Conjunto de funciones"
  description: "Potencie una seguridad sólida de los documentos mediante marcas de agua programáticas. Admite diversos formatos de archivo, incluidos: PDF, DOCX, XLSX, PPTX y formatos de imagen (PNG, JPG, etc.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Control preciso de marcas de agua"
      content: "Manipule con precisión las marcas de agua agregándolas o eliminándolas de secciones específicas, documentos completos o archivos adjuntos y formas individuales en diferentes formatos de archivo."

    # feature loop
    - icon: "watermark_style"
      title: "Personalización de la apariencia de la marca de agua"
      content: "Controle minuciosamente la estética de las marcas de agua modificando atributos como el color, la fuente, la opacidad, la rotación y la posición dentro del documento."

    # feature loop
    - icon: "hidden_print"
      title: "Imprimir PDF marcas de agua"
      content: "Implemente una marca de agua sigilosa que permanece invisible durante la visualización normal de los documentos, pero que solo se hace evidente durante el proceso de impresión, lo que mejora la seguridad de los documentos de forma discreta."

    # feature loop
    - icon: "image_only"
      title: "Marca de agua específica para imágenes"
      content: "Añade marcas de agua a imágenes específicas dentro de un documento con nuestra solución. Elige incrustar marcas de agua en una sección designada (por ejemplo, una página, una diapositiva) o en todo el documento."

    # feature loop
    - icon: "image_frame"
      title: "Marcas de agua para imágenes de varios fotogramas"
      content: "Aplica marcas de agua de forma selectiva a fotogramas específicos dentro de un formato de imagen de varios fotogramas, lo que garantiza un control granular sobre la colocación de las marcas de agua."

    # feature loop
    - icon: "attachments"
      title: "Protección integral del contenido"
      content: "Amplíe la protección a varios elementos del documento, como los archivos adjuntos de Excel documentos y las formas de imagen de las presentaciones, lo que proporciona un nivel de seguridad adicional."

    # feature loop
    - icon: "pdf_objects"
      title: "Marcas de agua avanzadas en PDF"
      content: "Marca con agua diferentes áreas de PDF s, incluidas Bleed Box, Art Box, Crop Box, Trim Box, etc."

    # feature loop
    - icon: "doc_background"
      title: "Marca de agua de imagen de fondo"
      content: "Gestione las marcas de agua en las imágenes de fondo de las hojas de cálculo y las presentaciones, ofreciendo opciones de personalización adicionales para las medidas de seguridad visual."

    # feature loop
    - icon: "unreadable_characters"
      title: "Marca de agua de texto con caracteres ilegibles"
      content: "Utilice caracteres ilegibles en las marcas de agua de texto incrustadas en las presentaciones, lo que refuerza la seguridad al hacer que la extracción no autorizada de marcas de agua sea mucho más difícil."

    # feature loop
    - icon: "watermark_text_search"
      title: "Búsqueda avanzada de marcas de agua"
      content: "Utilice funciones de búsqueda integrales para localizar marcas de agua en los documentos en función de parámetros específicos o mediante la combinación de varios criterios, lo que permite una recuperación y una gestión eficientes."

    # feature loop
    - icon: "watermark_image_search"
      title: "Detección de marcas de agua de imágenes similares"
      content: "Busque imágenes de marcas de agua similares en documentos que se parezcan visualmente a una imagen de origen."

    # feature loop
    - icon: "document_info"
      title: "Extracción programática de información de documentos"
      content: "Extraiga metadatos valiosos mediante programación, incluidos los detalles de configuración de página y otra información del documento para los formatos de archivo compatibles."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ejemplos de código"
  description: "Sumérjase en ejemplos de código que muestran funcionalidades comunes de GroupDocs.Watermark for Node.js via Java"
  items:
    # code sample loop
    - title: "Añade una marca de agua a un documento con una imagen"
      content: |
        Aproveche GroupDocs.Watermark for Node.js via Java para mejorar la seguridad de los documentos añadiendo marcas de agua a las imágenes. Más información: [Marcas de agua de imagen](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Cómo proteger un archivo con una marca de agua de imagen.">}}
        ```javascript {style=abap}
        // Cargar el documento fuente en Watermarker
        let watermarker = new Watermarker("document.pdf");
        
        // Especificar la ruta a una imagen con marca de agua
        let watermark = new ImageWatermark("watermark.jpg");

        // Proteja el archivo y guárdelo
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Buscar y modificar marcas de agua existentes"
      content: |
        GroupDocs.Watermark for Node.js via Java le permite gestionar las marcas de agua de los documentos. Seleccione las marcas de agua y modifique sus propiedades. Descubra cómo: [Modificar las marcas de agua](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Búsqueda y modificación de marcas de agua.">}}
        ```javascript {style=abap}   
        // Cargar documento fuente
        let watermarker = new Watermarker("document.pdf");

        // Busca marcas de agua para actualizarlas
        let searchCriteria = new TextSearchCriteria("test", false);                               
        let watermarks = watermarker.search(searchCriteria); 

        // Actualizar las propiedades deseadas
        watermarks.forEach((watermark)
        {  
            watermark.setText("New Text");
        }

        // Guardar el documento modificado en una ruta especificada
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
