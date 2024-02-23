---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "API de Java para agregar búsqueda Eliminar marcas de agua a PDF Word Excel Imágenes"
head_description: "API de marcas de agua de documentos Java: genere, busque y elimine marcas de agua de documentos: PDF, Word, Excel, presentaciones, Visio, correo electrónico y formatos de archivo de imagen."

############################# Header ############################
title: "API de Java para manipular marcas de agua"
description: "Desarrolle aplicaciones Java para realizar operaciones de marca de agua de imágenes y texto con búsqueda inteligente y seguridad robusta."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Watermark for Java"
        image: "/border/groupdocs-watermark-java.svg"
        product: "GroupDocs.Watermark"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Visión de conjunto"

            # button loop
            - link: "#features"
              text: "Características"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/watermark"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/watermark/java"
              text: "Precios"

    right:
        link_download: "https://downloads.groupdocs.com/watermark"
        link_learn: "https://docs.groupdocs.com/watermark/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Visión de conjunto ############################
overview:
    enable: true
    content: |
      GroupDocs.Watermark para Java le permite crear aplicaciones comerciales que permiten a sus usuarios finales aplicar nuevas marcas de agua, buscar y eliminar marcas de agua existentes en archivos de formatos admitidos. Puede asignar mediante programación marcas de agua digitales a muchos formatos de archivo y utilizar sus poderosas capacidades de búsqueda inteligente. GroupDocs.Watermark para Java proporciona varias medidas de seguridad integradas que se pueden emplear para evitar el uso indebido de documentos digitales que contienen información confidencial o contenido de propiedad intelectual.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          A continuación se muestra una descripción general de GroupDocs.Watermark para Java:

        rright:
          enable: true
          icon: "fab fa-html5"
          title: "Visión de conjunto"
          content: |
            * Agregar y quitar marca de agua
            * Buscar y reemplazar marca de agua
            * Buscar por formato
            * Búsqueda por comparación de imágenes
            * Trabajar con encabezados y pies de página
            * Trabajar con imágenes de fondo
            * Trabajar con archivos adjuntos
            * Rasterizar páginas
            * Aplicar restricciones de edición
      
      ## TAB TWO ##
      tab_two:
        description: |
          Los [formatos de documento y tipo de marca de agua] admitidos (https://docs.groupdocs.com/watermark/java/supported-document-formats/) para cada formato se enumeran a continuación:

        left:
          enable: true
          table:
            # table loop
            - title: "oficina de Microsoft"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
                * **Visio:** VSD, VDX, VSS, VSSX, VSX, VST, VSTX, VTX, VSDX, VDW, VSTM, VSSM, VSDM

            # table loop
            - title: "Agregar marca de agua"
              content: |
                * **PDF**: XObject, Artefacto, Anotación
                * **Palabra**: Forma
                * **Excel**: Forma, Encabezado y Pie de página
                * **PowerPoint**: Forma
                * **Visio**: Forma
                * **Imagen ráster**: Texto, Imagen
                * **TIFF multipágina**: Texto, Imagen
                * **Gif animado**: Texto, Imagen

        right:
          enable: true
          table:
            # table loop
            - title: "Documentos PDF y de imagen"
              content: |
                * **Portable Document Format**: PDF
                * **Open Document**: ODT
                * **Email**: EML, MSG, EMLX, OFT
                * **Images**: PNG, BMP, GIF, JPG, JPEG, JP2, TIF, TIFF, WebP

            # table loop
            - title: "Eliminación de marca de agua"
              content: |
                * **PDF**: XObject, Artefacto, Anotación, Texto regular
                * **Palabra**: Forma, Texto normal
                * **Excel**: forma, encabezado y pie de página, imagen de fondo, texto y fórmulas en las celdas
                * **PowerPoint**: Forma
                * **Visio**: Forma, Diagrama Comentarios
                * **Correo electrónico**: Imágenes adjuntas e incrustadas, Asunto y fragmentos de texto del cuerpo

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Watermark para Java es compatible con los siguientes sistemas operativos, marcos y administradores de paquetes:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Sistemas operativos"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Marcos compatibles"
              content: |
                * Java 7 (1.7) y superior

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Entornos de desarrollo"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Herramienta de automatización de compilación"
              content: |
                * Maven

############################# Características ############################
features:
    enable: true
    title: "GroupDocs.Watermark for Java Características"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Extraiga todos los documentos de varios formatos de una carpeta y aplique o elimine marcas de agua"

      # feature loop
      - icon: "fas fa-eye"
        content: "Emplear o eliminar marca de agua de una sección particular o documento completo"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Adjuntar marca de agua a los marcos seleccionados de una imagen con varios marcos"

      # feature loop
      - icon: "fas fa-code"
        content: "Aplicar marca de agua oculta a PDF para que aparezca al imprimir documentos"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Emplear marca de agua en archivos adjuntos en un documento de Excel y todas las formas de imagen en diapositivas"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Coloque una marca de agua o elimínela de las imágenes de fondo de las diapositivas o la hoja de Excel"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Establecer marca de agua en archivos admitidos en archivos adjuntos de un correo electrónico o archivo PDF"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Agregue o elimine marcas de agua como XObject, artefactos y anotaciones en archivos PDFe"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Eliminar marca de agua que coincida con el texto con un formato particular"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Encuentre marcas de agua de imagen que se parezcan a una imagen en particular"

      # feature loop
      - icon: "fas fa-columns"
        content: "Identifique la marca de agua de texto incluso si hay caracteres ilegibles entre letras"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Busque marcas de agua basadas en parámetros específicos o mediante la asignación de múltiples criterios"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Especifique el formato de fuente para ubicar la marca de agua de texto coincidente"

      # feature loop
      - icon: "fas fa-print"
        content: "Obtenga las dimensiones de página, diapositiva y celda para el tamaño absoluto y el posicionamiento de la marca de agua"

      # feature loop
      - icon: "fas fa-lock"
        content: "Agregar marca de agua a formas de imagen en un documento de Word y restringir la edición de marcas de agua"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Marca de agua de texto segura en presentaciones usando caracteres ilegibles"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Proteja las marcas de agua de documentos PDF rasterizando una sola página o todo el documento"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Modificar el formato de texto al reemplazar la marca de agua de texto actual"

      # feature loop
      - icon: "fas fa-heading"
        content: "Alinear la marca de agua con el cuadro de sangrado, el cuadro de arte, el cuadro de recorte o el cuadro de guillotinado en un archivo PDF"

    more_feature:
      # more_feature_loop
      - title: "Emplear marcas de agua"
        content: |
          GroupDocs.Watermark for Java le permite trabajar con numerosos tipos de marcas de agua. Es solo una cuestión de unas pocas líneas de código para agregar una marca de agua de cualquier tipo. El siguiente ejemplo comparte cómo puede agregar una marca de agua de imagen en un documento de Word usando Java:
          
          ```java
          Document doc = Document.load(Common.mapSourceFilePath("D://test.docx"));
          Font font = new Font("Times New Roman", 12);
          TextWatermark watermark = new TextWatermark("Test watermark", font);

          // Establecer tipo de tamaño
          watermark.setSizingType(SizingType.ScaleToParentDimensions);

          // Establecer escala de marca de agua
          watermark.setScaleFactor(0.5);

          doc.addWatermark(watermark);
          doc.save(Common.mapOutputFilePath("D://test.docx"));
          doc.close();
          ```
      # more_feature_loop
      - title: "Agregar marca de agua a archivos de diferentes formatos de una vez"
        content: "Con GroupDocs.Watermark para la API de Java, puede agregar o eliminar la marca de agua de todos los documentos presentes en una carpeta en particular en modo por lotes. No importa, si los documentos tienen un formato diferente, GroupDocs.Watermark for Java aplicará una marca de agua a todos los archivos con precisión.."

      # more_feature_loop
      - title: "Asigne seguridad infalible a sus marcas de agua"
        content: "Con un código mínimo, puede asignar seguridad infalible a sus marcas de agua y hacer que sea extremadamente difícil para cualquier herramienta de terceros modificar o eliminar su marca de agua asignada del archivo PDF. Es así porque GroupDocs.Watermark for Java le permite convertir todas las páginas de un archivo PDF en imágenes rasterizadas. Este enfoque hace que sus marcas de agua digitales sean seguras mientras mantiene su calidad cercana a la original."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Watermark ofrece API de visualización de documentos para otros entornos de desarrollo populares"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Watermark for .NET"
          image: "/border/groupdocs-watermark-net.svg"
          product: "GroupDocs.Watermark"
          platform: ".NET"
          link: "/watermark/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---