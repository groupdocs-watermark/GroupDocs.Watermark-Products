
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
head_title: "Edita Marcas de Agua en Archivos Excel"
head_description: "Con GroupDocs.Watermark for Python via .NET, puedes ajustar la configuración de las marcas de agua para proteger y personalizar tus documentos."

############################# Header ############################
title: "Actualiza Marcas de Agua en Hojas de Cálculo Excel Usando Python" 
description: "Asegura tus hojas de cálculo de Excel con nuestras herramientas flexibles de edición de marcas de agua para Python."
subtitle: "API de GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Consíguelo gratis en PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Biblioteca GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "Obtenga más información"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Edita Rápidamente las Marcas de Agua Excel:** GroupDocs.Watermark for Python via .NET proporciona a los desarrolladores de Python todas las herramientas necesarias para gestionar marcas de agua con un esfuerzo mínimo, mejorando tu flujo de trabajo y seguridad de documentos.

############################# Steps ############################
steps:
    enable: true
    title: "Modificar marcas de agua en documentos Excel con Python"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** ayuda a los desarrolladores de Python a actualizar marcas de agua en varios archivos Excel. A continuación, se muestra cómo puedes utilizarlo en tu proyecto:
      
      1. Primero, abre tu archivo Excel pasándolo al constructor **Watermarker**. Puedes usar una ruta de archivo, flujo de bytes o flujo de archivo.
      2. Luego, encuentra las marcas de agua que deseas cambiar utilizando **SearchCriteria**, que te permite buscar texto o propiedades de la marca de agua.
      3. Una vez encontradas, puedes cambiar detalles como texto, fuente, tamaño, posición, color y más. Esto te brinda control total sobre cómo se ve la marca de agua.
      4. Después de realizar los cambios, guarda el documento. Puedes escribir el resultado en un flujo o en una ruta de archivo.
   
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
        # Actualizar el texto de la marca de agua en EXCEL
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Crear un Watermarker utilizando un archivo EXCEL
        with gw.Watermarker("input.xslx") as watermarker:

            # Configurar TextSearchCriteria para encontrar el texto de la marca de agua
            search_criteria = gwss.TextSearchCriteria("test", False)

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # Modificar el texto de la marca de agua
                        watermark.text = "passed"
                    except Exception as e:
                        pass
            
            watermarker.save("output.xslx")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Descubre más formas de actualizar marcas de agua"
  description: "Con nuestra biblioteca, las aplicaciones Python pueden añadir, encontrar, editar o eliminar marcas de agua en muchos tipos de archivos."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Edición de Marcas de Agua"
  features:
    # feature loop
    - title: "Marca de Agua en Tus Archivos con Comodidad"
      content: "Utiliza GroupDocs.Watermark for Python via .NET para agregar y gestionar marcas de agua en tus documentos. Busca, actualiza o elimina marcas de agua según sea necesario utilizando una API sencilla."

    # feature loop
    - title: "Personaliza las Marcas de Agua según tus Necesidades"
      content: "Ajusta la configuración de las marcas de agua como fuente, tamaño, orientación y color utilizando nuestra flexible API para obtener exactamente el resultado que deseas."

    # feature loop
    - title: "Usa Características Específicas del Formato"
      content: "Dependiendo del formato de archivo, puedes utilizar características nativas como encabezados, pies de página, anotaciones o fondos como áreas de marcas de agua."
      
  code_samples:
    # code sample loop
    - title: "Editar Marca de Agua de Texto en Excel"
      content: |
        Este código muestra cómo cambiar el texto de la marca de agua en hojas de cálculo de Excel.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # Abrir archivo XLSX
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # Leer datos de la hoja de cálculo
        with gw.Watermarker("source.xlsx") as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,3]

            # Cambiar el texto de la marca de agua
            watermarks = watermarker.search(search_criteria)
            for watermark in watermarks:
                try:
                    watermark.formatted_text_fragments.clear()
                    watermark.formatted_text_fragments.add(
                       "passed", 
                        gww.Font("Calibri", 19.0, gww.FontStyle.bold), 
                        gww.Color.red, 
                        gww.Color.aqua
                    )
                except Exception as e:
                    pass
        
            # Guardar el resultado
            watermarker.save("output.xlsx")
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
    title: "Actualizar Marcas de Agua en Otros Formatos"
    exclude: "EXCEL"
    description: "Personaliza fácilmente la configuración de las marcas de agua en diferentes formatos de archivo utilizando GroupDocs.Watermark for Python via .NET."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/python-net/edit//pdf/"
          description: "Formato de documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/python-net/edit//word/"
          description: "MS Word y documentos de Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/python-net/edit//excel/"
          description: "MS Excel y hojas de cálculo de Open Office"

        # format loop 4
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/edit//powerpoint/"
          description: "MS PowerPoint y presentaciones de Open Office"

        # format loop 5
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/python-net/edit//docx/"
          description: "Documento XML abierto de Microsoft Word"
          
        # format loop 6
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/python-net/edit//pptx/"
          description: "PowerPoint Presentación XML abierta"
          
        # format loop 7
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/python-net/edit//xlsx/"
          description: "Hoja de cálculo XML abierta de Microsoft Excel"

        # format loop 8
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/python-net/edit//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/python-net/edit//xls/"
          description: "Libro de trabajo Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/python-net/edit//ppt/"
          description: "PowerPoint Presentación 97-2003"

        # format loop 11
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/python-net/edit//rtf/"
          description: "Formato de texto enriquecido"

---