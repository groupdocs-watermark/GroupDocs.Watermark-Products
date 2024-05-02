
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:27:03
draft: false
lang: es
format: Rtf
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Ajustar marca de agua en RTF - GroupDocs.Watermark"
head_description: "Pule tus documentos con precisión con GroupDocs.Watermark. Ajusta y actualiza las marcas de agua sin esfuerzo."

############################# Header ############################
title: "Pule tus RTF documentos: edición de marcas de agua" 
description: "Refina tus documentos con nuestras completas funciones de edición de marcas de agua. Pule tu contenido con precisión."
subtitle: "GroupDocs.Watermark for Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descárguelo gratis en Maven"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java API"
    link: "/watermark/java/"
    link_title: "Obtenga más información"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Pule tus documentos**: Nuestras completas funciones de edición de marcas de agua te permiten refinar tus documentos con precisión. Desde pequeños ajustes hasta transformaciones completas, consiga resultados impecables sin esfuerzo.

############################# Steps ############################
steps:
    enable: true
    title: "Ajuste las marcas de agua de los documentos Rtf con Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** permite a Java desarrolladores ajustar fácilmente las marcas de agua en muchos documentos mediante sus aplicaciones. Esta es una guía rápida:
      
      1. **Watermarker**. Proporcione un flujo de bytes o archivos o una ruta de disco local.
      2. **Criterios de búsqueda** para identificar las marcas de agua con las propiedades específicas que se agregaron anteriormente al documento.
      3. Tras la búsqueda, recibirás una lista de las marcas de agua relevantes. A continuación, podrás ajustar sus propiedades, como el tamaño, la alineación de la página, el texto, el color, el contenido de la imagen, etc. Esto ofrece un alto grado de personalización de sus datos.
      4. Cuando hayas terminado de ajustar las marcas de agua, guarda el documento actualizado. Puedes usar una ruta de archivo local o una transmisión para almacenar el resultado.
   
    code:
      platform: "net"
      copy_title: "Copiar"
      install:
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-watermark</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "haga clic para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Más ejemplos"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
        #  loop
        - title: "Documentación"
          link: "https://docs.groupdocs.com/watermark/java/"
          
      content: |
        ```java {style=abap}
        // Ajustar la marca de agua de la imagen RTF

        // Crea una instancia de Watermarker con RTF
        Watermarker watermarker = new Watermarker("input.rtf");
        
        // Inicialice los criterios de búsqueda para que coincidan con una imagen en particular
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);

        for (PossibleWatermark watermark : watermarks)
        {
            // Reemplazar la imagen que se encontró
            watermark.setImageData(imageData);
        }

        // Guardar archivo ajustado
        watermarker.save("output.rtf");
        
        ```
        
############################# More features ############################
more_features:
  enable: true
  title: "Administración avanzada de marcas de agua RTF para aplicaciones Java"
  description: "La API GroupDocs.Watermark permite a los desarrolladores integrar sin problemas la funcionalidad de marca de agua en sus Java aplicaciones. Permite añadir, editar, eliminar y buscar marcas de agua en una amplia gama de formatos de documentos."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Ajuste de marca de agua"
  features:
    # feature loop
    - title: "Integración sencilla de marcas de agua"
      content: "GroupDocs.Watermark simplifica el proceso de añadir diversas marcas de agua a varios documentos y archivos empresariales dentro de Java aplicaciones. Los desarrolladores no solo pueden aplicar marcas de agua, sino también actualizar o eliminar las existentes mediante programación."

    # feature loop
    - title: "Personalización granular de marcas de agua"
      content: "La API ofrece amplias opciones de personalización para las marcas de agua. Los desarrolladores pueden ajustar fácilmente el tamaño, la rotación, el color, la fuente, los estilos y otras propiedades para lograr el efecto visual deseado."

    # feature loop
    - title: "Aprovechar las funciones de los documentos nativos de RTF"
      content: "Según el formato del documento de destino, los desarrolladores pueden utilizar funcionalidades nativas para colocar marcas de agua. Estas funcionalidades pueden incluir el fondo de la página del documento, anotaciones, encabezados u otros objetos como contenedores de marcas de agua."
      
  code_samples:
    # code sample loop
    - title: "Ajustar la marca de agua de la imagen en las hojas de cálculo"
      content: |
        Este ejemplo muestra cómo ajustar la imagen de las formas particulares en una hoja de cálculo Excel.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Cargar documento como hoja de cálculo
        SpreadsheetLoadOptions loadOptions = new SpreadsheetLoadOptions();
        Watermarker watermarker = new Watermarker("source.xlsx", loadOptions);

        //  Obtenga nuevos bytes de marca de agua
        File file = new File("new_watermark.png");
        byte[] imageBytes = new byte[(int) file.length()];
        FileInputStream inputStream = new FileInputStream(file);
        inputStream.read(imageBytes);
        inputStream.close();

        //  Ajustar el contenido de una marca de agua en particular
        for (SpreadsheetShape shape : content.getWorksheets().get_Item(0).getShapes())
        {
            if (shape.getImage() != null)
            {
                shape.setImage(new SpreadsheetWatermarkableImage(imageBytes));
            }
        }

        //  Guardar documento de resultados
        watermarker.save("result.xlsx");
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
    - title: "Maven descargar"
      link: "https://releases.groupdocs.com/watermark/java/"
      color: "red"
        #  loop
    - title: "Licencias"
      link: "https://purchase.groupdocs.com/pricing/watermark/java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Documento polaco Marcas de agua en otros formatos con GroupDocs.Watermark for Java"
    exclude: "RTF"
    description: "Refina tus documentos con precisión con nuestras completas funciones de edición de marcas de agua. Mejore la autenticidad de los documentos sin esfuerzo."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/java/adjust//pdf/"
          description: "Formato de documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/java/adjust//word/"
          description: "MS Word y documentos de Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/java/adjust//excel/"
          description: "MS Excel y hojas de cálculo de Open Office"

        # format loop 4
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/adjust//powerpoint/"
          description: "MS PowerPoint y presentaciones de Open Office"

        # format loop 5
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/java/adjust//docx/"
          description: "Documento XML abierto de Microsoft Word"
          
        # format loop 6
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/java/adjust//pptx/"
          description: "PowerPoint Presentación XML abierta"
          
        # format loop 7
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/java/adjust//xlsx/"
          description: "Hoja de cálculo XML abierta de Microsoft Excel"

        # format loop 8
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/java/adjust//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/java/adjust//xls/"
          description: "Libro de trabajo Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/java/adjust//ppt/"
          description: "PowerPoint Presentación 97-2003"

        # format loop 11
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/java/adjust//rtf/"
          description: "Formato de texto enriquecido"

---