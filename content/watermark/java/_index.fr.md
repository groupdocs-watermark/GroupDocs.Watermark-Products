---
############################# Static ############################
layout: "landing"
date: 2024-04-29T14:27:12
draft: false

lang: fr
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

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
head_title: "Java Bibliothèque de filigranes | ajouter des filigranes aux documents"
head_description: "Logiciel natif Java pour ajouter et manipuler du texte et des filigranes d'images dans les fichiers PDF, Word, Excel, présentations, Visio diagrammes, e-mails et fichiers d'images."

############################# Header ############################
title: "Implémentez facilement le filigrane des documents dans Java projets"
description: "Améliorez vos applications Java avec la possibilité de filigraner les fichiers à l'aide de la bibliothèque GroupDocs.Watermark. Notre API propose des filigranes personnalisables pour un large éventail de formats de fichiers courants."
words:
  for: "pour"

actions:
  main: "Téléchargement gratuit depuis Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "Licences"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java/"
  title: "Prêt à démarrer ?"
  description: "Essayez GroupDocs.Watermark fonctionnalités gratuitement ou demandez une licence"

release:
  title: "Version {0} publiée"
  notes: "Découvrez les nouveautés"
  downloads: "Téléchargements"

code:
  title: "Filigrane PDF via Java"
  more: "Plus d'exemples"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-watermark</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Instanciez un filigrane en passant le chemin PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Personnalisez les options de filigrane
    TextWatermark textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Appliquer un filigrane au document PDF
    watermarker.add(textWatermark);

    // Enregistrer le document de résultats
    watermarker.save("result.pdf");
    watermarker.close();
      
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark en un coup d'œil"
  description: "Bibliothèque conçue pour ajouter des filigranes à l'aide des technologies Java"
  features:
    # feature loop
    - title: "Filigrane des fichiers via Java"
      content: "Protégez vos documents professionnels à l'aide de GroupDocs.Watermark for Java. Ajoutez du texte, des images, des diagrammes ou des pièces jointes à des e-mails sous forme de filigranes à différents formats de fichiers."

    # feature loop
    - title: "Personnalisez les filigranes en fonction de besoins spécifiques"
      content: "GroupDocs.Watermark for Java propose de nombreuses options de personnalisation pour les filigranes. Ajustez les styles de texte (gras, italique, police) et les propriétés de l'image (rotation, etc.) pour adapter le processus de filigrane à vos objectifs spécifiques."

    # feature loop
    - title: "Prise en charge de formats étendus"
      content: "GroupDocs.Watermark for Java s'intègre parfaitement à un large éventail de formats de fichiers, notamment : PDF, Microsoft Office (Word, Excel, PowerPoint), images (JPEG, PNG, GIF, BMP), Visio diagrammes et e-mails. Améliorez la sécurité des documents pour différents types de fichiers."

    # feature loop
    - title: "Recherche et gestion de filigranes en toute simplicité"
      content: "Gérez efficacement les filigranes existants dans les documents. Localisez des filigranes spécifiques, modifiez leur texte, leur style ou leurs images, ou supprimez-les complètement. GroupDocs.Watermark for Java simplifie le flux de travail de filigrane."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indépendance de la plateforme"
  description: "GroupDocs.Watermark for Java prend en charge différents systèmes d'exploitation et gestionnaires de packages."
  items:
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Formats de fichiers pris en charge"
  description: |
    GroupDocs.Watermark for Java permet de traiter un large éventail de formats de fichiers. [Voir la liste complète](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Java : Caractéristiques"
  description: "Protégez vos fichiers en ajoutant des filigranes. Supporte différents formats, notamment PDF, les documents Office et les images."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Filigrane de fichiers"
      content: "Ajoutez ou supprimez des filigranes à des sections spécifiques ou à des documents entiers pour les différents formats de fichiers pris en charge."

    # feature loop
    - icon: "watermark_style"
      title: "Personnalisation du filigrane"
      content: "Personnalisez l'apparence de votre filigrane avec des options telles que la couleur, la police, la rotation, etc."

    # feature loop
    - icon: "hidden_print"
      title: "Filigrane d'impression masqué pour PDF"
      content: "Ajoutez un filigrane qui n'apparaît que lors de l'impression d'un document PDF."

    # feature loop
    - icon: "image_only"
      title: "Filigrane d'image sélectif"
      content: "Ajoutez un filigrane à toutes les images d'une section, d'une page, d'une diapositive ou d'un document entier en particulier."

    # feature loop
    - icon: "image_frame"
      title: "Filigrane de cadres d'image spécifiques"
      content: "Appliquez des filigranes à des cadres spécifiques d'une image comportant plusieurs cadres."

    # feature loop
    - icon: "attachments"
      title: "Pièces jointes et formes de filigrane"
      content: "Ajoutez des filigranes à toutes les pièces jointes des documents Excel ou à toutes les formes d'image des présentations."

    # feature loop
    - icon: "pdf_objects"
      title: "Alignement des filigranes dans PDF"
      content: "Alignez les filigranes sur différentes zones d'un document PDF, notamment Bleed Box, Art Box, Crop Box et Trim Box."

    # feature loop
    - icon: "doc_background"
      title: "Filigrane par images d'arrière-plan"
      content: "Ajoutez ou supprimez un filigrane d'image d'arrière-plan à des feuilles de calcul ou à des présentations."

    # feature loop
    - icon: "unreadable_characters"
      title: "Protection contre les caractères illisibles"
      content: "Protégez les présentations à l'aide d'un filigrane textuel contenant des caractères illisibles."

    # feature loop
    - icon: "watermark_text_search"
      title: "Rechercher des filigranes"
      content: "Obtenez la liste des filigranes présentés dans un fichier, en utilisant divers paramètres, y compris des expressions régulières."

    # feature loop
    - icon: "watermark_image_search"
      title: "Rechercher des filigranes d'images similaires"
      content: "Localisez les filigranes qui ressemblent à une image spécifique."

    # feature loop
    - icon: "document_info"
      title: "Extraire les informations du document"
      content: "Obtenez diverses données de document, telles que la mise en page pour les formats de fichiers pris en charge."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de code"
  description: "Explorez des exemples de code illustrant les fonctionnalités typiques de GroupDocs.Watermark for Java"
  items:
    # code sample loop
    - title: "Ajouter un filigrane à un document à l'aide d'une image"
      content: |
        Utilisez GroupDocs.Watermark for Java pour améliorer la sécurité des documents en ajoutant des filigranes d'image. Pour en savoir plus : [Filigranes d'image](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Comment protéger un fichier par filigrane d'image.">}}
        ```csharp {style=abap}
        // Charger le document source dans Watermarker
        Watermarker watermarker = new Watermarker("document.pdf");
        
        // Spécifier le chemin d'accès à une image en filigrane
        ImageWatermark watermark = new ImageWatermark("watermark.jpg");

        // Protégez le fichier et enregistrez-le
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Modifier les filigranes"
      content: |
        GroupDocs.Watermark for Java vous permet de gérer les filigranes existants dans les documents. Localisez des filigranes spécifiques et [modifiez leurs propriétés](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Recherche et modification de filigranes.">}}
        ```csharp {style=abap}   
        // Charger le document source
        Watermarker watermarker = new Watermarker("document.pdf");

        // Rechercher les filigranes à mettre à jour
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);                               
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);                             

        // Mettre à jour les propriétés souhaitées
        for (PossibleWatermark watermark : watermarks)                                                           
        {  
            watermark.setText("New Text");
        }

        // Enregistrer le document modifié dans un chemin spécifié
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
