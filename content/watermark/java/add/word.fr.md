
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:26:57
draft: false
lang: fr
format: Word
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Composez des filigranes personnalisés pour Word avec Java"
head_description: "Intégrez des filigranes personnalisés dans Word documents à l'aide de Java. Renforcez la sécurité et ajoutez une touche professionnelle."

############################# Header ############################
title: "Création de filigranes personnalisés dans Word documents" 
description: "Sécurisez vos Word fichiers avec Java en incorporant du texte ou des filigranes d'image personnalisés. Cette ressource est idéale pour ceux qui ont besoin d'améliorer la sécurité des documents et leur attrait visuel avec un minimum d'effort."
subtitle: "GroupDocs.Watermark for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Téléchargez gratuitement sur Maven"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java"
    link: "/watermark/java/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java permet la création précise et flexible de filigranes dans Word documents. Cet outil permet à Java développeurs d'ajouter des filigranes personnalisés pouvant inclure du texte, des images ou des logos, adaptés à vos besoins spécifiques en matière de marque. Il prend en charge tous les principaux formats de documents Word et fournit des fonctionnalités complètes pour modifier et supprimer les filigranes, ainsi que pour rechercher dans les documents pour vérifier l'intégrité des filigranes. Compatible avec tous les systèmes d'exploitation pris en charge par Java, cette API est idéale pour les entreprises qui souhaitent renforcer leurs protocoles de sécurité des documents.

############################# Steps ############################
steps:
    enable: true
    title: "Ajouter un filigrane au document Word via Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** permet aux développeurs Java d'ajouter facilement des filigranes de différents types aux formats de fichiers professionnels les plus courants. Ajoutez notre bibliothèque à votre demande et filigranez les documents en quelques étapes simples, comme indiqué ci-dessous.
      
      1. **Watermarker**. Vous devez l'instancier avant le traitement du document. N'oubliez pas de transmettre le fichier Word au constructeur en tant que chemin ou objet de flux.
      2. **Watermark** du type souhaité. Il peut être placé non seulement sur une page de document spécifique, mais également dans des parties natives du document, telles que les pièces jointes ou les en-têtes.
      3. Définissez les propriétés du filigrane telles que la hauteur et la largeur, l'alignement de la page (en haut, à gauche, au centre, etc.), la famille de police et la couleur, et bien d'autres encore.
      4. **Watermarker** pour ajouter un nouveau filigrane. Vous pouvez ajouter autant de filigranes que vous le souhaitez. Il est recommandé d'enregistrer le document traité dans un autre emplacement.
   
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

        // Ajouter un filigrane de texte à WORD

        // Transmettre le fichier à filigraner au filigrane
        Watermarker watermarker = new Watermarker("input.docx");
        
        // Création d'un filigrane de texte et configuration des propriétés
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        watermark.setForegroundColor(Color.getRed());

        // Enregistrer le fichier filigrané
        watermarker.add(watermark);
        watermarker.save("output.docx");
        
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
    title: "Personnalisez vos fichiers MS Word avec la génération de filigranes Java."
    exclude: "WORD"
    description: "GroupDocs.Watermark for Java permet aux développeurs d'insérer facilement des filigranes personnalisés sous forme de texte ou d'image dans Word documents. Ces améliorations renforcent non seulement la sécurité des documents, mais enrichissent également les communications professionnelles avec une touche professionnelle."
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