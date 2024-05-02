
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:26:57
draft: false
lang: es
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Ajustar la herramienta de marca de agua Excel - GroupDocs.Watermark"
head_description: "Ajusta, actualiza y gestiona las marcas de agua sin esfuerzo con GroupDocs.Watermark. Personalice sus documentos con facilidad."

############################# Header ############################
title: "Herramienta de ajuste de hojas de cálculo y marcas de agua: poderosamente simple" 
description: "Mejore sus documentos con nuestra intuitiva herramienta de edición de marcas de agua. Simplifique su flujo de trabajo sin esfuerzo."
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
       **Herramienta de ajuste de marcas de agua**: Nuestra herramienta de marcas de agua ofrece una solución fácil de usar para mejorar y proteger sus documentos. Con funciones de edición intuitivas, administrar las marcas de agua es sencillo, lo que garantiza la seguridad y la autenticidad de los documentos.

############################# Steps ############################
steps:
    enable: true
    title: "Ajuste las marcas de agua en Excel documentos con Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** facilita a los Java desarrolladores el ajuste de las marcas de agua de texto en sus aplicaciones mediante la implementación de unos sencillos pasos:
      
      1. **Watermarker**. Puedes proporcionar el archivo para su posterior procesamiento como transmisión o como una ruta en un disco local.
      2. **Los criterios de búsqueda** ayudan a identificar las marcas de agua con las propiedades correctas que se agregaron previamente a un documento.
      3. **Búsqueda**. Ajuste las propiedades de las marcas de agua encontradas, como el tamaño, la alineación de la página, el texto, el color, el contenido de la imagen, etc. Hay muchas maneras de personalizar los datos.
      4. Después de completar el proceso de ajuste de las marcas de agua, debe guardar el documento actualizado. Utilice la ruta del archivo local, el archivo o el flujo de bytes para almacenar el resultado.
   
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

        // Ajustar la marca de agua del texto EXCEL

        // Instanciar Watermarker con el documento de entrada EXCEL
        Watermarker watermarker = new Watermarker("input.xslx");

        // Inicialice los TextSearchCriteria y busque marcas de agua de texto
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        
        // Ajustar las propiedades de las marcas de agua del texto
        for (PossibleWatermark watermark : watermarks)
        {
            watermark.getFormattedTextFragments().clear();
            watermark.getFormattedTextFragments().
                add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
        }

        // Guardar el documento actualizado
        watermarker.save("output.xslx");
        
        ```            
        
############################# More features ############################
more_features:
  enable: true
  title: "Sumérjase en el ajuste de marcas de agua de EXCEL"
  description: "Nuestra API permite a Java aplicaciones añadir, editar, eliminar y buscar marcas de agua en los formatos de documentos más populares."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Ajustar marca de agua"
  features:
    # feature loop
    - title: "Añade marcas de agua a tus documentos sin esfuerzo"
      content: "GroupDocs.Watermark simplifica la marca de agua para Java desarrolladores. Añada diversas marcas de agua a varios documentos y archivos empresariales. No solo puede aplicar marcas de agua, sino que también puede actualizar o eliminar las existentes."

    # feature loop
    - title: "Personalice las marcas de agua según sus necesidades"
      content: "Nuestra API ofrece amplias opciones de personalización. Ajusta fácilmente el tamaño, la rotación, el color, la fuente, los estilos y más para lograr la marca de agua perfecta."

    # feature loop
    - title: "Utilice EXCEL funciones de documentos nativos"
      content: "Según el formato específico del documento, puede utilizar las funcionalidades nativas. Estas pueden incluir el fondo de la página del documento, las anotaciones, los encabezados u otros objetos como contenedores de marcas de agua."
      
  code_samples:
    # code sample loop
    - title: "PDF ajustar la marca de agua del texto"
      content: |
        En este ejemplo se muestra cómo ajustar el texto de los artefactos en particular.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Cargar documento PDF
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Obtenga el contenido del documento
        PdfContent pdfContent = watermarker.getContent(PdfContent.class);

        //  Ajustar el texto de una marca de agua en particular
        for (PdfArtifact artifact : pdfContent.getPages().get_Item(0).getArtifacts())
        {
            if (artifact.getText().contains("Test"))
            {
                artifact.setText("Passed");
            }
        }

        //  Guarda el documento
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
    title: "Ajuste la marca de agua mediante GroupDocs.Watermark for Java para otros formatos"
    exclude: "EXCEL"
    description: "Personalice fácilmente las marcas de agua en una amplia gama de formatos de documentos. Mejore la seguridad y la autenticidad de los documentos sin esfuerzo."
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