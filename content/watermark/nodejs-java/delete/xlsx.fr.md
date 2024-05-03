
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:18
draft: false
lang: fr
format: Xlsx
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Suppression automatique du filigrane XLSX"
head_description: "Simplifiez les flux de travail de XLSX documents grâce à la suppression automatique des filigranes GroupDocs.Watermark."

############################# Header ############################
title: "Automatisez la suppression du filigrane XLSX" 
description: "Configurez des processus automatisés pour supprimer efficacement les filigranes avec GroupDocs.Watermark."
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "NPM Télécharger"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       Pour les flux de documents répétitifs, GroupDocs.Watermark propose des fonctionnalités de suppression automatique des filigranes. Les développeurs peuvent intégrer cette fonctionnalité pour rationaliser le traitement des documents en supprimant automatiquement les filigranes lors du téléchargement, de la conversion ou d'autres déclencheurs désignés. Améliorez l'efficacité et réduisez les interventions manuelles grâce à la suppression automatique des filigranes à l'aide de GroupDocs.Watermark.

############################# Steps ############################
steps:
    enable: true
    title: "Supprimez sans effort les filigranes de Xlsx par Node.js via Java"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/nodejs-java/)** rationalise le processus de suppression des filigranes des documents professionnels. Améliorez votre application Node.js via Java en intégrant de manière transparente notre bibliothèque et en suivant ces étapes simples :
      
      1. Lancez le processus en instanciant la classe principale, **Watermarker**, avec le document Xlsx. Notre API polyvalente traite de manière transparente les documents, qu'ils soient fournis sous forme de flux ou de chemin local.
      2. Tirez parti de **SearchCriteria** pour identifier précisément les filigranes à traiter. Utilisez divers paramètres tels que les images, le texte ou les fonctionnalités de formatage pour affiner votre recherche. Plus vos critères sont détaillés, plus vos résultats sont précis.
      3. Exécutez le processus de suppression sur la liste des filigranes de documents récupérés grâce à votre recherche. Supprimez-les sans effort du document.
      4. Une fois les filigranes supprimés avec succès, enregistrez en toute sécurité le document résultant en tant que fichier local ou flux d'octets, en préservant son intégrité.
   
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

        // Supprimer le filigrane de l'image dans le document XLSX

        // Obtenez Watermarker en passant le chemin XLSX comme argument
        const watermarker = new groupdocs.watermark.Watermarker("input.xlsx");
        
        // Effacer les filigranes d'image par critères de recherche
        const searchCriteria = 
            new groupdocs.watermark.ImageDctHashSearchCriteria("logo.png");
        const watermarks = watermarker.search(searchCriteria);
        watermarks.clear();

        // Enregistrer le fichier traité
        watermarker.save("output.xlsx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Node.js via Java API pour la suppression des filigranes | GroupDocs.Watermark"
  description: "Intégrez notre API Node.js via Java pour supprimer facilement les filigranes des documents, améliorant ainsi la clarté et l'esthétique des documents. Conçue pour les environnements Node.js via Java, cette API est idéale pour les applications qui ont besoin de traiter et de présenter des documents propres et exempts de filigranes."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "Supprimer le filigrane"
  features:
    # feature loop
    - title: "Suppression simplifiée des filigranes pour Node.js via Java"
      content: "Notre API propose des outils rationalisés de suppression des filigranes conçus spécifiquement pour Node.js via Java applications, permettant aux développeurs d'améliorer la lisibilité des documents et leur apparence professionnelle sans codage complexe."

    # feature loop
    - title: "Node.js via Java Nettoyage des filigranes par lots"
      content: "Tirez parti de la possibilité d'effacer les filigranes de plusieurs documents en une seule fois grâce à notre fonction de traitement par lots. Cela est particulièrement utile pour les applications qui doivent gérer des flux de documents volumineux rapidement et efficacement."

    # feature loop
    - title: "Édition flexible des filigranes via Node.js via Java"
      content: "Ajustez, modifiez ou supprimez complètement les filigranes à l'aide de nos outils d'édition flexibles. Cette fonctionnalité permet à Node.js via Java développeurs d'adapter le traitement des documents aux besoins spécifiques de l'entreprise ou aux demandes des clients, afin de garantir des résultats optimaux."
      
  code_samples:
    # code sample loop
    - title: "Supprimer les filigranes d'en-tête de feuille de calcul"
      content: |
        Cet exemple montre comment supprimer les filigranes placés dans les en-têtes XLSX
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Charger un classeur
            const loadOptions = new groupdocsWatermark.SpreadsheetLoadOptions();
            const watermarker = new groupdocsWatermark.Watermarker("source.xlsx", loadOptions);

            //  Obtenir la liste des sections d'en-tête
            const content = watermarker.getContent(groupdocsWatermark.SpreadsheetContent.class);
            const sections = content.getWorksheets().get_Item(0).getHeadersFooters()
                .getByOfficeHeaderFooterType(groupdocsWatermark.OfficeHeaderFooterType.HeaderPrimary).getSections();
  
            //  Supprimer les filigranes des en-têtes
            for (const section of sections.getInnerList().toArray()) {
                section.setScript(null);
                section.setImage(null);
            }

            //  Enregistrer le classeur effacé
            watermarker.save("result.xlsx");
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
    title: "Automatisez la suppression dans plusieurs formats"
    exclude: "XLSX"
    description: "Planifiez la suppression automatique des filigranes pour différents types de documents avec GroupDocs.Watermark."
    items: 
        # format loop 1
        - name: "Filigrane PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/delete//pdf/"
          description: "Format de document Adobe Portable"

        # format loop 2
        - name: "Filigrane Word"
          format: "WORD"
          link: "/watermark/nodejs-java/delete//word/"
          description: "MS Word et documents Open Office"
          
        # format loop 3
        - name: "Filigrane Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/delete//excel/"
          description: "MS Excel et feuilles de calcul Open Office"

        # format loop 4
        - name: "Filigrane PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/delete//powerpoint/"
          description: "MS PowerPoint et présentations Open Office"

        # format loop 5
        - name: "Filigrane DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/delete//docx/"
          description: "Microsoft Word Ouvrir un document XML"
          
        # format loop 6
        - name: "Filigrane PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/delete//pptx/"
          description: "PowerPoint Présentation Open XML"
          
        # format loop 7
        - name: "Filigrane XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/delete//xlsx/"
          description: "Feuille de calcul Microsoft Excel Open XML"

        # format loop 8
        - name: "Filigrane DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/delete//doc/"
          description: "Microsoft Word 97 - 2007 Documento"

        # format loop 9
        - name: "Filigrane XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/delete//xls/"
          description: "Classeur Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrane PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/delete//ppt/"
          description: "PowerPoint Présentation 97-2003"

        # format loop 11
        - name: "Filigrane RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/delete//rtf/"
          description: "Format de texte enrichi"

---