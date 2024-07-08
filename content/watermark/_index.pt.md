---
############################# Static ############################
layout: "family"
date:  2024-07-08T16:36:26
draft: false

product: "Watermark"
product_tag: "watermark"

lang: pt

############################# Head ############################
head_title: "Marca d'água do documento C# Java Node.js Python | Adicione uma Marca D'água"
head_description: "Adicione marca d'água a PDF, imagens e documentos. Solução de marca d'água para Microsoft Office, PDF, OpenDocument, imagens e etc."

############################# Header ############################
title: "Solução Documents Watermark"
description:  |
  Adicione marcas d'água de texto e imagem aos seus documentos e imagens.

  Pesquise e modifique marcas d'água de documentos de maneira conveniente.

  Obtenha informações sobre marcas d'água que são apresentadas em seus documentos.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Escolha sua plataforma"
  title: "Independência da plataforma"
  description: "A biblioteca GroupDocs.Watermark suporta os seguintes sistemas operacionais e estruturas:"
  details_link_title: "Saiba mais"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Watermark .NET 
      color: "blue"
      tag: "net"
      link: "/watermark/net/"
      features_link: "https://docs.groupdocs.com/watermark/net/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    .NET Framework 4.5 or higher <br> .NET Core 3.0 or higher <br> .NET 5.0 or higher
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Watermark Java
      color: "red"
      tag: "java"
      link: "/watermark/java/"
      features_link: "https://docs.groupdocs.com/watermark/java/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    Java 8 or higher <br> Kotlin
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Watermark Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/watermark/nodejs-java/"
      features_link: "https://docs.groupdocs.com/watermark/"
      features:
          # features loop
          - rows: "4"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Qualquer outro editor de texto
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Python"
      description: GroupDocs.Watermark Python
      color: "yellow"
      tag: "python-net"
      link: "/watermark/python-net/"
      features_link: "https://docs.groupdocs.com/watermark/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Python 3.9+ and .Net 6+
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "4"
            content: |
                    IDLE <br> PyCharm <br> Visual Studio Code
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

############################# Features ###############################
features:
  enable: true
  title: "Análise de características de GroupDocs.Watermark"
  description: "A biblioteca projetada para adicionar, pesquisar e atualizar vários tipos de marcas d'água para formatos de documentos populares."

  items:
    # items loop
    - icon: "protect"
      title: "Proteja arquivos com marcas d'água"
      content: "Adicione marcas d'água de texto e imagem aos seus documentos comerciais."

    # items loop
    - icon: "search"
      title: "Pesquise marcas d'água existentes"
      content: "Obtenha informações detalhadas sobre marcas d'água colocadas anteriormente no documento."

    # items loop
    - icon: "manipulate"
      title: "Manipular marcas d'água de documentos"
      content: "Controle texto, estilo, imagem e outros recursos de marca d'água."

    # items loop
    - icon: "additional"
      title: "Vários recursos adicionais"
      content: "Obtenha informações do documento, atualize hiperlinks ou plano de fundo das páginas, etc."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Proteja documentos com marcas d'água"
  description: "GroupDocs.Watermark exemplos de código de operações típicas."
  items:
    # code sample loop
    - title: "Criando uma marca d'água."
      content: |
       Para acrescentar uma marca d'água a um documento, forneça o caminho para o arquivo de destino. Você tem muitas opções para escolher para obter uma marca d'água personalizada em uma página específica.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Especifique o documento a ser marcado com marca d'água
            using (Watermarker watermarker = new Watermarker("source.docx"))
            {
                // Criar objeto de marca d'água
                TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                // Definir opções de marca d'água
                watermark.ForegroundColor = Color.Red;
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;

                // Adicione marca d'água e salve o arquivo processado
                watermarker.Add(watermark);
                watermarker.Save("result.docx");
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Especifique o documento a ser marcado com marca d'água
            Watermarker watermarker = new Watermarker("source.docx");

            // Criar objeto de marca d'água
            TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

            // Definir opções de marca d'água
            watermark.setForegroundColor(Color.getRed());
            watermark.setHorizontalAlignment(HorizontalAlignment.Center);
            watermark.setVerticalAlignment(VerticalAlignment.Center);

            // Adicione marca d'água e salve o arquivo processado
            watermarker.add(watermark);
            watermarker.save("result.docx");
            watermarker.close();
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            // Especifique o documento a ser marcado com marca d'água
            const watermarker = new Watermarker("source.docx");

            // Criar objeto de marca d'água
            const watermark = new TextWatermark("top secret", new Font("Arial", 36));

            // Definir opções de marca d'água
            watermark.setForegroundColor(Color.getRed());
            watermark.setHorizontalAlignment(HorizontalAlignment.Center);
            watermark.setVerticalAlignment(VerticalAlignment.Center);

            // Adicione marca d'água e salve o arquivo processado
            watermarker.add(watermark);
            watermarker.save("result.docx");
            ```
        - language: "Python"
          color: "yellow"
          content: |
            ```python {style=abap}  
            def run():
                # Especifique o documento a ser marcado com marca d'água
                with groupdocs.watermark.Watermarker("source.docx") as watermarker:
                    font = groupdocs.watermark.watermarks.Font("Arial", 36.0)

                    # Criar objeto de marca d'água
                    watermark = groupdocs.watermark.watermarks.TextWatermark("top secret", font)

                    # Definir opções de marca d'água
                    watermark.foreground_color = groupdocs.watermark.watermarks.Color.red;
                    watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
                    watermark.vertical_alignment = groupdocs.watermark.common.VerticalAlignment.CENTER

                    # Adicione marca d'água e salve o arquivo processado
                    watermarker.add(watermark)
                    watermarker.save("result.docx")
            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "Mais de 50 formatos de arquivo suportados"
  description: "GroupDocs.Watermark fornece marca d'água para formatos populares de documentos e arquivos."

############################# Metrics ###############################
metrics:
  enable: true
  title: "Dados estatísticos da nossa biblioteca"
  description: "Mergulhe profundamente nas principais métricas, revelando insights sobre nossas conquistas, impacto e crescimento."

  items:
    # items loop
    - number: "50+"
      title: "Formatos suportados"
      content: "A Biblioteca é capaz de processar mais de 50 dos formatos de arquivo mais populares."

    # items loop
    - number: "500k"
      title: "NuGet downloads"
      content: "GroupDocs.Watermark para .NET é uma biblioteca popular com mais de 500.000 downloads em NuGet."

    # items loop
    - number: "15k"
      title: "Downloads do Maven"
      content: "Com mais de 15 mil downloads no Maven, GroupDocs.Watermark é uma escolha popular para Java desenvolvedores."

    # items loop
    - number: "140+"
      title: "Clientes satisfeitos"
      content: "Desenvolvedores individuais e grandes empresas em todo o mundo preferem nossas bibliotecas para criar soluções inovadoras."


############################# Customers ###############################
customers:
  enable: true
  title: "Nossos clientes satisfeitos"
  description: "GroupDocs bibliotecas são empregadas por marcas mundialmente renomadas e ilustres em todo o mundo."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Pronto para começar?"
  description: "Experimente os GroupDocs.Watermark recursos gratuitamente em sua plataforma"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/watermark/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/watermark/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/watermark/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "Perguntas frequentes"
  description: "Confira nossas perguntas frequentes"

  items:
    # items loop
    - question: "As bibliotecas externas são exigidas por GroupDocs.Watermark para manipulação de documentos?"
      answer: "O GroupDocs.Watermark funciona de forma independente, sem necessidade de software de terceiros, como o Adobe Acrobat, Microsoft Office, etc."

    # items loop
    - question: "Posso testar GroupDocs.Watermark recursos antes de comprar?"
      answer: "Sim, GroupDocs.Watermark oferece um teste gratuito! Instale e experimente, mas lembre-se: as versões de teste adicionam “crachás de teste” aos seus documentos, somente as 3 primeiras páginas são processadas. Quer a experiência completa? Obtenha uma licença temporária gratuita de 30 dias para obter todas as funcionalidades. Veja os detalhes em [licença temporária](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Quais tipos de licença são fornecidos?"
      answer: "Precisa de uma licença GroupDocs.Watermark? Temos opções! Escolha entre licenças com base em várias opções. Número de desenvolvedores em sua equipe. Locais de implantação, como escritório único ou locais de trabalho remotos. A distribuição ao cliente final precisa compartilhar o SDK/API com os clientes? Como alternativa, há uma licença para uso mensal: pague somente pelo que você usa com planos limitados. Mergulhe mais fundo e encontre o [preço perfeito](https://purchase.groupdocs.com/pricing/watermark/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Watermark APIs de baixo código"
  description: "Adicione marcas d'água aos arquivos pelo seu aplicativo usando nossa API REST baseada em nuvem."
  
  items:
    # items loop
    - title: "GroupDocs.Watermark Cloud for cURL"
      content: "Use a API cURL REST ful para marcar com marca d'água PDF, Word, Excel, PowerPoint, JPEG e outros formatos de arquivo populares."
      icon: "groupdocs_watermark-for-curl"
      link: "https://products.groupdocs.cloud/watermark/curl"

    # items loop
    - title: "GroupDocs.Watermark Cloud for .NET"
      content: "Capacite seus .NET aplicativos com recursos de marcação d'água de documentos do Cloud SDK para .NET. Proteja documentos comerciais por conta própria."
      icon: "groupdocs_watermark-for-net"
      link: "https://products.groupdocs.cloud/watermark/net"

    # items loop
    - title: "GroupDocs.Watermark Cloud for Java"
      content: "O SDK GroupDocs.Watermark projetado para Java concede novas possibilidades para seus Java aplicativos e arquivos de negócios."
      icon: "groupdocs_watermark-for-java"
      link: "https://products.groupdocs.cloud/watermark/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Watermark Aplicativos da Web"
  description: "GroupDocs concede acesso a um aplicativo web para adicionar marcas d'água aos seus documentos. Mais de 50 formatos de arquivo populares podem ser marcados com marca d'água em seu navegador favorito GRATUITAMENTE."

  items:
    # items loop
    - title: "GroupDocs.Watermark Total"
      content: "Ferramenta on-line para adicionar marcas d'água aos documentos a partir de qualquer dispositivo."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/watermark/total"

    # items loop
    - title: "GroupDocs.Watermark DOCX"
      content: "Marca d'água MS Word DOCX on-line."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/watermark/docx"

    # items loop
    - title: "GroupDocs.Watermark PDF"
      content: "Proteja PDF documentos on-line."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/watermark/pdf"


      


---