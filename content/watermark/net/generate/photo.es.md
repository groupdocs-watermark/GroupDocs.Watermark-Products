
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:58
draft: false
lang: es
format: Photo
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Añade marcas de agua a tus fotos de forma rápida y sencilla"
head_description: "Proteja y reclame rápidamente los derechos de autor de sus fotos con .NET marcas de agua en C#. Empieza a proteger tu trabajo hoy mismo."

############################# Header ############################
title: "Marcar fotos de forma rápida y sencilla con .NET" 
description: "Nuestra potente biblioteca de C# permite añadir rápidamente marcas de agua a tus fotos, lo que te ayuda a proteger los derechos de autor y a mejorar la identidad de la marca sin comprometer la calidad de la imagen."
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descárguelo gratis en Nuget"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "Obtenga más información"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET ofrece una potente solución para los servicios de fotógrafos que buscan proteger sus derechos de autor y su identidad de marca. Esta API permite añadir rápidamente marcas de agua de texto o gráficos a las fotografías en una variedad de formatos, incluidos JPEG, PNG y RAW. Personalice sus marcas de agua en función de la transparencia, el tamaño y la posición para que se integren perfectamente con la foto, manteniendo la calidad estética, haciendo valer sus derechos legales y evitando el uso no autorizado.

############################# Steps ############################
steps:
    enable: true
    title: "Mejore sus documentos: genere marcas de agua para Photo con .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** es una biblioteca que simplifica la adición de marcas de agua a varios formatos de archivos empresariales para .NET desarrolladores. Integre nuestra biblioteca en su aplicación y añada fácilmente marcas de agua a los documentos siguiendo estos pasos:
      
      1. **Iniciando tu viaje con marcas de agua:** Empieza por familiarizarte con la clase**Watermarker**, la piedra angular de nuestra API. Para comenzar el proceso, asegúrate de crear una instancia antes de procesar el documento. No pases por alto la importancia de proporcionar el archivo Photo al constructor, ya sea una ruta o un objeto de flujo.
      2. **Elaboración de marcas de agua personalizadas:** Pase a la siguiente fase creando un objeto**Watermark** adaptado a sus especificaciones. Esta versátil herramienta no se limita a páginas de documentos específicas; también se puede integrar sin problemas en los elementos nativos del documento, como los archivos adjuntos o los encabezados.
      3. **Ajustar los atributos de las marcas de agua:** Refina tu experiencia con las marcas de agua ajustando propiedades como la altura, el ancho, la alineación de las páginas, la familia de fuentes y el color. Este nivel de personalización garantiza que las marcas de agua se combinen perfectamente con los documentos.
      4. **Aplicación de marcas de agua:** Utilice el método**Watermarker** para aplicar sin esfuerzo sus marcas de agua personalizadas a sus documentos. Ya sea que necesites añadir una o varias marcas de agua, este proceso ofrece flexibilidad. Para mayor seguridad, considera la posibilidad de guardar los documentos procesados en una ubicación diferente.
   
    code:
      platform: "net"
      copy_title: "Copiar"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "haga clic para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Más ejemplos"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "Documentación"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // Generar marca de agua de texto en el archivo PHOTO

        // Proporcione el archivo para ponerle una marca de agua
        using (Watermarker watermarker = new Watermarker("input.png"))
        {
            // Generar instancia de marca de agua de texto
            Font font = new Font("Arial", 19, FontStyle.Bold | FontStyle.Italic);
            TextWatermark watermark = new TextWatermark("my watermark", font);
            watermark.ForegroundColor = Color.Red;
            watermark.BackgroundColor = Color.Blue;
            watermarker.Add(watermark);

            // Guardar PHOTO resultado
            watermarker.Save("output.png");
        }
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Sumérjase en la adición de marcas de agua"
  description: "Aproveche nuestra potente API para renderizar, mostrar, convertir y gestionar documentos, diapositivas, diagramas y otros tipos de documentos en .NET aplicaciones. GroupDocs.Watermark integra a la perfección las funciones de creación de marcas de agua para mejorar la seguridad de los documentos y la protección de los derechos de autor."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Añadir marca de agua"
  features:
    # feature loop
    - title: "Añade marcas de agua a tus documentos sin esfuerzo."
      content: "GroupDocs.Watermark permite a .NET desarrolladores integrar fácilmente marcas de agua en sus aplicaciones. Añada texto, imágenes o marcas de agua dinámicas a los documentos y archivos empresariales más populares sin esfuerzo, garantizando que su contenido sea seguro y tenga una marca uniforme en todas las plataformas."

    # feature loop
    - title: "Personalice las marcas de agua para satisfacer sus necesidades."
      content: "Personalice las marcas de agua para que coincidan con sus requisitos específicos con las amplias funciones compatibles con GroupDocs.Watermark. Ajuste el tamaño, la rotación, la transparencia, el color y la fuente para garantizar que su marca de agua no solo tenga un aspecto perfecto, sino que también mejore la seguridad de los documentos sin obstruir la información importante."

    # feature loop
    - title: "Aproveche las funciones de los documentos nativos para la creación de marcas de agua"
      content: "Utilice las características inherentes de los formatos de documentos para crear marcas de agua sofisticadas. Ya sea que utilice PDF anotaciones nativas, MS Word fondos o Excel encabezados y pies de página, el GroupDocs.Watermark se integra perfectamente con las estructuras de los documentos para aplicar marcas de agua que son eficaces y mínimamente invasivas."
      
  code_samples:
    # code sample loop
    - title: "Generar marca de agua de imagen para DOCX"
      content: |
        En este ejemplo se muestra cómo aplicar efectos de imagen a las marcas de agua de las formas.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Cargar documento Word
            var loadOptions = new WordProcessingLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.docx", loadOptions))
            {
                //  Configurar las opciones de marca de agua
                using (ImageWatermark watermark = new ImageWatermark("logo.png"))
                {
                    WordProcessingImageEffects effects = new WordProcessingImageEffects();
                    effects.Brightness = 0.7;
                    effects.Contrast = 0.6;
                    effects.ChromaKey = Color.Red;
                    effects.BorderLineFormat.Enabled = true;
                    effects.BorderLineFormat.Weight = 1;

                    WordProcessingWatermarkSectionOptions options = new WordProcessingWatermarkSectionOptions();
                    options.Effects = effects;

                    //  Generar marca de agua
                    watermarker.Add(watermark, options);
                }

                //  Guardar documento actualizado
                watermarker.save("result.docx");
            }

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "¿Estás listo para empezar?"
  description: "Pruebe GroupDocs.Watermark funciones de forma gratuita o solicite una licencia"
  items:
    #  loop
    - title: "Nuget descargar"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "Licencias"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Proteja sus fotos con marcas de agua eficaces C#"
    exclude: "PHOTO"
    description: "Proteja y estilice su contenido fotográfico con marcas de agua personalizables mediante nuestra API C# .NET, diseñada para integrarse sin problemas y preservar la calidad de la imagen."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/net/generate//pdf/"
          description: "Formato de documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/net/generate//word/"
          description: "MS Word y documentos de Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/net/generate//excel/"
          description: "MS Excel y hojas de cálculo de Open Office"

        # format loop 4
        - name: "Imagen de marca de agua"
          format: "IMAGE"
          link: "/watermark/net/generate//image/"
          description: "Formatos de imagen populares"

        # format loop 5
        - name: "Foto con marca de agua"
          format: "PHOTO"
          link: "/watermark/net/generate//photo/"
          description: "Formatos de fotos"

        # format loop 6
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/generate//powerpoint/"
          description: "MS PowerPoint y presentaciones de Open Office"

        # format loop 7
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/net/generate//docx/"
          description: "Documento XML abierto de Microsoft Word"
          
        # format loop 8
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/net/generate//pptx/"
          description: "PowerPoint Presentación XML abierta"
          
        # format loop 9
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/net/generate//xlsx/"
          description: "Hoja de cálculo XML abierta de Microsoft Excel"

        # format loop 10
        - name: "Filigrana JPEG"
          format: "JPEG"
          link: "/watermark/net/generate//jpeg/"
          description: "JPEG Imagen"

        # format loop 11
        - name: "Filigrana PNG"
          format: "PNG"
          link: "/watermark/net/generate//png/"
          description: "Portable Gráfico de red"

        # format loop 12
        - name: "Filigrana TIFF"
          format: "TIFF"
          link: "/watermark/net/generate//tiff/"
          description: "Formato de archivo de imagen de etiqueta"

        # format loop 13
        - name: "Filigrana WEBP"
          format: "WEBP"
          link: "/watermark/net/generate//webp/"
          description: "Imagen WEB"

        # format loop 14
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/net/generate//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 15
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/net/generate//xls/"
          description: "Libro de trabajo Microsoft Excel 97-2003"

        # format loop 16
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/net/generate//ppt/"
          description: "PowerPoint Presentación 97-2003"

        # format loop 17
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/net/generate//rtf/"
          description: "Formato de texto enriquecido"

---