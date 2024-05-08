---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:29
draft: false

lang: pt
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Biblioteca de marcas d'água Node.js | marcas d'água de documentos"
head_description: "A solução Node.js protege documentos comerciais com marcas d'água de texto e imagem. Formatos populares como PDF, Word, Excel, PowerPoint são suportados."

############################# Header ############################
title: "Acesso à tecnologia de marca d'água no Node.js por meio de soluções Java"
description: "Proteja sua propriedade intelectual e evite cópias não autorizadas com esta solução Node.js. Ele permite que os usuários adicionem facilmente marcas d'água a documentos comerciais em vários formatos, incluindo PDF, Word, Excel, PowerPoint, imagens etc."
words:
  for: "pelo"

actions:
  main: "Use o NPM para baixar gratuitamente"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.watermark"
  alt: "Licenciamento"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
  title: "Pronto para começar?"
  description: "Experimente os GroupDocs.Watermark recursos gratuitamente ou solicite uma licença"

release:
  title: "Versão {0} lançada"
  notes: "Veja o que há de novo"
  downloads: "Downloads"
  link: "https://releases.groupdocs.com/watermark/nodejs-java/"

code:
  title: "Adicione marca d'água a PDF com TypeScript"
  more: "Mais exemplos"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.watermarker"
  content: |
    ```javascript {style=abap}

    // Instanciar o Watermarker passando pelo caminho PDF
    let loadOptions = new PdfLoadOptions();
    let watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Personalize as opções de marca d'água
    let textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Aplique marca d'água ao documento PDF
    watermarker.add(textWatermark);

    // Salvar documento de resultados
    watermarker.save("result.pdf");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark em um piscar de olhos"
  description: "Biblioteca Node.js TypeScript para marca d'água"
  features:
    # feature loop
    - title: "Marca d'água do arquivo Node.js"
      content: "Proteja seus documentos comerciais com GroupDocs.Watermark for Node.js via Java. Adicione texto, imagens, diagramas ou anexos de e-mail como marcas d'água em vários formatos de arquivo."

    # feature loop
    - title: "Personalize marcas d'água de acordo com suas necessidades"
      content: "GroupDocs.Watermark for Node.js via Java oferece amplas opções de personalização para marcas d'água. Estilos de texto ajustados (negrito, itálico, fonte) e propriedades de imagem (rotação, etc.) permitem personalizar o processamento de documentos."

    # feature loop
    - title: "Suporte abrangente de formatos"
      content: "O GroupDocs.Watermark for Node.js via Java se integra perfeitamente a uma ampla variedade de formatos de arquivo, incluindo: PDF, MS Office, como Word, Excel, PowerPoint, imagens como JPEG, PNG, GIF, BMP, Visio diagramas, e-mails etc. Capacite o processamento de documentos para atingir as metas de negócios."

    # feature loop
    - title: "Pesquisa e atualização poderosas de marcas d'água"
      content: "Obtenha e atualize marcas d'água existentes em documentos com marca d'água. Modifique o texto, o estilo, o conteúdo da imagem ou remova-os completamente. GroupDocs.Watermark for Node.js via Java fornece uma ampla variedade de processamento de marcas d'água."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independência da plataforma"
  description: "O GroupDocs.Watermark for Node.js via Java se integra facilmente a vários sistemas operacionais e gerenciadores de pacotes."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de arquivo suportados"
  description: |
    O GroupDocs.Watermark for Node.js via Java permite que você processe uma grande variedade de formatos de arquivo. [Explore a lista completa](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Node.js via Java: Conjunto de recursos"
  description: "Fortaleça a segurança robusta de documentos por meio de marcas d'água programáticas. Suporta diversos formatos de arquivo, incluindo: PDF, DOCX, XLSX, PPTX e formatos de imagem (PNG, JPG, etc.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Controle preciso de marca d'água"
      content: "Manipule marcas d'água com precisão adicionando ou removendo-as de seções específicas, documentos inteiros ou anexos e formas individuais em diferentes formatos de arquivo."

    # feature loop
    - icon: "watermark_style"
      title: "Personalização da aparência da marca d'água"
      content: "Exerça um controle refinado sobre a estética da marca d'água modificando atributos como cor, fonte, opacidade, rotação e posicionamento no documento."

    # feature loop
    - icon: "hidden_print"
      title: "Imprimir PDF Marca d'água"
      content: "Implante uma marca d'água furtiva que permaneça invisível durante a visualização normal do documento, mas se torne aparente somente durante o processo de impressão, aprimorando discretamente a segurança do documento."

    # feature loop
    - icon: "image_only"
      title: "Marca d'água de imagem específica"
      content: "Marque imagens específicas em um documento usando nossa solução. Escolha incorporar marcas d'água em uma seção designada (por exemplo, página, slide) ou em todo o documento."

    # feature loop
    - icon: "image_frame"
      title: "Marcas d'água de imagens com vários quadros"
      content: "Aplique marcas d'água seletivamente em quadros específicos em um formato de imagem com vários quadros, garantindo controle granular sobre o posicionamento da marca d'água."

    # feature loop
    - icon: "attachments"
      title: "Proteção abrangente de conteúdo"
      content: "Estenda a proteção a vários elementos do documento, como anexos em Excel documentos e formas de imagem em apresentações, fornecendo uma camada adicional de segurança."

    # feature loop
    - icon: "pdf_objects"
      title: "Marca d'água avançada em PDF"
      content: "Marque com marca d'água diferentes áreas de PDF s, incluindo Bleed Box, Art Box, Crop Box, Trim Box etc."

    # feature loop
    - icon: "doc_background"
      title: "Marca d'água de imagem de fundo"
      content: "Gerencie marcas d'água nas imagens de fundo de planilhas e apresentações, oferecendo opções adicionais de personalização para medidas de segurança visual."

    # feature loop
    - icon: "unreadable_characters"
      title: "Marca d'água de texto com caracteres ilegíveis"
      content: "Use caracteres ilegíveis em marcas d'água de texto incorporadas às apresentações, reforçando a segurança ao tornar a extração não autorizada de marcas d'água significativamente mais desafiadora."

    # feature loop
    - icon: "watermark_text_search"
      title: "Pesquisa avançada de marca d'água"
      content: "Utilize recursos de pesquisa abrangentes para localizar marcas d'água em documentos com base em parâmetros específicos ou combinando vários critérios, permitindo recuperação e gerenciamento eficientes."

    # feature loop
    - icon: "watermark_image_search"
      title: "Detecção de marca d'água de imagem semelhante"
      content: "Encontre imagens de marca d'água semelhantes em documentos que se assemelham visualmente a uma imagem de origem."

    # feature loop
    - icon: "document_info"
      title: "Extração programática de informações de documentos"
      content: "Extraia metadados valiosos de forma programática, incluindo detalhes de configuração da página e outras informações do documento para formatos de arquivo compatíveis."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Amostras de código"
  description: "Mergulhe em exemplos de código que mostram as funcionalidades comuns de GroupDocs.Watermark for Node.js via Java"
  items:
    # code sample loop
    - title: "Marcar um documento com uma imagem"
      content: |
        Aproveite GroupDocs.Watermark for Node.js via Java para aprimorar a segurança do documento adicionando marcas d'água de imagem. Saiba mais: [Marcas d'água da imagem](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Como proteger o arquivo pela marca d'água da imagem.">}}
        ```javascript {style=abap}
        // Carregar documento de origem no Watermarker
        let watermarker = new Watermarker("document.pdf");
        
        // Especifique o caminho para uma imagem de marca d'água
        let watermark = new ImageWatermark("watermark.jpg");

        // Proteja o arquivo e salve-o
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Pesquisar e modificar marcas d'água existentes"
      content: |
        O GroupDocs.Watermark for Node.js via Java permite que você gerencie marcas d'água de documentos. Selecione marcas d'água, modifique suas propriedades. Descubra como: [Modificar marcas d'água](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Pesquisa e modificação de marcas d'água.">}}
        ```javascript {style=abap}   
        // Carregar documento de origem
        let watermarker = new Watermarker("document.pdf");

        // Procure marcas d'água a serem atualizadas
        let searchCriteria = new TextSearchCriteria("test", false);                               
        let watermarks = watermarker.search(searchCriteria); 

        // Atualizar as propriedades desejadas
        watermarks.forEach((watermark)
        {  
            watermark.setText("New Text");
        }

        // Salvar documento modificado em um caminho especificado
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
