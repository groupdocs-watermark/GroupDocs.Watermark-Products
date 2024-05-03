
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:10
draft: false
lang: fr
format: Doc
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Réglez DOC filigranes de manière professionnelle - GroupDocs.Watermark"
head_description: "Gérez et personnalisez les filigranes de manière professionnelle avec GroupDocs.Watermark. Sécurisez vos documents en toute confiance."

############################# Header ############################
title: "Ajuster DOC filigranes : assurance professionnelle" 
description: "Garantissez des normes professionnelles grâce à notre solution de gestion des filigranes. Protégez vos documents de manière fiable."
subtitle: "GroupDocs.Watermark for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Téléchargez le package depuis Maven"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java"
    link: "/watermark/java/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Gérer les filigranes** : notre solution professionnelle de gestion des filigranes garantit la protection de vos documents. Simplifiez votre flux de travail grâce à des outils efficaces pour ajouter, modifier et supprimer des filigranes.

############################# Steps ############################
steps:
    enable: true
    title: "Ajustez les filigranes de document Doc à l'aide de Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** permet aux développeurs Java d'ajuster facilement les filigranes dans de nombreux documents à l'aide de leurs applications. Voici un guide rapide :
      
      1. Tout d'abord, vous devez passer le fichier Doc comme paramètre du constructeur de classe **Watermarker**. Fournissez un flux d’octets ou de fichiers ou un chemin de disque local.
      2. Deuxièmement, localisez les filigranes qui doivent être ajustés. Utilisez **SearchCriteria** pour identifier les filigranes avec les propriétés spécifiques précédemment ajoutées au document.
      3. Suite à la recherche, vous recevrez une liste de filigranes pertinents. Vous pouvez ensuite ajuster leurs propriétés, notamment la taille, l'alignement de la page, le texte, la couleur, le contenu de l'image, etc. Cela offre un haut degré de personnalisation de vos données.
      4. Une fois que vous avez fini d'ajuster les filigranes, enregistrez le document mis à jour. Vous pouvez utiliser un chemin de fichier local ou un flux pour stocker le résultat.
   
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
        // Ajuster le filigrane de l'image DOC

        // Instancier Watermarker avec DOC
        Watermarker watermarker = new Watermarker("input.doc");
        
        // Initialisez le SearchCriteria pour qu'il corresponde à une image particulière
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);

        for (PossibleWatermark watermark : watermarks)
        {
            // Remplacer l'image trouvée
            watermark.setImageData(imageData);
        }

        // Enregistrer le fichier ajusté
        watermarker.save("output.doc");
        
        ```
        
############################# More features ############################
more_features:
  enable: true
  title: "Gestion avancée des filigranes DOC pour Java applications"
  description: "L'API GroupDocs.Watermark permet aux développeurs d'intégrer de manière fluide la fonctionnalité de filigrane dans leurs Java applications. Il prend en charge l'ajout, la modification, la suppression et la recherche de filigranes dans un large éventail de formats de documents."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Réglage du filigrane"
  features:
    # feature loop
    - title: "Intégration sans effort des filigranes"
      content: "GroupDocs.Watermark simplifie le processus d'ajout de divers filigranes à divers documents et fichiers commerciaux au sein d' Java applications. Les développeurs peuvent non seulement appliquer des filigranes, mais également mettre à jour ou supprimer les filigranes existants par programmation."

    # feature loop
    - title: "Personnalisation granulaire du filigrane"
      content: "L'API fournit de nombreuses options de personnalisation pour les filigranes. Les développeurs peuvent facilement ajuster la taille, la rotation, la couleur, la police, les styles et d'autres propriétés pour obtenir l'effet visuel souhaité."

    # feature loop
    - title: "Tirer parti des fonctionnalités natives des documents DOC"
      content: "Selon le format du document cible, les développeurs peuvent utiliser des fonctionnalités natives pour le placement des filigranes. Ces fonctionnalités peuvent inclure l'arrière-plan de la page du document, des annotations, des en-têtes ou d'autres objets tels que des conteneurs de filigranes."
      
  code_samples:
    # code sample loop
    - title: "Ajuster le filigrane de l'image dans les feuilles de calcul"
      content: |
        Cet exemple montre comment ajuster l'image de formes particulières dans une feuille de travail Excel.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Charger le document sous forme de feuille de calcul
        SpreadsheetLoadOptions loadOptions = new SpreadsheetLoadOptions();
        Watermarker watermarker = new Watermarker("source.xlsx", loadOptions);

        //  Obtenir de nouveaux octets de filigrane
        File file = new File("new_watermark.png");
        byte[] imageBytes = new byte[(int) file.length()];
        FileInputStream inputStream = new FileInputStream(file);
        inputStream.read(imageBytes);
        inputStream.close();

        //  Ajuster le contenu d'un filigrane particulier
        for (SpreadsheetShape shape : content.getWorksheets().get_Item(0).getShapes())
        {
            if (shape.getImage() != null)
            {
                shape.setImage(new SpreadsheetWatermarkableImage(imageBytes));
            }
        }

        //  Enregistrer le document de résultats
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
    title: "Modifiez les filigranes dans d'autres formats via GroupDocs.Watermark for Java"
    exclude: "DOC"
    description: "Simplifiez la gestion des filigranes dans différents formats de documents. Notre solution propose des outils efficaces pour ajouter, modifier et supprimer facilement des filigranes."
    items: 
        # format loop 1
        - name: "Filigrane PDF"
          format: "PDF"
          link: "/watermark/java/adjust//pdf/"
          description: "Format de document Adobe Portable"

        # format loop 2
        - name: "Filigrane Word"
          format: "WORD"
          link: "/watermark/java/adjust//word/"
          description: "MS Word et documents Open Office"
          
        # format loop 3
        - name: "Filigrane Excel"
          format: "EXCEL"
          link: "/watermark/java/adjust//excel/"
          description: "MS Excel et feuilles de calcul Open Office"

        # format loop 4
        - name: "Filigrane PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/adjust//powerpoint/"
          description: "MS PowerPoint et présentations Open Office"

        # format loop 5
        - name: "Filigrane DOCX"
          format: "DOCX"
          link: "/watermark/java/adjust//docx/"
          description: "Microsoft Word Ouvrir un document XML"
          
        # format loop 6
        - name: "Filigrane PPTX"
          format: "PPTX"
          link: "/watermark/java/adjust//pptx/"
          description: "PowerPoint Présentation Open XML"
          
        # format loop 7
        - name: "Filigrane XLSX"
          format: "XLSX"
          link: "/watermark/java/adjust//xlsx/"
          description: "Feuille de calcul Microsoft Excel Open XML"

        # format loop 8
        - name: "Filigrane DOC"
          format: "DOC"
          link: "/watermark/java/adjust//doc/"
          description: "Microsoft Word 97 - 2007 Documento"

        # format loop 9
        - name: "Filigrane XLS"
          format: "XLS"
          link: "/watermark/java/adjust//xls/"
          description: "Classeur Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrane PPT"
          format: "PPT"
          link: "/watermark/java/adjust//ppt/"
          description: "PowerPoint Présentation 97-2003"

        # format loop 11
        - name: "Filigrane RTF"
          format: "RTF"
          link: "/watermark/java/adjust//rtf/"
          description: "Format de texte enrichi"

---