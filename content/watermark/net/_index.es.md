---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET API para agregar búsqueda Eliminar marcas de agua a imágenes PDF de Word Excel"
head_description: "API C# .NET para agregar, buscar y eliminar imágenes y marcas de agua basadas en texto de documentos: PDF, Word, Excel, presentaciones, Visio, correo electrónico y formatos de archivo de imagen."

############################# Header ############################
title: ".NET API para la manipulación de marcas de agua"
description: "Cree aplicaciones .NET para operar marcas de agua basadas en texto e imágenes con búsqueda inteligente y características de seguridad sólidas."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Watermark for .NET"
        image: "/border/groupdocs-watermark-net.svg"
        product: "GroupDocs.Watermark"
        platform: ".NET"

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
            - link: "https://purchase.groupdocs.com/pricing/watermark/net"
              text: "Precios"

    right:
        link_download: "https://downloads.groupdocs.com/watermark"
        link_learn: "https://docs.groupdocs.com/watermark/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Visión de conjunto ############################
overview:
    enable: true
    content: |
      GroupDocs.Watermark para .NET le permite crear aplicaciones comerciales listas para el mercado en C#, ASP.NET y otras tecnologías relacionadas con .NET, que permiten a sus usuarios finales agregar nuevas marcas de agua, buscar y eliminar marcas de agua existentes en formatos de archivo admitidos . Con GroupDocs.Watermark para .NET, puede aplicar marcas de agua digitales mediante programación a multitud de formatos de archivo y desalentar el uso no autorizado de propiedad intelectual y etiquetar de forma segura documentos de naturaleza confidencial mediante el empleo de diversas medidas de seguridad integradas que ofrece esta API.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          A continuación se muestra una descripción general de GroupDocs.Watermark para .NET:
      
        right:
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
          Los [formatos de documento y tipo de marca de agua](https://docs.groupdocs.com/watermark/net/supported-document-formats/) para cada formato se enumeran a continuación:

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
          GroupDocs.Watermark for .NET supports following Sistemas operativos, Frameworks & Gerente de empaquetacións:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Sistemas operativos"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux

            # table loop
            - icon: "fas fa-code"
              title: "Marcos compatibles"
              content: |
                * .NET Framework 2.0 o superior
                * Mono Framework 1.2 o superior
                * .NET estándar 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Gerente de empaquetación"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Entornos de desarrollo"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Características ############################
features:
    enable: true
    title: "GroupDocs.Watermark for .NET Características"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Agregue o elimine marcas de agua de una sección en particular o de un documento completo de varios formatos de archivo"

      # feature loop
      - icon: "fas fa-eye"
        content: "Adjuntar marca de agua a todas las imágenes en una sección, página, diapositiva o documento en particular"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Asignar marca de agua solo a fotogramas particulares de una imagen de varios fotogramas"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Asignar marca de agua oculta a PDF que solo aparece al imprimir documentos"

      # feature loop
      - icon: "fas fa-code"
        content: "Establecer marca de agua en todos los archivos adjuntos en un documento de Excel y todas las formas de imagen en diapositivas"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Coloque una marca de agua o elimínela de las imágenes de fondo de la hoja de cálculo o las diapositivas"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Emplear marca de agua en archivos admitidos en todos los archivos adjuntos de un correo electrónico o documento PDF"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Aplicar o eliminar marcas de agua como XObjects, artefactos y anotaciones en documentos PDF"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Elimine la marca de agua que contiene texto con un formato particular"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Busque marcas de agua de imagen que se parezcan a una imagen en particular"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Identificar marca de agua de texto incluso si hay caracteres ilegibles entre letras"

      # feature loop
      - icon: "fas fa-columns"
        content: "Busque marcas de agua en función de parámetros específicos o mediante la combinación de varios criterios"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Especifique el formato de fuente para buscar una marca de agua de texto coincidente"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Extraiga mediante programación la configuración de la página y otra información para los formatos admitidos"

      # feature loop
      - icon: "fas fa-print"
        content: "Agregar marca de agua a las imágenes dentro de cualquier encabezado y pie de página en formatos de documentos compatibles"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Agregar marca de agua a formas de imagen en un documento de Word y bloquear marcas de agua para restringir la edición"

      # feature loop
      - icon: "fas fa-lock"
        content: "Proteja la marca de agua de texto usando caracteres ilegibles en las presentaciones"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Rasterice una página en particular o un documento PDF completo para proteger las marcas de agua añadidas"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Cambiar el formato de texto al reemplazar la marca de agua de texto existente"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Alinear la marca de agua con el cuadro de sangrado, el cuadro de arte, el cuadro de recorte o el cuadro de guillotinado en un documento PDF"

      # feature loop
      - icon: "fas fa-heading"
        content: "Editar propiedades de formas en documentos de Microsoft Visio"

    more_feature:
      # more_feature_loop
      - title: "Agregar marca de aguas"
        content: |
          GroupDocs.Watermark para .NET admite varios tipos de marcas de agua. Agregar marcas de agua de cualquier tipo es solo cuestión de unas pocas líneas de código. El siguiente ejemplo demuestra cómo aplicar una marca de agua de imagen a un documento de Word usando C#:

          ```cs
          // Cargue el documento
          using (FileStream stream = File.Open("document.docx", FileMode.Open, FileAccess.ReadWrite))
          {
            using (Watermarker watermarker = new(Watermarker(stream))
            {
                // Use la ruta a la imagen como parámetro del constructor
                using (ImageWatermark watermark = new ImageWatermark("logo.png"))
                {
                  watermark.HorizontalAlignment = HorizontalAlignment.Center;
                  watermark.VerticalAlignment = VerticalAlignment.Center;
                  watermarker.Add(watermark);
                }
                // Guardar el documento resultante
                watermarker.Save("document_watermarked.docx");
                }
          }
          ```
      # more_feature_loop
      - title: "Aplicar marca de agua to Files of Different Formats in a Go"
        content: "GroupDocs.Watermark API le permite aplicar una marca de agua o eliminar una marca de agua de todos los archivos en una carpeta específica de una sola vez. Los archivos pueden incluso tener un formato diferente y, sin embargo, la marca de agua se aplicará a todos ellos con precisión."

      # more_feature_loop
      - title: "Seguridad infalible para marca de agua"
        content: "Con solo una línea de código, puede hacer que sea muy difícil para cualquier herramienta eliminar su marca de agua de los archivos PDF. Esto se logra convirtiendo todas las páginas de un documento PDF en imágenes de trama manteniendo intacta la calidad original."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Watermark ofrece API de visualización de documentos para otros entornos de desarrollo populares"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Watermark for Java"
          image: "/border/groupdocs-watermark-java.svg"
          product: "GroupDocs.Watermark"
          platform: "Java"
          link: "/watermark/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---