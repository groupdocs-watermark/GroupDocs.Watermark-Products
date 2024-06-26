
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:23
draft: false
lang: es
format: Xlsx
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Incrustar marcas de agua en XLSX con C#"
head_description: "Aproveche .NET C# para generar y aplicar marcas de agua en XLSX archivos y proteger sus Excel documentos."

############################# Header ############################
title: "Proteja XLSX hojas con .NET C#" 
description: "Usa .NET C# para crear marcas de agua personalizables para XLSX archivos, perfectas para mejorar la integridad de los documentos y proteger la información confidencial."
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
       GroupDocs.Watermark for .NET proporciona una potente solución para que los desarrolladores de .NET C# generen, agreguen y administren marcas de agua en archivos XLSX. Esta API es esencial para mantener la confidencialidad y la autenticidad de los Excel documentos, especialmente en entornos corporativos, financieros y legales. Personalice sus marcas de agua con una variedad de opciones, incluidas las superposiciones de texto e imágenes, diseñadas para ser tanto funcionales como sutiles. Las funciones adicionales permiten crear marcas de agua automatizadas en función de las propiedades del documento y las condiciones definidas por el usuario, lo que garantiza que las marcas de agua se apliquen de forma coherente y solo cuando sea necesario. GroupDocs.Watermark es compatible con las plataformas .NET actuales y admite Excel funcionalidades avanzadas.

############################# Steps ############################
steps:
    enable: true
    title: "Genere marcas de agua sin esfuerzo para documentos Xlsx"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/):** Biblioteca avanzada de marcas de agua para aplicaciones .NET. Potencia tu solución y protege documentos con marcas de agua justo a tiempo.
      
      1. **Clase principal: Watermarker.** La clase principal de nuestra API es **Watermarker**. Debe crear una instancia antes de procesar el documento. No olvide pasar el archivo Xlsx al constructor como una ruta o un objeto de secuencia.
      2. **Elaboración de su marca de agua.** El siguiente paso es construir un objeto de marca de agua del tipo deseado. Se puede colocar no sólo en una página de documento específica sino también en partes del documento nativo, como imágenes o encabezados.
      3. **Ajuste de apariencia.** Establezca propiedades de marca de agua como altura y ancho, alineaciones superior, izquierda, central, fuentes y colores, etc.
      4. **Aplicar y guardar.** Utilice el método **Watermarker** para agregar una nueva marca de agua. Siéntase libre de agregar tantas marcas de agua como necesite. Puede guardar el documento con marca de agua en cualquier ubicación.
   
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
        // Generar marca de agua de imagen en el archivo XLSX

        // Proporcione la ruta del archivo fuente al constructor Watermarker
        using (Watermarker watermarker = new Watermarker("input.xlsx"))
        {
            // Generar instancia de marca de agua de imagen con archivo de imagen
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // Guardar el resultado XLSX con marca de agua
            watermarker.Save("output.xlsx");
        }
        
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "Mejora tu juego de marcas de agua"
  description: "Desbloquee funciones avanzadas de creación de marcas de agua con nuestra API GroupDocs.Watermark para .NET. Esta potente herramienta permite la personalización y la aplicación precisas de las marcas de agua en varios tipos de documentos para garantizar la máxima seguridad y el respeto de los derechos de autor con una interrupción visual mínima."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Soluciones integrales de marcas de agua"
  features:
    # feature loop
    - title: "Opciones sofisticadas de ordenamiento"
      content: "Amplíe sus marcas de agua en documentos enteros sin problemas con nuestras opciones de ordenamiento en teselas. Esta función permite que las marcas de agua cubran toda el área del documento, lo que evita que se eliminen y garantiza una protección completa de los documentos sin comprometer el diseño ni la legibilidad."

    # feature loop
    - title: "Personalización de colores vibrantes"
      content: "¡Añade un toque de color a tus marcas de agua! Nuestra API permite la personalización completa del espectro de colores, lo que le permite aplicar marcas de agua que se adapten perfectamente a su marca corporativa o al estilo de su documento. Mejore el atractivo visual a la vez que mantiene sólidas funciones de seguridad."

    # feature loop
    - title: "Configuración de seguridad mejorada"
      content: "Lleve la seguridad de los documentos al siguiente nivel con la configuración avanzada de marcas de agua. Configure marcas de agua de varias capas, que incorporen elementos visibles e invisibles, para protegerse contra las copias no autorizadas y garantizar que solo los destinatarios previstos puedan acceder a la información crítica."
      
  code_samples:
    # code sample loop
    - title: "Generar marca de agua PowerPoint"
      content: |
        Este ejemplo muestra cómo añadir una marca de agua a las PPTX imágenes de fondo
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Cargar presentación de PPTX
            var loadOptions = new PresentationLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pptx", loadOptions))
            {
                //  Configurar las propiedades de las marcas de agua
                TextWatermark watermark = new TextWatermark("Protected image", new Font("Arial", 8));
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermark.RotateAngle = 45;
                watermark.SizingType = SizingType.ScaleToParentDimensions;
                watermark.ScaleFactor = 1;

                //  Fondo de diapositivas con marca de agua
                PresentationContent content = watermarker.GetContent<PresentationContent>();
                foreach (PresentationSlide slide in content.Slides)
                {
                    if (slide.ImageFillFormat.BackgroundImage != null)
                    {
                        slide.ImageFillFormat.BackgroundImage.Add(watermark);
                    }
                }

                //  Guardar presentación procesada
                watermarker.save("result.pptx");
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
    title: "Implementación de marcas de agua en XLSX con C#"
    exclude: "XLSX"
    description: "Implemente .NET C# para agregar de manera eficiente marcas de agua avanzadas y seguras a XLSX archivos, a fin de proteger sus datos profesionales Excel."
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