
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:23
draft: false
lang: fr
format: Pptx
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Intégrer des filigranes dans PPTX avec C#"
head_description: "Sécurisez vos PPTX présentations avec .NET filigranes appliqués en C#, protégeant ainsi la propriété intellectuelle."

############################# Header ############################
title: "Filigrane C# avancé pour PPTX" 
description: "Implémentez .NET C# pour créer des filigranes robustes dans les fichiers PPTX, ce qui est idéal pour renforcer la sécurité des présentations professionnelles et pédagogiques."
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Téléchargez gratuitement sur Nuget"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET fournit une solution complète .NET C# pour le filigrane des fichiers PPTX, adaptée aux professionnels qui ont besoin de sécuriser des supports de présentation. Cette API prend en charge l'intégration de filigranes personnalisables et pouvant inclure du texte, des logos ou d'autres graphiques. Il offre des fonctionnalités telles que le réglage de la transparence, de la taille et du positionnement, permettant aux filigranes d'être à la fois efficaces et subtils. Idéal pour les entreprises, les enseignants et toute personne présentant des informations sensibles ou confidentielles, GroupDocs.Watermark garantit la sécurité de vos présentations, tout en préservant leur qualité esthétique. Compatible avec .NET 5 et versions ultérieures, cet outil étend le support robuste aux environnements Microsoft Office modernes.

############################# Steps ############################
steps:
    enable: true
    title: "Générez sans effort des filigranes pour les documents Pptx"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/) :** Bibliothèque de filigrane avancée pour les applications .NET. Renforcez votre solution et sécurisez les documents avec des filigranes juste à temps.
      
      1. **Classe principale : Watermarker.** La classe principale de notre API est **Watermarker**. Vous devez l'instancier avant le traitement du document. N'oubliez pas de transmettre le fichier Pptx au constructeur en tant que chemin ou objet flux.
      2. **Création de votre filigrane.** L'étape suivante consiste à construire un objet Watermark du type souhaité. Il peut être placé non seulement sur une page de document spécifique, mais également dans des parties natives du document telles que des images ou des en-têtes.
      3. **Affinage de l'apparence.** Définissez les propriétés du filigrane telles que la hauteur et la largeur, les alignements haut, gauche, central, les polices et les couleurs, etc.
      4. **Application et enregistrement.** Utilisez la méthode **Watermarker** pour ajouter un nouveau filigrane. N'hésitez pas à ajouter autant de filigranes que nécessaire. Vous pouvez enregistrer le document filigrané à n’importe quel emplacement.
   
    code:
      platform: "net"
      copy_title: "Copier"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "cliquez pour copier"
        copy_done: "copié"
      links:
        #  loop
        - title: "Plus d'exemples"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // Générer un filigrane d'image dans le fichier PPTX

        // Fournir le chemin du fichier source au constructeur Watermarker
        using (Watermarker watermarker = new Watermarker("input.pptx"))
        {
            // Générer une instance de filigrane d'image avec un fichier image
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // Enregistrer le résultat PPTX filigrané
            watermarker.Save("output.pptx");
        }
        
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "Améliorez votre jeu de filigrane"
  description: "Débloquez des fonctionnalités avancées de filigrane grâce à notre API GroupDocs.Watermark pour .NET. Cet outil puissant permet de personnaliser et d'appliquer des filigranes avec précision sur différents types de documents afin de garantir une sécurité maximale et le respect des droits d'auteur avec un minimum de perturbations visuelles."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Solutions complètes de filigrane"
  features:
    # feature loop
    - title: "Options de carrelage sophistiquées"
      content: "Étendez facilement vos filigranes à des documents entiers grâce à nos options de tuilage. Cette fonctionnalité permet aux filigranes de couvrir toute la zone du document, empêchant ainsi leur suppression et garantissant une protection complète du document sans compromettre la conception ou la lisibilité."

    # feature loop
    - title: "Personnalisation des couleurs éclatantes"
      content: "Ajoutez une touche de couleur à vos filigranes ! Notre API permet une personnalisation complète des couleurs, ce qui vous permet d'appliquer des filigranes qui correspondent parfaitement à l'image de marque de votre entreprise ou au style de vos documents. Améliorez l'attrait visuel tout en conservant des fonctionnalités de sécurité robustes."

    # feature loop
    - title: "Paramètres de sécurité améliorés"
      content: "Améliorez la sécurité des documents grâce à des paramètres avancés de filigrane. Configurez des filigranes multicouches, incorporant à la fois des éléments visibles et invisibles, pour vous protéger contre les copies non autorisées et garantir que seuls les destinataires prévus peuvent accéder aux informations critiques."
      
  code_samples:
    # code sample loop
    - title: "Générer un filigrane PowerPoint"
      content: |
        Cet exemple montre comment ajouter un filigrane aux images d'arrière-plan PPTX
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Charger la présentation PPTX
            var loadOptions = new PresentationLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pptx", loadOptions))
            {
                //  Configurer les propriétés du filigrane
                TextWatermark watermark = new TextWatermark("Protected image", new Font("Arial", 8));
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermark.RotateAngle = 45;
                watermark.SizingType = SizingType.ScaleToParentDimensions;
                watermark.ScaleFactor = 1;

                //  Fond de diapositives en filigrane
                PresentationContent content = watermarker.GetContent<PresentationContent>();
                foreach (PresentationSlide slide in content.Slides)
                {
                    if (slide.ImageFillFormat.BackgroundImage != null)
                    {
                        slide.ImageFillFormat.BackgroundImage.Add(watermark);
                    }
                }

                //  Enregistrer la présentation traitée
                watermarker.save("result.pptx");
            }

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Prêt à démarrer ?"
  description: "Essayez GroupDocs.Watermark fonctionnalités gratuitement ou demandez une licence"
  items:
    #  loop
    - title: "Nuget télécharger"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "Licences"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Solutions de filigrane C# pour les fichiers PPTX"
    exclude: "PPTX"
    description: "Tirez parti de .NET C# pour appliquer des filigranes discrets dans les fichiers PPTX, protégeant ainsi vos présentations contre toute distribution non autorisée."
    items: 
        # format loop 1
        - name: "Filigrane PDF"
          format: "PDF"
          link: "/watermark/net/generate//pdf/"
          description: "Format de document Adobe Portable"

        # format loop 2
        - name: "Filigrane Word"
          format: "WORD"
          link: "/watermark/net/generate//word/"
          description: "MS Word et documents Open Office"
          
        # format loop 3
        - name: "Filigrane Excel"
          format: "EXCEL"
          link: "/watermark/net/generate//excel/"
          description: "MS Excel et feuilles de calcul Open Office"

        # format loop 4
        - name: "Image en filigrane"
          format: "IMAGE"
          link: "/watermark/net/generate//image/"
          description: "Formats d'image populaires"

        # format loop 5
        - name: "Photo en filigrane"
          format: "PHOTO"
          link: "/watermark/net/generate//photo/"
          description: "Formats de photos"

        # format loop 6
        - name: "Filigrane PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/generate//powerpoint/"
          description: "MS PowerPoint et présentations Open Office"

        # format loop 7
        - name: "Filigrane DOCX"
          format: "DOCX"
          link: "/watermark/net/generate//docx/"
          description: "Microsoft Word Ouvrir un document XML"
          
        # format loop 8
        - name: "Filigrane PPTX"
          format: "PPTX"
          link: "/watermark/net/generate//pptx/"
          description: "PowerPoint Présentation Open XML"
          
        # format loop 9
        - name: "Filigrane XLSX"
          format: "XLSX"
          link: "/watermark/net/generate//xlsx/"
          description: "Feuille de calcul Microsoft Excel Open XML"

        # format loop 10
        - name: "Filigrane JPEG"
          format: "JPEG"
          link: "/watermark/net/generate//jpeg/"
          description: "JPEG Photo"

        # format loop 11
        - name: "Filigrane PNG"
          format: "PNG"
          link: "/watermark/net/generate//png/"
          description: "Portable Graphique du réseau"

        # format loop 12
        - name: "Filigrane TIFF"
          format: "TIFF"
          link: "/watermark/net/generate//tiff/"
          description: "Format de fichier d'image de balise"

        # format loop 13
        - name: "Filigrane WEBP"
          format: "WEBP"
          link: "/watermark/net/generate//webp/"
          description: "Photo WEB"

        # format loop 14
        - name: "Filigrane DOC"
          format: "DOC"
          link: "/watermark/net/generate//doc/"
          description: "Microsoft Word 97 - 2007 Documento"

        # format loop 15
        - name: "Filigrane XLS"
          format: "XLS"
          link: "/watermark/net/generate//xls/"
          description: "Classeur Microsoft Excel 97-2003"

        # format loop 16
        - name: "Filigrane PPT"
          format: "PPT"
          link: "/watermark/net/generate//ppt/"
          description: "PowerPoint Présentation 97-2003"

        # format loop 17
        - name: "Filigrane RTF"
          format: "RTF"
          link: "/watermark/net/generate//rtf/"
          description: "Format de texte enrichi"

---