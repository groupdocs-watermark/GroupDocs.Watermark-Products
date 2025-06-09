
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:16
draft: false
lang: pt
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Editar Marcas d'Água em arquivos Powerpoint"
head_description: "Use GroupDocs.Watermark for Python via .NET para alterar rapidamente o conteúdo da marca d'água em apresentações Powerpoint e manter seus documentos seguros."

############################# Header ############################
title: "Edição Precisa de Marcas d'Água em Powerpoint em Python" 
description: "Tenha controle total sobre o layout e a visibilidade das marcas d'água em suas apresentações usando GroupDocs.Watermark for Python via .NET."
subtitle: "Biblioteca GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download gratuito do PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET API"
    link: "/watermark/python-net/"
    link_title: "Saiba mais"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Controle o Layout da Marca d'Água em Arquivos Powerpoint:** Com GroupDocs.Watermark for Python via .NET, você pode posicionar marcas d'água exatamente onde necessário e proteger suas apresentações facilmente.

############################# Steps ############################
steps:
    enable: true
    title: "Modificar marcas d'água em documentos Powerpoint com Python"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** ajuda desenvolvedores Python a atualizar marcas d'água em diversos arquivos Powerpoint. Veja como usá-lo em seu projeto:
      
      1. Primeiro, abra seu arquivo Powerpoint passando-o para o construtor **Watermarker**. Você pode usar um caminho de arquivo, fluxo de bytes ou fluxo de arquivo.
      2. Em seguida, encontre as marcas d'água que deseja alterar usando **SearchCriteria**, que permite pesquisar texto ou propriedades da marca d'água.
      3. Uma vez encontradas, você pode alterar detalhes como texto, fonte, tamanho, posição, cor e mais. Isso lhe dá controle total sobre a aparência da marca d'água.
      4. Após realizar as alterações, salve o documento. Você pode gravar o resultado em um fluxo ou em um caminho de arquivo.
   
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
        # Atualizar texto da marca d'água em POWERPOINT
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Criar um Watermarker usando um arquivo POWERPOINT
        with gw.Watermarker("input.pptx") as watermarker:

            # Configurar TextSearchCriteria para localizar texto de marca d'água
            search_criteria = gwss.TextSearchCriteria("test", False)

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # Modificar texto da marca d'água
                        watermark.text = "passed"
                    except Exception as e:
                        pass
            
            watermarker.save("output.pptx")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Descubra mais maneiras de atualizar marcas d'água"
  description: "Com nossa biblioteca, aplicativos Python podem adicionar, encontrar, editar ou excluir marcas d'água em muitos tipos de arquivos."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Edição de Marcas d'Água"
  features:
    # feature loop
    - title: "Marque Seus Arquivos com Facilidade"
      content: "Use GroupDocs.Watermark for Python via .NET para adicionar e gerenciar marcas d'água em seus documentos. Pesquise, atualize ou remova marcas d'água conforme necessário usando uma API simples."

    # feature loop
    - title: "Personalize Marcas d'Água para Atender Suas Necessidades"
      content: "Ajuste as configurações da marca d'água, como fonte, tamanho, orientação e cor usando nossa API flexível para obter exatamente o resultado que deseja."

    # feature loop
    - title: "Use Recursos Específicos do Formato"
      content: "Dependendo do formato do arquivo, você pode usar recursos nativos como cabeçalhos, rodapés, anotações ou fundos como áreas de marca d'água."
      
  code_samples:
    # code sample loop
    - title: "Editar Texto de Marca d'Água no Excel"
      content: |
        Este código mostra como alterar o texto da marca d'água em planilhas do Excel.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # Abrir arquivo XLSX
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # Ler dados da planilha
        with gw.Watermarker("source.xlsx") as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,3]

            # Alterar texto da marca d'água
            watermarks = watermarker.search(search_criteria)
            for watermark in watermarks:
                try:
                    watermark.formatted_text_fragments.clear()
                    watermark.formatted_text_fragments.add(
                       "passed", 
                        gww.Font("Calibri", 19.0, gww.FontStyle.bold), 
                        gww.Color.red, 
                        gww.Color.aqua
                    )
                except Exception as e:
                    pass
        
            # Salvar o resultado
            watermarker.save("output.xlsx")
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
    title: "Editar Marcas d'Água em Outros Tipos de Arquivo"
    exclude: "POWERPOINT"
    description: "Use GroupDocs.Watermark for Python via .NET para trabalhar com marcas d'água em diferentes formatos de documentos."
    items: 
        # format loop 1
        - name: "Marca d'água PDF"
          format: "PDF"
          link: "/watermark/python-net/edit//pdf/"
          description: "Formato de documento Adobe Portable"

        # format loop 2
        - name: "Marca d'água Word"
          format: "WORD"
          link: "/watermark/python-net/edit//word/"
          description: "MS Word e documentos do Open Office"
          
        # format loop 3
        - name: "Marca d'água Excel"
          format: "EXCEL"
          link: "/watermark/python-net/edit//excel/"
          description: "MS Excel e planilhas do Open Office"

        # format loop 4
        - name: "Marca d'água PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/edit//powerpoint/"
          description: "MS PowerPoint e apresentações do Open Office"

        # format loop 5
        - name: "Marca d'água DOCX"
          format: "DOCX"
          link: "/watermark/python-net/edit//docx/"
          description: "Documento XML aberto da Microsoft Word"
          
        # format loop 6
        - name: "Marca d'água PPTX"
          format: "PPTX"
          link: "/watermark/python-net/edit//pptx/"
          description: "PowerPoint Apresentação XML aberta"
          
        # format loop 7
        - name: "Marca d'água XLSX"
          format: "XLSX"
          link: "/watermark/python-net/edit//xlsx/"
          description: "Planilha Microsoft Excel Open XML"

        # format loop 8
        - name: "Marca d'água DOC"
          format: "DOC"
          link: "/watermark/python-net/edit//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Marca d'água XLS"
          format: "XLS"
          link: "/watermark/python-net/edit//xls/"
          description: "Pasta de trabalho Microsoft Excel 97-2003"

        # format loop 10
        - name: "Marca d'água PPT"
          format: "PPT"
          link: "/watermark/python-net/edit//ppt/"
          description: "PowerPoint Apresentação 97-2003"

        # format loop 11
        - name: "Marca d'água RTF"
          format: "RTF"
          link: "/watermark/python-net/edit//rtf/"
          description: "Formato de texto rico"

---