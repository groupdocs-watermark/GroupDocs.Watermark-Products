
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:22
draft: false
lang: pt
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Ajustar marcas d'água em DOCX documentos - GroupDocs.Watermark"
head_description: "Edite marcas d'água de forma eficiente em diversos formatos de documentos usando GroupDocs.Watermark. Melhore a autenticidade do documento."

############################# Header ############################
title: "Ajuste DOCX marcas d'água: personalização perfeita" 
description: "Personalize perfeitamente seus documentos com nossa eficiente ferramenta de edição de marcas d'água. Melhore a imagem da sua marca sem esforço."
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
       **Editar marcas d'água**: personalize perfeitamente seus documentos com nossas poderosas ferramentas de edição. Seja ajustando o posicionamento ou alterando o conteúdo, obtenha os efeitos de marca d'água desejados sem esforço.

############################# Steps ############################
steps:
    enable: true
    title: "Ajuste as marcas d'água do documento Docx usando Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** permite que os desenvolvedores do Java ajustem facilmente marcas d'água em muitos documentos usando seus aplicativos. Aqui está um guia rápido:
      
      1. Primeiramente, você precisa passar o arquivo Docx como parâmetro do construtor da classe **Watermarker**. Forneça fluxo de bytes ou arquivos ou um caminho de disco local.
      2. Em segundo lugar, localize as marcas d'água que precisam ser ajustadas. Use **SearchCriteria** para identificar marcas d'água com as propriedades específicas adicionadas anteriormente ao documento.
      3. Após a pesquisa, você receberá uma lista de marcas d'água relevantes. Você pode então ajustar suas propriedades, incluindo tamanho, alinhamento de página, texto, cor, conteúdo da imagem e muito mais. Isso oferece um alto grau de personalização para seus dados.
      4. Depois de terminar de ajustar as marcas d'água, salve o documento atualizado. Você pode usar um caminho de arquivo local ou fluxo para armazenar o resultado.
   
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
        // Ajustar marca d'água da imagem DOCX

        // Instancie Watermarker com DOCX
        Watermarker watermarker = new Watermarker("input.docx");
        
        // Inicialize o SearchCriteria para corresponder a uma imagem específica
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);

        for (PossibleWatermark watermark : watermarks)
        {
            // Substitua a imagem que foi encontrada
            watermark.setImageData(imageData);
        }

        // Salvar arquivo ajustado
        watermarker.save("output.docx");
        
        ```
        
############################# More features ############################
more_features:
  enable: true
  title: "Gerenciamento avançado de marcas d'água DOCX para Java aplicativos"
  description: "A API GroupDocs.Watermark permite que os desenvolvedores integrem perfeitamente a funcionalidade de marca d'água em seus Java aplicativos. Ele suporta adicionar, editar, remover e pesquisar marcas d'água em uma ampla variedade de formatos de documentos."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Ajuste da marca d'água"
  features:
    # feature loop
    - title: "Integração fácil de marcas d'água"
      content: "O GroupDocs.Watermark simplifica o processo de adicionar diversas marcas d'água a vários documentos e arquivos comerciais em Java aplicativos. Os desenvolvedores podem não apenas aplicar marcas d'água, mas também atualizar ou remover as existentes programaticamente."

    # feature loop
    - title: "Personalização granular de marca d'água"
      content: "A API oferece amplas opções de personalização para marcas d'água. Os desenvolvedores podem ajustar facilmente o tamanho, a rotação, a cor, a fonte, os estilos e outras propriedades para obter o efeito visual desejado."

    # feature loop
    - title: "Aproveitando os DOCX recursos de documentos nativos"
      content: "Dependendo do formato do documento de destino, os desenvolvedores podem utilizar funcionalidades nativas para colocar marcas d'água. Essas funcionalidades podem incluir o plano de fundo da página do documento, anotações, cabeçalhos ou outros objetos como contêineres de marca d'água."
      
  code_samples:
    # code sample loop
    - title: "Ajuste a marca d'água da imagem nas planilhas"
      content: |
        Este exemplo mostra como ajustar a imagem das formas específicas em uma planilha Excel.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Carregar documento como planilha
        SpreadsheetLoadOptions loadOptions = new SpreadsheetLoadOptions();
        Watermarker watermarker = new Watermarker("source.xlsx", loadOptions);

        //  Obtenha novos bytes de marca d'água
        File file = new File("new_watermark.png");
        byte[] imageBytes = new byte[(int) file.length()];
        FileInputStream inputStream = new FileInputStream(file);
        inputStream.read(imageBytes);
        inputStream.close();

        //  Ajustar o conteúdo de uma marca d'água específica
        for (SpreadsheetShape shape : content.getWorksheets().get_Item(0).getShapes())
        {
            if (shape.getImage() != null)
            {
                shape.setImage(new SpreadsheetWatermarkableImage(imageBytes));
            }
        }

        //  Salvar documento de resultados
        watermarker.save("result.xlsx");
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
    title: "Modifique marcas d'água em vários formatos usando GroupDocs.Watermark for Java"
    exclude: "DOCX"
    description: "Edite marcas d'água sem problemas em vários formatos de documento. Personalize seus documentos sem esforço e, ao mesmo tempo, garanta proteção e autenticidade."
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