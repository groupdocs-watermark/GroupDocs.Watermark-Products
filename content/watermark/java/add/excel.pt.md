
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:26
draft: false
lang: pt
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Gere marca d'água em Excel planilhas para Java"
head_description: "Implemente facilmente a geração de marcas d'água de texto e imagem em Excel com Java para proteger suas Excel planilhas de dados"

############################# Header ############################
title: "Automatize a marca d'água Excel com o código Java" 
description: "Implemente marcas d'água personalizadas de texto ou imagem em planilhas Excel usando Java. Este guia oferece instruções detalhadas para aprimorar a segurança e a identidade visual dos documentos, adaptadas para uma variedade de necessidades profissionais."
subtitle: "GroupDocs.Watermark for Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download gratuito de Maven"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "biblioteca GroupDocs.Watermark for Java"
    link: "/watermark/java/"
    link_title: "Saiba mais"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       O GroupDocs.Watermark for Java oferece gerenciamento abrangente de marcas d'água em Excel planilhas, permitindo que os desenvolvedores gerem, ajustem e limpem marcas d'água com facilidade. Ele suporta todos os formatos de arquivo Excel populares, permitindo a incorporação de marcas d'água de texto e imagem que podem ser personalizadas em fonte, cor, tamanho e posição. GroupDocs.Watermark também inclui recursos para pesquisa de marcas d'água, garantindo que suas marcas d'água estejam intactas e invioláveis. Ideal para aplicativos que exigem aprimoramentos na segurança de documentos em ambientes Java.

############################# Steps ############################
steps:
    enable: true
    title: "Adicionar marca d'água ao documento Excel via Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** torna mais fácil para os desenvolvedores do Java adicionar marcas d'água de vários tipos a formatos de arquivos comerciais populares. Adicione nossa biblioteca ao seu aplicativo e marque documentos com marca d'água em algumas etapas fáceis, conforme listado abaixo.
      
      1. A classe principal da nossa API é **Watermarker**. Você precisa instanciá-lo antes do processamento do documento. Não se esqueça de passar o arquivo Excel para o construtor como um caminho ou objeto de fluxo.
      2. A próxima etapa é construir um objeto **Watermark** do tipo desejado. Ele pode ser colocado não apenas em uma página específica do documento, mas também em partes nativas do documento, como anexos ou cabeçalhos.
      3. Defina propriedades da marca d'água, como altura e largura, alinhamento da página (superior, esquerda, central, etc.), família e cor da fonte e muitos outros.
      4. Chame o método **Watermarker** para adicionar uma nova marca d'água. Você pode adicionar quantas marcas d'água precisar. Recomenda-se salvar o documento processado em outro local.
   
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
        copy_tip: "clique para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Mais exemplos"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
        #  loop
        - title: "Documentação"
          link: "https://docs.groupdocs.com/watermark/java/"
          
      content: |
        ```java {style=abap}

        // Adicione marca d'água de texto a EXCEL

        // Passe o arquivo para ter marca d'água para Watermarker
        Watermarker watermarker = new Watermarker("input.xslx");
        
        // Crie marca d'água de texto e configure propriedades
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        watermark.setForegroundColor(Color.getRed());

        // Salvar arquivo com marca d'água
        watermarker.add(watermark);
        watermarker.save("output.xslx");
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Melhore suas marcas d'água facilmente"
  description: "Aproveite o poder do GroupDocs.Watermark para gerar, compor e adicionar marcas d'água em vários formatos de documentos. Essa API não apenas aprimora a segurança dos documentos, mas também protege sua propriedade intelectual ao incorporar marcas d'água personalizáveis que são versáteis e robustas."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Adicionar marca d'água"
  features:
    # feature loop
    - title: "Opções versáteis de marca d'água."
      content: "Explore uma ampla variedade de opções de marca d'água com GroupDocs.Watermark. Desde o ajuste da opacidade e rotação até o dimensionamento proporcional do tamanho, nossa API permite que você personalize as marcas d'água com precisão de acordo com suas necessidades, garantindo que elas se misturem perfeitamente aos seus documentos e, ao mesmo tempo, mantenha a integridade do conteúdo."

    # feature loop
    - title: "Estilo avançado de marca d'água."
      content: "GroupDocs.Watermark permite que você estilize suas marcas d'água com várias fontes, cores e sombras, tornando-as distintas e difíceis de remover. Melhore o apelo estético de seus documentos e imagens protegidos com marcas d'água elegantes que refletem a identidade e o profissionalismo da sua marca."

    # feature loop
    - title: "Posicionamento e ladrilhos com marca d'água"
      content: "Com GroupDocs.Watermark, implemente efeitos de ladrilhos para cobrir todo o documento, garantindo proteção completa. Posicione as marcas d'água exatamente onde você precisa delas: no centro, nos cantos ou em locais personalizados. Nossas opções flexíveis de posicionamento ajudam a proteger seus documentos contra uso e duplicação não autorizados."
      
  code_samples:
    # code sample loop
    - title: "PDF marca d'água de anotação"
      content: |
        Este exemplo mostra como adicionar uma anotação de marca d'água a um documento PDF
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Carregar documento como PDF
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Crie marca d'água com base na anotação PDF
        PdfAnnotationWatermarkOptions options = new PdfAnnotationWatermarkOptions();
        TextWatermark textWatermark = new TextWatermark("Annotation watermark", new Font("Arial", 8));

        //  Configurar opções de marca d'água
        textWatermark.setHorizontalAlignment(HorizontalAlignment.Left);
        textWatermark.setVerticalAlignment(VerticalAlignment.Top);

        //  Adicionar marca d'água de texto ao documento resultante
        watermarker.add(textWatermark, options);
        watermarker.save("result.pdf");

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Pronto para começar?"
  description: "Experimente os GroupDocs.Watermark recursos gratuitamente ou solicite uma licença"
  items:
    #  loop
    - title: "Maven baixar"
      link: "https://releases.groupdocs.com/watermark/java/"
      color: "red"
        #  loop
    - title: "Licenciamento"
      link: "https://purchase.groupdocs.com/pricing/watermark/java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Java Técnicas para Excel Marca-d'água"
    exclude: "EXCEL"
    description: "Usando GroupDocs.Watermark for Java, aplique facilmente marcas d'água baseadas em texto ou imagem em Excel planilhas, aumentando significativamente a segurança dos documentos e a identidade visual como parte do fluxo de trabalho da sua empresa."
    items: 
        # format loop 1
        - name: "Marca d'água PDF"
          format: "PDF"
          link: "/watermark/java/add//pdf/"
          description: "Formato de documento Adobe Portable"

        # format loop 2
        - name: "Marca d'água Word"
          format: "WORD"
          link: "/watermark/java/add//word/"
          description: "MS Word e documentos do Open Office"
          
        # format loop 3
        - name: "Marca d'água Excel"
          format: "EXCEL"
          link: "/watermark/java/add//excel/"
          description: "MS Excel e planilhas do Open Office"

        # format loop 4
        - name: "Imagem de marca d'água"
          format: "IMAGE"
          link: "/watermark/java/add//image/"
          description: "Formatos de imagem populares"

        # format loop 5
        - name: "Foto com marca d'água"
          format: "PHOTO"
          link: "/watermark/java/add//photo/"
          description: "Formatos de fotos"

        # format loop 6
        - name: "Marca d'água PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/add//powerpoint/"
          description: "MS PowerPoint e apresentações do Open Office"

        # format loop 7
        - name: "Marca d'água DOCX"
          format: "DOCX"
          link: "/watermark/java/add//docx/"
          description: "Documento XML aberto da Microsoft Word"
          
        # format loop 8
        - name: "Marca d'água PPTX"
          format: "PPTX"
          link: "/watermark/java/add//pptx/"
          description: "PowerPoint Apresentação XML aberta"
          
        # format loop 9
        - name: "Marca d'água XLSX"
          format: "XLSX"
          link: "/watermark/java/add//xlsx/"
          description: "Planilha Microsoft Excel Open XML"

        # format loop 10
        - name: "Marca d'água JPEG"
          format: "JPEG"
          link: "/watermark/java/add//jpeg/"
          description: "JPEG Imagem"

        # format loop 11
        - name: "Marca d'água PNG"
          format: "PNG"
          link: "/watermark/java/add//png/"
          description: "Portable Gráfico de rede"

        # format loop 12
        - name: "Marca d'água TIFF"
          format: "TIFF"
          link: "/watermark/java/add//tiff/"
          description: "Formato de arquivo de imagem de tag"

        # format loop 13
        - name: "Marca d'água WEBP"
          format: "WEBP"
          link: "/watermark/java/add//webp/"
          description: "Imagem da WEB"

        # format loop 14
        - name: "Marca d'água DOC"
          format: "DOC"
          link: "/watermark/java/add//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 15
        - name: "Marca d'água XLS"
          format: "XLS"
          link: "/watermark/java/add//xls/"
          description: "Pasta de trabalho Microsoft Excel 97-2003"

        # format loop 16
        - name: "Marca d'água PPT"
          format: "PPT"
          link: "/watermark/java/add//ppt/"
          description: "PowerPoint Apresentação 97-2003"

        # format loop 17
        - name: "Marca d'água RTF"
          format: "RTF"
          link: "/watermark/java/add//rtf/"
          description: "Formato de texto rico"

---