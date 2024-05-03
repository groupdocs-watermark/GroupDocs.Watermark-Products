
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:05
draft: false
lang: pt
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Ajustar ferramenta de marca d'água Excel - GroupDocs.Watermark"
head_description: "Ajuste, atualize e gerencie marcas d'água sem esforço com GroupDocs.Watermark. Personalize seus documentos com facilidade."

############################# Header ############################
title: "Ferramenta de ajuste de marcas d'água de planilhas: extremamente simples" 
description: "Melhore seus documentos com nossa ferramenta intuitiva de edição de marcas d'água. Simplifique seu fluxo de trabalho sem esforço."
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
    title: "GroupDocs.Watermark for Java API"
    link: "/watermark/java/"
    link_title: "Saiba mais"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Ferramenta de ajuste de marca d'água**: Nossa ferramenta de marca d'água oferece uma solução fácil de usar para aprimorar e proteger seus documentos. Com recursos de edição intuitivos, o gerenciamento de marcas d'água se torna fácil, garantindo a segurança e a autenticidade dos documentos.

############################# Steps ############################
steps:
    enable: true
    title: "Ajuste marcas d'água em documentos Excel com Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** facilita para os desenvolvedores do Java ajustar marcas d'água de texto em seus aplicativos implementando algumas etapas fáceis:
      
      1. Carregue seu arquivo Excel no objeto principal de nossa API chamado **Watermarker**. Você pode fornecer o arquivo para processamento posterior como fluxo ou como um caminho em um disco local.
      2. O próximo passo é localizar marcas d'água que devem ser ajustadas. **SearchCriteria** ajuda a identificar marcas d'água com propriedades corretas que foram adicionadas anteriormente a um documento.
      3. Obtenha uma lista de marcas d'água adequadas como resultado do procedimento **Search**. Ajuste as propriedades das marcas d’água encontradas, como tamanho, alinhamento da página, texto, cor, conteúdo da imagem, etc.
      4. Após a conclusão do processo de ajuste de marcas d'água, você precisa salvar o documento atualizado. Use o caminho do arquivo local, arquivo ou fluxo de bytes para armazenar o resultado.
   
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

        // Ajustar marca d'água de texto EXCEL

        // Instancie Watermarker com o documento de entrada EXCEL
        Watermarker watermarker = new Watermarker("input.xslx");

        // Inicialize o TextSearchCriteria e encontre marcas d'água de texto
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        
        // Ajustar propriedades de marca d'água de texto
        for (PossibleWatermark watermark : watermarks)
        {
            watermark.getFormattedTextFragments().clear();
            watermark.getFormattedTextFragments().
                add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
        }

        // Salve o documento atualizado
        watermarker.save("output.xslx");
        
        ```            
        
############################# More features ############################
more_features:
  enable: true
  title: "Mergulhe profundamente no ajuste da marca d'água EXCEL"
  description: "Nossa API permite que Java aplicativos adicionem, editem, removam e pesquisem marcas d'água em formatos de documentos populares."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Ajustar marca d'água"
  features:
    # feature loop
    - title: "Marque seus documentos com marca d'água sem esforço"
      content: "GroupDocs.Watermark simplifica a marca d'água para Java desenvolvedores. Adicione marcas d'água diversas a vários documentos e arquivos comerciais. Além de aplicar marcas d'água, você também pode atualizar ou remover as existentes."

    # feature loop
    - title: "Personalize marcas d'água de acordo com suas necessidades"
      content: "Nossa API oferece amplas opções de personalização. Ajuste facilmente tamanho, rotação, cor, fonte, estilos e muito mais para obter a marca d'água perfeita."

    # feature loop
    - title: "Use EXCEL recursos de documentos nativos"
      content: "Dependendo do formato específico do documento, você pode utilizar funcionalidades nativas. Isso pode incluir o plano de fundo da página do documento, anotações, cabeçalhos ou outros objetos como contêineres de marca d'água."
      
  code_samples:
    # code sample loop
    - title: "PDF ajustar marca d'água de texto"
      content: |
        Esse exemplo mostra como ajustar o texto dos artefatos específicos.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Carregar documento PDF
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Obtenha o conteúdo do documento
        PdfContent pdfContent = watermarker.getContent(PdfContent.class);

        //  Ajuste um texto específico da marca d'água
        for (PdfArtifact artifact : pdfContent.getPages().get_Item(0).getArtifacts())
        {
            if (artifact.getText().contains("Test"))
            {
                artifact.setText("Passed");
            }
        }

        //  Salve o documento
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
    title: "Ajuste a marca d'água via GroupDocs.Watermark for Java para outros formatos"
    exclude: "EXCEL"
    description: "Personalize marcas d'água em uma ampla variedade de formatos de documentos com facilidade. Melhore a segurança e a autenticidade dos documentos sem esforço."
    items: 
        # format loop 1
        - name: "Marca d'água PDF"
          format: "PDF"
          link: "/watermark/java/adjust//pdf/"
          description: "Formato de documento Adobe Portable"

        # format loop 2
        - name: "Marca d'água Word"
          format: "WORD"
          link: "/watermark/java/adjust//word/"
          description: "MS Word e documentos do Open Office"
          
        # format loop 3
        - name: "Marca d'água Excel"
          format: "EXCEL"
          link: "/watermark/java/adjust//excel/"
          description: "MS Excel e planilhas do Open Office"

        # format loop 4
        - name: "Marca d'água PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/adjust//powerpoint/"
          description: "MS PowerPoint e apresentações do Open Office"

        # format loop 5
        - name: "Marca d'água DOCX"
          format: "DOCX"
          link: "/watermark/java/adjust//docx/"
          description: "Documento XML aberto da Microsoft Word"
          
        # format loop 6
        - name: "Marca d'água PPTX"
          format: "PPTX"
          link: "/watermark/java/adjust//pptx/"
          description: "PowerPoint Apresentação XML aberta"
          
        # format loop 7
        - name: "Marca d'água XLSX"
          format: "XLSX"
          link: "/watermark/java/adjust//xlsx/"
          description: "Planilha Microsoft Excel Open XML"

        # format loop 8
        - name: "Marca d'água DOC"
          format: "DOC"
          link: "/watermark/java/adjust//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Marca d'água XLS"
          format: "XLS"
          link: "/watermark/java/adjust//xls/"
          description: "Pasta de trabalho Microsoft Excel 97-2003"

        # format loop 10
        - name: "Marca d'água PPT"
          format: "PPT"
          link: "/watermark/java/adjust//ppt/"
          description: "PowerPoint Apresentação 97-2003"

        # format loop 11
        - name: "Marca d'água RTF"
          format: "RTF"
          link: "/watermark/java/adjust//rtf/"
          description: "Formato de texto rico"

---