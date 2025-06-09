
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: pt
format: Photo
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Marque Suas Fotos Facilmente"
head_description: "Adicione marcas d'água às suas fotos em Python para proteger seu trabalho e copyright."

############################# Header ############################
title: "Marcação Rápida de Fotos com Python" 
description: "Use nossa biblioteca Python para adicionar rapidamente marcas d'água às suas fotos. Proteja seu copyright e marca sem perder qualidade de imagem."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixe PyPi gratuitamente"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "Saiba mais"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET é ideal para fotógrafos que desejam proteger seu trabalho. Adicione marcas d'água de texto ou imagem a fotos em formatos como JPEG, PNG e RAW. Ajuste a transparência, tamanho e posição para que sua marca d'água se encaixe perfeitamente e sua foto ainda fique boa.

############################# Steps ############################
steps:
    enable: true
    title: "Adicione Marcas d'Água: Marcação Python para Photo"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** é uma biblioteca que facilita a adição de marcas d'água a vários tipos de arquivos de negócios. Siga estas etapas para adicionar rapidamente marcas d'água aos seus documentos em Python:
      
      1. **Comece com a Marcação:** Comece criando uma instância da classe **Watermarker**. Passe seu arquivo Photo (como um caminho ou fluxo) para o construtor para abri-lo para marcação.
      2. **Crie sua Marca d'Água:** Crie um objeto **Watermark** com o texto e as configurações desejadas. Você pode adicionar marcas d'água a qualquer página ou até mesmo a elementos do documento, como cabeçalhos ou anexos.
      3. **Personalize a Marca d'Água:** Ajuste o tamanho, posição, fonte, cor e alinhamento da marca d'água para atender às suas necessidades. Isso ajuda sua marca d'água a ficar exatamente certa no documento.
      4. **Aplique e Salve:** Use o método **Watermarker** para adicionar suas marcas d'água ao documento. Salve o resultado, idealmente em um novo arquivo para segurança.
   
    code:
      platform: "python-net"
      copy_title: "Copiar"
      install:
        command: |
        command: "pip install groupdocs-watermark-net"
        copy_tip: "clique para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Mais exemplos"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
        #  loop
        - title: "Documentação"
          link: "https://docs.groupdocs.com/watermark/python-net/"
          
      content: |
        ```python {style=abap}
        # Adicione uma marca d'água de texto a um arquivo PHOTO
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # Selecione o arquivo que deseja marcar com a água
        with gw.Watermarker("input.png") as watermarker:

            # Crie um objeto de marca d'água de texto
            font = gww.Font("Arial", 36.0)
            watermark = gww.TextWatermark("top secret", font)
            watermark.foreground_color = gww.Color.red
            watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
            watermark.opacity = 0.4

            watermarker.add(watermark)

            # Salve o arquivo PHOTO atualizado
            watermarker.save("output.png")
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Explore Mais Recursos de Marcação d'Água"
  description: "Use nossa API Python para adicionar, visualizar, converter e gerenciar marcas d'água em documentos, apresentações, diagramas e mais. GroupDocs.Watermark for Python via .NET ajuda você a proteger seus arquivos e adicionar informações de copyright de forma rápida."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Adicionar Marca d'Água"
  features:
    # feature loop
    - title: "Adicione Marcas d'Água Facilmente"
      content: "GroupDocs.Watermark permite que desenvolvedores Python adicionem rapidamente marcas d'água de texto, imagem ou dinâmicas a documentos empresariais. Mantenha seus arquivos seguros e com marca de forma simples."

    # feature loop
    - title: "Marcas d'Água Totalmente Customizáveis"
      content: "Altere o tamanho, rotação, transparência, cor e fonte da marca d'água com GroupDocs.Watermark. Faça sua marca d'água se encaixar perfeitamente no seu documento e mantenha o conteúdo importante visível."

    # feature loop
    - title: "Use Recursos de Documento para Marcação d'Água"
      content: "Aproveite os recursos nativos do documento, como anotações PDF, fundos do Word ou cabeçalhos do Excel para adicionar marcas d'água. GroupDocs.Watermark trabalha com estruturas de documentos para uma marcação eficaz e não intrusiva."
      
  code_samples:
    # code sample loop
    - title: "Adicione uma Marca d'Água de Imagem ao DOCX"
      content: |
        Este exemplo mostra como aplicar efeitos de imagem a marcas d'água de forma.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.wordprocessing as gwow

        # Abra um documento do Word
        load_options = gwow.WordProcessingLoadOptions()
        with gw.Watermarker("source.docx", load_options) as watermarker:

            # Defina as opções da marca d'água
            with gww.ImageWatermark("logo.png") as watermark:

                effects = gwow.WordProcessingImageEffects()
                effects.brightness = 0.7
                effects.contrast = 0.6
                effects.chroma_key = gww.Color.red

                options = gwow.WordProcessingWatermarkSectionOptions()
                options.Effects = effects;

                # Crie a marca d'água
                watermarker.add(watermark, options)

                # Salve o documento com a marca d'água
                watermarker.save("result.docx")
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Pronto para começar?"
  description: "Experimente os GroupDocs.Watermark recursos gratuitamente ou solicite uma licença"
  items:
    #  loop
    - title: "PyPi baixar"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      color: "red"
        #  loop
    - title: "Licenciamento"
      link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Proteja Suas Fotos com Marcas d'Água em Python"
    exclude: "PHOTO"
    description: "Adicione marcas d'água personalizadas às suas fotos usando nossa API Python. Mantenha suas imagens seguras e com aparência profissional."
    items: 
        # format loop 1
        - name: "Marca d'água PDF"
          format: "PDF"
          link: "/watermark/python-net/add//pdf/"
          description: "Formato de documento Adobe Portable"

        # format loop 2
        - name: "Marca d'água Word"
          format: "WORD"
          link: "/watermark/python-net/add//word/"
          description: "MS Word e documentos do Open Office"
          
        # format loop 3
        - name: "Marca d'água Excel"
          format: "EXCEL"
          link: "/watermark/python-net/add//excel/"
          description: "MS Excel e planilhas do Open Office"

        # format loop 4
        - name: "Imagem de marca d'água"
          format: "IMAGE"
          link: "/watermark/python-net/add//image/"
          description: "Formatos de imagem populares"

        # format loop 5
        - name: "Foto com marca d'água"
          format: "PHOTO"
          link: "/watermark/python-net/add//photo/"
          description: "Formatos de fotos"

        # format loop 6
        - name: "Marca d'água PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/add//powerpoint/"
          description: "MS PowerPoint e apresentações do Open Office"

        # format loop 7
        - name: "Marca d'água DOCX"
          format: "DOCX"
          link: "/watermark/python-net/add//docx/"
          description: "Documento XML aberto da Microsoft Word"
          
        # format loop 8
        - name: "Marca d'água PPTX"
          format: "PPTX"
          link: "/watermark/python-net/add//pptx/"
          description: "PowerPoint Apresentação XML aberta"
          
        # format loop 9
        - name: "Marca d'água XLSX"
          format: "XLSX"
          link: "/watermark/python-net/add//xlsx/"
          description: "Planilha Microsoft Excel Open XML"

        # format loop 10
        - name: "Marca d'água JPEG"
          format: "JPEG"
          link: "/watermark/python-net/add//jpeg/"
          description: "JPEG Imagem"

        # format loop 11
        - name: "Marca d'água PNG"
          format: "PNG"
          link: "/watermark/python-net/add//png/"
          description: "Portable Gráfico de rede"

        # format loop 12
        - name: "Marca d'água TIFF"
          format: "TIFF"
          link: "/watermark/python-net/add//tiff/"
          description: "Formato de arquivo de imagem de tag"

        # format loop 13
        - name: "Marca d'água WEBP"
          format: "WEBP"
          link: "/watermark/python-net/add//webp/"
          description: "Imagem da WEB"

        # format loop 14
        - name: "Marca d'água DOC"
          format: "DOC"
          link: "/watermark/python-net/add//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 15
        - name: "Marca d'água XLS"
          format: "XLS"
          link: "/watermark/python-net/add//xls/"
          description: "Pasta de trabalho Microsoft Excel 97-2003"

        # format loop 16
        - name: "Marca d'água PPT"
          format: "PPT"
          link: "/watermark/python-net/add//ppt/"
          description: "PowerPoint Apresentação 97-2003"

        # format loop 17
        - name: "Marca d'água RTF"
          format: "RTF"
          link: "/watermark/python-net/add//rtf/"
          description: "Formato de texto rico"

---