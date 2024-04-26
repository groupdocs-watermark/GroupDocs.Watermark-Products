
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:59
draft: false
lang: pt
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Atualizar marcas d'água para Excel planilhas"
head_description: "Atualize marcas d'água em planilhas de vários formatos usando GroupDocs.Watermark for Node.js via Java. Enriqueça seus Node.js via Java aplicativos."

############################# Header ############################
title: "Revolucione a marca d'água de planilhas usando Node.js via Java" 
description: "Experimente o poder de GroupDocs.Watermark for Node.js via Java. Proteja seus documentos comerciais com várias marcas d'água. Atualize o tamanho da marca d'água, alinhamento, ângulo de rotação, posição etc."
subtitle: "GroupDocs.Watermark for Node.js via Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download gratuito de NPM"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "biblioteca GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "Saiba mais"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java é uma solução abrangente para gerenciar marcas d'água usando o ambiente Node.js via Java. Com essa ferramenta, os desenvolvedores podem facilmente realizar operações como adicionar, editar, pesquisar e remover marcas d'água de documentos em vários formatos de arquivo, incluindo PDF, Microsoft Word, Excel, PowerPoint, Visio, e-mail e formatos de imagem. GroupDocs.Watermark suporta todos os principais sistemas operacionais e versões do Node.js.

############################# Steps ############################
steps:
    enable: true
    title: "Atualize marcas d'água em EXCEL via Node.js via Java"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** equipa Node.js via Java desenvolvedores com uma API robusta para atualizar programaticamente marcas d'água em vários documentos EXCEL. Este guia descreve o processo:
      
      1. **Watermarker**. Dependendo de suas demandas, o arquivo pode ser fornecido como um stream ou uma referência a um local de disco local.
      2. **SearchCriteria** para identificar as marcas d'água específicas que precisam ser modificadas. Esse objeto permite a identificação de marcas d'água com base nas propriedades desejadas.
      3. Após a execução bem-sucedida da pesquisa, você receberá uma coleção de marcas d'água relevantes. Essas marcas d'água oferecem controle granular, permitindo que você atualize propriedades como dimensões, posicionamento da página, conteúdo de texto, esquema de cores, dados de imagem e muito mais.
      4. Após a conclusão das atualizações da marca d'água, mantenha o documento modificado. A API facilita o armazenamento usando um caminho de arquivo local ou um objeto de fluxo.
   
    code:
      platform: "net"
      copy_title: "Copiar"
      install:
        command: "npm i @groupdocs/groupdocs.watermark"
        copy_tip: "clique para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Mais exemplos"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
        #  loop
        - title: "Documentação"
          link: "https://docs.groupdocs.com/watermark/nodejs-java/"
          
      content: |
        ```javascript {style=abap}

        // Atualizar marca d'água de texto EXCEL

        // Forneça uma instância Watermarker para o arquivo EXCEL
        const watermarker = new groupdocs.watermark.Watermarker("input.xslx");

        // Use TextSearchCriteria para encontrar marcas d'água de texto
        const searchCriteria = 
            new groupdocs.watermark.TextSearchCriteria("test", false);
        const watermarks = watermarker.search(searchCriteria);
        
        // Atualizar marca d'água de texto
        for (const watermark of watermarks.getInnerList().toArray())
        {
            watermark.setText("passed");
        }

        // Aproveite o resultado
        watermarker.save("output.xslx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Dominando a edição de marca d'água em PDF s com GroupDocs.Watermark"
  description: "Explore recursos abrangentes de API para ajustar e gerenciar marcas d'água em PDF s em Node.js via Java aplicativos."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Editar marca d'água"
  features:
    # feature loop
    - title: "Edite marcas d'água sem esforço em PDF s"
      content: "O GroupDocs.Watermark oferece ferramentas robustas em Node.js via Java para editar perfeitamente marcas d'água existentes em PDF documentos. Ajuste a posição, a transparência e muito mais com facilidade."

    # feature loop
    - title: "Refine os detalhes da marca d'água para obter precisão"
      content: "Assuma o controle sobre os detalhes. Nossa API permite que você ajuste a aparência das marcas d'água, permitindo modificações precisas de tamanho, opacidade e cor em seus PDF s."

    # feature loop
    - title: "Gerenciamento simplificado de marcas d'água"
      content: "Nossa API simplifica o gerenciamento de marcas d'água. Seja atualizando ou removendo, você pode gerenciar marcas d'água com eficiência, mantendo a integridade do documento e atendendo às suas necessidades de marca."
      
  code_samples:
    # code sample loop
    - title: "Java Exemplo: Editar marca d'água PDF"
      content: |
        Este exemplo Java demonstra como editar uma marca d'água existente em um documento PDF, mostrando como ajustar suas propriedades programaticamente.
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Carregue o documento PDF para processamento
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  Pesquise marcas d'água específicas que atendam aos seus critérios
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria("test", false);
            const watermarks = watermarker.search(searchCriteria);
  
            //  Edite as configurações da marca d'água, como tamanho, cor e posição
            for (const watermark of watermarks.getInnerList().toArray()) {
                watermark.getFormattedTextFragments().clear();
                watermark.getFormattedTextFragments().add("passed", 
                    new groupdocsWatermark.Font("Calibri", 19, groupdocsWatermark.FontStyle.Bold), 
                    groupdocsWatermark.Color.getRed(), groupdocsWatermark.Color.getAqua());
            }

            //  Salve o documento atualizado em um sistema local ou transmita-o diretamente
            watermarker.save("result.pdf");
            watermarker.close();

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Pronto para começar?"
  description: "Experimente os GroupDocs.Watermark recursos gratuitamente ou solicite uma licença"
  items:
    #  loop
    - title: "NPM baixar"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licenciamento"
      link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Atualize marcas d'água em todos os formatos de arquivo compatíveis"
    exclude: "EXCEL"
    description: "Atualize com eficiência as marcas d'água em PDF, Word, Excel e muito mais com GroupDocs.Watermark for Node.js via Java. Documentos com marca d'água podem enriquecer seus processos de negócios."
    items: 
        # format loop 1
        - name: "Marca d'água PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/update//pdf/"
          description: "Formato de documento Adobe Portable"

        # format loop 2
        - name: "Marca d'água Word"
          format: "WORD"
          link: "/watermark/nodejs-java/update//word/"
          description: "MS Word e documentos do Open Office"
          
        # format loop 3
        - name: "Marca d'água Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/update//excel/"
          description: "MS Excel e planilhas do Open Office"

        # format loop 4
        - name: "Marca d'água PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/update//powerpoint/"
          description: "MS PowerPoint e apresentações do Open Office"

        # format loop 5
        - name: "Marca d'água DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/update//docx/"
          description: "Documento XML aberto da Microsoft Word"
          
        # format loop 6
        - name: "Marca d'água PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/update//pptx/"
          description: "PowerPoint Apresentação XML aberta"
          
        # format loop 7
        - name: "Marca d'água XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/update//xlsx/"
          description: "Planilha Microsoft Excel Open XML"

        # format loop 8
        - name: "Marca d'água DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/update//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Marca d'água XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/update//xls/"
          description: "Pasta de trabalho Microsoft Excel 97-2003"

        # format loop 10
        - name: "Marca d'água PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/update//ppt/"
          description: "PowerPoint Apresentação 97-2003"

        # format loop 11
        - name: "Marca d'água RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/update//rtf/"
          description: "Formato de texto rico"

---