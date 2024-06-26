---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:49
draft: false

lang: pt
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

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
    # supported_platforms loop
    - title: "Python"
      tag: "python-net"

############################# Head ############################
head_title: "Python Biblioteca de marcas d’água | Marcas d'água de documentos"
head_description: "Python protege documentos comerciais com marcas d'água de texto e imagem. Formatos de arquivo como PDF, Word, Excel e PowerPoint são suportados."

############################# Header ############################
title: "Acesse a tecnologia de marca d'água Python via .NET"
description: "Proteja seus dados e evite cópias não autorizadas com esta solução Python. Adicione facilmente marcas d'água a documentos comerciais em vários formatos, incluindo PDF, Word, Excel, PowerPoint, imagens, etc."
words:
  for: "pelo"

actions:
  main: "Baixe PyPi gratuitamente"
  main_link: "https://pypi.org/project/groupdocs-watermark-net/"
  alt: "Licenciamento"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
  title: "Pronto para começar?"
  description: "Experimente os GroupDocs.Watermark recursos gratuitamente ou solicite uma licença"

release:
  title: "Versão {0} lançada"
  notes: "Veja o que há de novo"
  downloads: "Downloads"
  link: "https://releases.groupdocs.com/watermark/python-net/"

code:
  title: "Adicione marca d'água ao PDF usando Python"
  more: "Mais exemplos"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
  install: "pip install groupdocs-watermark-net"
  content: |
    ```python {style=abap}

    import groupdocs.watermark as gw
    import groupdocs.watermark.watermarks as gww
    import groupdocs.watermark.options.pdf as gwop
    import groupdocs.watermark.common as gwc

    # Instanciar o Watermarker passando pelo caminho PDF
    pdf_lo = gwop.PdfLoadOptions()
    with gw.Watermarker("source.pdf", pdf_lo) as watermarker:
        options = gwop.PdfArtifactWatermarkOptions()

        # Personalize as opções de marca d'água
        text_watermark = 
            gww.TextWatermark("Approved", gww.Font("Arial", 8.0))
        text_watermark.horizontal_alignment = 
            gwc.HorizontalAlignment.RIGHT

        # Aplique marca d'água ao documento PDF
        watermarker.add(text_watermark, options)

        # Salvar documento de resultados
        watermarker.save("result.pdf")

    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark em um piscar de olhos"
  description: "Python Biblioteca para marca d'água"
  features:
    # feature loop
    - title: "Marca d'água de documento Python"
      content: "Proteja seus dados confidenciais com GroupDocs.Watermark for Python via .NET. Coloque texto ou imagens em vários formatos de arquivo como marcas d'água."

    # feature loop
    - title: "Personalizar marcas d'água"
      content: "Muitas opções de personalização estão disponíveis em GroupDocs.Watermark for Python via .NET. Configure estilos de texto (negrito, itálico, fonte) ou propriedades de imagem como tamanho ou rotação para ajustar a marca d'água do documento."

    # feature loop
    - title: "Suporte a formatos de arquivo populares"
      content: "GroupDocs.Watermark for Python via .NET oferece suporte a uma ampla variedade de formatos de arquivo, incluindo PDF, documentos do MS Office como Word, Excel, PowerPoint e imagens como JPEG, PNG, GIF, BMP, diagramas do Visio, e-mails, etc. metas."

    # feature loop
    - title: "Pesquisa e atualização de marca d'água"
      content: "Recupere e atualize marcas d'água colocadas em documentos. Modifique o estilo do texto, o conteúdo da imagem ou remova-os completamente. GroupDocs.Watermark for Python via .NET oferece uma ampla variedade de recursos de processamento de marca d'água."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independência da plataforma"
  description: "GroupDocs.Watermark for Python via .NET integra-se perfeitamente com vários sistemas operacionais e gerenciadores de pacotes."
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
    GroupDocs.Watermark for Python via .NET permite que você processe uma ampla variedade de formatos de arquivo. [Explore a lista completa](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "Recursos do GroupDocs.Watermark for Python via .NET"
  description: "Reforce a segurança dos documentos através de marcas d’água programáticas. Processe diversos formatos de arquivo, incluindo PDF, DOCX, XLSX, PPTX e formatos de imagem (PNG, JPG, etc.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Controle preciso de marca d’água"
      content: "Gerencie marcas d'água com precisão adicionando ou removendo-as de seções específicas, documentos inteiros ou anexos e formas individuais em diferentes formatos de arquivo."

    # feature loop
    - icon: "watermark_style"
      title: "Personalize a aparência da marca d'água"
      content: "Exerça controle refinado sobre a estética da marca d'água, modificando atributos como cor, fonte, opacidade, rotação e posicionamento no documento."

    # feature loop
    - icon: "hidden_print"
      title: "Imprimir marca d'água em PDF"
      content: "Adicione marcas d'água ocultas em documentos regulares que se tornam visíveis apenas durante o processo de impressão, aumentando discretamente a segurança dos documentos."

    # feature loop
    - icon: "image_only"
      title: "Marca d'água de imagem específica"
      content: "Marque imagens específicas em um documento usando nossa solução. Incorpore marcas d'água em uma seção designada (por exemplo, página, slide) ou em todo o documento."

    # feature loop
    - icon: "image_frame"
      title: "Marcas d'água de imagem multicamadas"
      content: "Adicione marcas d'água com precisão a quadros específicos em um formato de imagem com vários quadros, obtendo controle granular sobre o posicionamento da marca d'água."

    # feature loop
    - icon: "attachments"
      title: "Proteção abrangente de conteúdo"
      content: "Estenda a proteção a vários elementos de documentos, como anexos em documentos Excel e formas de imagem em apresentações, fornecendo uma camada adicional de segurança."

    # feature loop
    - icon: "pdf_objects"
      title: "Marca d’água avançada em PDF"
      content: "Coloque marcas d'água em diferentes áreas de PDFs, incluindo Bleed Box, Art Box, Crop Box, Trim Box, etc."

    # feature loop
    - icon: "doc_background"
      title: "Marca d'água da imagem de fundo"
      content: "Gerencie marcas d'água nas imagens de fundo de planilhas e apresentações, oferecendo opções adicionais de personalização para medidas de segurança visual."

    # feature loop
    - icon: "unreadable_characters"
      title: "Marca d'água de texto com caracteres ilegíveis"
      content: "Empregue caracteres ilegíveis em marcas d'água de texto incorporadas em apresentações, reforçando a segurança ao tornar a extração não autorizada de marcas d'água significativamente mais desafiadora."

    # feature loop
    - icon: "watermark_text_search"
      title: "Pesquisa avançada de marca d'água"
      content: "Use recursos de pesquisa abrangentes para localizar marcas d'água em documentos com base em parâmetros específicos ou combinando vários critérios."

    # feature loop
    - icon: "watermark_image_search"
      title: "Detecção de marca d'água de imagem semelhante"
      content: "Encontre imagens de marcas d'água semelhantes em documentos que se pareçam visualmente com uma imagem de origem."

    # feature loop
    - icon: "document_info"
      title: "Analisar informações do documento"
      content: "Extraia dados essenciais de documentos, como configuração de página, para análise posterior."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Amostras de código"
  description: "Explore exemplos de código que mostram funcionalidades comuns do GroupDocs.Watermark for Python via .NET."
  items:
    # code sample loop
    - title: "Marca d'água em um documento com uma imagem"
      content: |
        Use GroupDocs.Watermark for Python via .NET para proteger documentos adicionando marcas d’água de imagem. [Saiba mais](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Como proteger o arquivo pela marca d'água da imagem.">}}
        ```python {style=abap}

        # Carregar documento de origem no Watermarker
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Especifique o caminho para uma imagem de marca d'água
            watermark = groupdocs.watermark.watermarks.ImageWatermark("watermark.jpg")
            watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwgroupdocs.watermark.common.VerticalAlignment.CENTER

            # Proteja o arquivo e salve-o
            watermarker.add(watermark)
            watermarker.save("result.pdf")
       
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Pesquise e modifique marcas d'água existentes"
      content: |
        GroupDocs.Watermark for Python via .NET permite que você gerencie marcas d'água de documentos. Selecione marcas d'água e modifique suas propriedades. [Descubra como](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Pesquisa e modificação de marcas d'água.">}}
        ```python {style=abap}

        # Carregar documento de origem
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Procure marcas d'água a serem atualizadas
            search_criteria = groupdocs.watermark.search.searchcriteria.TextSearchCriteria("annotation", False)
            watermarks = watermarker.search(search_criteria)
            
            # Atualizar as propriedades desejadas
            for watermark in watermarks:
                watermark.text = "passed"

            # Salvar documento modificado em um caminho especificado
            watermarker.save("result.pdf")


        ```
        {{< /landing/code >}}

---
