
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:29
draft: false
lang: fr
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Édition personnalisée de filigranes dans des fichiers Docx"
head_description: "Personnalisez le contenu des filigranes dans les fichiers Docx avec les outils GroupDocs.Watermark for Python via .NET pour répondre aux besoins de branding."

############################# Header ############################
title: "Adapter les filigranes Docx dans vos projets Python" 
description: "Éditez et gérez les filigranes à travers divers types de documents avec GroupDocs.Watermark for Python via .NET."
subtitle: "Suite API GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Accédez via PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Outils de filigrane flexibles :** Adaptez et personnalisez le filigranage à travers les formats en utilisant GroupDocs.Watermark for Python via .NET dans votre flux de travail Python.

############################# Steps ############################
steps:
    enable: true
    title: "Utiliser l'API Python pour modifier des filigranes dans des documents Docx"
    content: |
      Avec **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)**, les développeurs Python peuvent modifier le contenu des filigranes dans divers documents Docx. Voici un aperçu rapide :
      
      1. Commencez par charger le document Docx à l'aide de la classe **Watermarker**, acceptant les chemins de fichiers, les flux mémoire ou les tableaux d'octets comme entrée.
      2. Construisez un objet **SearchCriteria** pour rechercher des éléments de filigrane existants dans votre document, qu'ils soient textuels ou graphiques.
      3. Une fois identifiés, l'outil fournit une collection d'instances de filigranes correspondants que vous pouvez mettre à jour - ajustez des paramètres tels que la couleur, l'alignement, la police ou même les données d'image intégrées.
      4. Finalisez le processus en sauvegardant votre document révisé sur disque ou sur tout flux de sortie pris en charge en utilisant les méthodes de sauvegarde intégrées.
   
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
        # Mettre à jour le filigrane d'image dans un fichier DOCX
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Créer une instance de Watermarker avec le fichier d'entrée
        with gw.Watermarker("input.docx") as watermarker:

            # Utiliser SearchCriteria pour localiser les filigranes basés sur des images
            search_criteria = gwss.ImageDctHashSearchCriteria("logo.png")

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # Appliquer les modifications au filigrane d'image
                        watermark.ImageData = imageData
                    except Exception as e:
                        pass

            # Exporter le fichier DOCX mis à jour
            watermarker.save("output.docx")
        ```     

############################# More features ############################
more_features:
  enable: true
  title: "Boostez votre productivité avec des outils de filigrane avancés"
  description: "Accélérez le branding et la protection des documents en Python avec notre API dynamique de filigrane. Insérez, détectez, modifiez ou supprimez des couches de filigranes avec un minimum d'effort."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Flux de travail avancé d'édition de filigrane"
  features:
    # feature loop
    - title: "Contrôle de filigrane intégré"
      content: "Apportez un contrôle complet du cycle de vie du filigrane à vos applications Python en utilisant GroupDocs.Watermark for Python via .NET. Évitez les tâches répétitives en automatisant la configuration, les mises à jour et la suppression des filigranes."

    # feature loop
    - title: "Ajustement de précision des attributs de filigrane"
      content: "Prenez le contrôle total de l'esthétique du filigrane : redimensionnez, recouvrez de couleur, faites pivoter ou repositionnez-les pour répondre à toutes les exigences visuelles avec notre API flexible."

    # feature loop
    - title: "Exploitez les fonctionnalités des formats natifs"
      content: "Adaptez-vous à n'importe quel format de fichier en intégrant des filigranes dans les en-têtes, les pieds de page, les annotations ou les arrière-plans. Notre API respecte les structures natives pour une intégration optimale."
      
  code_samples:
    # code sample loop
    - title: "Modifier un filigrane dans un fichier PDF"
      content: |
        Démontre comment changer les propriétés du filigrane dans un document PDF.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # Ouvrir le fichier PDF
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.pdf as gwop

        # Lire le contenu du filigrane
        load_options = gwop.PdfLoadOptions()
        with gw.Watermarker("source.pdf", load_options) as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,5,8]

            # Appliquer la mise à jour du filigrane
            watermarks = watermarker.search(search_criteria)
            for watermark in watermarks:
                try:
                    watermark.formatted_text_fragments.clear()
                    watermark.formatted_text_fragments.add(
                        "New text", 
                        gww.Font("Calibri", 5.0, gww.FontStyle.bold), 
                        gww.Color.white, 
                        gww.Color.aqua
                    )
                except Exception as e:
                    pass
        
            # Enregistrer le résultat modifié
            watermarker.save("output.pdf")
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
    title: "Contrôle de filigrane pour d'autres formats"
    exclude: "DOCX"
    description: "Utilisez des outils d'édition de filigrane cohérents à travers tous les types de fichiers pris en charge avec GroupDocs.Watermark for Python via .NET."
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