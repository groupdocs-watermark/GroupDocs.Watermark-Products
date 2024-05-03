
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:04
draft: false
lang: es
format: Photo
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "La creación rápida de marcas de agua para fotografías es más fácil en Java"
head_description: "Optimice la protección de sus fotografías con marcas de agua. Rápido y fiable."

############################# Header ############################
title: "Herramientas eficientes de Java para la creación de marcas de agua en fotografías" 
description: "Añade marcas de agua a tus fotos de forma rápida y eficaz con nuestra API Java. Perfecto para proteger imágenes digitales y mejorar la visibilidad de la marca con un mínimo esfuerzo."
subtitle: "GroupDocs.Watermark for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descárguelo gratis en Maven"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java"
    link: "/watermark/java/"
    link_title: "Obtenga más información"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java está optimizado para crear marcas de agua rápidas y eficaces en los archivos de fotos. Esta herramienta permite la integración rápida de marcas de agua de texto e imágenes en una amplia gama de formatos fotográficos, incluidos JPEG, PNG y BMP. Personalice sus marcas de agua con amplias opciones de estilo, transparencia y ubicación para garantizar que se combinen perfectamente sin disminuir la calidad de la fotografía. Adecuado para operaciones de gran volumen, admite el procesamiento por lotes para aplicar marcas de agua a varias fotografías a la vez, lo que lo hace ideal para empresas y creadores de contenido digital que necesitan proteger sus activos visuales y ponerles marca de manera eficiente

############################# Steps ############################
steps:
    enable: true
    title: "Agregar marca de agua al documento Photo a través de Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** facilita a los desarrolladores de Java agregar marcas de agua de varios tipos a formatos de archivos comerciales populares. Agregue nuestra biblioteca a sus documentos de solicitud y marca de agua en unos sencillos pasos, como se detalla a continuación.
      
      1. La clase principal de nuestra API es **Watermarker**. Debe crear una instancia antes de procesar el documento. No olvide pasar el archivo Photo al constructor como una ruta o un objeto de secuencia.
      2. El siguiente paso es construir un objeto **Watermark** del tipo deseado. Se puede colocar no sólo en una página de documento específica sino también en partes del documento nativo, como archivos adjuntos o encabezados.
      3. Establezca propiedades de marca de agua como alto y ancho, alineación de la página (arriba, izquierda, central, etc.), familia y color de fuente, y muchas otras.
      4. Llame al método **Watermarker** para agregar una nueva marca de agua. Puede agregar tantas marcas de agua como necesite. Se recomienda guardar el documento procesado en otra ubicación.
   
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

        // Agregar marca de agua de texto a PHOTO

        // Pase el archivo al que se le aplicará la marca de agua a Watermarker
        Watermarker watermarker = new Watermarker("input.png");
        
        // Crear marca de agua de texto y configurar propiedades
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        watermark.setForegroundColor(Color.getRed());

        // Guardar archivo con marca de agua
        watermarker.add(watermark);
        watermarker.save("output.png");
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Mejore sus marcas de agua fácilmente"
  description: "Aproveche el poder de GroupDocs.Watermark para generar, redactar y añadir marcas de agua en varios formatos de documentos. Esta API no solo mejora la seguridad de los documentos, sino que también protege su propiedad intelectual al incorporar marcas de agua personalizables que son versátiles y sólidas."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Añadir marca de agua"
  features:
    # feature loop
    - title: "Opciones versátiles de marcas de agua."
      content: "Explore una amplia gama de opciones de marcas de agua con GroupDocs.Watermark. Desde ajustar la opacidad y la rotación hasta escalar el tamaño proporcionalmente, nuestra API te permite personalizar las marcas de agua con precisión según tus necesidades, garantizando que se combinen perfectamente con tus documentos y, al mismo tiempo, manteniendo la integridad del contenido."

    # feature loop
    - title: "Estilo de marca de agua avanzado."
      content: "GroupDocs.Watermark te permite diseñar tus marcas de agua con diferentes fuentes, colores y sombras, lo que las hace distintivas y más difíciles de eliminar. Mejore el atractivo estético de sus documentos e imágenes protegidos con elegantes marcas de agua que reflejen la identidad y el profesionalismo de su marca."

    # feature loop
    - title: "Posicionamiento y ordenamiento de marcas de agua"
      content: "Con GroupDocs.Watermark, implemente efectos de ordenamiento en teselas para cubrir todo el documento y garantizar una protección completa. Coloque las marcas de agua exactamente donde las necesite: en el centro, en las esquinas o en ubicaciones personalizadas. Nuestras opciones de posicionamiento flexibles ayudan a proteger sus documentos contra el uso no autorizado y la duplicación."
      
  code_samples:
    # code sample loop
    - title: "PDF marca de agua de anotación"
      content: |
        En este ejemplo se muestra cómo añadir una anotación de marca de agua a un documento PDF
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Cargar documento como PDF
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Crear marca de agua basada en la anotación PDF
        PdfAnnotationWatermarkOptions options = new PdfAnnotationWatermarkOptions();
        TextWatermark textWatermark = new TextWatermark("Annotation watermark", new Font("Arial", 8));

        //  Configurar las opciones de marca de agua
        textWatermark.setHorizontalAlignment(HorizontalAlignment.Left);
        textWatermark.setVerticalAlignment(VerticalAlignment.Top);

        //  Añadir marca de agua de texto al documento de resultados
        watermarker.add(textWatermark, options);
        watermarker.save("result.pdf");

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
    title: "Integración rápida de marcas de agua para fotos a través de Java"
    exclude: "PHOTO"
    description: "Aproveche nuestra API Java para aplicar rápidamente marcas de agua a las fotos, lo que mejora la seguridad y la identidad de la marca. Los procesos automatizados permiten una aplicación masiva, lo que garantiza resultados consistentes y profesionales."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/java/add//pdf/"
          description: "Formato de documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/java/add//word/"
          description: "MS Word y documentos de Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/java/add//excel/"
          description: "MS Excel y hojas de cálculo de Open Office"

        # format loop 4
        - name: "Imagen de marca de agua"
          format: "IMAGE"
          link: "/watermark/java/add//image/"
          description: "Formatos de imagen populares"

        # format loop 5
        - name: "Foto con marca de agua"
          format: "PHOTO"
          link: "/watermark/java/add//photo/"
          description: "Formatos de fotos"

        # format loop 6
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/add//powerpoint/"
          description: "MS PowerPoint y presentaciones de Open Office"

        # format loop 7
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/java/add//docx/"
          description: "Documento XML abierto de Microsoft Word"
          
        # format loop 8
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/java/add//pptx/"
          description: "PowerPoint Presentación XML abierta"
          
        # format loop 9
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/java/add//xlsx/"
          description: "Hoja de cálculo XML abierta de Microsoft Excel"

        # format loop 10
        - name: "Filigrana JPEG"
          format: "JPEG"
          link: "/watermark/java/add//jpeg/"
          description: "JPEG Imagen"

        # format loop 11
        - name: "Filigrana PNG"
          format: "PNG"
          link: "/watermark/java/add//png/"
          description: "Portable Gráfico de red"

        # format loop 12
        - name: "Filigrana TIFF"
          format: "TIFF"
          link: "/watermark/java/add//tiff/"
          description: "Formato de archivo de imagen de etiqueta"

        # format loop 13
        - name: "Filigrana WEBP"
          format: "WEBP"
          link: "/watermark/java/add//webp/"
          description: "Imagen WEB"

        # format loop 14
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/java/add//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 15
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/java/add//xls/"
          description: "Libro de trabajo Microsoft Excel 97-2003"

        # format loop 16
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/java/add//ppt/"
          description: "PowerPoint Presentación 97-2003"

        # format loop 17
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/java/add//rtf/"
          description: "Formato de texto enriquecido"

---