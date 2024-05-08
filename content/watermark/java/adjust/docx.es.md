
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:21
draft: false
lang: es
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Ajustar marcas de agua en DOCX documentos - GroupDocs.Watermark"
head_description: "Edite las marcas de agua de manera eficiente en diversos formatos de documentos con GroupDocs.Watermark. Mejore la autenticidad de los documentos."

############################# Header ############################
title: "Ajustar DOCX marcas de agua: personalización perfecta" 
description: "Personalice sus documentos sin problemas con nuestra eficiente herramienta de edición de marcas de agua. Mejore la imagen de su marca sin esfuerzo."
subtitle: "GroupDocs.Watermark for Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descarga gratuita de Maven"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java API"
    link: "/watermark/java/"
    link_title: "Obtenga más información"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Editar marcas de agua**: personalice sin problemas sus documentos con nuestras potentes herramientas de edición. Ya sea para ajustar la ubicación o modificar el contenido, consiga los efectos de marca de agua que desee sin esfuerzo.

############################# Steps ############################
steps:
    enable: true
    title: "Ajuste las marcas de agua del documento Docx usando Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** permite a los desarrolladores de Java ajustar fácilmente las marcas de agua en muchos documentos utilizando sus aplicaciones. Aquí tienes una guía rápida:
      
      1. En primer lugar, debe pasar el archivo Docx como parámetro del constructor de la clase **Watermarker**. Proporcione una secuencia de bytes o archivos o una ruta de disco local.
      2. En segundo lugar, ubique las marcas de agua que deben ajustarse. Utilice **SearchCriteria** para identificar marcas de agua con las propiedades específicas agregadas previamente al documento.
      3. Después de la búsqueda, recibirá una lista de marcas de agua relevantes. Luego puede ajustar sus propiedades, incluido el tamaño, la alineación de la página, el texto, el color, el contenido de la imagen y más. Esto ofrece un alto grado de personalización de sus datos.
      4. Una vez que haya terminado de ajustar las marcas de agua, guarde el documento actualizado. Puede utilizar una ruta de archivo local o una secuencia para almacenar el resultado.
   
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
        // Ajustar la marca de agua de la imagen DOCX

        // Crear una instancia de Watermarker con DOCX
        Watermarker watermarker = new Watermarker("input.docx");
        
        // Inicialice SearchCriteria para que coincida con una imagen en particular
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);

        for (PossibleWatermark watermark : watermarks)
        {
            // Reemplazar la imagen que se encontró
            watermark.setImageData(imageData);
        }

        // Guardar archivo ajustado
        watermarker.save("output.docx");
        
        ```
        
############################# More features ############################
more_features:
  enable: true
  title: "Administración avanzada de marcas de agua DOCX para aplicaciones Java"
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
    - title: "Aprovechar las funciones de los documentos nativos de DOCX"
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
    title: "Modifique las marcas de agua en muchos formatos con GroupDocs.Watermark for Java"
    exclude: "DOCX"
    description: "Edita sin problemas marcas de agua en varios formatos de documentos. Personalice sus documentos sin esfuerzo a la vez que garantiza la protección y la autenticidad."
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