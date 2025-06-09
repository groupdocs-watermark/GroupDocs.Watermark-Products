
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: fr
format: Image
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Filigranez des images avec Python"
head_description: "Apprenez à ajouter des filigranes à des images en Python. Protégez vos photos sans perdre de qualité."

############################# Header ############################
title: "Filigranage rapide d'image avec Python" 
description: "Notre outil Python vous permet d'ajouter rapidement des filigranes aux images. Prend en charge de nombreux formats, des photos à l'art numérique."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Téléchargez PyPi gratuitement"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET vous aide à ajouter des filigranes aux images en Python. Il prend en charge JPEG, PNG, BMP, TIFF et plus encore. Vous pouvez modifier l'opacité, la taille et la position du filigrane pour répondre à vos besoins. Utilisez-le pour protéger vos images ou ajouter une marque, tout en préservant la qualité originale.

############################# Steps ############################
steps:
    enable: true
    title: "Ajoutez des filigranes : Filtrage Python pour Image"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** est une bibliothèque qui facilite l'ajout de filigranes à de nombreux types de fichiers commerciaux. Suivez ces étapes pour rapidement ajouter des filigranes à vos documents en Python :
      
      1. **Commencez avec le Filigranage :** Commencez par créer une instance de la classe **Watermarker**. Passez votre fichier Image (sous forme de chemin ou de flux) au constructeur pour l'ouvrir pour le filigranage.
      2. **Créez Votre Filigrane :** Créez un objet **Watermark** avec le texte et les paramètres souhaités. Vous pouvez ajouter des filigranes à n'importe quelle page ou même à des éléments de document comme les en-têtes ou les pièces jointes.
      3. **Personnalisez le Filigrane :** Ajustez la taille, la position, la police, la couleur et l'alignement du filigrane pour qu'il convienne à vos besoins. Cela permet à votre filigrane d'apparaître juste comme il faut dans votre document.
      4. **Appliquez et Enregistrez :** Utilisez la méthode **Watermarker** pour ajouter votre ou vos filigranes au document. Enregistrez le résultat, de préférence dans un nouveau fichier pour plus de sécurité.
   
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
        # Ajoutez un filigrane de texte à un fichier IMAGE
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # Sélectionnez le fichier que vous souhaitez filigraner
        with gw.Watermarker("input.jpeg") as watermarker:

            # Créez un objet de filigrane de texte
            font = gww.Font("Arial", 36.0)
            watermark = gww.TextWatermark("top secret", font)
            watermark.foreground_color = gww.Color.red
            watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
            watermark.opacity = 0.4

            watermarker.add(watermark)

            # Enregistrez le fichier IMAGE mis à jour
            watermarker.save("output.jpeg")
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Découvrez plus de fonctionnalités de filigranage"
  description: "Utilisez notre API Python pour ajouter, afficher, convertir et gérer des filigranes dans des documents, des diaporamas, des diagrammes et plus encore. GroupDocs.Watermark for Python via .NET vous aide à protéger vos fichiers et à ajouter des informations sur les droits d'auteur facilement."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Ajouter un filigrane"
  features:
    # feature loop
    - title: "Ajoutez des filigranes facilement"
      content: "GroupDocs.Watermark permet aux développeurs Python d'ajouter rapidement des filigranes de texte, d'image ou dynamiques à des documents commerciaux. Gardez vos fichiers sécurisés et de marque avec un minimum d'effort."

    # feature loop
    - title: "Filigranes entièrement personnalisables"
      content: "Changez la taille, la rotation, la transparence, la couleur et la police du filigrane avec GroupDocs.Watermark. Faites en sorte que votre filigrane s'adapte parfaitement à votre document et que le contenu important reste visible."

    # feature loop
    - title: "Utilisez les fonctionnalités du document pour le filigranage"
      content: "Profitez des fonctionnalités intégrées des documents comme les annotations PDF, les arrière-plans Word ou les en-têtes Excel pour ajouter des filigranes. GroupDocs.Watermark fonctionne avec les structures de documents pour un filigranage efficace et non intrusif."
      
  code_samples:
    # code sample loop
    - title: "Ajouter un filigrane d'image à DOCX"
      content: |
        Cet exemple montre comment appliquer des effets d'image à des filigranes de forme.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.wordprocessing as gwow

        # Ouvrez un document Word
        load_options = gwow.WordProcessingLoadOptions()
        with gw.Watermarker("source.docx", load_options) as watermarker:

            # Définissez les options de filigrane
            with gww.ImageWatermark("logo.png") as watermark:

                effects = gwow.WordProcessingImageEffects()
                effects.brightness = 0.7
                effects.contrast = 0.6
                effects.chroma_key = gww.Color.red

                options = gwow.WordProcessingWatermarkSectionOptions()
                options.Effects = effects;

                # Créez le filigrane
                watermarker.add(watermark, options)

                # Enregistrez le document avec le filigrane
                watermarker.save("result.docx")
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
    title: "Ajoutez des filigranes aux images avec Python"
    exclude: "IMAGE"
    description: "Protégez vos images avec notre boîte à outils Python. Ajoutez des filigranes à de nombreux formats d'image rapidement."
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