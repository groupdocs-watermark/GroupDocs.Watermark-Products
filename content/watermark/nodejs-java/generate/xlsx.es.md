
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:16
draft: false
lang: es
format: Xlsx
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Inserte marcas de agua en XLSX con Node.js"
head_description: "Aproveche Node.js para generar y aplicar marcas de agua en XLSX archivos y proteger sus Excel documentos."

############################# Header ############################
title: "Proteja XLSX hojas con Node.js" 
description: "Utilice la API Node.js para crear marcas de agua personalizables para XLSX archivos, perfectas para mejorar la integridad de los documentos y proteger la información confidencial."
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descárguelo gratis en NPM"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "Obtenga más información"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java proporciona una solución eficaz para que los desarrolladores de Node.js generen, añadan y gestionen marcas de agua en archivos XLSX. Esta API es esencial para mantener la confidencialidad y la autenticidad de los Excel documentos, especialmente en entornos corporativos, financieros y legales. Personalice sus marcas de agua con una variedad de opciones, incluidas las superposiciones de texto e imágenes, diseñadas para ser tanto funcionales como sutiles. Las funciones adicionales permiten crear marcas de agua automatizadas en función de las propiedades del documento y las condiciones definidas por el usuario, lo que garantiza que las marcas de agua se apliquen de forma coherente y solo cuando sea necesario. GroupDocs.Watermark es compatible con las plataformas .NET actuales y admite Excel funcionalidades avanzadas.

############################# Steps ############################
steps:
    enable: true
    title: "Proteja documentos comerciales: genere Xlsx marcas de agua"
    content: |
      Fortalezca la seguridad de los documentos con **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/):**: una potente solución de generación de marcas de agua para Node.js via Java.
      
      1. **Simplifique la creación de marcas de agua seguras en sus aplicaciones Node.js via Java:** La clase **Watermarker** actúa como el componente principal de la API GroupDocs.Watermark. Esta biblioteca simplifica la generación de marcas de agua en varios formatos de documentos, incluido Xlsx. Para comenzar, cree una instancia de Watermarker antes de procesar su documento. Proporcione la ruta del archivo Xlsx o un objeto de secuencia al constructor durante la inicialización.
      2. **Genere marcas de agua para una protección mejorada:** Ofrezca marcas de agua que se alineen perfectamente con sus necesidades de seguridad. Construya un objeto **Watermark** especificando el tipo deseado. A diferencia de la ubicación de páginas tradicional, puede incrustar marcas de agua dentro de elementos nativos del documento, como encabezados o archivos adjuntos, fortaleciendo la seguridad del documento y agregando un toque profesional.
      3. **Ajuste la apariencia de las marcas de agua para lograr un impacto óptimo:** Controle los aspectos visuales de sus marcas de agua. Personalice propiedades como altura, ancho, alineación (arriba, izquierda, centro, etc.), familias de fuentes y colores para lograr un resultado visualmente efectivo y consistente que refuerce la legitimidad del documento.
      4. **Aplicación de marca de agua y almacenamiento seguro**: incorpore sus marcas de agua utilizando el método **Watermarker**. La biblioteca le permite agregar múltiples marcas de agua si es necesario para una protección mejorada. Se recomienda guardar el documento Xlsx modificado en una ubicación segura e independiente para conservar el archivo original y salvaguardar sus documentos con marca de agua.
   
    code:
      platform: "net"
      copy_title: "Copiar"
      install:
        command: "npm i @groupdocs/groupdocs.watermark"
        copy_tip: "haga clic para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Más ejemplos"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
        #  loop
        - title: "Documentación"
          link: "https://docs.groupdocs.com/watermark/nodejs-java/"
          
      content: |
        ```javascript {style=abap}

        // Generar marca de agua de imagen para XLSX

        // Crear una instancia de Watermarker pasando el archivo fuente
        const watermarker = new groupdocs.watermark.Watermarker("input.xlsx");
        
        // Generar marca de agua proporcionando un archivo de imagen
        const watermark = new groupdocs.watermark.ImageWatermark("watermark.png");

        // Obtener el resultado XLSX
        watermarker.add(watermark);
        watermarker.save("output.xlsx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Integración refinada de marcas de agua"
  description: "Nuestra API GroupDocs.Watermark para desarrolladores de .NET ofrece soluciones refinadas para integrar marcas de agua sin problemas en cualquier documento. Esta herramienta está diseñada para crear marcas de agua sofisticadas y discretas que garanticen la protección de los derechos de autor y, al mismo tiempo, mantengan la estética del documento."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Integración de Precision Watermark"
  features:
    # feature loop
    - title: "Efectos de marca de agua de gradiente"
      content: "Implemente marcas de agua con degradado que se mezclen sin problemas en sus documentos. Esta función permite utilizar degradados lineales o radiales, lo que añade un aspecto moderno a las funciones de seguridad y mejora tanto la protección como la interacción visual sin sobrecargar el contenido."

    # feature loop
    - title: "Marcas de agua con patrones para mayor seguridad"
      content: "Usa marcas de agua basadas en patrones para agregar una capa adicional de seguridad. Nuestra API admite varios patrones que pueden diseñarse de forma compleja y repetirse en todo el documento, lo que hace que la marca de agua sea más resistente a la manipulación y la eliminación."

    # feature loop
    - title: "Marcas de agua específicas del documento"
      content: "Personalice las marcas de agua de forma exclusiva para los diferentes tipos de documentos. Ya se trate de contratos legales, planes de negocios o informes científicos, personalice las marcas de agua para que se adapten al propósito del documento y a la accesibilidad del lector, garantizando una integración y una seguridad óptimas."
      
  code_samples:
    # code sample loop
    - title: "Generar marca de agua de imagen PDF"
      content: |
        Genere marcas de agua para todas las imágenes presentadas dentro de un documento PDF
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Cargar documento como PDF
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  Crear marca de agua basada en la anotación PDF
            const imageWatermark = new groupdocsWatermark.ImageWatermark("watermark.jpg");
            imageWatermark.setHorizontalAlignment(groupdocsWatermark.HorizontalAlignment.Center);
            imageWatermark.setVerticalAlignment(groupdocsWatermark.VerticalAlignment.Center);
            imageWatermark.setRotateAngle(-45);
            imageWatermark.setSizingType(groupdocsWatermark.SizingType.ScaleToParentDimensions);
            imageWatermark.setScaleFactor(1);
  
            //  Configurar las opciones de marca de agua
            const images = watermarker.getImages();
            for (let i = 0; i < images.getCount(); i++) {
                if (images.get_Item(i).getWidth() > 100 && images.get_Item(i).getHeight() > 100) {
                    images.get_Item(i).add(imageWatermark);
                }
            }

            //  Añadir marca de agua de texto al documento de resultados
            watermarker.save("result.pdf");
            watermarker.close();

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "¿Estás listo para empezar?"
  description: "Pruebe GroupDocs.Watermark funciones de forma gratuita o solicite una licencia"
  items:
    #  loop
    - title: "NPM descargar"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licencias"
      link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Implementación de marcas de agua en XLSX con Node.js"
    exclude: "XLSX"
    description: "Implemente Node.js para añadir de manera eficiente marcas de agua avanzadas y seguras a XLSX archivos, protegiendo así sus Excel datos profesionales."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/generate//pdf/"
          description: "Formato de documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/nodejs-java/generate//word/"
          description: "MS Word y documentos de Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/generate//excel/"
          description: "MS Excel y hojas de cálculo de Open Office"

        # format loop 4
        - name: "Imagen de marca de agua"
          format: "IMAGE"
          link: "/watermark/nodejs-java/generate//image/"
          description: "Formatos de imagen populares"

        # format loop 5
        - name: "Foto con marca de agua"
          format: "PHOTO"
          link: "/watermark/nodejs-java/generate//photo/"
          description: "Formatos de fotos"

        # format loop 6
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/generate//powerpoint/"
          description: "MS PowerPoint y presentaciones de Open Office"

        # format loop 7
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/generate//docx/"
          description: "Documento XML abierto de Microsoft Word"
          
        # format loop 8
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/generate//pptx/"
          description: "PowerPoint Presentación XML abierta"
          
        # format loop 9
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/generate//xlsx/"
          description: "Hoja de cálculo XML abierta de Microsoft Excel"

        # format loop 10
        - name: "Filigrana JPEG"
          format: "JPEG"
          link: "/watermark/nodejs-java/generate//jpeg/"
          description: "JPEG Imagen"

        # format loop 11
        - name: "Filigrana PNG"
          format: "PNG"
          link: "/watermark/nodejs-java/generate//png/"
          description: "Portable Gráfico de red"

        # format loop 12
        - name: "Filigrana TIFF"
          format: "TIFF"
          link: "/watermark/nodejs-java/generate//tiff/"
          description: "Formato de archivo de imagen de etiqueta"

        # format loop 13
        - name: "Filigrana WEBP"
          format: "WEBP"
          link: "/watermark/nodejs-java/generate//webp/"
          description: "Imagen WEB"

        # format loop 14
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/generate//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 15
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/generate//xls/"
          description: "Libro de trabajo Microsoft Excel 97-2003"

        # format loop 16
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/generate//ppt/"
          description: "PowerPoint Presentación 97-2003"

        # format loop 17
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/generate//rtf/"
          description: "Formato de texto enriquecido"

---