
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:06
draft: false
lang: pt
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Edite marcas d'água nos formatos Excel"
head_description: "Personalize e proteja seus documentos sem esforço com GroupDocs.Watermark for .NET. Melhore a integridade do documento e edite Excel marcas d'água com facilidade."

############################# Header ############################
title: "Edite suas Excel planilhas Marcas d'água: .NET Eficiência" 
description: "Aumente a segurança de seus documentos com nossa ferramenta de marca d'água personalizável projetada para eficiência de .NET. Edite Excel marcas d'água sem esforço."
subtitle: "GroupDocs.Watermark for .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download gratuito de Nuget"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "Biblioteca GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "Saiba mais"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Edite Excel marcas d'água com nossa ferramenta:** Nossas GroupDocs.Watermark for .NET ferramentas oferecem estratégias eficientes para aprimorar e proteger seus documentos. Com vários recursos para .NET desenvolvedores, gerenciar marcas d'água se torna muito fácil, garantindo a segurança e a autenticidade dos documentos.

############################# Steps ############################
steps:
    enable: true
    title: "Edite marcas d'água em documentos Excel usando .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** permite que os desenvolvedores do .NET editem facilmente marcas d'água em vários documentos do Excel. Aqui está um guia simplificado de como usar nossa API em sua aplicação:
      
      1. Comece passando seu arquivo Excel como parâmetro para o construtor da classe **Watermarker**. Você pode fornecer o arquivo como um fluxo de bytes, um fluxo de arquivos ou um caminho de disco local.
      2. A seguir, localize as marcas d'água específicas que requerem edição. Utilize o **SearchCriteria** para identificar marcas d'água com as propriedades correspondentes adicionadas anteriormente ao documento.
      3. Após a pesquisa, você obterá uma lista de marcas d'água relevantes. Você pode então personalizar suas propriedades, como tamanho, alinhamento de página, texto, cor, conteúdo da imagem e muito mais. Isso concede a você amplo controle sobre seus dados.
      4. Depois de concluir a edição das marcas d'água, salve o documento atualizado. Você pode utilizar um caminho de arquivo local ou um fluxo para armazenar o resultado final.
   
    code:
      platform: "net"
      copy_title: "Copiar"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "clique para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Mais exemplos"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "Documentação"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // Editar marca d'água de texto EXCEL

        // Faça Watermarker fornecendo o arquivo EXCEL
        using (Watermarker watermarker = new Watermarker("input.xslx"))
        {
            // Construa o TextSearchCriteria e obtenha marcas d'água de texto
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                 // Editar marca d'água de texto
                 watermark.FormattedTextFragments.Clear();
                 watermark.FormattedTextFragments.Add("passed", 
                    new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
            }

            // Salve o documento
            watermarker.Save("output.xslx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Saiba mais sobre a modificação de marcas d'água"
  description: "Capacite seus .NET aplicativos com nossa biblioteca e adicione, edite, remova ou pesquise marcas d'água em vários formatos de arquivo."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Editar marca d'água"
  features:
    # feature loop
    - title: "Arquivos de marca d'água para sua empresa"
      content: "Use GroupDocs.Watermark for .NET para marcar arquivos e documentos com marca d'água. Adicione e gerencie marcas d'água sem esforços extras implementando nossa API em seus aplicativos. Pesquise, edite e remova marcas d'água adicionadas anteriormente."

    # feature loop
    - title: "Ajuste as marcas d'água de acordo com suas necessidades"
      content: "Nossa API oferece um conjunto abrangente de opções de personalização. Modifique facilmente aspectos como tamanho, orientação, esquema de cores, família de fontes e muito mais para criar a marca d'água ideal."

    # feature loop
    - title: "Aproveite os recursos específicos do documento"
      content: "Dependendo do formato de arquivo usado, você pode incorporar funcionalidades integradas. Isso pode incluir o plano de fundo do documento, anotações, cabeçalhos ou outros elementos para servir como contêineres de marca d'água."
      
  code_samples:
    # code sample loop
    - title: "Excel edição de texto com marca d'água"
      content: |
        Este exemplo mostra como editar texto para marcas d'água específicas em Excel Planilhas
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Carregar planilha XLSX
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  Carregar conteúdo da planilha
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();

                //  Editar texto interno da marca d'água
                foreach (SpreadsheetShape shape in content.Worksheets[0].Shapes)
                {
                    if (shape.Text == "GroupDocs 2016")
                    {
                        shape.Text = "GroupDocs 2017";
                    }
                }

                //  Salvar resultado de saída
                watermarker.save("result.xlsx");
            }

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Pronto para começar?"
  description: "Experimente os GroupDocs.Watermark recursos gratuitamente ou solicite uma licença"
  items:
    #  loop
    - title: "Nuget baixar"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "Licenciamento"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Personalize suas marcas d'água em outros formatos"
    exclude: "EXCEL"
    description: "Marque uma variedade de formatos de documentos de acordo com suas necessidades com GroupDocs.Watermark for .NET."
    items: 
        # format loop 1
        - name: "Marca d'água PDF"
          format: "PDF"
          link: "/watermark/net/edit//pdf/"
          description: "Formato de documento Adobe Portable"

        # format loop 2
        - name: "Marca d'água Word"
          format: "WORD"
          link: "/watermark/net/edit//word/"
          description: "MS Word e documentos do Open Office"
          
        # format loop 3
        - name: "Marca d'água Excel"
          format: "EXCEL"
          link: "/watermark/net/edit//excel/"
          description: "MS Excel e planilhas do Open Office"

        # format loop 4
        - name: "Marca d'água PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/edit//powerpoint/"
          description: "MS PowerPoint e apresentações do Open Office"

        # format loop 5
        - name: "Marca d'água DOCX"
          format: "DOCX"
          link: "/watermark/net/edit//docx/"
          description: "Documento XML aberto da Microsoft Word"
          
        # format loop 6
        - name: "Marca d'água PPTX"
          format: "PPTX"
          link: "/watermark/net/edit//pptx/"
          description: "PowerPoint Apresentação XML aberta"
          
        # format loop 7
        - name: "Marca d'água XLSX"
          format: "XLSX"
          link: "/watermark/net/edit//xlsx/"
          description: "Planilha Microsoft Excel Open XML"

        # format loop 8
        - name: "Marca d'água DOC"
          format: "DOC"
          link: "/watermark/net/edit//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Marca d'água XLS"
          format: "XLS"
          link: "/watermark/net/edit//xls/"
          description: "Pasta de trabalho Microsoft Excel 97-2003"

        # format loop 10
        - name: "Marca d'água PPT"
          format: "PPT"
          link: "/watermark/net/edit//ppt/"
          description: "PowerPoint Apresentação 97-2003"

        # format loop 11
        - name: "Marca d'água RTF"
          format: "RTF"
          link: "/watermark/net/edit//rtf/"
          description: "Formato de texto rico"

---