
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:26:59
draft: false
lang: pt
format: Photo
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Marque suas fotos com rapidez e facilidade"
head_description: "Proteja e reivindique rapidamente os direitos autorais de suas fotos com .NET marcas d'água C#. Comece a proteger seu trabalho hoje mesmo."

############################# Header ############################
title: "Marcação d'água fotográfica rápida e fácil com .NET" 
description: "Nossa poderosa biblioteca C# permite a criação rápida de marcas d'água em suas fotos, ajudando você a proteger os direitos autorais e aprimorar a identidade da marca sem comprometer a qualidade da imagem."
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
       GroupDocs.Watermark for .NET oferece uma solução poderosa para serviços de fotógrafos que buscam proteger seus direitos autorais e identidade de marca. Essa API permite a adição rápida de marcas d'água gráficas ou de texto às fotos em vários formatos, incluindo JPEG, PNG e RAW. Personalize suas marcas d'água para obter transparência, tamanho e posição para combinar perfeitamente com a foto, mantendo a qualidade estética e, ao mesmo tempo, afirmando seus direitos legais e impedindo o uso não autorizado.

############################# Steps ############################
steps:
    enable: true
    title: "Melhore seus documentos: gere marcas d'água para Photo usando .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** é uma biblioteca que simplifica a adição de marcas d'água a vários formatos de arquivo de negócios para .NET desenvolvedores. Integre nossa biblioteca ao seu aplicativo e marque documentos com marcas d'água sem esforço usando estas etapas a seguir:
      
      1. **Iniciando sua jornada com a marca d'água:** Comece familiarizando-se com a classe **Watermarker**, a base da nossa API. Para iniciar o processo, certifique-se de instanciá-lo antes do processamento do documento. Não negligencie a importância de fornecer o arquivo Photo ao construtor, seja ele um caminho ou um objeto de fluxo.
      2. **Criação de marcas d'água personalizadas:** Vá para a próxima fase criando um objeto **Marca d'água** adaptado às suas especificações. Essa ferramenta versátil não se limita a páginas específicas do documento; ela também pode ser perfeitamente integrada aos elementos nativos do documento, como anexos ou cabeçalhos.
      3. **Ajustando os atributos da marca d'água:** Refine sua experiência com a marca d'água ajustando propriedades como altura, largura, alinhamento da página, família da fonte e cor. Esse nível de personalização garante que suas marcas d'água se misturem perfeitamente aos seus documentos.
      4. **Aplicando suas marcas d'água:** Utilize o método **Marcador d'água** para aplicar facilmente suas marcas d'água personalizadas aos seus documentos. Se você precisar adicionar uma ou várias marcas d'água, esse processo oferece flexibilidade. Para maior segurança, considere salvar seus documentos processados em um local separado.
   
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
        // Gere marca d'água de texto no arquivo PHOTO

        // Forneça o arquivo a ser marcado com marca d'água
        using (Watermarker watermarker = new Watermarker("input.png"))
        {
            // Gerar instância de marca d'água de texto
            Font font = new Font("Arial", 19, FontStyle.Bold | FontStyle.Italic);
            TextWatermark watermark = new TextWatermark("my watermark", font);
            watermark.ForegroundColor = Color.Red;
            watermark.BackgroundColor = Color.Blue;
            watermarker.Add(watermark);

            // Salvar PHOTO resultado
            watermarker.Save("output.png");
        }
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Mergulhe profundamente na adição de marcas d'água"
  description: "Aproveite nossa poderosa API para renderizar, exibir, converter e gerenciar documentos, slides, diagramas e vários outros tipos de documentos em .NET aplicativos. O GroupDocs.Watermark integra perfeitamente os recursos de marca d'água para aprimorar a segurança dos documentos e a proteção de direitos autorais."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Adicionar marca d'água"
  features:
    # feature loop
    - title: "Marque seus documentos com marca d'água sem esforço."
      content: "O GroupDocs.Watermark permite que .NET desenvolvedores integrem facilmente a marca d'água em seus aplicativos. Adicione texto, imagem ou marcas d'água dinâmicas a documentos e arquivos comerciais populares sem esforço, garantindo que seu conteúdo esteja seguro e com a marca registrada de forma consistente em todas as plataformas."

    # feature loop
    - title: "Personalize marcas d'água para atender às suas necessidades."
      content: "Personalize marcas d'água para atender às suas necessidades específicas com recursos abrangentes suportados pelo GroupDocs.Watermark. Ajuste o tamanho, a rotação, a transparência, a cor e a fonte para garantir que sua marca d'água não apenas tenha uma aparência perfeita, mas também aprimore a segurança do documento sem obstruir informações importantes."

    # feature loop
    - title: "Aproveite os recursos nativos de documentos para marcar a água"
      content: "Utilize os recursos inerentes aos formatos de documentos para criar marcas d'água sofisticadas. Seja usando PDF anotações nativas, MS Word planos de fundo ou Excel cabeçalhos e rodapés, o GroupDocs.Watermark se integra profundamente às estruturas do documento para aplicar marcas d'água que são eficazes e minimamente invasivas."
      
  code_samples:
    # code sample loop
    - title: "Gere marca d'água de imagem para DOCX"
      content: |
        Este exemplo mostra como aplicar efeitos de imagem às marcas d'água da forma.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Carregar documento Word
            var loadOptions = new WordProcessingLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.docx", loadOptions))
            {
                //  Configurar opções de marca d'água
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

                    //  Gere marca d'água
                    watermarker.Add(watermark, options);
                }

                //  Salvar documento atualizado
                watermarker.save("result.docx");
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
    title: "Proteja suas fotos com marcas d'água eficazes C#"
    exclude: "PHOTO"
    description: "Proteja e estilize seu conteúdo fotográfico com marcas d'água personalizáveis usando nossa API .NET C#, projetada para se integrar perfeitamente e preservar a qualidade da imagem."
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