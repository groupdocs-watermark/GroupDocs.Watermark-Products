
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:59
draft: false
lang: fr
format: Image
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Filigrane dynamique pour la protection des images"
head_description: "Protégez les droits d'auteur de vos images avec le filigrane dynamique Node.js. Supporte JPG, PNG, WEBP et plus encore."

############################# Header ############################
title: "Filigrane dynamique pour la protection des images avec Node.js" 
description: "Utilisez notre boîte à outils Node.js pour générer des filigranes dynamiques et sécurisés sur vos images, en prenant en charge des formats tels que JPG, PNG et WEBP. Garantissez les droits d'auteur de vos images grâce à des fonctionnalités de protection avancées."
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
    title: "GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       Avec GroupDocs.Watermark for Node.js via Java, l'application de filigranes aux images est simple et personnalisable. Cette boîte à outils prend en charge un large éventail de formats d'image, y compris les images matricielles traditionnelles telles que JPG et PNG, ainsi que des formats plus récents tels que WEBP. Il permet aux développeurs d'ajouter dynamiquement des filigranes qui sont non seulement sécurisés, mais qui se fondent également naturellement dans le contenu de l'image, offrant ainsi une protection robuste contre les violations du droit d'auteur sans nuire à l'attrait original de l'image.

############################# Steps ############################
steps:
    enable: true
    title: "Documents commerciaux sécurisés : générez des filigranes pour les formats Image"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/) :** Injectez notre API dans vos applications et générez des filigranes pour de nombreux formats de fichiers pris en charge.
      
      1. **Lancer le filigrane :** Démarrez le traitement des documents avec la classe **Watermarker** fournissant nos principales fonctionnalités. Instanciez-le en passant au constructeur le fichier Image qui est censé être sécurisé par des filigranes générés.
      2. **Créez un objet filigrane principal :** Améliorez vos documents en sculptant des objets **Filigrane** sur mesure. Au-delà de simples pages, ils s'intègrent parfaitement aux éléments natifs tels que les pièces jointes ou les en-têtes, ajoutant ainsi des niveaux de sécurité et de professionnalisme.
      3. **Affiner les attributs des filigranes :** Affinez vos filigranes avec précision, en ajustant les dimensions, l'alignement et les combinaisons de couleurs. Chaque détail améliore l'intégrité des documents, faisant de vos fichiers les vôtres sans aucun doute.
      4. **Implémentez avec précision :** Utilisez la méthode **Watermarker** pour appliquer parfaitement vos filigranes personnalisés. Qu'il soit unique ou multiple, chaque filigrane ajoute une couche de protection supplémentaire. Pour plus de sécurité, pensez à stocker vos documents traités dans un endroit distinct et sécurisé.
   
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

        // Générer un filigrane de texte pour IMAGE

        // Transmettre le fichier source à l'instance Watermarker
        const watermarker = new groupdocs.watermark.Watermarker("input.jpeg");
        
        // Générez un filigrane de texte et définissez ses options
        const  watermark = new groupdocs.watermark.TextWatermark
            ("My Watermark", groupdocs.watermark.new Font("Arial", 36));

        // Obtenir le résultat IMAGE
        watermarker.add(watermark);
        watermarker.save("output.jpeg");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Techniques de filigrane avancées"
  description: "Découvrez des techniques de filigrane de pointe grâce à notre API robuste, conçue pour s'intégrer parfaitement dans .NET environnements. Parfait pour ajouter des filigranes sophistiqués et sécurisés à un large éventail de types de documents, notamment des présentations, des documents juridiques et des diagrammes techniques."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Filigrane sophistiqué"
  features:
    # feature loop
    - title: "Placement dynamique des filigranes"
      content: "Notre API propose des options de placement dynamiques qui adaptent le positionnement des filigranes en fonction du contenu du document. Idéale pour les mises en page complexes dans les présentations et les diagrammes techniques, cette fonctionnalité garantit que les filigranes sont toujours placés de manière optimale sans nuire à la lisibilité des informations sous-jacentes."

    # feature loop
    - title: "Sécurité renforcée grâce à des filigranes invisibles"
      content: "Implémentez des filigranes invisibles qui offrent une protection robuste sans altérer l'apparence de vos documents. Ces filigranes sont conçus pour être détectés uniquement par le biais d'outils logiciels spécifiques, ce qui les rend parfaits pour protéger les informations sensibles contenues dans les documents juridiques et financiers."

    # feature loop
    - title: "Flux de travail de filigrane automatisés"
      content: "Rationalisez vos processus de sécurité des documents grâce à des flux de travail de filigrane automatisés. Configurez des règles en fonction du type de document, de la sensibilité du contenu et des niveaux d'accès des utilisateurs pour appliquer automatiquement des filigranes, garantissant ainsi la cohérence des protocoles de sécurité sur tous les documents."
      
  code_samples:
    # code sample loop
    - title: "Générer un filigrane pour PDF pièces jointes"
      content: |
        Cet exemple montre comment générer des filigranes dans toutes les pièces jointes PDF
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Charger le document PDF
            const loadOptions = new groupdocsWatermark.PdfLoadOptions();
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf", loadOptions);
            const pdfContent = watermarker.getContent(groupdocsWatermark.PdfContent.class);

            //  Générer un filigrane de texte
            const watermark = new groupdocsWatermark.TextWatermark('WaterMark', new groupdocsWatermark.Font('Arial', 19));
  
            //  Ajouter un filigrane aux pièces jointes appropriées
            for (const attachment of pdfContent.getAttachments().getInnerList().toArray()) {
                const info = attachment.getDocumentInfo();
                if (info.getFileType() !== groupdocsWatermark.FileType.Unknown && !info.isEncrypted()) {
                    const attachedWatermarker = attachment.createWatermarker();
                    attachedWatermarker.add(watermark);
                    attachment.updateContent(attachedWatermarker);
                    attachedWatermarker.close();
                }
            }

            //  Sauvegarde traitée PDF
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
    title: "Implémentation de superbes filigranes dans les images via JavaScript"
    exclude: "IMAGE"
    description: "Protégez efficacement les droits d'auteur de vos images grâce à notre API Node.js. Ajoutez dynamiquement des filigranes aux fichiers JPG, PNG et WEBP, en vous assurant que chaque image est marquée pour son propriétaire légitime."
    items: 
        # format loop 1
        - name: "Filigrane PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/generate//pdf/"
          description: "Format de document Adobe Portable"

        # format loop 2
        - name: "Filigrane Word"
          format: "WORD"
          link: "/watermark/nodejs-java/generate//word/"
          description: "MS Word et documents Open Office"
          
        # format loop 3
        - name: "Filigrane Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/generate//excel/"
          description: "MS Excel et feuilles de calcul Open Office"

        # format loop 4
        - name: "Image en filigrane"
          format: "IMAGE"
          link: "/watermark/nodejs-java/generate//image/"
          description: "Formats d'image populaires"

        # format loop 5
        - name: "Photo en filigrane"
          format: "PHOTO"
          link: "/watermark/nodejs-java/generate//photo/"
          description: "Formats de photos"

        # format loop 6
        - name: "Filigrane PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/generate//powerpoint/"
          description: "MS PowerPoint et présentations Open Office"

        # format loop 7
        - name: "Filigrane DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/generate//docx/"
          description: "Microsoft Word Ouvrir un document XML"
          
        # format loop 8
        - name: "Filigrane PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/generate//pptx/"
          description: "PowerPoint Présentation Open XML"
          
        # format loop 9
        - name: "Filigrane XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/generate//xlsx/"
          description: "Feuille de calcul Microsoft Excel Open XML"

        # format loop 10
        - name: "Filigrane JPEG"
          format: "JPEG"
          link: "/watermark/nodejs-java/generate//jpeg/"
          description: "JPEG Photo"

        # format loop 11
        - name: "Filigrane PNG"
          format: "PNG"
          link: "/watermark/nodejs-java/generate//png/"
          description: "Portable Graphique du réseau"

        # format loop 12
        - name: "Filigrane TIFF"
          format: "TIFF"
          link: "/watermark/nodejs-java/generate//tiff/"
          description: "Format de fichier d'image de balise"

        # format loop 13
        - name: "Filigrane WEBP"
          format: "WEBP"
          link: "/watermark/nodejs-java/generate//webp/"
          description: "Photo WEB"

        # format loop 14
        - name: "Filigrane DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/generate//doc/"
          description: "Microsoft Word 97 - 2007 Documento"

        # format loop 15
        - name: "Filigrane XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/generate//xls/"
          description: "Classeur Microsoft Excel 97-2003"

        # format loop 16
        - name: "Filigrane PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/generate//ppt/"
          description: "PowerPoint Présentation 97-2003"

        # format loop 17
        - name: "Filigrane RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/generate//rtf/"
          description: "Format de texte enrichi"

---