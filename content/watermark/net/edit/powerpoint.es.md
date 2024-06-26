
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:19
draft: false
lang: es
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Editar marcas de agua en Powerpoint documentos"
head_description: "Simplifique la edición de Powerpoint marcas de agua y proteja sus documentos con la biblioteca GroupDocs.Watermark for .NET. Logre un control y una versatilidad precisos."

############################# Header ############################
title: "Editar Powerpoint Ubicación de las marcas de agua: .NET Precisión" 
description: "Logre un control preciso sobre la colocación de las marcas de agua y la seguridad de los documentos con la solución GroupDocs.Watermark for .NET. Edite Powerpoint marcas de agua con precisión."
subtitle: "GroupDocs.Watermark for .NET Biblioteca" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar en Nuget"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET API"
    link: "/watermark/net/"
    link_title: "Obtenga más información"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Edite Powerpoint la ubicación de las marcas de agua:** Logre un control preciso sobre la colocación de las marcas de agua y la seguridad de los documentos con GroupDocs.Watermark for .NET desarrolladores. Optimice su flujo de trabajo y garantice la autenticidad sin esfuerzo.

############################# Steps ############################
steps:
    enable: true
    title: "Edite marcas de agua en documentos Powerpoint usando .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** permite a los desarrolladores de .NET editar sin esfuerzo marcas de agua dentro de varios documentos Powerpoint. Aquí hay una guía simplificada sobre cómo usar nuestra API en su aplicación:
      
      1. Comience pasando su archivo Powerpoint como parámetro al constructor de clase **Watermarker**. Puede proporcionar el archivo como una secuencia de bytes, una secuencia de archivos o una ruta de disco local.
      2. A continuación, ubique las marcas de agua específicas que requieren edición. Utilice **SearchCriteria** para identificar marcas de agua con las propiedades correspondientes agregadas previamente al documento.
      3. Después de la búsqueda, obtendrá una lista de marcas de agua relevantes. Luego puedes personalizar sus propiedades, como tamaño, alineación de la página, texto, color, contenido de la imagen y más. Esto le otorga un amplio control sobre sus datos.
      4. Una vez que haya terminado de editar las marcas de agua, guarde el documento actualizado. Puede utilizar una ruta de archivo local o una secuencia para almacenar el resultado final.
   
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
        // Editar marca de agua de texto POWERPOINT

        // Crea Watermarker proporcionando el archivo POWERPOINT
        using (Watermarker watermarker = new Watermarker("input.pptx"))
        {
            // Construya TextSearchCriteria y obtenga marcas de agua de texto
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                 // Editar marca de agua de texto
                 watermark.FormattedTextFragments.Clear();
                 watermark.FormattedTextFragments.Add("passed", 
                    new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
            }

            // guardar el documento
            watermarker.Save("output.pptx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Más información sobre la modificación de marcas de agua"
  description: "Potencie sus .NET aplicaciones con nuestra biblioteca y añada, edite, elimine o busque marcas de agua en varios formatos de archivo."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Editar marca de agua"
  features:
    # feature loop
    - title: "Archivos de marcas de agua para su empresa"
      content: "Usa GroupDocs.Watermark for .NET para marcar archivos y documentos con marcas de agua. Añada y gestione marcas de agua sin ningún esfuerzo adicional al implementar nuestra API en sus aplicaciones. Busca, edita y elimina las marcas de agua añadidas anteriormente."

    # feature loop
    - title: "Ajuste las marcas de agua según sus necesidades"
      content: "Nuestra API ofrece un conjunto completo de opciones de personalización. Modifica sin esfuerzo aspectos como el tamaño, la orientación, la combinación de colores, la familia de fuentes y más para crear la marca de agua ideal."

    # feature loop
    - title: "Aproveche las funciones específicas de los documentos"
      content: "Según el formato de archivo que utilices, puedes incorporar funcionalidades integradas. Estas pueden incluir el fondo del documento, las anotaciones, los encabezados u otros elementos que sirvan como contenedores de marcas de agua."
      
  code_samples:
    # code sample loop
    - title: "Excel edición de texto con marca de agua"
      content: |
        Este ejemplo muestra cómo editar el texto de determinadas marcas de agua en hojas de trabajo Excel
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Cargar hoja de cálculo XLSX
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  Cargar contenido de hojas de cálculo
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();

                //  Editar el texto interior de la marca de agua
                foreach (SpreadsheetShape shape in content.Worksheets[0].Shapes)
                {
                    if (shape.Text == "GroupDocs 2016")
                    {
                        shape.Text = "GroupDocs 2017";
                    }
                }

                //  Guardar el resultado de salida
                watermarker.save("result.xlsx");
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
    title: "Refinar las marcas de agua en otros formatos"
    exclude: "POWERPOINT"
    description: "Edite marcas de agua en varios formatos de documento con GroupDocs.Watermark for .NET."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/net/edit//pdf/"
          description: "Formato de documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/net/edit//word/"
          description: "MS Word y documentos de Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/net/edit//excel/"
          description: "MS Excel y hojas de cálculo de Open Office"

        # format loop 4
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/edit//powerpoint/"
          description: "MS PowerPoint y presentaciones de Open Office"

        # format loop 5
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/net/edit//docx/"
          description: "Documento XML abierto de Microsoft Word"
          
        # format loop 6
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/net/edit//pptx/"
          description: "PowerPoint Presentación XML abierta"
          
        # format loop 7
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/net/edit//xlsx/"
          description: "Hoja de cálculo XML abierta de Microsoft Excel"

        # format loop 8
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/net/edit//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/net/edit//xls/"
          description: "Libro de trabajo Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/net/edit//ppt/"
          description: "PowerPoint Presentación 97-2003"

        # format loop 11
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/net/edit//rtf/"
          description: "Formato de texto enriquecido"

---