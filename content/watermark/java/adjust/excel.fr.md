
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:57
draft: false
lang: fr
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Ajuster l'outil de filigrane Excel - GroupDocs.Watermark"
head_description: "Ajustez, mettez à jour et gérez les filigranes sans effort avec GroupDocs.Watermark. Personnalisez facilement vos documents."

############################# Header ############################
title: "Outil Ajuster les filigranes de SpreadSheets : extrêmement simple" 
description: "Améliorez vos documents grâce à notre outil intuitif d'édition de filigranes. Simplifiez votre flux de travail sans effort."
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
    title: "GroupDocs.Watermark for Java API"
    link: "/watermark/java/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Outil de réglage des filigranes** : Notre outil de filigrane offre une solution conviviale pour améliorer et protéger vos documents. Grâce à des fonctionnalités d'édition intuitives, la gestion des filigranes devient un jeu d'enfant, garantissant ainsi la sécurité et l'authenticité des documents.

############################# Steps ############################
steps:
    enable: true
    title: "Ajustez les filigranes dans Excel documents avec Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** permet aux développeurs Java d'ajuster facilement les filigranes de texte dans leurs applications en mettant en œuvre quelques étapes simples :
      
      1. **Watermarker**. Vous pouvez fournir un fichier pour le traitement ultérieur sous forme de flux ou de chemin sur un disque local.
      2. **SearchCriteria** permet d'identifier les filigranes dotés des bonnes propriétés qui ont été précédemment ajoutés à un document.
      3. **Recherche**. Ajustez les propriétés des filigranes trouvés, telles que la taille, l'alignement des pages, le texte, la couleur, le contenu de l'image, etc. Il existe de nombreuses façons de personnaliser vos données.
      4. Une fois le processus de réglage des filigranes terminé, vous devez enregistrer le document mis à jour. Utilisez le chemin de fichier local, le fichier ou le flux d'octets pour stocker le résultat.
   
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

        // Ajuster le filigrane du texte EXCEL

        // Instanciation d'un filigrane avec saisie du document EXCEL
        Watermarker watermarker = new Watermarker("input.xslx");

        // Initialisez les TextSearchCriteria et recherchez les filigranes de texte
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        
        // Ajuster les propriétés du filigrane de texte
        for (PossibleWatermark watermark : watermarks)
        {
            watermark.getFormattedTextFragments().clear();
            watermark.getFormattedTextFragments().
                add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
        }

        // Enregistrez le document mis à jour
        watermarker.save("output.xslx");
        
        ```            
        
############################# More features ############################
more_features:
  enable: true
  title: "Approfondissement du réglage du filigrane EXCEL"
  description: "Notre API permet à Java applications d'ajouter, de modifier, de supprimer et de rechercher des filigranes dans les formats de documents courants."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Ajuster le filigrane"
  features:
    # feature loop
    - title: "Ajoutez un filigrane à vos documents sans effort"
      content: "GroupDocs.Watermark simplifie le filigrane pour Java développeurs. Ajoutez divers filigranes à divers documents et fichiers commerciaux. Vous pouvez non seulement appliquer des filigranes, mais vous pouvez également mettre à jour ou supprimer ceux qui existent déjà."

    # feature loop
    - title: "Personnalisez les filigranes selon vos besoins"
      content: "Notre API propose de nombreuses options de personnalisation. Ajustez facilement la taille, la rotation, la couleur, la police, les styles, etc. pour obtenir le filigrane parfait."

    # feature loop
    - title: "Utiliser les fonctionnalités natives du document EXCEL"
      content: "En fonction du format de document spécifique, vous pouvez utiliser les fonctionnalités natives. Il peut s'agir de l'arrière-plan de la page du document, d'annotations, d'en-têtes ou d'autres objets tels que des conteneurs de filigranes."
      
  code_samples:
    # code sample loop
    - title: "PDF ajuster le filigrane du texte"
      content: |
        Cet exemple montre comment ajuster le texte de chaque artefact.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Charger le document PDF
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Obtenir le contenu du document
        PdfContent pdfContent = watermarker.getContent(PdfContent.class);

        //  Ajuster un texte de filigrane particulier
        for (PdfArtifact artifact : pdfContent.getPages().get_Item(0).getArtifacts())
        {
            if (artifact.getText().contains("Test"))
            {
                artifact.setText("Passed");
            }
        }

        //  Enregistrez le document
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
    title: "Ajustez le filigrane via GroupDocs.Watermark for Java pour les autres formats"
    exclude: "EXCEL"
    description: "Personnalisez facilement les filigranes dans un large éventail de formats de documents. Améliorez la sécurité et l'authenticité des documents sans effort."
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