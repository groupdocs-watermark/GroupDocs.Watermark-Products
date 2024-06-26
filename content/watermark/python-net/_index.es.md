---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:49
draft: false

lang: es
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
head_title: "Python Biblioteca de marcas de agua | Marcas de agua de documentos"
head_description: "Python protege los documentos comerciales con marcas de agua de texto e imagen. Se admiten formatos de archivo como PDF, Word, Excel y PowerPoint."

############################# Header ############################
title: "Acceda a la tecnología de marca de agua Python via .NET"
description: "Proteja sus datos y evite copias no autorizadas con esta solución Python. Agregue fácilmente marcas de agua a documentos comerciales en varios formatos, incluidos PDF, Word, Excel, PowerPoint, imágenes, etc."
words:
  for: "por"

actions:
  main: "PyPi descarga gratis"
  main_link: "https://pypi.org/project/groupdocs-watermark-net/"
  alt: "Licencias"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
  title: "¿Estás listo para empezar?"
  description: "Pruebe GroupDocs.Watermark funciones de forma gratuita o solicite una licencia"

release:
  title: "Publicada la versión {0}"
  notes: "Vea qué hay de nuevo"
  downloads: "Descargas"
  link: "https://releases.groupdocs.com/watermark/python-net/"

code:
  title: "Agregue marca de agua a PDF usando Python"
  more: "Más ejemplos"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
  install: "pip install groupdocs-watermark-net"
  content: |
    ```python {style=abap}

    import groupdocs.watermark as gw
    import groupdocs.watermark.watermarks as gww
    import groupdocs.watermark.options.pdf as gwop
    import groupdocs.watermark.common as gwc

    # Instanciar Watermarker que pase por la ruta PDF
    pdf_lo = gwop.PdfLoadOptions()
    with gw.Watermarker("source.pdf", pdf_lo) as watermarker:
        options = gwop.PdfArtifactWatermarkOptions()

        # Personalice las opciones de marca de agua
        text_watermark = 
            gww.TextWatermark("Approved", gww.Font("Arial", 8.0))
        text_watermark.horizontal_alignment = 
            gwc.HorizontalAlignment.RIGHT

        # Aplicar marca de agua al documento PDF
        watermarker.add(text_watermark, options)

        # Guardar documento de resultados
        watermarker.save("result.pdf")

    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark de un vistazo"
  description: "Biblioteca Python para marcas de agua"
  features:
    # feature loop
    - title: "Python Marca de agua del documento"
      content: "Proteja sus datos confidenciales con GroupDocs.Watermark for Python via .NET. Coloque texto o imágenes en varios formatos de archivo como marcas de agua."

    # feature loop
    - title: "Personalizar marcas de agua"
      content: "Muchas opciones de personalización están disponibles en GroupDocs.Watermark for Python via .NET. Configure estilos de texto (negrita, cursiva, fuente) o propiedades de imagen como tamaño o rotación para ajustar las marcas de agua del documento."

    # feature loop
    - title: "Compatibilidad con formatos de archivos populares"
      content: "GroupDocs.Watermark for Python via .NET admite una amplia gama de formatos de archivos, incluidos PDF, documentos de MS Office como Word, Excel, PowerPoint e imágenes como JPEG, PNG, GIF, BMP, diagramas de Visio, correos electrónicos, etc. Mejore el procesamiento de documentos para satisfacer las necesidades comerciales. objetivos."

    # feature loop
    - title: "Búsqueda y actualización de marcas de agua"
      content: "Recupere y actualice marcas de agua colocadas en documentos. Modifique el estilo del texto y el contenido de la imagen o elimínelos por completo. GroupDocs.Watermark for Python via .NET ofrece una amplia gama de capacidades de procesamiento de marcas de agua."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independencia de la plataforma"
  description: "GroupDocs.Watermark for Python via .NET se integra perfectamente con varios sistemas operativos y administradores de paquetes."
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
    GroupDocs.Watermark for Python via .NET le permite procesar una amplia gama de formatos de archivos. [Explore la lista completa](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "Funciones de GroupDocs.Watermark for Python via .NET"
  description: "Fortalezca la seguridad de los documentos mediante marcas de agua programáticas. Procese diversos formatos de archivos, incluidos PDF, DOCX, XLSX, PPTX y formatos de imagen (PNG, JPG, etc.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Control preciso de marcas de agua"
      content: "Administre con precisión marcas de agua agregándolas o eliminándolas de secciones específicas, documentos completos o archivos adjuntos y formas individuales dentro de diferentes formatos de archivo."

    # feature loop
    - icon: "watermark_style"
      title: "Personalizar la apariencia de la marca de agua"
      content: "Ejerza un control detallado sobre la estética de las marcas de agua modificando atributos como el color, la fuente, la opacidad, la rotación y la posición dentro del documento."

    # feature loop
    - icon: "hidden_print"
      title: "Imprimir PDF Marca de agua"
      content: "Agregue marcas de agua ocultas en documentos normales que se vuelven visibles solo durante el proceso de impresión, mejorando discretamente la seguridad de los documentos."

    # feature loop
    - icon: "image_only"
      title: "Marca de agua de imagen específica"
      content: "Marca de agua imágenes específicas dentro de un documento utilizando nuestra solución. Incruste marcas de agua en una sección designada (por ejemplo, página, diapositiva) o en todo el documento."

    # feature loop
    - icon: "image_frame"
      title: "Marcas de agua de imagen multicapa"
      content: "Agregue marcas de agua con precisión a fotogramas específicos dentro de un formato de imagen de varios fotogramas, logrando un control granular sobre la ubicación de las marcas de agua."

    # feature loop
    - icon: "attachments"
      title: "Protección integral de contenido"
      content: "Amplíe la protección a varios elementos del documento, como archivos adjuntos en documentos de Excel y formas de imágenes en presentaciones, proporcionando una capa adicional de seguridad."

    # feature loop
    - icon: "pdf_objects"
      title: "Marca de agua PDF avanzada"
      content: "Marca de agua en diferentes áreas de archivos PDF, incluidos Bleed Box, Art Box, Crop Box, Trim Box, etc."

    # feature loop
    - icon: "doc_background"
      title: "Marca de agua de imagen de fondo"
      content: "Administre marcas de agua dentro de las imágenes de fondo de hojas de cálculo y presentaciones, ofreciendo opciones de personalización adicionales para medidas de seguridad visual."

    # feature loop
    - icon: "unreadable_characters"
      title: "Marca de agua de texto con caracteres ilegibles"
      content: "Emplee caracteres ilegibles dentro de marcas de agua de texto incrustadas en presentaciones, lo que refuerza la seguridad al hacer que la extracción no autorizada de marcas de agua sea significativamente más desafiante."

    # feature loop
    - icon: "watermark_text_search"
      title: "Búsqueda avanzada de marcas de agua"
      content: "Utilice funciones de búsqueda integrales para localizar marcas de agua en documentos según parámetros específicos o combinando varios criterios."

    # feature loop
    - icon: "watermark_image_search"
      title: "Detección de marcas de agua de imágenes similares"
      content: "Encuentre imágenes de marcas de agua similares dentro de documentos que visualmente se parezcan a una imagen original."

    # feature loop
    - icon: "document_info"
      title: "Analizar información del documento"
      content: "Extraiga datos esenciales del documento, como la configuración de la página, para su posterior análisis."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ejemplos de código"
  description: "Explore ejemplos de código que muestran funcionalidades comunes de GroupDocs.Watermark for Python via .NET."
  items:
    # code sample loop
    - title: "Marcar un documento con una imagen"
      content: |
        Utilice GroupDocs.Watermark for Python via .NET para proteger documentos agregando marcas de agua de imagen. [Más información](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Cómo proteger un archivo con una marca de agua de imagen.">}}
        ```python {style=abap}

        # Cargar el documento fuente en Watermarker
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Especificar la ruta a una imagen con marca de agua
            watermark = groupdocs.watermark.watermarks.ImageWatermark("watermark.jpg")
            watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwgroupdocs.watermark.common.VerticalAlignment.CENTER

            # Proteja el archivo y guárdelo
            watermarker.add(watermark)
            watermarker.save("result.pdf")
       
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Buscar y modificar marcas de agua existentes"
      content: |
        GroupDocs.Watermark for Python via .NET le permite administrar marcas de agua de documentos. Selecciona marcas de agua y modifica sus propiedades. [Descubra cómo](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Búsqueda y modificación de marcas de agua.">}}
        ```python {style=abap}

        # Cargar documento fuente
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Busca marcas de agua para actualizarlas
            search_criteria = groupdocs.watermark.search.searchcriteria.TextSearchCriteria("annotation", False)
            watermarks = watermarker.search(search_criteria)
            
            # Actualizar las propiedades deseadas
            for watermark in watermarks:
                watermark.text = "passed"

            # Guardar el documento modificado en una ruta especificada
            watermarker.save("result.pdf")


        ```
        {{< /landing/code >}}

---
