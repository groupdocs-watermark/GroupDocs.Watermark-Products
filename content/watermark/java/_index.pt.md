---
############################# Static ############################
layout: "landing"
date: 2024-05-06T23:13:47
draft: false

lang: pt
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

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
head_title: "Java Biblioteca de marcas d'água | adicionar marcas d'água aos documentos"
head_description: "Software nativo Java para adicionar e manipular marcas d'água de texto e imagem em PDF, Word, Excel, apresentações, Visio diagramas, arquivos de e-mail e imagens."

############################# Header ############################
title: "Implemente marcas d'água de documentos em Java projetos com facilidade"
description: "Melhore seus Java aplicativos com a capacidade de marcar arquivos com marca d'água usando a biblioteca GroupDocs.Watermark. Nossa API oferece marcas d'água personalizáveis para uma ampla variedade de formatos de arquivo populares."
words:
  for: "pelo"

actions:
  main: "Download grátis do Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "Licenciamento"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java/"
  title: "Pronto para começar?"
  description: "Experimente os GroupDocs.Watermark recursos gratuitamente ou solicite uma licença"

release:
  title: "Versão {0} lançada"
  notes: "Veja o que há de novo"
  downloads: "Downloads"

code:
  title: "Marca d'água PDF s via Java"
  more: "Mais exemplos"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-watermark</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Instanciar o Watermarker passando pelo caminho PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Personalize as opções de marca d'água
    TextWatermark textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Aplique marca d'água ao documento PDF
    watermarker.add(textWatermark);

    // Salvar documento de resultados
    watermarker.save("result.pdf");
    watermarker.close();
      
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark em um piscar de olhos"
  description: "Biblioteca projetada para adicionar marcas d'água usando as tecnologias Java"
  features:
    # feature loop
    - title: "Marcar arquivos com marca d'água via Java"
      content: "Proteja seus documentos comerciais usando GroupDocs.Watermark for Java. Adicione texto, imagens, diagramas ou anexos de e-mail como marcas d'água em vários formatos de arquivo."

    # feature loop
    - title: "Personalize marcas d'água para necessidades específicas"
      content: "GroupDocs.Watermark for Java oferece amplas opções de personalização para marcas d'água. Ajuste os estilos de texto (negrito, itálico, fonte) e as propriedades da imagem (rotação etc.) para adaptar o processo de marca d'água às suas metas específicas."

    # feature loop
    - title: "Suporte para formatos amplos"
      content: "O GroupDocs.Watermark for Java se integra perfeitamente a uma ampla variedade de formatos de arquivo, incluindo: PDF, Microsoft Office (Word, Excel, PowerPoint), imagens (JPEG, PNG, GIF, BMP), Visio diagramas e e-mails. Melhore a segurança dos documentos em diversos tipos de arquivos."

    # feature loop
    - title: "Pesquisa e gerenciamento de marcas d'água sem esforço"
      content: "Gerencie com eficiência as marcas d'água existentes nos documentos. Localize marcas d'água específicas, modifique seu texto, estilo ou imagens ou remova-as completamente. GroupDocs.Watermark for Java simplifica o fluxo de trabalho da marca d'água."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independência da plataforma"
  description: "O GroupDocs.Watermark for Java suporta vários sistemas operacionais e gerenciadores de pacotes."
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de arquivo suportados"
  description: |
    GroupDocs.Watermark for Java permite o processamento de uma ampla variedade de formatos de arquivo. [Veja a lista completa](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Java: Características"
  description: "Proteja seus arquivos adicionando marcas d'água. Suporta vários formatos, incluindo PDF, documentos do Office e imagens."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Marcação d'água de arquivos"
      content: "Adicione ou remova marcas d'água de seções específicas ou documentos inteiros para vários formatos de arquivo compatíveis."

    # feature loop
    - icon: "watermark_style"
      title: "Personalização de marca d'água"
      content: "Personalize a aparência da sua marca d'água com opções como cor, fonte, rotação e muito mais."

    # feature loop
    - icon: "hidden_print"
      title: "Marca d'água de impressão oculta para PDF"
      content: "Adicione uma marca d'água que só aparece ao imprimir um documento PDF."

    # feature loop
    - icon: "image_only"
      title: "Marca d'água seletiva de imagens"
      content: "Marque todas as imagens com marca d'água em uma seção, página, slide ou documento inteiro específico."

    # feature loop
    - icon: "image_frame"
      title: "Marcar água em quadros de imagem específicos"
      content: "Aplique marcas d'água em quadros específicos em uma imagem com vários quadros."

    # feature loop
    - icon: "attachments"
      title: "Anexos e formas com marca d'água"
      content: "Adicione marcas d'água em todos os anexos em Excel documentos ou em todas as formas de imagem nas Apresentações."

    # feature loop
    - icon: "pdf_objects"
      title: "Alinhamento de marca d'água em PDF"
      content: "Alinhe marcas d'água em diferentes áreas de um documento PDF, incluindo Bleed Box, Art Box, Crop Box e Trim Box."

    # feature loop
    - icon: "doc_background"
      title: "Marca d'água por imagens de fundo"
      content: "Adicione ou remova a marca d'água da imagem de fundo em planilhas ou apresentações."

    # feature loop
    - icon: "unreadable_characters"
      title: "Proteção com caracteres ilegíveis"
      content: "Proteja apresentações usando marca d'água de texto com caracteres ilegíveis."

    # feature loop
    - icon: "watermark_text_search"
      title: "Pesquisar marcas d'água"
      content: "Obtenha uma lista de marcas d'água apresentadas no arquivo, usando vários parâmetros, incluindo expressões regulares."

    # feature loop
    - icon: "watermark_image_search"
      title: "Encontre marcas d'água de imagens semelhantes"
      content: "Localize marcas d'água de imagem que se pareçam com uma imagem específica."

    # feature loop
    - icon: "document_info"
      title: "Extrair informações do documento"
      content: "Obtenha vários dados de documentos, como configuração de página para formatos de arquivo compatíveis."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Amostras de código"
  description: "Explore exemplos de código que ilustram as funcionalidades típicas de GroupDocs.Watermark for Java"
  items:
    # code sample loop
    - title: "Marcar um documento com marca d'água usando uma imagem"
      content: |
        Utilize GroupDocs.Watermark for Java para aprimorar a segurança do documento adicionando marcas d'água de imagens. Saiba mais: [Marcas d'água da imagem](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Como proteger o arquivo pela marca d'água da imagem.">}}
        ```csharp {style=abap}
        // Carregar documento de origem no Watermarker
        Watermarker watermarker = new Watermarker("document.pdf");
        
        // Especifique o caminho para uma imagem de marca d'água
        ImageWatermark watermark = new ImageWatermark("watermark.jpg");

        // Proteja o arquivo e salve-o
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Modificar marcas d'água"
      content: |
        O GroupDocs.Watermark for Java permite que você gerencie marcas d'água existentes em documentos. Localize marcas d'água específicas e [modifique suas propriedades](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Pesquisa e modificação de marcas d'água.">}}
        ```csharp {style=abap}   
        // Carregar documento de origem
        Watermarker watermarker = new Watermarker("document.pdf");

        // Procure marcas d'água a serem atualizadas
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);                               
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);                             

        // Atualizar as propriedades desejadas
        for (PossibleWatermark watermark : watermarks)                                                           
        {  
            watermark.setText("New Text");
        }

        // Salvar documento modificado em um caminho especificado
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
