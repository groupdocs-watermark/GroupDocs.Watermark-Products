---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:29
draft: false

lang: pt
product: "Watermark"
product_tag: "watermark"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Software de marca d'água de documentos C# .NET | adicionar marca d'água"
head_description: "Biblioteca C# .NET para adicionar, pesquisar e remover marcas d'água em documentos: PDF, Word, Excel, apresentações, Visio diagramas, formatos de arquivo de e-mail e imagem."

############################# Header ############################
title: "Marque documentos com facilidade em seus aplicativos C# .NET"
description: "Fortaleça suas soluções de C# com uma API flexível de marca d'água de documentos que fornece a adição de marcas d'água personalizáveis a todos os formatos de documentos populares."
words:
  for: "pelo"

actions:
  main: "Download grátis de NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Watermark"
  alt: "Licenciamento"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/net/"
  title: "Pronto para começar?"
  description: "Experimente os GroupDocs.Watermark recursos gratuitamente ou solicite uma licença"

release:
  title: "Versão {0} lançada"
  notes: "Veja o que há de novo"
  downloads: "Downloads"

code:
  title: "Marcar com marca d'água os arquivos PDF em C#"
  more: "Mais exemplos"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
  install: "dotnet add package GroupDocs.Watermark"
  content: |
    ```csharp {style=abap}   
    // Instanciar o Watermarker passando pelo caminho PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    using (Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions))
    {
        // Personalize as opções de marca d'água
        TextWatermark textWatermark = 
            new TextWatermark("Approved", new Font("Arial", 8));
        
        // Aplique marca d'água ao documento PDF
        watermarker.Add(textWatermark);

        // Salvar documento de resultados
        watermarker.Save("result.pdf");
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark em um piscar de olhos"
  description: "API para colocar marcas d'água em documentos via .NET"
  features:
    # feature loop
    - title: "Marca d'água de arquivos C#"
      content: "Adicione marcas d'água aos seus arquivos comerciais usando GroupDocs.Watermark. Use texto, imagens, diagramas ou anexos de e-mail."

    # feature loop
    - title: "Personalize marcas d'água de acordo com suas metas"
      content: "O software GroupDocs.Watermark for .NET permite personalizar marcas d'água de várias maneiras. Estilos de texto como negrito, itálico, tipos de fonte, juntamente com propriedades de imagem, como rotação, etc. enriquecem o processo de marca d'água."

    # feature loop
    - title: "Todos os formatos de arquivo populares são suportados"
      content: "Muitos formatos de arquivo e documento são suportados pela solução GroupDocs.Watermark. PDF, Microsoft Office Word, Excel, PowerPoint, imagens como JPEG, PNG, GIF, BMP, Visio diagramas, e-mails etc. podem ser protegidas com nossas marcas d'água."

    # feature loop
    - title: "Pesquise e atualize marcas d'água"
      content: "As marcas d'água que já estão apresentadas em um documento podem ser encontradas e processadas novamente. Modifique texto, estilo, imagens ou remova marcas d'água reveladas sem esforços extras."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independência da plataforma"
  description: "GroupDocs.Watermark for .NET suporta sistemas operacionais, estruturas e gerenciadores de pacotes listados abaixo"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de arquivo suportados"
  description: |
    GroupDocs.Watermark for .NET fornece o processamento dos seguintes [formatos de arquivo](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### formatos Microsoft Office e OpenDocument
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### Imagens e gráficos
        * **Formatos de imagem populares:** BMP, JPG, JPEG, PNG
        * **Imagens de várias páginas:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### Outros
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark características"
  description: "Proteja PDF, Office, imagens e outros formatos com marca d'água"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Marcação d'água de documentos"
      content: "Adicione ou remova marcas d'água de uma seção específica ou de um documento inteiro de vários formatos de arquivo."

    # feature loop
    - icon: "watermark_style"
      title: "Estilize sua marca d'água"
      content: "Personalize várias propriedades de marca d'água, como cor, fonte, rotação etc."

    # feature loop
    - icon: "hidden_print"
      title: "PDF marca d'água de impressão oculta"
      content: "Aloque a marca d'água oculta para PDF que só aparece ao imprimir o documento."

    # feature loop
    - icon: "image_only"
      title: "Marcar somente imagens com marca d'água em documentos"
      content: "Marque todas as imagens em uma seção, página, slide ou documento específico."

    # feature loop
    - icon: "image_frame"
      title: "Processar quadros de imagem selecionados"
      content: "Atribua marca d'água somente a quadros específicos de uma imagem com vários quadros."

    # feature loop
    - icon: "attachments"
      title: "Anexos e formas"
      content: "Defina marca d'água em todos os anexos em um documento Excel e em todas as formas de imagem nos slides."

    # feature loop
    - icon: "pdf_objects"
      title: "PDF objetos"
      content: "Alinhe a marca d'água à caixa de sangria, caixa de arte, caixa de corte ou caixa de corte no documento PDF."

    # feature loop
    - icon: "doc_background"
      title: "Plano de fundo de documentos"
      content: "Coloque uma marca d'água ou remova-a das imagens de fundo da planilha ou dos slides."

    # feature loop
    - icon: "unreadable_characters"
      title: "Proteção de caracteres ilegíveis"
      content: "Proteja a marca d'água de texto usando caracteres ilegíveis em apresentações."

    # feature loop
    - icon: "watermark_text_search"
      title: "Pesquisar marcas d'água em documentos"
      content: "Pesquise marcas d'água com base em parâmetros específicos ou combinando vários critérios."

    # feature loop
    - icon: "watermark_image_search"
      title: "Pesquisar marcas d'água de imagens semelhantes"
      content: "Procure marcas d'água de imagem que se assemelhem a uma imagem específica."

    # feature loop
    - icon: "document_info"
      title: "Obtenha informações do documento"
      content: "Extraia programaticamente a configuração da página e outras informações para os formatos suportados."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Amostras de código"
  description: "Alguns casos de uso de operações GroupDocs.Watermark for .NET típicas"
  items:
    # code sample loop
    - title: "Marque água adicionando uma imagem a um documento."
      content: |
        Para proteger qualquer documento, você pode usar [marcas d'água de imagem](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/):
        {{< landing/code title="Como proteger o arquivo pela marca d'água da imagem.">}}
        ```csharp {style=abap}
        // Carregar documento de origem no Watermarker
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Especifique o caminho para uma imagem de marca d'água
            using (ImageWatermark watermark = new ImageWatermark("watermark.jpg"))
            {
                // Proteja o arquivo e salve-o
                watermarker.Add(watermark);

                watermarker.Save("result.pdf");
            }
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Pesquise e modifique marcas d'água existentes."
      content: |
        GroupDocs.Watermark é capaz de [modificar marcas d'água](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/) que já estão apresentadas em um documento. Pesquise os itens desejados e atualize suas propriedades.
        {{< landing/code title="Pesquisa e modificação de marcas d'água.">}}
        ```csharp {style=abap}   
        // Carregar documento de origem
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Procure marcas d'água a serem atualizadas
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                // Atualizar as propriedades desejadas
                watermark.Text = "New Text";
            }

            // Salvar documento modificado em um caminho especificado
            watermarker.Save("document.pdf");
        }
        ```
        {{< /landing/code >}}

---
