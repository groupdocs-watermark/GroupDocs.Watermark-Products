
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:30
draft: false
lang: fr
format: Pptx
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Supprimer les filigranes PowerPoint avec Python"
head_description: "Effacez rapidement les filigranes des diapositives PowerPoint en utilisant notre API Python pour des présentations professionnelles."

############################# Header ############################
title: "Supprimer des filigranes des diapositives PPTX avec Python" 
description: "Utilisez l'API GroupDocs.Watermark for Python via .NET pour supprimer les filigranes des diapositives PPTX et garder vos présentations à leur meilleur."
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
       La bibliothèque GroupDocs.Watermark for Python via .NET vous fournit tous les outils nécessaires pour gérer les filigranes dans les présentations PowerPoint. Supprimez ou ajustez les filigranes pour garder vos diapositives propres et professionnelles.

############################# Steps ############################
steps:
    enable: true
    title: "Supprimer des filigranes de fichiers Pptx en Python"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/python-net/)** permet aux développeurs Python de supprimer rapidement les filigranes des fichiers Pptx. Voici comment procéder :
      
      1. Commencez par passer votre fichier Pptx au constructeur **Watermarker**. Vous pouvez utiliser un chemin de fichier, un flux d'octets ou un flux de fichier.
      2. Utilisez l'objet **SearchCriteria** pour rechercher les filigranes à supprimer. Filtrez par image, texte ou formatage pour obtenir des résultats précis.
      3. Après la recherche, vous obtiendrez une liste de filigranes. Sélectionnez et supprimez ceux dont vous n'avez pas besoin.
      4. Une fois terminé, enregistrez le document sur un fichier ou un flux.
   
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
        # Supprimer le filigrane d'image d'un fichier PPTX
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Créer une instance de Watermarker avec votre fichier PPTX
        with gw.Watermarker("input.pptx") as watermarker:

            # Trouver et supprimer le filigrane détecté
            search_criteria = gwss.ImageDctHashSearchCriteria("logo.png")

            possible_watermarks = watermarker.search(search_criteria)
            del possible_watermarks[i]

            # Enregistrer votre document mis à jour
            watermarker.save("output.pptx")
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "Suppression de filigranes puissante avec Python | GroupDocs.Watermark"
  description: "Profitez de notre API Python pour supprimer des filigranes de fichiers PDF et Office. Obtenez des documents propres et professionnels prêts à l'emploi."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "Effacer le filigrane"
  features:
    # feature loop
    - title: "Suppression précise des filigranes en Python"
      content: "Notre API Python est conçue pour une suppression précise des filigranes, garantissant que vos fichiers conservent leur apparence originale et leur formatage. Idéal pour les documents professionnels, juridiques ou académiques."

    # feature loop
    - title: "Suppression de filigranes par lots avec Python"
      content: "Accélérez votre flux de travail en supprimant les filigranes de plusieurs fichiers à la fois. Parfait pour gérer efficacement de grandes collections de documents."

    # feature loop
    - title: "Modification et suppression flexible des filigranes"
      content: "Modifiez ou supprimez les filigranes selon vos besoins. L'API vous propose des options pour maintenir vos documents dans un format optimal pour tous les besoins."
      
  code_samples:
    # code sample loop
    - title: "Supprimer l'arrière-plan d'une présentation"
      content: |
        Cet exemple montre comment supprimer un filigrane de lien hypertexte.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.presentation as gwop

        # Ouvrir la présentation
        load_options = gwop.PresentationLoadOptions()
        with gw.Watermarker("source.pptx", load_options) as watermarker:

            # Accéder au contenu de la diapositive
            search_criteria = gwss.TextSearchCriteria("Lorem ipsum")

            # Supprimer le filigrane de lien hypertexte
            watermarks = watermarker.search(search_criteria)

            for i in range(len(watermarks) - 1, -1, -1):
                if isinstance(watermarks[i], gws.HyperlinkPossibleWatermark):
                    del watermarks[i]

            # Enregistrer la présentation
            watermarker.save("result.pptx");
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
    title: "Supprimer les filigranes de PowerPoint en Python"
    exclude: "PPTX"
    description: "Découvrez comment l'API GroupDocs.Watermark for Python via .NET peut vous aider à supprimer les filigranes des diapositives PPTX pour un résultat propre et professionnel."
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