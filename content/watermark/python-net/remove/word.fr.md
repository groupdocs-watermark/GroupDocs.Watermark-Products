
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:16
draft: false
lang: fr
format: Word
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Supprimer les filigranes des Word avec Python"
head_description: "Supprimez rapidement ou modifiez les filigranes dans les fichiers Word en utilisant notre API Python pour des documents professionnels et propres."

############################# Header ############################
title: "Éliminateur de filigranes Word pour Python" 
description: "Utilisez l'API GroupDocs.Watermark for Python via .NET pour supprimer les filigranes des fichiers Word, gardant vos documents juridiques et professionnels en ordre."
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
    title: "Bibliothèque GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       Avec GroupDocs.Watermark for Python via .NET, vous pouvez facilement trouver et supprimer les filigranes dans les fichiers Word. Détectez, modifiez ou supprimez à la fois les filigranes de texte et d'image tout en préservant la mise en page de votre document.

############################# Steps ############################
steps:
    enable: true
    title: "Comment supprimer les filigranes des fichiers Word en Python"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/python-net/)** permet de supprimer rapidement les filigranes de vos documents professionnels. Ajoutez notre bibliothèque à votre projet Python et suivez ces étapes :
      
      1. Commencez par créer un objet **Watermarker** avec votre fichier Word. Vous pouvez utiliser un chemin de fichier ou un flux comme entrée.
      2. Utilisez **SearchCriteria** pour filtrer quels filigranes vous souhaitez retirer. Vous pouvez rechercher par texte, image ou mise en forme. Plus vous êtes précis, plus votre recherche sera pertinente.
      3. Parcourez les filigranes trouvés et supprimez ceux dont vous n'avez pas besoin dans le document.
      4. Une fois terminé, enregistrez le document nettoyé sous forme de fichier ou de flux.
   
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
        # Supprimer le filigrane de texte d'un fichier Word
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Ouvrir le fichier Word avec une instance de Watermarker
        with gw.Watermarker("input.docx") as watermarker:

            # Trouver et supprimer les filigranes choisis
            search_criteria = gwss.TextFormattingSearchCriteria("test", False)
            criteria.ForegroundColorRange = gwss.ColorRange()
            criteria.FontBold = True

            possible_watermarks = watermarker.search(search_criteria)
            watermarks.clear()

            # Enregistrer le fichier mis à jour à l'emplacement choisi
            watermarker.save("output.docx")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Suppression efficace des filigranes avec Python"
  description: "Notre API Python vous aide à supprimer rapidement les filigranes des fichiers PDF et bureautiques, gardant vos documents propres et originaux."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "Effacer le Filigrane"
  features:
    # feature loop
    - title: "Suppression précise des filigranes"
      content: "L'API Python vous permet de supprimer les filigranes sans endommager la mise en page ou la qualité de votre document. Elle est conçue pour des développeurs ayant besoin de résultats fiables."

    # feature loop
    - title: "Supprimer des filigranes en masse"
      content: "Effacez facilement les filigranes de plusieurs fichiers à la fois. Ceci est idéal pour les entreprises qui ont besoin de traiter de nombreux documents rapidement et en toute sécurité."

    # feature loop
    - title: "Édition avancée pour les filigranes"
      content: "Utilisez des options avancées pour peaufiner ou modifier les filigranes avant de les supprimer. Cela vous aide à garder vos documents professionnels et sécurisés."
      
  code_samples:
    # code sample loop
    - title: "Supprimer un filigrane de texte d'Excel"
      content: |
        Cet exemple montre comment supprimer des filigranes de texte avec un formatage spécial dans les fichiers Excel.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Ouvrir le fichier Excel
        with gw.Watermarker("source.xlsx") as watermarker:

            # Rechercher le filigrane
            search_criteria = gwss.TextSearchCriteria("someurl.com")

            # Supprimer le filigrane
            watermarks = watermarker.search(search_criteria)

            for i in range(len(watermarks) - 1, -1, -1):
                if isinstance(watermarks[i], gws.HyperlinkPossibleWatermark):
                    del watermarks[i]

            # Enregistrer le XLSX nettoyé
            watermarker.save("result.xlsx");
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
    title: "Gestion des filigranes dans Word avec Python"
    exclude: "WORD"
    description: "Découvrez comment gérer et supprimer les filigranes dans les fichiers Word en utilisant notre API Python pour une meilleure qualité de document."
    items: 
        # format loop 1
        - name: "Filigrane PDF"
          format: "PDF"
          link: "/watermark/python-net/remove//pdf/"
          description: "Format de document Adobe Portable"

        # format loop 2
        - name: "Filigrane Word"
          format: "WORD"
          link: "/watermark/python-net/remove//word/"
          description: "MS Word et documents Open Office"
          
        # format loop 3
        - name: "Filigrane Excel"
          format: "EXCEL"
          link: "/watermark/python-net/remove//excel/"
          description: "MS Excel et feuilles de calcul Open Office"

        # format loop 4
        - name: "Filigrane PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/remove//powerpoint/"
          description: "MS PowerPoint et présentations Open Office"

        # format loop 5
        - name: "Filigrane DOCX"
          format: "DOCX"
          link: "/watermark/python-net/remove//docx/"
          description: "Microsoft Word Ouvrir un document XML"
          
        # format loop 6
        - name: "Filigrane PPTX"
          format: "PPTX"
          link: "/watermark/python-net/remove//pptx/"
          description: "PowerPoint Présentation Open XML"
          
        # format loop 7
        - name: "Filigrane XLSX"
          format: "XLSX"
          link: "/watermark/python-net/remove//xlsx/"
          description: "Feuille de calcul Microsoft Excel Open XML"

        # format loop 8
        - name: "Filigrane DOC"
          format: "DOC"
          link: "/watermark/python-net/remove//doc/"
          description: "Microsoft Word 97 - 2007 Documento"

        # format loop 9
        - name: "Filigrane XLS"
          format: "XLS"
          link: "/watermark/python-net/remove//xls/"
          description: "Classeur Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrane PPT"
          format: "PPT"
          link: "/watermark/python-net/remove//ppt/"
          description: "PowerPoint Présentation 97-2003"

        # format loop 11
        - name: "Filigrane RTF"
          format: "RTF"
          link: "/watermark/python-net/remove//rtf/"
          description: "Format de texte enrichi"

---