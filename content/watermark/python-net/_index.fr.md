---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:49
draft: false

lang: fr
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
head_title: "Python Bibliothèque de filigranes | Filigranes de documents"
head_description: "Python protège les documents professionnels avec des filigranes de texte et d'image. Les formats de fichiers tels que PDF, Word, Excel et PowerPoint sont pris en charge."

############################# Header ############################
title: "Accédez à la technologie de filigrane Python via .NET"
description: "Protégez vos données et empêchez toute copie non autorisée avec cette solution Python. Ajoutez facilement des filigranes à des documents professionnels dans différents formats, notamment PDF, Word, Excel, PowerPoint, images, etc."
words:
  for: "pour"

actions:
  main: "PyPi télécharger gratuitement"
  main_link: "https://pypi.org/project/groupdocs-watermark-net/"
  alt: "Licences"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
  title: "Prêt à démarrer ?"
  description: "Essayez GroupDocs.Watermark fonctionnalités gratuitement ou demandez une licence"

release:
  title: "Version {0} publiée"
  notes: "Découvrez les nouveautés"
  downloads: "Téléchargements"
  link: "https://releases.groupdocs.com/watermark/python-net/"

code:
  title: "Ajouter un filigrane au PDF à l'aide de Python"
  more: "Plus d'exemples"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
  install: "pip install groupdocs-watermark-net"
  content: |
    ```python {style=abap}

    import groupdocs.watermark as gw
    import groupdocs.watermark.watermarks as gww
    import groupdocs.watermark.options.pdf as gwop
    import groupdocs.watermark.common as gwc

    # Instanciez un filigrane en passant le chemin PDF
    pdf_lo = gwop.PdfLoadOptions()
    with gw.Watermarker("source.pdf", pdf_lo) as watermarker:
        options = gwop.PdfArtifactWatermarkOptions()

        # Personnalisez les options de filigrane
        text_watermark = 
            gww.TextWatermark("Approved", gww.Font("Arial", 8.0))
        text_watermark.horizontal_alignment = 
            gwc.HorizontalAlignment.RIGHT

        # Appliquer un filigrane au document PDF
        watermarker.add(text_watermark, options)

        # Enregistrer le document de résultats
        watermarker.save("result.pdf")

    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark en un coup d'œil"
  description: "Python Bibliothèque pour le filigrane"
  features:
    # feature loop
    - title: "Python Filigrane de documents"
      content: "Sécurisez vos données sensibles avec GroupDocs.Watermark for Python via .NET. Mettez du texte ou des images sur différents formats de fichiers sous forme de filigranes."

    # feature loop
    - title: "Personnaliser les filigranes"
      content: "De nombreuses options de personnalisation sont disponibles dans GroupDocs.Watermark for Python via .NET. Configurez les styles de texte (gras, italique, police) ou les propriétés de l'image telles que la taille ou la rotation pour affiner le filigrane des documents."

    # feature loop
    - title: "Prise en charge des formats de fichiers populaires"
      content: "GroupDocs.Watermark for Python via .NET prend en charge une large gamme de formats de fichiers, notamment PDF, les documents MS Office tels que Word, Excel, PowerPoint et les images telles que JPEG, PNG, GIF, BMP, les diagrammes Visio, les e-mails, etc. Améliorez le traitement des documents pour répondre aux besoins des entreprises. objectifs."

    # feature loop
    - title: "Recherche et mise à jour de filigrane"
      content: "Récupérez et mettez à jour les filigranes placés dans les documents. Modifiez le style du texte, le contenu de l’image ou supprimez-les entièrement. GroupDocs.Watermark for Python via .NET offre une large gamme de fonctionnalités de traitement des filigranes."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indépendance de la plateforme"
  description: "GroupDocs.Watermark for Python via .NET s'intègre de manière transparente à divers systèmes d'exploitation et gestionnaires de packages."
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
  title: "Formats de fichiers pris en charge"
  description: |
    GroupDocs.Watermark for Python via .NET vous permet de traiter une large gamme de formats de fichiers. [Explorez la liste complète](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### formats Microsoft Office et OpenDocument
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### Images et graphiques
        * **Formats d'image populaires:** BMP, JPG, JPEG, PNG
        * **Images de plusieurs pages:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### Autres
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark for Python via .NET fonctionnalités"
  description: "Renforcez la sécurité des documents grâce au filigrane programmatique. Traitez divers formats de fichiers, notamment PDF, DOCX, XLSX, PPTX et formats d'image (PNG, JPG, etc.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Contrôle précis du filigrane"
      content: "Gérez avec précision les filigranes en les ajoutant ou en les supprimant de sections spécifiques, de documents entiers ou de pièces jointes et de formes individuelles dans différents formats de fichiers."

    # feature loop
    - icon: "watermark_style"
      title: "Personnaliser l'apparence du filigrane"
      content: "Exercez un contrôle précis sur l’esthétique du filigrane en modifiant des attributs tels que la couleur, la police, l’opacité, la rotation et le positionnement dans le document."

    # feature loop
    - icon: "hidden_print"
      title: "Imprimer le filigrane PDF"
      content: "Ajoutez des filigranes cachés dans les documents ordinaires qui ne deviennent visibles que pendant le processus d'impression, améliorant ainsi discrètement la sécurité des documents."

    # feature loop
    - icon: "image_only"
      title: "Filigrane d’image spécifique"
      content: "Filigranez des images spécifiques dans un document à l’aide de notre solution. Intégrez des filigranes dans une section désignée (par exemple, une page, une diapositive) ou dans l'ensemble du document."

    # feature loop
    - icon: "image_frame"
      title: "Filigranes d'images multicouches"
      content: "Ajoutez des filigranes avec précision à des images spécifiques dans un format d'image multi-images, obtenant ainsi un contrôle granulaire sur le placement des filigranes."

    # feature loop
    - icon: "attachments"
      title: "Protection complète du contenu"
      content: "Étendez la protection à divers éléments de documents tels que les pièces jointes dans les documents Excel et les formes d'image dans les présentations, offrant ainsi une couche de sécurité supplémentaire."

    # feature loop
    - icon: "pdf_objects"
      title: "Filigrane PDF avancé"
      content: "Filigranez différentes zones des PDF, notamment la zone de fond perdu, la zone d'art, la zone de recadrage, la zone de rognage, etc."

    # feature loop
    - icon: "doc_background"
      title: "Filigrane d’image d’arrière-plan"
      content: "Gérez les filigranes dans les images d'arrière-plan des feuilles de calcul et des présentations, en offrant des options de personnalisation supplémentaires pour les mesures de sécurité visuelle."

    # feature loop
    - icon: "unreadable_characters"
      title: "Filigrane de texte avec des caractères illisibles"
      content: "Utilisez des caractères illisibles dans les filigranes de texte intégrés dans les présentations, renforçant ainsi la sécurité en rendant l'extraction non autorisée de filigranes beaucoup plus difficile."

    # feature loop
    - icon: "watermark_text_search"
      title: "Recherche avancée de filigrane"
      content: "Utilisez des fonctionnalités de recherche complètes pour localiser les filigranes dans les documents en fonction de paramètres spécifiques ou en combinant divers critères."

    # feature loop
    - icon: "watermark_image_search"
      title: "Détection de filigrane d’image similaire"
      content: "Recherchez des images de filigrane similaires dans des documents qui ressemblent visuellement à une image source."

    # feature loop
    - icon: "document_info"
      title: "Analyser les informations du document"
      content: "Extrayez les données essentielles du document, telles que la mise en page, pour une analyse plus approfondie."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de code"
  description: "Explorez des exemples de code présentant les fonctionnalités courantes de GroupDocs.Watermark for Python via .NET."
  items:
    # code sample loop
    - title: "Filigraner un document avec une image"
      content: |
        Utilisez GroupDocs.Watermark for Python via .NET pour protéger les documents en ajoutant des filigranes d'image. [En savoir plus](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Comment protéger un fichier par filigrane d'image.">}}
        ```python {style=abap}

        # Charger le document source dans Watermarker
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Spécifier le chemin d'accès à une image en filigrane
            watermark = groupdocs.watermark.watermarks.ImageWatermark("watermark.jpg")
            watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwgroupdocs.watermark.common.VerticalAlignment.CENTER

            # Protégez le fichier et enregistrez-le
            watermarker.add(watermark)
            watermarker.save("result.pdf")
       
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Rechercher et modifier des filigranes existants"
      content: |
        GroupDocs.Watermark for Python via .NET vous permet de gérer les filigranes de documents. Sélectionnez les filigranes et modifiez leurs propriétés. [Découvrez comment](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Recherche et modification de filigranes.">}}
        ```python {style=abap}

        # Charger le document source
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Rechercher les filigranes à mettre à jour
            search_criteria = groupdocs.watermark.search.searchcriteria.TextSearchCriteria("annotation", False)
            watermarks = watermarker.search(search_criteria)
            
            # Mettre à jour les propriétés souhaitées
            for watermark in watermarks:
                watermark.text = "passed"

            # Enregistrer le document modifié dans un chemin spécifié
            watermarker.save("result.pdf")


        ```
        {{< /landing/code >}}

---
