
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:24
draft: false
lang: pt
format: Xls
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Crie marcas d'água em XLS com C#"
head_description: "Use .NET C# para adicionar e gerenciar marcas d'água em XLS arquivos, aumentando a segurança de seus Excel documentos."

############################# Header ############################
title: "Gere marcas d'água C# para XLS arquivos" 
description: "Implemente marcas d'água robustas em XLS planilhas com .NET C#, personalizadas para proteger dados financeiros e pessoais em Excel."
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixe em Nuget gratuitamente"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "Saiba mais"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       O GroupDocs.Watermark for .NET equipa .NET desenvolvedores de C# com as ferramentas para criar, compor e incorporar marcas d'água em XLS arquivos de forma eficaz. Essa API foi projetada para uma integração perfeita em Excel fluxos de trabalho, facilitando a adição de marcas d'água visíveis e invisíveis que são personalizáveis para opacidade, texto e imagens. Ideal para proteger informações confidenciais em planilhas financeiras, relatórios de clientes ou qualquer documento Excel que exija confidencialidade, o GroupDocs.Watermark oferece recursos avançados, como posicionamento condicional de marca d'água com base na análise de conteúdo. Com suporte para todos os .NET ambientes, essa solução garante que seus documentos sejam protegidos contra uso e distribuição não autorizados.

############################# Steps ############################
steps:
    enable: true
    title: "Gere facilmente marcas d'água para documentos Xls"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/):** Biblioteca avançada de marca d'água para aplicativos .NET. Capacite sua solução e proteja documentos com marcas d'água na hora certa.
      
      1. **Classe principal: Watermarker.** A classe principal de nossa API é **Watermarker**. Você precisa instanciá-lo antes do processamento do documento. Não se esqueça de passar o arquivo Xls para o construtor como um caminho ou objeto de fluxo.
      2. **Elaborando sua marca d'água.** A próxima etapa é construir um objeto Marca d'água do tipo desejado. Ele pode ser colocado não apenas em uma página específica do documento, mas também em partes nativas do documento, como imagens ou cabeçalhos.
      3. **Ajuste fino da aparência.** Defina as propriedades da marca d'água, como altura e largura, alinhamento superior, esquerdo, central, fontes e cores, etc.
      4. **Aplicando e salvando.** Use o método **Watermarker** para adicionar uma nova marca d'água. Sinta-se à vontade para adicionar quantas marcas d'água você precisar. Você pode salvar o documento com marca d'água em qualquer local.
   
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
        // Gerar marca d'água de imagem no arquivo XLS

        // Forneça o caminho do arquivo de origem para o construtor Watermarker
        using (Watermarker watermarker = new Watermarker("input.xls"))
        {
            // Gerar instância de marca d'água de imagem com arquivo de imagem
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // Salvar resultado XLS com marca d'água
            watermarker.Save("output.xls");
        }
        
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "Eleve seu jogo de marca d'água"
  description: "Desbloqueie recursos avançados de marca d'água com nossa API GroupDocs.Watermark para .NET. Essa ferramenta poderosa permite a personalização e a aplicação precisas de marcas d'água em vários tipos de documentos para garantir a máxima segurança e o cumprimento dos direitos autorais com o mínimo de interrupção visual."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Soluções abrangentes de marca d'água"
  features:
    # feature loop
    - title: "Opções sofisticadas de ladrilhos"
      content: "Estenda suas marcas d'água em documentos inteiros sem problemas com nossas opções de ladrilhos. Esse recurso permite que as marcas d'água cubram toda a área do documento, impedindo a remoção e garantindo a proteção completa do documento sem comprometer o design ou a legibilidade."

    # feature loop
    - title: "Personalização de cores vibrantes"
      content: "Adicione um toque de cor às suas marcas d'água! Nossa API permite a personalização de cores de espectro total, permitindo que você aplique marcas d'água que combinam perfeitamente com sua marca corporativa ou estilo de documento. Melhore o apelo visual enquanto mantém recursos de segurança robustos."

    # feature loop
    - title: "Configurações de segurança aprimoradas"
      content: "Leve a segurança dos documentos para o próximo nível com configurações avançadas de marca d'água. Configure marcas d'água de várias camadas, incorporando elementos visíveis e invisíveis, para proteger contra cópias não autorizadas e garantir que somente os destinatários pretendidos possam acessar informações críticas."
      
  code_samples:
    # code sample loop
    - title: "Gere PowerPoint marca d'água"
      content: |
        Este exemplo mostra como adicionar marca d'água às PPTX imagens de fundo
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Carregar apresentação PPTX
            var loadOptions = new PresentationLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pptx", loadOptions))
            {
                //  Configurar propriedades de marca d'água
                TextWatermark watermark = new TextWatermark("Protected image", new Font("Arial", 8));
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermark.RotateAngle = 45;
                watermark.SizingType = SizingType.ScaleToParentDimensions;
                watermark.ScaleFactor = 1;

                //  Fundo de slides com marca d'água
                PresentationContent content = watermarker.GetContent<PresentationContent>();
                foreach (PresentationSlide slide in content.Slides)
                {
                    if (slide.ImageFillFormat.BackgroundImage != null)
                    {
                        slide.ImageFillFormat.BackgroundImage.Add(watermark);
                    }
                }

                //  Salvar apresentação processada
                watermarker.save("result.pptx");
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
    title: "Aplicando marcas d'água a XLS com C#"
    exclude: "XLS"
    description: "Utilize .NET C# para gerar e integrar dinamicamente marcas d'água personalizadas em XLS arquivos, protegendo seus Excel dados de forma eficaz."
    items: 
        # format loop 1
        - name: "Marca d'água PDF"
          format: "PDF"
          link: "/watermark/net/generate//pdf/"
          description: "Formato de documento Adobe Portable"

        # format loop 2
        - name: "Marca d'água Word"
          format: "WORD"
          link: "/watermark/net/generate//word/"
          description: "MS Word e documentos do Open Office"
          
        # format loop 3
        - name: "Marca d'água Excel"
          format: "EXCEL"
          link: "/watermark/net/generate//excel/"
          description: "MS Excel e planilhas do Open Office"

        # format loop 4
        - name: "Imagem de marca d'água"
          format: "IMAGE"
          link: "/watermark/net/generate//image/"
          description: "Formatos de imagem populares"

        # format loop 5
        - name: "Foto com marca d'água"
          format: "PHOTO"
          link: "/watermark/net/generate//photo/"
          description: "Formatos de fotos"

        # format loop 6
        - name: "Marca d'água PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/generate//powerpoint/"
          description: "MS PowerPoint e apresentações do Open Office"

        # format loop 7
        - name: "Marca d'água DOCX"
          format: "DOCX"
          link: "/watermark/net/generate//docx/"
          description: "Documento XML aberto da Microsoft Word"
          
        # format loop 8
        - name: "Marca d'água PPTX"
          format: "PPTX"
          link: "/watermark/net/generate//pptx/"
          description: "PowerPoint Apresentação XML aberta"
          
        # format loop 9
        - name: "Marca d'água XLSX"
          format: "XLSX"
          link: "/watermark/net/generate//xlsx/"
          description: "Planilha Microsoft Excel Open XML"

        # format loop 10
        - name: "Marca d'água JPEG"
          format: "JPEG"
          link: "/watermark/net/generate//jpeg/"
          description: "JPEG Imagem"

        # format loop 11
        - name: "Marca d'água PNG"
          format: "PNG"
          link: "/watermark/net/generate//png/"
          description: "Portable Gráfico de rede"

        # format loop 12
        - name: "Marca d'água TIFF"
          format: "TIFF"
          link: "/watermark/net/generate//tiff/"
          description: "Formato de arquivo de imagem de tag"

        # format loop 13
        - name: "Marca d'água WEBP"
          format: "WEBP"
          link: "/watermark/net/generate//webp/"
          description: "Imagem da WEB"

        # format loop 14
        - name: "Marca d'água DOC"
          format: "DOC"
          link: "/watermark/net/generate//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 15
        - name: "Marca d'água XLS"
          format: "XLS"
          link: "/watermark/net/generate//xls/"
          description: "Pasta de trabalho Microsoft Excel 97-2003"

        # format loop 16
        - name: "Marca d'água PPT"
          format: "PPT"
          link: "/watermark/net/generate//ppt/"
          description: "PowerPoint Apresentação 97-2003"

        # format loop 17
        - name: "Marca d'água RTF"
          format: "RTF"
          link: "/watermark/net/generate//rtf/"
          description: "Formato de texto rico"

---