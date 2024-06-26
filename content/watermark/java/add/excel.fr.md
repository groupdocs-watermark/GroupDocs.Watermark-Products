
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:17
draft: false
lang: fr
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Générer un filigrane dans Excel feuilles de calcul pour Java"
head_description: "Implémentez facilement la génération de filigranes de texte et d'image dans Excel avec Java pour protéger vos feuilles de calcul de données Excel"

############################# Header ############################
title: "Automatisez le filigrane Excel avec le code Java" 
description: "Implémentez des filigranes de texte ou d'image personnalisés dans Excel feuilles de calcul à l'aide de Java. Ce guide propose des instructions étape par étape pour améliorer la sécurité des documents et l'image de marque, adaptées à divers besoins professionnels."
subtitle: "GroupDocs.Watermark for Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Téléchargement gratuit Maven"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java bibliothèque"
    link: "/watermark/java/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java propose une gestion complète des filigranes dans Excel feuilles de calcul, permettant aux développeurs de générer, d'ajuster et d'effacer facilement les filigranes. Il prend en charge tous les formats de fichiers Excel courants, ce qui permet d'intégrer des filigranes de texte et d'image qui peuvent être personnalisés en termes de police, de couleur, de taille et de position. GroupDocs.Watermark inclut également des fonctionnalités de recherche de filigranes, garantissant ainsi que vos filigranes sont intacts et inviolables. Idéal pour les applications nécessitant des améliorations de la sécurité des documents dans les environnements Java.

############################# Steps ############################
steps:
    enable: true
    title: "Ajouter un filigrane au document Excel via Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** permet aux développeurs Java d'ajouter facilement des filigranes de différents types aux formats de fichiers professionnels courants. Ajoutez notre bibliothèque à votre candidature et filigranez les documents en quelques étapes simples, comme indiqué ci-dessous.
      
      1. La classe principale de notre API est **Watermarker**. Vous devez l'instancier avant le traitement du document. N'oubliez pas de transmettre le fichier Excel au constructeur en tant que chemin ou objet flux.
      2. L'étape suivante consiste à construire un objet **Watermark** du type souhaité. Il peut être placé non seulement sur une page de document spécifique, mais également dans des parties natives du document telles que des pièces jointes ou des en-têtes.
      3. Définissez les propriétés du filigrane telles que la hauteur et la largeur, l'alignement de la page (en haut, à gauche, au centre, etc.), la famille et la couleur de la police, et bien d'autres.
      4. Appelez la méthode **Watermarker** pour ajouter un nouveau filigrane. Vous pouvez ajouter autant de filigranes que nécessaire. Il est recommandé de sauvegarder le document traité dans un autre emplacement.
   
    code:
      platform: "net"
      copy_title: "Copier"
      install:
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-watermark</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "cliquez pour copier"
        copy_done: "copié"
      links:
        #  loop
        - title: "Plus d'exemples"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/watermark/java/"
          
      content: |
        ```java {style=abap}

        // Ajouter un filigrane de texte à EXCEL

        // Transmettre le fichier à filigraner à Watermarker
        Watermarker watermarker = new Watermarker("input.xslx");
        
        // Créer un filigrane de texte et configurer les propriétés
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        watermark.setForegroundColor(Color.getRed());

        // Enregistrer le fichier filigrané
        watermarker.add(watermark);
        watermarker.save("output.xslx");
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Améliorez facilement vos filigranes"
  description: "Exploitez la puissance de GroupDocs.Watermark pour générer, composer et ajouter des filigranes dans différents formats de documents. Cette API améliore non seulement la sécurité des documents, mais protège également votre propriété intellectuelle en intégrant des filigranes personnalisables à la fois polyvalents et robustes."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Ajouter un filigrane"
  features:
    # feature loop
    - title: "Options de filigrane polyvalentes."
      content: "Explorez un large éventail d'options de filigrane avec GroupDocs.Watermark. Qu'il s'agisse de régler l'opacité et la rotation ou de redimensionner proportionnellement la taille, notre API vous permet de personnaliser les filigranes précisément selon vos besoins, en veillant à ce qu'ils s'intègrent parfaitement à vos documents tout en préservant l'intégrité du contenu."

    # feature loop
    - title: "Style de filigrane avancé."
      content: "GroupDocs.Watermark vous permet de personnaliser vos filigranes avec différentes polices, couleurs et ombres, afin de les rendre uniques et plus difficiles à supprimer. Améliorez l'esthétique de vos documents et images protégés grâce à des filigranes stylés qui reflètent l'identité et le professionnalisme de votre marque."

    # feature loop
    - title: "Carrelage et positionnement des filigranes"
      content: "Avec GroupDocs.Watermark, implémentez des effets de mosaïque pour couvrir l'intégralité de votre document, garantissant ainsi une protection complète. Positionnez les filigranes exactement là où vous en avez besoin : au centre, dans un coin ou à des emplacements personnalisés. Nos options de positionnement flexibles contribuent à protéger vos documents contre toute utilisation non autorisée et toute duplication."
      
  code_samples:
    # code sample loop
    - title: "Filigrane d'annotation PDF"
      content: |
        Cet exemple montre comment ajouter une annotation en filigrane à un document PDF
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Charger le document sous le nom PDF
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Créer un filigrane en fonction de l'annotation PDF
        PdfAnnotationWatermarkOptions options = new PdfAnnotationWatermarkOptions();
        TextWatermark textWatermark = new TextWatermark("Annotation watermark", new Font("Arial", 8));

        //  Configurer les options de filigrane
        textWatermark.setHorizontalAlignment(HorizontalAlignment.Left);
        textWatermark.setVerticalAlignment(VerticalAlignment.Top);

        //  Ajouter un filigrane de texte au document de résultat
        watermarker.add(textWatermark, options);
        watermarker.save("result.pdf");

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Prêt à démarrer ?"
  description: "Essayez GroupDocs.Watermark fonctionnalités gratuitement ou demandez une licence"
  items:
    #  loop
    - title: "Maven télécharger"
      link: "https://releases.groupdocs.com/watermark/java/"
      color: "red"
        #  loop
    - title: "Licences"
      link: "https://purchase.groupdocs.com/pricing/watermark/java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Java Techniques de filigrane Excel"
    exclude: "EXCEL"
    description: "À l'aide de GroupDocs.Watermark for Java, appliquez facilement des filigranes à base de texte ou d'image à Excel feuilles de calcul, renforçant ainsi considérablement la sécurité des documents et l'image de marque dans le cadre de votre flux de travail professionnel."
    items: 
        # format loop 1
        - name: "Filigrane PDF"
          format: "PDF"
          link: "/watermark/java/add//pdf/"
          description: "Format de document Adobe Portable"

        # format loop 2
        - name: "Filigrane Word"
          format: "WORD"
          link: "/watermark/java/add//word/"
          description: "MS Word et documents Open Office"
          
        # format loop 3
        - name: "Filigrane Excel"
          format: "EXCEL"
          link: "/watermark/java/add//excel/"
          description: "MS Excel et feuilles de calcul Open Office"

        # format loop 4
        - name: "Image en filigrane"
          format: "IMAGE"
          link: "/watermark/java/add//image/"
          description: "Formats d'image populaires"

        # format loop 5
        - name: "Photo en filigrane"
          format: "PHOTO"
          link: "/watermark/java/add//photo/"
          description: "Formats de photos"

        # format loop 6
        - name: "Filigrane PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/add//powerpoint/"
          description: "MS PowerPoint et présentations Open Office"

        # format loop 7
        - name: "Filigrane DOCX"
          format: "DOCX"
          link: "/watermark/java/add//docx/"
          description: "Microsoft Word Ouvrir un document XML"
          
        # format loop 8
        - name: "Filigrane PPTX"
          format: "PPTX"
          link: "/watermark/java/add//pptx/"
          description: "PowerPoint Présentation Open XML"
          
        # format loop 9
        - name: "Filigrane XLSX"
          format: "XLSX"
          link: "/watermark/java/add//xlsx/"
          description: "Feuille de calcul Microsoft Excel Open XML"

        # format loop 10
        - name: "Filigrane JPEG"
          format: "JPEG"
          link: "/watermark/java/add//jpeg/"
          description: "JPEG Photo"

        # format loop 11
        - name: "Filigrane PNG"
          format: "PNG"
          link: "/watermark/java/add//png/"
          description: "Portable Graphique du réseau"

        # format loop 12
        - name: "Filigrane TIFF"
          format: "TIFF"
          link: "/watermark/java/add//tiff/"
          description: "Format de fichier d'image de balise"

        # format loop 13
        - name: "Filigrane WEBP"
          format: "WEBP"
          link: "/watermark/java/add//webp/"
          description: "Photo WEB"

        # format loop 14
        - name: "Filigrane DOC"
          format: "DOC"
          link: "/watermark/java/add//doc/"
          description: "Microsoft Word 97 - 2007 Documento"

        # format loop 15
        - name: "Filigrane XLS"
          format: "XLS"
          link: "/watermark/java/add//xls/"
          description: "Classeur Microsoft Excel 97-2003"

        # format loop 16
        - name: "Filigrane PPT"
          format: "PPT"
          link: "/watermark/java/add//ppt/"
          description: "PowerPoint Présentation 97-2003"

        # format loop 17
        - name: "Filigrane RTF"
          format: "RTF"
          link: "/watermark/java/add//rtf/"
          description: "Format de texte enrichi"

---