---
############################# Static ############################
layout: "landing"
date: 2024-04-26T21:39:08
draft: false

lang: fr
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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

############################# Head ############################
head_title: "Bibliothèque de filigranes Node.js | filigranes de documents"
head_description: "La solution Node.js protège les documents professionnels avec des filigranes de texte et d'image. Les formats courants tels que PDF, Word, Excel, PowerPoint sont pris en charge."

############################# Header ############################
title: "Accès à la technologie de filigrane dans Node.js via les solutions Java"
description: "Protégez votre propriété intellectuelle et empêchez toute copie non autorisée grâce à cette solution Node.js. Il permet aux utilisateurs d'ajouter facilement des filigranes à des documents commerciaux dans différents formats, notamment PDF, Word, Excel, PowerPoint, images, etc."
words:
  for: "pour"

actions:
  main: "Utilisez NPM pour télécharger gratuitement"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.watermark"
  alt: "Licences"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
  title: "Prêt à démarrer ?"
  description: "Essayez GroupDocs.Watermark fonctionnalités gratuitement ou demandez une licence"

release:
  title: "Version {0} publiée"
  notes: "Découvrez les nouveautés"
  downloads: "Téléchargements"
  link: "https://releases.groupdocs.com/watermark/nodejs-java/"

code:
  title: "Ajouter un filigrane à PDF avec TypeScript"
  more: "Plus d'exemples"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.watermarker"
  content: |
    ```javascript {style=abap}

    // Instanciez un filigrane en passant le chemin PDF
    let loadOptions = new PdfLoadOptions();
    let watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Personnalisez les options de filigrane
    let textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Appliquer un filigrane au document PDF
    watermarker.add(textWatermark);

    // Enregistrer le document de résultats
    watermarker.save("result.pdf");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark en un coup d'œil"
  description: "Bibliothèque TypeScript Node.js pour le filigrane"
  features:
    # feature loop
    - title: "Filigrane du fichier Node.js"
      content: "Protégez vos documents professionnels avec GroupDocs.Watermark for Node.js via Java. Ajoutez du texte, des images, des diagrammes ou des pièces jointes à des e-mails sous forme de filigranes à différents formats de fichiers."

    # feature loop
    - title: "Personnalisez les filigranes selon vos besoins"
      content: "GroupDocs.Watermark for Node.js via Java propose de nombreuses options de personnalisation pour les filigranes. Ajustez les styles de texte (gras, italique, police) et les propriétés de l'image (rotation, etc.) pour personnaliser le traitement des documents."

    # feature loop
    - title: "Prise en charge complète des formats"
      content: "GroupDocs.Watermark for Node.js via Java s'intègre parfaitement à un large éventail de formats de fichiers, notamment : PDF, MS Office comme Word, Excel, PowerPoint, images telles que JPEG, PNG, GIF, BMP, Visio diagrammes, e-mails, etc. Renforcez le traitement des documents pour atteindre vos objectifs commerciaux."

    # feature loop
    - title: "Recherche et mise à jour puissantes de filigranes"
      content: "Obtenez et mettez à jour les filigranes existants dans les documents filigranés. Modifiez le texte, le style, le contenu de l'image ou supprimez-les complètement. GroupDocs.Watermark for Node.js via Java fournit une large gamme de traitements des filigranes."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indépendance de la plateforme"
  description: "GroupDocs.Watermark for Node.js via Java s'intègre facilement à divers systèmes d'exploitation et gestionnaires de packages."
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
    GroupDocs.Watermark for Node.js via Java vous permet de traiter un large éventail de formats de fichiers. [Explorez la liste complète](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Node.js via Java : Ensemble de fonctionnalités"
  description: "Renforcez la sécurité des documents grâce au filigrane programmatique. Supporte divers formats de fichiers, notamment : PDF, DOCX, XLSX, PPTX et les formats d'image (PNG, JPG, etc.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Contrôle précis du filigrane"
      content: "Manipulez avec précision les filigranes en les ajoutant ou en les supprimant dans des sections spécifiques, des documents entiers ou des pièces jointes et des formes individuelles dans différents formats de fichiers."

    # feature loop
    - icon: "watermark_style"
      title: "Personnalisation de l'apparence du filigrane"
      content: "Contrôlez avec précision l'esthétique des filigranes en modifiant des attributs tels que la couleur, la police, l'opacité, la rotation et le positionnement dans le document."

    # feature loop
    - icon: "hidden_print"
      title: "Imprimer PDF Filigrane"
      content: "Déployez un filigrane furtif qui reste invisible lors de l'affichage normal des documents mais qui n'apparaît que pendant le processus d'impression, renforçant ainsi la sécurité des documents en toute discrétion."

    # feature loop
    - icon: "image_only"
      title: "Filigrane d'image spécifique"
      content: "Ajoutez un filigrane à des images spécifiques dans un document à l'aide de notre solution. Choisissez d'intégrer des filigranes dans une section spécifique (par exemple, page, diapositive) ou dans l'ensemble du document."

    # feature loop
    - icon: "image_frame"
      title: "Filigrane d'images à plusieurs images"
      content: "Appliquez des filigranes de manière sélective à des images spécifiques dans un format d'image à plusieurs images, garantissant ainsi un contrôle précis du placement des filigranes."

    # feature loop
    - icon: "attachments"
      title: "Protection complète du contenu"
      content: "Étendez la protection à divers éléments du document, tels que les pièces jointes dans Excel documents et les formes d'image dans les présentations, afin d'apporter un niveau de sécurité supplémentaire."

    # feature loop
    - icon: "pdf_objects"
      title: "Filigrane avancé dans PDF"
      content: "Ajoutez un filigrane à différentes zones de PDF s, notamment la Bleed Box, la Art Box, la Crop Box, la Trim Box, etc."

    # feature loop
    - icon: "doc_background"
      title: "Filigrane d'image d'arrière-plan"
      content: "Gérez les filigranes dans les images d'arrière-plan des feuilles de calcul et des présentations, en offrant des options de personnalisation supplémentaires pour les mesures de sécurité visuelle."

    # feature loop
    - icon: "unreadable_characters"
      title: "Filigrane de texte avec caractères illisibles"
      content: "Utilisez des caractères illisibles dans les filigranes de texte intégrés dans les présentations, afin de renforcer la sécurité en compliquant considérablement l'extraction non autorisée de filigranes."

    # feature loop
    - icon: "watermark_text_search"
      title: "Recherche avancée de filigranes"
      content: "Utilisez des fonctionnalités de recherche complètes pour localiser les filigranes dans les documents en fonction de paramètres spécifiques ou en combinant différents critères, ce qui permet une récupération et une gestion efficaces."

    # feature loop
    - icon: "watermark_image_search"
      title: "Détection de filigranes d'images similaires"
      content: "Trouvez des filigranes similaires dans des documents qui ressemblent visuellement à une image source."

    # feature loop
    - icon: "document_info"
      title: "Extraction programmatique d'informations sur les documents"
      content: "Extrayez des métadonnées importantes par programmation, y compris les détails de mise en page et d'autres informations sur les documents pour les formats de fichiers pris en charge."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de code"
  description: "Découvrez des exemples de code présentant les fonctionnalités courantes de GroupDocs.Watermark for Node.js via Java"
  items:
    # code sample loop
    - title: "Ajouter une image à un document en filigrane"
      content: |
        Tirez parti de GroupDocs.Watermark for Node.js via Java pour améliorer la sécurité des documents en ajoutant des filigranes d'image. Pour en savoir plus : [Filigranes d'image](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Comment protéger un fichier par filigrane d'image.">}}
        ```javascript {style=abap}
        // Charger le document source dans Watermarker
        let watermarker = new Watermarker("document.pdf");
        
        // Spécifier le chemin d'accès à une image en filigrane
        let watermark = new ImageWatermark("watermark.jpg");

        // Protégez le fichier et enregistrez-le
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Rechercher et modifier des filigranes existants"
      content: |
        GroupDocs.Watermark for Node.js via Java vous permet de gérer les filigranes des documents. Sélectionnez les filigranes, modifiez leurs propriétés. Découvrez comment : [Modifier les filigranes](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Recherche et modification de filigranes.">}}
        ```javascript {style=abap}   
        // Charger le document source
        let watermarker = new Watermarker("document.pdf");

        // Rechercher les filigranes à mettre à jour
        let searchCriteria = new TextSearchCriteria("test", false);                               
        let watermarks = watermarker.search(searchCriteria); 

        // Mettre à jour les propriétés souhaitées
        watermarks.forEach((watermark)
        {  
            watermark.setText("New Text");
        }

        // Enregistrer le document modifié dans un chemin spécifié
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
