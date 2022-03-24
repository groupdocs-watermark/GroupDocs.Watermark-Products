---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET API pour ajouter la recherche supprimer les filigranes aux images Word Excel PDF"
head_description: "API C# .NET pour ajouter, rechercher et supprimer des filigranes d'image et de texte à partir de documents : PDF, Word, Excel, présentations, Visio, e-mail et formats de fichier image."

############################# Header ############################
title: ".NET API pour la manipulation de filigrane"
description: "Créez des applications .NET pour exploiter des filigranes basés sur du texte et des images avec une recherche intelligente et des caractéristiques de sécurité renforcées."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Watermark for .NET"
        image: "/border/groupdocs-watermark-net.svg"
        product: "GroupDocs.Watermark"
        platform: ".NET"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Aperçu"

            # button loop
            - link: "#features"
              text: "Caractéristiques"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/watermark"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/watermark/net"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/watermark"
        link_learn: "https://docs.groupdocs.com/watermark/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Aperçu ############################
overview:
    enable: true
    content: |
      GroupDocs.Watermark pour .NET vous permet de créer des applications commerciales prêtes à commercialiser en C#, ASP.NET et d'autres technologies liées à .NET, qui permettent à vos utilisateurs finaux d'ajouter de nouveaux filigranes, de rechercher et de supprimer des filigranes existants dans les formats de fichiers pris en charge. . En utilisant GroupDocs.Watermark pour .NET, vous pouvez appliquer par programmation des filigranes numériques à une multitude de formats de fichiers et décourager l'utilisation non autorisée de la propriété intellectuelle et étiqueter en toute sécurité les documents de nature sensible en utilisant diverses mesures de sécurité intégrées offertes par cette API.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Voici un aperçu de GroupDocs.Watermark pour .NET :
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Aperçu"
          content: |
            * Ajouter et supprimer un filigrane
            * Rechercher et remplacer le filigrane
            * Rechercher par mise en forme
            * Recherche par comparaison d'images
            * Travailler avec les en-têtes et pieds de page
            * Travailler avec des images d'arrière-plan
            * Travailler avec des pièces jointes
            * Pixelliser les pages
            * Appliquer les restrictions d'édition
      
      ## TAB TWO ##
      tab_two:
        description: |
          Les [formats de document et type de filigrane](https://docs.groupdocs.com/watermark/net/supported-document-formats/) pris en charge pour chaque format sont répertoriés ci-dessous :

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
                * **Visio:** VSD, VDX, VSS, VSSX, VSX, VST, VSTX, VTX, VSDX, VDW, VSTM, VSSM, VSDM

            # table loop
            - title: "Ajouter un filigrane"
              content: |
                * **PDF** : XObject, Artefact, Annotation
                * **Mot** : Forme
                * **Excel** : forme, en-tête et pied de page
                * **PowerPoint** : Forme
                * **Visio** : Forme
                * **Image raster** : texte, image
                * **Tiff multipage** : texte, image
                * **Gif animé** : texte, image

        right:
          enable: true
          table:
            # table loop
            - title: "Documents PDF et images"
              content: |
                * **Portable Document Format**: PDF
                * **Open Document**: ODT
                * **Email**: EML, MSG, EMLX, OFT
                * **Images**: PNG, BMP, GIF, JPG, JPEG, JP2, TIF, TIFF, WebP

            # table loop
            - title: "Suppression du filigrane"
              content: |
                * **PDF** : XObject, Artefact, Annotation, Texte normal
                * **Mot** : forme, texte normal
                * **Excel** : forme, en-tête et pied de page, image d'arrière-plan, texte et formules dans les cellules
                * **PowerPoint** : Forme
                * **Visio** : Forme, Diagramme Commentaires
                * **E-mail** : images jointes et intégrées, fragments de l'objet et du corps du texte

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Watermark for .NET prend en charge la suite Systèmes d'exploitation, Frameworks & Directeur chargé d'emballages:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Systèmes d'exploitation"
              content: |
                * Bureau Windows
                * Serveur Windows
                * windows Azure
                * Linux

            # table loop
            - icon: "fas fa-code"
              title: "Cadres pris en charge"
              content: |
                * .NET Framework 2.0 ou supérieur
                * Mono Framework 1.2 ou supérieur
                * Norme .NET 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Directeur chargé d'emballage"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Environnements de développement"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Caractéristiques ############################
features:
    enable: true
    title: "GroupDocs.Watermark for .NET Caractéristiques"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Ajouter ou supprimer des filigranes d'une section particulière ou d'un document entier de divers formats de fichiers"

      # feature loop
      - icon: "fas fa-eye"
        content: "Joindre un filigrane à toutes les images d'une section, d'une page, d'une diapositive ou d'un document particulier"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Attribuer un filigrane uniquement à des cadres particuliers d'une image à plusieurs cadres"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Attribuer un filigrane masqué au PDF qui n'apparaît que lors de l'impression d'un document"

      # feature loop
      - icon: "fas fa-code"
        content: "Définir un filigrane sur toutes les pièces jointes d'un document Excel et toutes les formes d'image dans les diapositives"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Placer un filigrane ou le supprimer des images d'arrière-plan de la feuille de calcul ou des diapositives"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Utiliser un filigrane pour les fichiers pris en charge dans toutes les pièces jointes d'un e-mail ou d'un document PDF"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Appliquer ou supprimer le filigrane en tant que XObjects, artefacts et annotations dans les documents PDF"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Éliminer le filigrane contenant du texte avec un formatage particulier"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Rechercher des filigranes d'image qui ressemblent à une image particulière"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Identifier le filigrane de texte même s'il y a des caractères illisibles entre les lettres"

      # feature loop
      - icon: "fas fa-columns"
        content: "Rechercher des filigranes en fonction de paramètres spécifiques ou en combinant plusieurs critères"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Spécifiez la mise en forme de la police pour rechercher le filigrane de texte correspondant"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Extraire par programmation la mise en page et d'autres informations pour les formats pris en charge"

      # feature loop
      - icon: "fas fa-print"
        content: "Ajouter un filigrane aux images dans n'importe quel en-tête et pied de page dans les formats de document pris en charge"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Ajouter un filigrane aux formes d'image dans un document Word et verrouiller les filigranes pour restreindre l'édition"

      # feature loop
      - icon: "fas fa-lock"
        content: "Protéger le filigrane de texte à l'aide de caractères illisibles dans les présentations"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Rasteriser une page particulière ou un document PDF entier pour protéger les filigranes ajoutés"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Modifier la mise en forme du texte lors du remplacement du filigrane de texte existant"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Aligner le filigrane sur la zone de fond perdu, la zone d'illustration, la zone de recadrage ou la zone de rognage dans le document PDF"

      # feature loop
      - icon: "fas fa-heading"
        content: "Modifier les propriétés de forme dans les documents Microsoft Visio"

    more_feature :
      # more_feature_loop
      - title: "Ajouter un filigranes"
        content: |
          GroupDocs.Watermark pour .NET prend en charge plusieurs types de filigranes. L'ajout de filigranes de tout type n'est qu'une question de quelques lignes de code. L'exemple suivant montre comment appliquer un filigrane d'image à un document Word à l'aide de C# :

          ```cs
          // Charger le document
          using (FileStream stream = File.Open("document.docx", FileMode.Open, FileAccess.ReadWrite))
          {
            using (Watermarker watermarker = new(Watermarker(stream))
            {
                // Utiliser le chemin d'accès à l'image comme paramètre du constructeur
                using (ImageWatermark watermark = new ImageWatermark("logo.png"))
                {
                    watermark.HorizontalAlignment = HorizontalAlignment.Center;
                    watermark.VerticalAlignment = VerticalAlignment.Center;
                    watermarker.Add(watermark);
                }
                // Enregistrer le document résultant
                watermarker.Save("document_watermarked.docx");
                }
          }
          ```
      # more_feature_loop
      - title: "Appliquer un filigrane à des fichiers de différents formats en une seule fois"
        content: "L'API GroupDocs.Watermark vous permet d'appliquer un filigrane ou de supprimer le filigrane de tous les fichiers d'un dossier spécifique en une seule fois. Les fichiers peuvent même être de format différent et pourtant le filigrane sera appliqué à chacun d'eux avec précision."

      # more_feature_loop
      - title: "Sécurité infaillible pour Watermark"
        content: "Avec une seule ligne de code, il est très difficile pour n'importe quel outil de supprimer votre filigrane des fichiers PDF. Ceci est réalisé en convertissant toutes les pages d'un document PDF en images raster tout en conservant la qualité d'origine intacte."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Watermark propose des API de visualisation de documents pour d'autres environnements de développement populaires"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Watermark for Java"
          image: "/border/groupdocs-watermark-java.svg"
          product: "GroupDocs.Watermark"
          platform: "Java"
          link: "/watermark/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---