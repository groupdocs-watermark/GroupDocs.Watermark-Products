
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:27
draft: false
lang: fr
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Mettez à jour les filigranes dans DOCX de manière fluide"
head_description: "Mettez facilement à jour les filigranes dans DOCX documents avec GroupDocs.Watermark for Node.js via Java. Installez notre bibliothèque sur votre application."

############################# Header ############################
title: "Traiter le filigrane dans DOCX documents" 
description: "Ajustez sans effort les filigranes avec précision à l'aide de GroupDocs.Watermark for Node.js via Java. Préservez la confidentialité des documents de votre entreprise en appliquant différents filigranes. Personnalisez les caractéristiques du filigrane, notamment la taille, l'alignement, l'angle de rotation et la position, selon vos spécifications."
subtitle: "GroupDocs.Watermark for Node.js via Java Bibliothèque" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Téléchargement gratuit sur NPM"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Enquêter sur GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java permet aux développeurs de mettre facilement à jour les filigranes des documents DOCX. Ce puissant outil permet d'ajuster avec précision les filigranes dans différents formats de fichiers, notamment PDF, Microsoft Word, Excel, PowerPoint, Visio, e-mail et formats d'image. GroupDocs.Watermark for Node.js via Java peut être utilisé sur de nombreuses plateformes populaires.

############################# Steps ############################
steps:
    enable: true
    title: "Modification dynamique du filigrane pour DOCX dans Node.js via Java"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** offre aux développeurs Node.js via Java une API puissante pour modifier les filigranes dans divers documents DOCX. Voici un guide complet pour rationaliser votre flux de travail :
      
      1. **Démarrez le processus :** Commencez par fournir votre fichier DOCX comme argument au constructeur de classe **Watermarker**. Selon vos besoins, le fichier peut provenir soit d'un flux, soit d'un emplacement de disque local.
      2. **Identifier les filigranes :** Utilisez l'objet **SearchCriteria** pour identifier les filigranes à modifier. Cet outil polyvalent permet une sélection ciblée de filigranes en fonction de propriétés spécifiques.
      3. **Affiner avec précision :** Une fois la recherche exécutée avec succès, accédez à une collection de filigranes pertinents. Profitez d'un contrôle granulaire sur chaque élément, avec la possibilité de mettre à jour les dimensions, le positionnement des pages, le contenu du texte, la couleur, les données d'image, etc.
      4. **Persistance transparente :** Une fois les mises à jour des filigranes terminées, stockez en toute sécurité le document modifié. L'API offre des options de stockage flexibles, vous permettant d'enregistrer dans un chemin de fichier local ou en tant qu'objet de flux.
   
    code:
      platform: "net"
      copy_title: "Copier"
      install:
        command: "npm i @groupdocs/groupdocs.watermark"
        copy_tip: "cliquez pour copier"
        copy_done: "copié"
      links:
        #  loop
        - title: "Plus d'exemples"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/watermark/nodejs-java/"
          
      content: |
        ```javascript {style=abap}

        // Mettre à jour le filigrane de l'image DOCX

        // Composez Watermarker pour le fichier DOCX
        const watermarker = new groupdocs.watermark.Watermarker("input.docx");

        // Utilisez SearchCriteria pour trouver une image particulière
        const searchCriteria = 
            new groupdocs.watermark.ImageDctHashSearchCriteria("logo.png");
        const watermarks = watermarker.search(searchCriteria);
        
        // Mettre à jour le contenu de l'image
        for (const watermark of watermarks.getInnerList().toArray())
        {
            watermark.setImageData(imageData);
        }

        // Enregistrer le fichier mis à jour
        watermarker.save("output.docx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "En savoir plus sur l'ajout d'un filigrane"
  description: "API pour le rendu, l'affichage et la conversion de documents, de diapositives, de diagrammes et de nombreux autres types de documents dans .NET applications"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Ajouter un filigrane"
  features:
    # feature loop
    - title: "Modifiez sans effort les filigranes en PDF s"
      content: "GroupDocs.Watermark propose des outils robustes dans Node.js via Java pour modifier facilement les filigranes existants dans PDF documents. Ajustez facilement la position, la transparence et bien plus encore."

    # feature loop
    - title: "Affinez les détails du filigrane pour plus de précision"
      content: "Prenez le contrôle des détails. Notre API vous permet d'affiner l'apparence des filigranes, ce qui permet de modifier avec précision la taille, l'opacité et la couleur de vos PDF s."

    # feature loop
    - title: "Gestion rationalisée des filigranes"
      content: "Notre API simplifie la gestion des filigranes. Qu'il s'agisse de les mettre à jour ou de les supprimer, vous pouvez gérer les filigranes de manière efficace, en préservant l'intégrité des documents tout en répondant à vos besoins en matière de marque."
      
  code_samples:
    # code sample loop
    - title: "Mettre à jour le contenu du filigrane de présentation"
      content: |
        Cet exemple montre comment mettre à jour le contenu textuel des filigranes de présentation.
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Chargez le document PDF pour traitement
            const watermarker = new groupdocsWatermark.Watermarker("source.pptx");

            //  Recherchez des filigranes spécifiques qui répondent à vos critères
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria("denied", false);
            const watermarks = watermarker.search(searchCriteria);
  
            //  Modifier les paramètres du filigrane, tels que la taille, la couleur et la position
            for (const watermark of watermarks.getInnerList().toArray()) {
                watermark.setText("accepted");
            }

            //  Enregistrez le document mis à jour sur un système local ou diffusez-le directement
            watermarker.save("result.pptx");
            watermarker.close();

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Prêt à démarrer ?"
  description: "Essayez GroupDocs.Watermark fonctionnalités gratuitement ou demandez une licence"
  items:
    #  loop
    - title: "NPM télécharger"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licences"
      link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Mettre à jour les filigranes pour d'autres formats"
    exclude: "DOCX"
    description: "Ajustez facilement les filigranes dans PDF, Word, Excel, et plus encore avec GroupDocs.Watermark for Node.js via Java. De nombreux autres formats sont pris en charge."
    items: 
        # format loop 1
        - name: "Filigrane PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/update//pdf/"
          description: "Format de document Adobe Portable"

        # format loop 2
        - name: "Filigrane Word"
          format: "WORD"
          link: "/watermark/nodejs-java/update//word/"
          description: "MS Word et documents Open Office"
          
        # format loop 3
        - name: "Filigrane Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/update//excel/"
          description: "MS Excel et feuilles de calcul Open Office"

        # format loop 4
        - name: "Filigrane PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/update//powerpoint/"
          description: "MS PowerPoint et présentations Open Office"

        # format loop 5
        - name: "Filigrane DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/update//docx/"
          description: "Microsoft Word Ouvrir un document XML"
          
        # format loop 6
        - name: "Filigrane PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/update//pptx/"
          description: "PowerPoint Présentation Open XML"
          
        # format loop 7
        - name: "Filigrane XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/update//xlsx/"
          description: "Feuille de calcul Microsoft Excel Open XML"

        # format loop 8
        - name: "Filigrane DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/update//doc/"
          description: "Microsoft Word 97 - 2007 Documento"

        # format loop 9
        - name: "Filigrane XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/update//xls/"
          description: "Classeur Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrane PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/update//ppt/"
          description: "PowerPoint Présentation 97-2003"

        # format loop 11
        - name: "Filigrane RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/update//rtf/"
          description: "Format de texte enrichi"

---