
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:27:01
draft: false
lang: fr
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "API Node.js via Java pour la suppression des filigranes Excel"
head_description: "Intégrez des fonctionnalités de suppression des filigranes dans les fichiers Excel grâce à notre API Node.js via Java, améliorant ainsi la clarté des documents et la présentation des données."

############################# Header ############################
title: "Node.js via Java API pour la gestion des filigranes Excel" 
description: "Utilisez l'API GroupDocs.Watermark for Node.js via Java pour supprimer ou modifier les filigranes dans Excel documents, ce qui est idéal pour garantir des fiches techniques propres dans les flux de travail automatisés."
subtitle: "GroupDocs.Watermark for Node.js via Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Téléchargement gratuit sur NPM"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java bibliothèque"
    link: "/watermark/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       La bibliothèque GroupDocs.Watermark for Node.js via Java simplifie la gestion des filigranes dans les fichiers Excel, permettant aux développeurs de supprimer, d'ajuster ou d'effacer complètement les filigranes. Cet outil est essentiel pour préserver l'intégrité et la présentation des données financières et analytiques dans Excel feuilles, prenant en charge divers processus métier.

############################# Steps ############################
steps:
    enable: true
    title: "Excel Suppression des filigranes à l'aide de Node.js via Java"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/nodejs-java/)** fournit à Node.js via Java développeurs une API complète pour la suppression par programmation de filigranes spécifiques intégrés dans divers Excel documents. Ce guide aborde le processus technique :
      
      1. **Watermarker** et en fournissant votre fichier Excel comme argument constructeur. Le fichier peut être fourni sous la forme d'un flux d'octets, d'un flux de fichiers ou d'une référence de chemin vers un emplacement de disque local.
      2. **SearchCriteria**. Cet objet facilite la construction de filtres complexes basés sur des propriétés précédemment intégrées dans le document. Vous pouvez utiliser une image comme paramètre de recherche à côté du texte ou des attributs de mise en forme pour permettre un processus de sélection très précis.
      3. Après l'exécution de la recherche, vous recevrez une collection de filigranes identifiés. Ces filigranes peuvent être supprimés facilement.
      4. Une fois le filigrane supprimé, conservez le document modifié. L'API offre une flexibilité de stockage, vous permettant d'utiliser soit un chemin de fichier local, soit un objet de flux pour la sortie finale.
   
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

        // Supprimer le filigrane de texte dans le document Excel

        // Instanciez un filigrane avec le document Excel
        const watermarker = new groupdocs.watermark.Watermarker("input.xslx");
        
        // Les filigranes en texte clair conviennent aux conditions de recherche
        const criteria = new groupdocs.watermark.TextFormattingSearchCriteria();
        criteria.setFontBold(true);
        const watermarks = watermarker.search(criteria);
        watermarks.clear();

        // Enregistrer le fichier traité
        watermarker.save("output.xslx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Node.js via Java API pour une suppression efficace des filigranes"
  description: "Tirez parti de notre API Node.js via Java pour supprimer ou effacer facilement les filigranes de divers formats de documents, y compris les PDF et les fichiers Office. Conçue pour les développeurs, cette API s'intègre facilement à vos applications Node.js via Java, garantissant ainsi des documents propres et clairs."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "Supprimer le filigrane"
  features:
    # feature loop
    - title: "Node.js via Java Suppression du filigrane"
      content: "Utilisez notre API Node.js via Java pour supprimer les filigranes avec précision et facilité. Parfait pour les demandes nécessitant des documents non marqués à des fins de présentation ou de traitement ultérieur."

    # feature loop
    - title: "Traitement de suppression des filigranes par lots"
      content: "Gérez efficacement plusieurs documents grâce à notre fonction de suppression en masse des filigranes. Économisez du temps et des ressources serveur en traitant de grands lots de fichiers simultanément dans vos Node.js via Java applications."

    # feature loop
    - title: "Modifier et supprimer les filigranes de manière flexible"
      content: "Notre API permet de modifier et de supprimer de manière flexible les éléments de filigrane, répondant ainsi à divers besoins commerciaux et types de documents. Adaptez vos documents pour conserver une apparence professionnelle tout en garantissant l'intégrité du contenu."
      
  code_samples:
    # code sample loop
    - title: "Supprimer les filigranes de liens hypertextes PDF"
      content: |
        Cet exemple montre comment supprimer tous les filigranes à l'aide d'un lien hypertexte approprié depuis un fichier PDF
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Charger PDF dans Watermarker
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  Rechercher des filigranes à l'aide d'un hyperlien
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria('someurl.com');
            const watermarks = watermarker.search(searchCriteria);
  
            //  Supprimer les filigranes sélectionnés
            for (let i = watermarks.getCount() - 1; i >= 0; i--) {
                if (watermarks.get_Item(i) instanceof groupdocsWatermark.HyperlinkPossibleWatermark) {
                    console.log(watermarks.get_Item(i).getText());
                    watermarks.removeAt(i);
                }
            }

            //  Enregistrer les modifications dans le document
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
    title: "Améliorer Excel fichiers avec Node.js via Java"
    exclude: "EXCEL"
    description: "Découvrez comment l'API GroupDocs.Watermark for Node.js via Java peut vous aider à gérer et à supprimer les filigranes des documents Excel, en garantissant une visibilité totale des données et une esthétique professionnelle des documents."
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