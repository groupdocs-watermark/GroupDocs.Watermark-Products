
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: es
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Añadir Marcas de Agua a Archivos de Excel"
head_description: "Añade automáticamente marcas de agua de imagen a archivos de Excel con Python. Procesa muchos archivos a la vez para una protección consistente."

############################# Header ############################
title: "Añadir Marcas de Agua a Excel con Python" 
description: "Añade fácilmente marcas de agua de texto o imagen a archivos de Excel usando Python. Nuestras guías te muestran cómo mantener tus hojas de cálculo profesionales y seguras con poco trabajo manual."
subtitle: "API GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar PyPi gratis"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Biblioteca GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "Obtenga más información"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET te permite añadir marcas de agua a hojas de cálculo de Excel en Python. Puedes utilizar diferentes tipos de marcas de agua y personalizar la opacidad, la rotación y la alineación. La biblioteca también te ayuda a encontrar y gestionar marcas de agua existentes para mantener tus archivos seguros contra manipulaciones.

############################# Steps ############################
steps:
    enable: true
    title: "Añadir Marcas de Agua: Python Marca de Agua para Excel"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** es una biblioteca que facilita la adición de marcas de agua a muchos tipos de archivos empresariales. Sigue estos pasos para añadir rápidamente marcas de agua a tus documentos en Python:
      
      1. **Comienza con la Marca de Agua:** Empieza creando una instancia de la clase **Watermarker**. Pasa tu archivo Excel (como una ruta o un flujo) al constructor para abrirlo para la marcación con agua.
      2. **Crea Tu Marca de Agua:** Crea un objeto **Watermark** con el texto y las configuraciones deseadas. Puedes añadir marcas de agua a cualquier página o incluso a elementos del documento como encabezados o adjuntos.
      3. **Personaliza la Marca de Agua:** Ajusta el tamaño, la posición, la fuente, el color y la alineación de la marca de agua según tus necesidades. Esto ayuda a que tu marca de agua se vea adecuada en tu documento.
      4. **Aplica y Guarda:** Usa el método **Watermarker** para añadir tus marcas de agua al documento. Guarda el resultado, idealmente en un nuevo archivo por motivos de seguridad.
   
    code:
      platform: "python-net"
      copy_title: "Copiar"
      install:
        command: |
        command: "pip install groupdocs-watermark-net"
        copy_tip: "haga clic para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Más ejemplos"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
        #  loop
        - title: "Documentación"
          link: "https://docs.groupdocs.com/watermark/python-net/"
          
      content: |
        ```python {style=abap}
        # Añadir una marca de agua de texto a un archivo EXCEL
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # Selecciona el archivo que deseas marcar con una marca de agua
        with gw.Watermarker("input.xslx") as watermarker:

            # Crea un objeto de marca de agua de texto
            font = gww.Font("Arial", 36.0)
            watermark = gww.TextWatermark("top secret", font)
            watermark.foreground_color = gww.Color.red
            watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
            watermark.opacity = 0.4

            watermarker.add(watermark)

            # Guarda el archivo EXCEL actualizado
            watermarker.save("output.xslx")
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Explora Más Características de Marcado con Agua"
  description: "Utiliza nuestra API Python para añadir, ver, convertir y gestionar marcas de agua en documentos, diapositivas, diagramas y más. GroupDocs.Watermark for Python via .NET te ayuda a proteger tus archivos y añadir información de derechos de autor de forma sencilla."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Añadir Marca de Agua"
  features:
    # feature loop
    - title: "Añadir Marcas de Agua Rápidamente"
      content: "GroupDocs.Watermark permite a los desarrolladores Python añadir rápidamente marcas de agua de texto, imagen o dinámicas a documentos empresariales. Mantén tus archivos seguros y con marca con un esfuerzo mínimo."

    # feature loop
    - title: "Marcas de Agua Totalmente Personalizables"
      content: "Cambia el tamaño, la rotación, la transparencia, el color y la fuente de la marca de agua con GroupDocs.Watermark. Haz que tu marca de agua se ajuste perfectamente a tu documento y manten el contenido importante visible."

    # feature loop
    - title: "Utiliza Características del Documento para Marcas de Agua"
      content: "Aprovecha las características integradas del documento como anotaciones PDF, fondos de Word o encabezados de Excel para añadir marcas de agua. GroupDocs.Watermark trabaja con estructuras de documentos para un marcado con agua eficaz y no intrusivo."
      
  code_samples:
    # code sample loop
    - title: "Añadir una Marca de Agua de Imagen a DOCX"
      content: |
        Este ejemplo muestra cómo aplicar efectos de imagen a marcas de agua de forma.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.wordprocessing as gwow

        # Abre un documento de Word
        load_options = gwow.WordProcessingLoadOptions()
        with gw.Watermarker("source.docx", load_options) as watermarker:

            # Establece las opciones de la marca de agua
            with gww.ImageWatermark("logo.png") as watermark:

                effects = gwow.WordProcessingImageEffects()
                effects.brightness = 0.7
                effects.contrast = 0.6
                effects.chroma_key = gww.Color.red

                options = gwow.WordProcessingWatermarkSectionOptions()
                options.Effects = effects;

                # Crea la marca de agua
                watermarker.add(watermark, options)

                # Guarda el documento con la marca de agua
                watermarker.save("result.docx")
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "¿Estás listo para empezar?"
  description: "Pruebe GroupDocs.Watermark funciones de forma gratuita o solicite una licencia"
  items:
    #  loop
    - title: "PyPi descargar"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      color: "red"
        #  loop
    - title: "Licencias"
      link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Añadir Marcas de Agua de Texto e Imagen a Excel con Python"
    exclude: "EXCEL"
    description: "Utiliza GroupDocs.Watermark para añadir rápidamente marcas de agua personalizadas a archivos de Excel. Mejora la seguridad del documento y la marca con herramientas flexibles de marcado con agua."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/python-net/add//pdf/"
          description: "Formato de documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/python-net/add//word/"
          description: "MS Word y documentos de Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/python-net/add//excel/"
          description: "MS Excel y hojas de cálculo de Open Office"

        # format loop 4
        - name: "Imagen de marca de agua"
          format: "IMAGE"
          link: "/watermark/python-net/add//image/"
          description: "Formatos de imagen populares"

        # format loop 5
        - name: "Foto con marca de agua"
          format: "PHOTO"
          link: "/watermark/python-net/add//photo/"
          description: "Formatos de fotos"

        # format loop 6
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/add//powerpoint/"
          description: "MS PowerPoint y presentaciones de Open Office"

        # format loop 7
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/python-net/add//docx/"
          description: "Documento XML abierto de Microsoft Word"
          
        # format loop 8
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/python-net/add//pptx/"
          description: "PowerPoint Presentación XML abierta"
          
        # format loop 9
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/python-net/add//xlsx/"
          description: "Hoja de cálculo XML abierta de Microsoft Excel"

        # format loop 10
        - name: "Filigrana JPEG"
          format: "JPEG"
          link: "/watermark/python-net/add//jpeg/"
          description: "JPEG Imagen"

        # format loop 11
        - name: "Filigrana PNG"
          format: "PNG"
          link: "/watermark/python-net/add//png/"
          description: "Portable Gráfico de red"

        # format loop 12
        - name: "Filigrana TIFF"
          format: "TIFF"
          link: "/watermark/python-net/add//tiff/"
          description: "Formato de archivo de imagen de etiqueta"

        # format loop 13
        - name: "Filigrana WEBP"
          format: "WEBP"
          link: "/watermark/python-net/add//webp/"
          description: "Imagen WEB"

        # format loop 14
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/python-net/add//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 15
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/python-net/add//xls/"
          description: "Libro de trabajo Microsoft Excel 97-2003"

        # format loop 16
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/python-net/add//ppt/"
          description: "PowerPoint Presentación 97-2003"

        # format loop 17
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/python-net/add//rtf/"
          description: "Formato de texto enriquecido"

---