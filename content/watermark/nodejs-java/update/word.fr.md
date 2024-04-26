
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:59
draft: false
lang: fr
format: Word
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Mettez facilement à jour les filigranes dans WORD"
head_description: "Simplifiez la mise à jour des filigranes dans les formats de document WORD avec GroupDocs.Watermark à l'aide de Node.js via Java. Renforcez vos solutions d'entreprise."

############################# Header ############################
title: "Simplifier la mise à jour des filigranes des documents WORD" 
description: "Débloquez des fonctionnalités efficaces de mise à jour des filigranes avec GroupDocs.Watermark for Node.js via Java. Protégez vos documents professionnels à l'aide de divers filigranes. Mettez à jour les attributs du filigrane tels que la taille, l'alignement, l'angle de rotation et la position en fonction de vos besoins."
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Téléchargez gratuitement sur NPM"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java capacités"
    link: "/watermark/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java offre une solution fluide pour gérer les filigranes à l'aide des applications Node.js via Java. Cet outil polyvalent permet aux développeurs de modifier facilement les filigranes dans des documents de différents formats de fichiers, notamment PDF, Microsoft Word, Excel, PowerPoint, Visio, e-mail et formats d'image. GroupDocs.Watermark prend en charge tous les principaux systèmes d'exploitation et versions Node.js via Java.

############################# Steps ############################
steps:
    enable: true
    title: "Mettre à jour les filigranes dans WORD via Node.js via Java"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** fournit aux développeurs Node.js via Java une API robuste pour mettre à jour par programmation les filigranes dans divers documents WORD. Ce guide décrit le processus :
      
      1. **Watermarker**. En fonction de vos besoins, le fichier peut être fourni sous forme de flux ou de référence à un emplacement de disque local.
      2. **SearchCriteria** pour identifier les filigranes spécifiques nécessitant une modification. Cet objet permet de localiser les filigranes en fonction des propriétés souhaitées.
      3. Une fois la recherche exécutée avec succès, vous recevrez une collection de filigranes pertinents. Ces filigranes offrent un contrôle granulaire, vous permettant de mettre à jour des propriétés telles que les dimensions, le positionnement des pages, le contenu du texte, la palette de couleurs, les données d'image, etc.
      4. Une fois les mises à jour des filigranes terminées, conservez le document modifié. L'API facilite le stockage à l'aide d'un chemin de fichier local ou d'un objet de flux.
   
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

        // Mettre à jour le filigrane de texte WORD

        // Fournir une instance de filigrane pour le fichier WORD
        const watermarker = new groupdocs.watermark.Watermarker("input.docx");

        // Utilisez TextSearchCriteria pour rechercher des filigranes de texte
        const searchCriteria = 
            new groupdocs.watermark.TextSearchCriteria("test", false);
        const watermarks = watermarker.search(searchCriteria);
        
        // Mettre à jour le filigrane de texte
        for (const watermark of watermarks.getInnerList().toArray())
        {
            watermark.setText("passed");
        }

        // Profitez du résultat
        watermarker.save("output.docx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Maîtriser l'édition de filigranes en PDF s avec GroupDocs.Watermark"
  description: "Explorez les fonctionnalités complètes de l'API pour ajuster et gérer les filigranes dans PDF s au sein de Node.js via Java applications."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Modifier le filigrane"
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
    - title: "Java Exemple : Modifier le filigrane PDF"
      content: |
        Cet exemple Java montre comment modifier un filigrane existant dans un document PDF, en montrant comment ajuster ses propriétés par programmation.
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Chargez le document PDF pour traitement
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  Recherchez des filigranes spécifiques qui répondent à vos critères
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria("test", false);
            const watermarks = watermarker.search(searchCriteria);
  
            //  Modifier les paramètres du filigrane, tels que la taille, la couleur et la position
            for (const watermark of watermarks.getInnerList().toArray()) {
                watermark.getFormattedTextFragments().clear();
                watermark.getFormattedTextFragments().add("passed", 
                    new groupdocsWatermark.Font("Calibri", 19, groupdocsWatermark.FontStyle.Bold), 
                    groupdocsWatermark.Color.getRed(), groupdocsWatermark.Color.getAqua());
            }

            //  Enregistrez le document mis à jour sur un système local ou diffusez-le directement
            watermarker.save("result.pdf");
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
    title: "Mettre à jour les filigranes dans d'autres formats de fichiers"
    exclude: "WORD"
    description: "Simplifiez l'édition des filigranes dans PDF, Word, Excel, et plus encore avec GroupDocs.Watermark for Node.js via Java. Tous les formats professionnels courants sont pris en charge."
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