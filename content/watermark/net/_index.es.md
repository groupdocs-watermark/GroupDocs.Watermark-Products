---
############################# Static ############################
layout: "landing"
date: 2024-04-29T14:27:13
draft: false

lang: es
product: "Watermark"
product_tag: "watermark"
platform: "Net"
platform_tag: "net"

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
head_title: "Software de marcas de agua para documentos C# .NET | agregar marca de agua"
head_description: "Biblioteca C# .NET para agregar, buscar y eliminar marcas de agua en documentos: PDF, Word, Excel, presentaciones, Visio diagramas, formatos de archivos de imagen y correo electrónico."

############################# Header ############################
title: "Añade marcas de agua a los documentos fácilmente en tus aplicaciones de C# .NET"
description: "Potencie sus soluciones de C# con una API flexible de marcas de agua de documentos que permite agregar marcas de agua personalizables a todos los formatos de documentos populares."
words:
  for: "por"

actions:
  main: "Descarga gratuita de NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Watermark"
  alt: "Licencias"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/net/"
  title: "¿Estás listo para empezar?"
  description: "Pruebe GroupDocs.Watermark funciones de forma gratuita o solicite una licencia"

release:
  title: "Publicada la versión {0}"
  notes: "Vea qué hay de nuevo"
  downloads: "Descargas"

code:
  title: "Marca con marca de agua PDF archivos en C#"
  more: "Más ejemplos"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
  install: "dotnet add package GroupDocs.Watermark"
  content: |
    ```csharp {style=abap}   
    // Instanciar Watermarker que pase por la ruta PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    using (Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions))
    {
        // Personalice las opciones de marca de agua
        TextWatermark textWatermark = 
            new TextWatermark("Approved", new Font("Arial", 8));
        
        // Aplicar marca de agua al documento PDF
        watermarker.Add(textWatermark);

        // Guardar documento de resultados
        watermarker.Save("result.pdf");
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark de un vistazo"
  description: "API para poner marcas de agua en los documentos a través de .NET"
  features:
    # feature loop
    - title: "Marca de agua de archivos C#"
      content: "Añade marcas de agua a tus archivos empresariales con GroupDocs.Watermark. Usa texto, imágenes, diagramas o archivos adjuntos de correo electrónico."

    # feature loop
    - title: "Personaliza las marcas de agua según tus objetivos"
      content: "El software GroupDocs.Watermark for .NET permite personalizar las marcas de agua de varias maneras. Los estilos de texto como la negrita, la cursiva y los tipos de fuente, junto con las propiedades de la imagen, como la rotación, etc., enriquecen el proceso de creación de marcas de agua."

    # feature loop
    - title: "Se admiten todos los formatos de archivo populares"
      content: "La solución GroupDocs.Watermark admite muchos formatos de archivos y documentos. PDF, Microsoft Office Word, Excel, PowerPoint, imágenes como JPEG, PNG, GIF, BMP, Visio diagramas, correos electrónicos, etc. podrían protegerse con nuestras marcas de agua."

    # feature loop
    - title: "Búsqueda y actualización de marcas de agua"
      content: "Las marcas de agua que ya están presentadas en un documento se pueden encontrar y procesar de nuevo. Modifique el texto, el estilo, las imágenes o elimine las marcas de agua reveladas sin esfuerzo adicional."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independencia de la plataforma"
  description: "GroupDocs.Watermark for .NET admite los sistemas operativos, los marcos y los administradores de paquetes que se enumeran a continuación"
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de archivo compatibles"
  description: |
    GroupDocs.Watermark for .NET permite procesar los siguientes [formatos de archivo](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark características"
  description: "Proteja PDF, Office, imágenes y otros formatos con una marca de agua"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Marcas de agua de documentos"
      content: "Agregue o elimine marcas de agua de una sección en particular o de un documento completo de varios formatos de archivo."

    # feature loop
    - icon: "watermark_style"
      title: "Dale estilo a tu marca de agua"
      content: "Personalice varias propiedades de marca de agua como el color, la fuente, la rotación, etc."

    # feature loop
    - icon: "hidden_print"
      title: "PDF filigrana de impresión oculta"
      content: "Asigne una marca de agua oculta a PDF que solo aparece al imprimir un documento."

    # feature loop
    - icon: "image_only"
      title: "Añade marcas de agua solo a las imágenes de los documentos"
      content: "Añade marcas de agua a todas las imágenes de una sección, página, diapositiva o documento en particular."

    # feature loop
    - icon: "image_frame"
      title: "Procesar los marcos de imagen seleccionados"
      content: "Asigne marcas de agua solo a fotogramas particulares de una imagen con varios marcos."

    # feature loop
    - icon: "attachments"
      title: "Adjuntos y formas"
      content: "Establezca una marca de agua en todos los archivos adjuntos de un documento Excel y en todas las formas de imagen de las diapositivas."

    # feature loop
    - icon: "pdf_objects"
      title: "PDF objetos"
      content: "Alinee Watermark con Bleed Box, Art Box, Crop Box o Trim Box en el documento PDF."

    # feature loop
    - icon: "doc_background"
      title: "Antecedentes de los documentos"
      content: "Coloque una marca de agua o elimínela de las imágenes de fondo de la hoja de cálculo o las diapositivas."

    # feature loop
    - icon: "unreadable_characters"
      title: "Protección de caracteres ilegibles"
      content: "Proteja la marca de agua del texto con caracteres ilegibles en las presentaciones."

    # feature loop
    - icon: "watermark_text_search"
      title: "Buscar marcas de agua en documentos"
      content: "Busque marcas de agua en función de parámetros específicos o mediante la combinación de varios criterios."

    # feature loop
    - icon: "watermark_image_search"
      title: "Buscar marcas de agua de imágenes similares"
      content: "Busque marcas de agua de imagen que se parezcan a una imagen en particular."

    # feature loop
    - icon: "document_info"
      title: "Obtenga información del documento"
      content: "Extraiga programáticamente la configuración de la página y otra información para los formatos compatibles."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ejemplos de código"
  description: "Algunos casos de uso de operaciones típicas de GroupDocs.Watermark for .NET"
  items:
    # code sample loop
    - title: "Añade una marca de agua añadiendo una imagen a un documento."
      content: |
        Para proteger cualquier documento, puedes usar [marcas de agua de imagen](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/):
        {{< landing/code title="Cómo proteger un archivo con una marca de agua de imagen.">}}
        ```csharp {style=abap}
        // Cargar el documento fuente en Watermarker
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Especificar la ruta a una imagen con marca de agua
            using (ImageWatermark watermark = new ImageWatermark("watermark.jpg"))
            {
                // Proteja el archivo y guárdelo
                watermarker.Add(watermark);

                watermarker.Save("result.pdf");
            }
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Busca y modifica las marcas de agua existentes."
      content: |
        GroupDocs.Watermark puede [modificar las marcas de agua](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/) que ya están presentadas en un documento. Busque los elementos deseados y actualice sus propiedades.
        {{< landing/code title="Búsqueda y modificación de marcas de agua.">}}
        ```csharp {style=abap}   
        // Cargar documento fuente
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Busca marcas de agua para actualizarlas
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                // Actualizar las propiedades deseadas
                watermark.Text = "New Text";
            }

            // Guardar el documento modificado en una ruta especificada
            watermarker.Save("document.pdf");
        }
        ```
        {{< /landing/code >}}

---
