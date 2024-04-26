
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:59
draft: false
lang: es
format: Word
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Actualiza fácilmente las marcas de agua en WORD"
head_description: "Simplifique la actualización de marcas de agua en formatos de documento WORD con GroupDocs.Watermark utilizando Node.js via Java. Potencie sus soluciones empresariales."

############################# Header ############################
title: "Optimice la actualización de marcas de agua de documentos de WORD" 
description: "Desbloquee capacidades eficientes de actualización de marcas de agua con GroupDocs.Watermark for Node.js via Java. Proteja sus documentos empresariales con una variedad de marcas de agua. Actualice los atributos de las marcas de agua, como el tamaño, la alineación, el ángulo de rotación y la posición, según sus necesidades."
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
    title: "GroupDocs.Watermark for Node.js via Java habilidades"
    link: "/watermark/nodejs-java/"
    link_title: "Obtenga más información"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java ofrece una solución perfecta para gestionar marcas de agua mediante aplicaciones Node.js via Java. Esta versátil herramienta permite a los desarrolladores editar sin esfuerzo marcas de agua en documentos de varios formatos de archivo, incluidos PDF, Microsoft Word, Excel, PowerPoint, Visio, correo electrónico y formatos de imagen. GroupDocs.Watermark es compatible con los principales sistemas operativos y versiones Node.js via Java.

############################# Steps ############################
steps:
    enable: true
    title: "Actualiza las marcas de agua en WORD a través de Node.js via Java"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** equipa a Node.js via Java desarrolladores con una API sólida para actualizar mediante programación las marcas de agua de varios WORD documentos. Esta guía describe el proceso:
      
      1. **Watermarker**. En función de sus necesidades, el archivo se puede proporcionar como una transmisión o como referencia a una ubicación de disco local.
      2. **SearchCriteria** para identificar las marcas de agua específicas que requieren modificación. Este objeto permite localizar las marcas de agua en función de las propiedades deseadas.
      3. Al ejecutar correctamente la búsqueda, recibirás una colección de marcas de agua relevantes. Estas marcas de agua ofrecen un control detallado, lo que te permite actualizar propiedades como las dimensiones, el posicionamiento de la página, el contenido del texto, la combinación de colores, los datos de las imágenes, etc.
      4. Tras completar las actualizaciones de las marcas de agua, conserve el documento modificado. La API facilita el almacenamiento mediante una ruta de archivo local o un objeto de transmisión.
   
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

        // Actualizar marca de agua de texto WORD

        // Proporcione una instancia de Watermarker para el archivo WORD
        const watermarker = new groupdocs.watermark.Watermarker("input.docx");

        // Usa TextSearchCriteria para buscar marcas de agua de texto
        const searchCriteria = 
            new groupdocs.watermark.TextSearchCriteria("test", false);
        const watermarks = watermarker.search(searchCriteria);
        
        // Actualizar marca de agua de texto
        for (const watermark of watermarks.getInnerList().toArray())
        {
            watermark.setText("passed");
        }

        // Disfruta el resultado
        watermarker.save("output.docx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Dominar la edición de marcas de agua en PDF s con GroupDocs.Watermark"
  description: "Explore las funciones integrales de la API para ajustar y administrar las marcas de agua en PDF s dentro de Node.js via Java aplicaciones."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Editar marca de agua"
  features:
    # feature loop
    - title: "Edita marcas de agua sin esfuerzo en PDF s"
      content: "GroupDocs.Watermark ofrece herramientas sólidas en Node.js via Java para editar sin problemas las marcas de agua existentes en PDF documentos. Ajusta la posición, la transparencia y más con facilidad."

    # feature loop
    - title: "Refina los detalles de las marcas de agua para mayor precisión"
      content: "Toma el control de los detalles. Nuestra API te permite ajustar la apariencia de las marcas de agua, lo que permite modificar con precisión el tamaño, la opacidad y el color de tus PDF s."

    # feature loop
    - title: "Gestión simplificada de marcas de agua"
      content: "Nuestra API simplifica la administración de marcas de agua. Ya sea que actualices o elimines, puedes administrar las marcas de agua de manera eficiente, manteniendo la integridad de los documentos y, al mismo tiempo, satisfaciendo tus necesidades de marca."
      
  code_samples:
    # code sample loop
    - title: "Java Ejemplo: Editar PDF Filigrana"
      content: |
        En este ejemplo de Java se muestra cómo editar una marca de agua existente en un documento PDF y se muestra cómo ajustar sus propiedades mediante programación.
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Cargue el documento PDF para procesarlo
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  Busca marcas de agua específicas que cumplan tus criterios
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria("test", false);
            const watermarks = watermarker.search(searchCriteria);
  
            //  Edita la configuración de la marca de agua, como el tamaño, el color y la posición
            for (const watermark of watermarks.getInnerList().toArray()) {
                watermark.getFormattedTextFragments().clear();
                watermark.getFormattedTextFragments().add("passed", 
                    new groupdocsWatermark.Font("Calibri", 19, groupdocsWatermark.FontStyle.Bold), 
                    groupdocsWatermark.Color.getRed(), groupdocsWatermark.Color.getAqua());
            }

            //  Guarde el documento actualizado en un sistema local o transfiéralo directamente
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
    title: "Actualizar marcas de agua en otros formatos de archivo"
    exclude: "WORD"
    description: "Simplifica la edición de marcas de agua en PDF, Word, Excel y más con GroupDocs.Watermark for Node.js via Java. Se admiten todos los formatos empresariales más populares."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/update//pdf/"
          description: "Formato de documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/nodejs-java/update//word/"
          description: "MS Word y documentos de Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/update//excel/"
          description: "MS Excel y hojas de cálculo de Open Office"

        # format loop 4
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/update//powerpoint/"
          description: "MS PowerPoint y presentaciones de Open Office"

        # format loop 5
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/update//docx/"
          description: "Documento XML abierto de Microsoft Word"
          
        # format loop 6
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/update//pptx/"
          description: "PowerPoint Presentación XML abierta"
          
        # format loop 7
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/update//xlsx/"
          description: "Hoja de cálculo XML abierta de Microsoft Excel"

        # format loop 8
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/update//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/update//xls/"
          description: "Libro de trabajo Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/update//ppt/"
          description: "PowerPoint Presentación 97-2003"

        # format loop 11
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/update//rtf/"
          description: "Formato de texto enriquecido"

---