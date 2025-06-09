
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:27
draft: false
lang: es
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Marcas de Agua Python para Archivos DOCX"
head_description: "Añada marcas de agua a archivos DOCX en Python para mantener seguros sus documentos de Word."

############################# Header ############################
title: "Asegure DOCX con Marcas de Agua de Python" 
description: "Aplique marcas de agua avanzadas a archivos DOCX en Python—perfecto para proteger sus documentos de Word en cualquier industria."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Consíguelo gratis en PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "Obtenga más información"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET aporta potentes características de marcas de agua a archivos DOCX. Añada marcas de agua que escalen, se muevan y se integren con su documento. Úselo para archivos legales, empresariales o confidenciales, y elija entre marcas de agua de texto o imagen con colocación flexible. GroupDocs.Watermark soporta las últimas características de Python para una protección documentaria de primer nivel.

############################# Steps ############################
steps:
    enable: true
    title: "Añada Marcas de Agua a Archivos Docx Rápidamente"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/):** Una poderosa biblioteca de Python que le permite añadir marcas de agua a sus documentos.
      
      1. **Clase Principal: Watermarker.** Comience creando un objeto **Watermarker**. Proporciónelo su archivo Docx, ya sea como un camino de archivo o como un flujo, para empezar.
      2. **Construya Su Marca de Agua.** A continuación, haga un objeto Watermark del tipo que desee. Puede colocarla en cualquier página o incluso en elementos del documento como imágenes o encabezados.
      3. **Ajuste la Apariencia.** Configure el tamaño, la posición, la fuente y el color de la marca de agua según sus necesidades.
      4. **Añadir y Guardar.** Utilice el método **Watermarker** para insertar su marca de agua. Añada tantas como desee y luego guarde el archivo donde desee.
   
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
        # Añadir una marca de agua de imagen a un archivo DOCX
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # Pase la ruta del archivo al constructor de Watermarker
        with gw.Watermarker("input.docx") as watermarker:

            # Cree una marca de agua de imagen utilizando su archivo de imagen
            watermark = gww.ImageWatermark("watermark.png")

            watermarker.add(watermark)

            # Guarde el archivo DOCX con la marca de agua
            watermarker.save("output.docx")
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "Descubra Más Herramientas de Marcas de Agua"
  description: "GroupDocs.Watermark for Python via .NET le ofrece opciones avanzadas para añadir y personalizar marcas de agua en muchos tipos de archivos. Proteja sus documentos e imágenes con características flexibles y fáciles de usar."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Marca de Agua Todo-en-Uno"
  features:
    # feature loop
    - title: "Tiling a toda página"
      content: "Cubra todo su documento con marcas de agua en mosaico. Esto dificulta la eliminación de marcas de agua y mantiene sus archivos protegidos sin arruinar el diseño."

    # feature loop
    - title: "Colores Personalizados"
      content: "Elija cualquier color para su marca de agua que coincida con su marca o estilo de documento. Haga que su marca de agua se destaque o se mezcle según sea necesario."

    # feature loop
    - title: "Opciones de Seguridad Adicionales"
      content: "Aumente la seguridad de su documento con marcas de agua en capas. Combine marcas visibles y ocultas para evitar la copia y asegúrese de que solo las personas adecuadas puedan acceder a sus archivos."
      
  code_samples:
    # code sample loop
    - title: "Añadir una Marca de Agua a PowerPoint"
      content: |
        Este ejemplo muestra cómo poner una marca de agua en el fondo de las diapositivas de PPTX.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.presentation as gwop

        # Abrir un archivo PPTX
        load_options = gwop.PresentationLoadOptions()
        with gw.Watermarker("source.pptx", load_options) as watermarker:

            # Establecer detalles de la marca de agua
            with TextWatermark("Protected image", gww.Font("Arial", 8.0)) as watermark:

                watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
                watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
                watermark.rotate_angle = 45
                watermark.scale_factor = 1

                # Aplicar la marca de agua a los fondos de las diapositivas
                watermarker.add(watermark)

                # Guardar la presentación actualizada
                watermarker.save("result.pptx")
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
    title: "Añadir Marcas de Agua a DOCX con Python"
    exclude: "DOCX"
    description: "Aprenda a añadir marcas de agua seguras y personalizadas a archivos DOCX en Python para una mejor seguridad documental y control de derechos de autor."
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