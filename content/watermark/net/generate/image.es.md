
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:06
draft: false
lang: es
format: Image
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Añadir marcas de agua a las imágenes con .NET C#"
head_description: "Aprenda a aplicar marcas de agua sin fisuras en las imágenes con .NET C#. Proteja sus activos sin comprometer la calidad."

############################# Header ############################
title: "Marca de agua rápida y personalizada para imágenes con .NET" 
description: "Nuestra herramienta C# .NET proporciona una solución rápida para incrustar marcas de agua en las imágenes. La compatibilidad con formatos de imagen extensos garantiza una cobertura total, desde fotografías hasta obras de arte digitales."
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
       GroupDocs.Watermark for .NET está diseñado para automatizar el proceso de creación de marcas de agua en las imágenes y admite una amplia gama de formatos, como JPEG, PNG, BMP y TIFF. Esta sólida API permite la inserción rápida de marcas de agua de texto e imágenes que se pueden ajustar en opacidad, tamaño y posición, según sus requisitos específicos. Ya sea para proteger los derechos de autor o mejorar el material de marketing, nuestro conjunto de herramientas garantiza que las marcas de agua se apliquen con alta fidelidad y con un impacto mínimo en la calidad de la imagen original.

############################# Steps ############################
steps:
    enable: true
    title: "Mejore sus documentos: genere marcas de agua para Image usando .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** es una biblioteca que simplifica la adición de marcas de agua a varios formatos de archivos comerciales para los desarrolladores de .NET. Integre nuestra biblioteca en su aplicación y agregue marcas de agua a los documentos sin esfuerzo siguiendo estos pasos:
      
      1. **Iniciando su viaje hacia la marca de agua:** Comience familiarizándose con la clase **Watermarker**, la piedra angular de nuestra API. Para comenzar el proceso, asegúrese de crear una instancia antes de procesar el documento. No pase por alto la importancia de proporcionar el archivo Image al constructor, ya sea una ruta o un objeto de secuencia.
      2. **Creación de marcas de agua personalizadas:** Pase a la siguiente fase creando un objeto **Watermark** adaptado a sus especificaciones. Esta herramienta versátil no se limita a páginas de documentos específicas; también se puede integrar perfectamente en elementos nativos del documento, como archivos adjuntos o encabezados.
      3. **Ajuste de los atributos de la marca de agua:** Refine su experiencia con la marca de agua ajustando propiedades como la altura, el ancho, la alineación de la página, la familia de fuentes y el color. Este nivel de personalización garantiza que sus marcas de agua se combinen perfectamente con sus documentos.
      4. **Aplicación de marcas de agua:** Utilice el método **Watermarker** para aplicar sin esfuerzo sus marcas de agua personalizadas a sus documentos. Ya sea que necesite agregar una o varias marcas de agua, este proceso ofrece flexibilidad. Para mayor seguridad, considere guardar sus documentos procesados ​​en una ubicación separada.
   
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
        // Generar marca de agua de texto en el archivo IMAGE

        // Proporcionar un archivo para ponerle una marca de agua
        using (Watermarker watermarker = new Watermarker("input.jpeg"))
        {
            // Generar instancia de marca de agua de texto
            Font font = new Font("Arial", 19, FontStyle.Bold | FontStyle.Italic);
            TextWatermark watermark = new TextWatermark("my watermark", font);
            watermark.ForegroundColor = Color.Red;
            watermark.BackgroundColor = Color.Blue;
            watermarker.Add(watermark);

            // Guardar resultado de IMAGE
            watermarker.Save("output.jpeg");
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
    title: "Implemente marcas de agua rápidamente en todos los formatos de imagen mediante C#"
    exclude: "IMAGE"
    description: "Mejore la protección de sus imágenes con nuestro kit de herramientas C# .NET, capaz de manejar varios formatos de imagen con rapidez y eficiencia. Personalice sus marcas de agua para que se mezclen perfectamente con su contenido visual."
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