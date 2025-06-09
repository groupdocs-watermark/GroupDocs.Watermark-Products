
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: fr
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Modifier les filigranes dans les fichiers Excel"
head_description: "Avec GroupDocs.Watermark for Python via .NET, vous pouvez ajuster les paramètres des filigranes pour protéger et personnaliser vos documents."

############################# Header ############################
title: "Mettre à jour les filigranes dans les feuilles de calcul Excel avec Python" 
description: "Sécurisez vos feuilles de calcul Excel avec nos outils flexibles d'édition de filigranes pour Python."
subtitle: "API GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Obtenez-le gratuitement sur PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET Library"
    link: "/watermark/python-net/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Modifiez rapidement les filigranes Excel :** GroupDocs.Watermark for Python via .NET donne aux développeurs Python tous les outils nécessaires pour gérer les filigranes avec un minimum d'effort, améliorant votre flux de travail et la sécurité de vos documents.

############################# Steps ############################
steps:
    enable: true
    title: "Modifier les filigranes dans les documents Excel avec Python"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** aide les développeurs Python à actualiser les filigranes dans divers fichiers Excel. Voici comment vous pouvez l'utiliser dans votre projet :
      
      1. Tout d'abord, ouvrez votre fichier Excel en le passant au constructeur **Watermarker**. Vous pouvez utiliser un chemin de fichier, un flux d'octets ou un flux de fichiers.
      2. Ensuite, trouvez les filigranes que vous souhaitez modifier à l'aide de **SearchCriteria**, qui vous permet de rechercher du texte ou des propriétés de filigrane.
      3. Une fois trouvés, vous pouvez changer des détails comme le texte, la police, la taille, la position, la couleur, et plus encore. Cela vous donne un contrôle total sur l'apparence du filigrane.
      4. Après avoir effectué les modifications, enregistrez le document. Vous pouvez écrire le résultat dans un flux ou à un chemin de fichier.
   
    code:
      platform: "python-net"
      copy_title: "Copier"
      install:
        command: |
        command: "pip install groupdocs-watermark-net"
        copy_tip: "cliquez pour copier"
        copy_done: "copié"
      links:
        #  loop
        - title: "Plus d'exemples"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/watermark/python-net/"
          
      content: |
        ```python {style=abap}
        # Mettre à jour le texte du filigrane dans EXCEL
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Créer un Watermarker à l'aide d'un fichier EXCEL
        with gw.Watermarker("input.xslx") as watermarker:

            # Configurer TextSearchCriteria pour trouver le texte du filigrane
            search_criteria = gwss.TextSearchCriteria("test", False)

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # Modifier le texte du filigrane
                        watermark.text = "passed"
                    except Exception as e:
                        pass
            
            watermarker.save("output.xslx")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Découvrez d'autres façons de mettre à jour les filigranes"
  description: "Avec notre bibliothèque, les applications Python peuvent ajouter, trouver, modifier ou supprimer des filigranes dans de nombreux types de fichiers."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Édition de filigrane"
  features:
    # feature loop
    - title: "Filigrate vos fichiers sans difficulté"
      content: "Utilisez GroupDocs.Watermark for Python via .NET pour ajouter et gérer des filigranes dans vos documents. Recherchez, mettez à jour ou supprimez des filigranes selon vos besoins grâce à une API simple."

    # feature loop
    - title: "Personnalisez les filigranes selon vos besoins"
      content: "Ajustez les paramètres des filigranes tels que la police, la taille, l'orientation et la couleur à l'aide de notre API flexible pour obtenir exactement le résultat souhaité."

    # feature loop
    - title: "Utilisez les fonctionnalités spécifiques aux formats"
      content: "En fonction du format de fichier, vous pouvez utiliser des fonctionnalités natives telles que des en-têtes, des pieds de page, des annotations ou des zones d'arrière-plan comme zones de filigrane."
      
  code_samples:
    # code sample loop
    - title: "Modifier le texte du filigrane dans Excel"
      content: |
        Ce code montre comment changer le texte du filigrane dans les feuilles de calcul Excel.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # Ouvrir le fichier XLSX
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # Lire les données de la feuille de calcul
        with gw.Watermarker("source.xlsx") as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,3]

            # Changer le texte du filigrane
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
        
            # Enregistrer le résultat
            watermarker.save("output.xlsx")
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Prêt à démarrer ?"
  description: "Essayez GroupDocs.Watermark fonctionnalités gratuitement ou demandez une licence"
  items:
    #  loop
    - title: "PyPi télécharger"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      color: "red"
        #  loop
    - title: "Licences"
      link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Mettre à jour les filigranes dans d'autres formats"
    exclude: "EXCEL"
    description: "Personnalisez facilement les paramètres des filigranes dans différents formats de fichiers à l'aide de GroupDocs.Watermark for Python via .NET."
    items: 
        # format loop 1
        - name: "Filigrane PDF"
          format: "PDF"
          link: "/watermark/python-net/edit//pdf/"
          description: "Format de document Adobe Portable"

        # format loop 2
        - name: "Filigrane Word"
          format: "WORD"
          link: "/watermark/python-net/edit//word/"
          description: "MS Word et documents Open Office"
          
        # format loop 3
        - name: "Filigrane Excel"
          format: "EXCEL"
          link: "/watermark/python-net/edit//excel/"
          description: "MS Excel et feuilles de calcul Open Office"

        # format loop 4
        - name: "Filigrane PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/edit//powerpoint/"
          description: "MS PowerPoint et présentations Open Office"

        # format loop 5
        - name: "Filigrane DOCX"
          format: "DOCX"
          link: "/watermark/python-net/edit//docx/"
          description: "Microsoft Word Ouvrir un document XML"
          
        # format loop 6
        - name: "Filigrane PPTX"
          format: "PPTX"
          link: "/watermark/python-net/edit//pptx/"
          description: "PowerPoint Présentation Open XML"
          
        # format loop 7
        - name: "Filigrane XLSX"
          format: "XLSX"
          link: "/watermark/python-net/edit//xlsx/"
          description: "Feuille de calcul Microsoft Excel Open XML"

        # format loop 8
        - name: "Filigrane DOC"
          format: "DOC"
          link: "/watermark/python-net/edit//doc/"
          description: "Microsoft Word 97 - 2007 Documento"

        # format loop 9
        - name: "Filigrane XLS"
          format: "XLS"
          link: "/watermark/python-net/edit//xls/"
          description: "Classeur Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrane PPT"
          format: "PPT"
          link: "/watermark/python-net/edit//ppt/"
          description: "PowerPoint Présentation 97-2003"

        # format loop 11
        - name: "Filigrane RTF"
          format: "RTF"
          link: "/watermark/python-net/edit//rtf/"
          description: "Format de texte enrichi"

---