
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:28
draft: false
lang: fr
format: Xls
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Ajoutez des filigranes à XLS avec Python"
head_description: "Utilisez Python pour ajouter et gérer des filigranes dans des fichiers XLS pour une meilleure sécurité Excel."

############################# Header ############################
title: "Créez des filigranes Python pour les fichiers XLS" 
description: "Ajoutez des filigranes aux feuilles de calcul XLS en Python—idéal pour protéger les données financières et personnelles."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Obtenez-le gratuitement sur PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET vous permet d'ajouter des filigranes aux fichiers XLS en Python. Utilisez des marques visibles ou invisibles et personnalisez leur apparence pour répondre à vos besoins. Idéal pour garder des données financières ou clients en sécurité, GroupDocs.Watermark fonctionne avec tous les environnements Python.

############################# Steps ############################
steps:
    enable: true
    title: "Ajoutez rapidement des filigranes aux fichiers Xls"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/):** Une bibliothèque puissante Python qui vous permet d'ajouter des filigranes à vos documents.
      
      1. **Classe principale : Watermarker.** Commencez par créer un objet **Watermarker**. Donnez-lui votre fichier Xls, soit en tant que chemin de fichier soit en tant que flux, pour commencer.
      2. **Construisez votre filigrane.** Ensuite, créez un objet Watermark du type que vous souhaitez. Vous pouvez le placer sur n'importe quelle page ou même dans des éléments de document comme des images ou des en-têtes.
      3. **Ajustez l'apparence.** Configurez la taille, la position, la police et la couleur du filigrane en fonction de vos besoins.
      4. **Ajoutez et enregistrez.** Utilisez la méthode **Watermarker** pour insérer votre filigrane. Ajoutez-en autant que nécessaire, puis enregistrez le fichier où vous le souhaitez.
   
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
        # Ajoutez un filigrane image à un fichier XLS
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # Passez le chemin du fichier au constructeur Watermarker
        with gw.Watermarker("input.xls") as watermarker:

            # Créez un filigrane image à l'aide de votre fichier image
            watermark = gww.ImageWatermark("watermark.png")

            watermarker.add(watermark)

            # Enregistrez le fichier XLS avec le filigrane
            watermarker.save("output.xls")
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "Découvrez d'autres outils de filigrane"
  description: "GroupDocs.Watermark for Python via .NET vous offre des options avancées pour ajouter et personnaliser des filigranes dans de nombreux types de fichiers. Protégez vos documents et images avec des fonctionnalités flexibles et faciles à utiliser."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Filtrage tout-en-un"
  features:
    # feature loop
    - title: "Tiling pleine page"
      content: "Couvrez l'ensemble de votre document avec des filigranes en mosaïque. Cela rend difficile la suppression des filigranes et protège vos fichiers sans altérer la mise en page."

    # feature loop
    - title: "Couleurs personnalisées"
      content: "Choisissez n'importe quelle couleur pour votre filigrane afin de l'adapter à votre marque ou au style de votre document. Faites en sorte que votre filigrane se démarque ou s'intègre selon vos besoins."

    # feature loop
    - title: "Options de sécurité supplémentaires"
      content: "Renforcez la sécurité de vos documents grâce à des filigranes superposés. Combinez des marques visibles et cachées pour empêcher la copie et pour vous assurer que seules les bonnes personnes peuvent accéder à vos fichiers."
      
  code_samples:
    # code sample loop
    - title: "Ajouter un filigrane à PowerPoint"
      content: |
        Cet exemple montre comment placer un filigrane sur l'arrière-plan des diapositives PPTX.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.presentation as gwop

        # Ouvrez un fichier PPTX
        load_options = gwop.PresentationLoadOptions()
        with gw.Watermarker("source.pptx", load_options) as watermarker:

            # Définissez les détails du filigrane
            with TextWatermark("Protected image", gww.Font("Arial", 8.0)) as watermark:

                watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
                watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
                watermark.rotate_angle = 45
                watermark.scale_factor = 1

                # Appliquez le filigrane aux arrière-plans des diapositives
                watermarker.add(watermark)

                # Enregistrez la présentation mise à jour
                watermarker.save("result.pptx")
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
    title: "Ajoutez des filigranes à XLS avec Python"
    exclude: "XLS"
    description: "Utilisez Python pour ajouter des filigranes personnalisés aux fichiers XLS et garder vos données Excel sécurisées."
    items: 
        # format loop 1
        - name: "Filigrane PDF"
          format: "PDF"
          link: "/watermark/python-net/add//pdf/"
          description: "Format de document Adobe Portable"

        # format loop 2
        - name: "Filigrane Word"
          format: "WORD"
          link: "/watermark/python-net/add//word/"
          description: "MS Word et documents Open Office"
          
        # format loop 3
        - name: "Filigrane Excel"
          format: "EXCEL"
          link: "/watermark/python-net/add//excel/"
          description: "MS Excel et feuilles de calcul Open Office"

        # format loop 4
        - name: "Image en filigrane"
          format: "IMAGE"
          link: "/watermark/python-net/add//image/"
          description: "Formats d'image populaires"

        # format loop 5
        - name: "Photo en filigrane"
          format: "PHOTO"
          link: "/watermark/python-net/add//photo/"
          description: "Formats de photos"

        # format loop 6
        - name: "Filigrane PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/add//powerpoint/"
          description: "MS PowerPoint et présentations Open Office"

        # format loop 7
        - name: "Filigrane DOCX"
          format: "DOCX"
          link: "/watermark/python-net/add//docx/"
          description: "Microsoft Word Ouvrir un document XML"
          
        # format loop 8
        - name: "Filigrane PPTX"
          format: "PPTX"
          link: "/watermark/python-net/add//pptx/"
          description: "PowerPoint Présentation Open XML"
          
        # format loop 9
        - name: "Filigrane XLSX"
          format: "XLSX"
          link: "/watermark/python-net/add//xlsx/"
          description: "Feuille de calcul Microsoft Excel Open XML"

        # format loop 10
        - name: "Filigrane JPEG"
          format: "JPEG"
          link: "/watermark/python-net/add//jpeg/"
          description: "JPEG Photo"

        # format loop 11
        - name: "Filigrane PNG"
          format: "PNG"
          link: "/watermark/python-net/add//png/"
          description: "Portable Graphique du réseau"

        # format loop 12
        - name: "Filigrane TIFF"
          format: "TIFF"
          link: "/watermark/python-net/add//tiff/"
          description: "Format de fichier d'image de balise"

        # format loop 13
        - name: "Filigrane WEBP"
          format: "WEBP"
          link: "/watermark/python-net/add//webp/"
          description: "Photo WEB"

        # format loop 14
        - name: "Filigrane DOC"
          format: "DOC"
          link: "/watermark/python-net/add//doc/"
          description: "Microsoft Word 97 - 2007 Documento"

        # format loop 15
        - name: "Filigrane XLS"
          format: "XLS"
          link: "/watermark/python-net/add//xls/"
          description: "Classeur Microsoft Excel 97-2003"

        # format loop 16
        - name: "Filigrane PPT"
          format: "PPT"
          link: "/watermark/python-net/add//ppt/"
          description: "PowerPoint Présentation 97-2003"

        # format loop 17
        - name: "Filigrane RTF"
          format: "RTF"
          link: "/watermark/python-net/add//rtf/"
          description: "Format de texte enrichi"

---