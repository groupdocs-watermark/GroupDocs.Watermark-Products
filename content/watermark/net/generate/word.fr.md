
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:06
draft: false
lang: fr
format: Word
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Générer un filigrane de document Word"
head_description: "Simplifiez les flux de travail de Word documents à l'aide de filigranes. Représentez l'intégrité de votre marque de manière professionnelle."

############################# Header ############################
title: "Créez des filigranes dynamiques dans Word et OpenOffice avec C#" 
description: "Déployez des filigranes de manière stratégique dans vos Word documents à l'aide de notre robuste boîte à outils C#. Personnalisez-le pour répondre facilement aux normes de la marque ou aux exigences de sécurité."
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
       GroupDocs.Watermark for .NET transforme votre capacité à apposer un filigrane sur les documents Microsoft Word. Cette API polyvalente s'intègre parfaitement à votre environnement de développement, permettant l'ajout de filigranes de texte et d'image sophistiqués qui peuvent être positionnés de manière absolue ou relative dans le document. Il prend en charge les formats DOC, DOCX et RTF, offrant une flexibilité entre plusieurs versions Word. Améliorez vos documents avec des filigranes qui sont non seulement sécurisés, mais qui se fondent subtilement dans le contenu, préservant ainsi la lisibilité et l'intégrité de la mise en page.

############################# Steps ############################
steps:
    enable: true
    title: "Améliorez vos documents : générez des filigranes pour Word à l'aide de .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** est une bibliothèque qui simplifie l'ajout de filigranes à divers formats de fichiers professionnels pour les développeurs .NET. Intégrez notre bibliothèque dans votre application et filigranez facilement les documents en suivant les étapes suivantes :
      
      1. **Lancez votre parcours de filigrane :** Commencez par vous familiariser avec la classe **Watermarker**, la pierre angulaire de notre API. Pour commencer le processus, assurez-vous de l'instancier avant le traitement du document. Ne négligez pas l'importance de fournir le fichier Word au constructeur, qu'il s'agisse d'un chemin ou d'un objet flux.
      2. **Création de filigranes personnalisés :** Passez à la phase suivante en créant un objet **Watermark** adapté à vos spécifications. Cet outil polyvalent ne se limite pas à des pages de document spécifiques ; il peut également être intégré de manière transparente aux éléments natifs du document tels que les pièces jointes ou les en-têtes.
      3. **Réglage précis des attributs du filigrane :** Affinez votre expérience de filigrane en ajustant des propriétés telles que la hauteur, la largeur, l'alignement de la page, la famille de polices et la couleur. Ce niveau de personnalisation garantit que vos filigranes se fondent parfaitement dans vos documents.
      4. **Application de vos filigranes :** Utilisez la méthode **Watermarker** pour appliquer sans effort vos filigranes personnalisés à vos documents. Que vous ayez besoin d'ajouter un ou plusieurs filigranes, ce processus offre une certaine flexibilité. Pour plus de sécurité, pensez à enregistrer vos documents traités dans un emplacement distinct.
   
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
        // Générer un filigrane de texte dans le fichier WORD

        // Fournir le fichier à filigraner
        using (Watermarker watermarker = new Watermarker("input.docx"))
        {
            // Générer une instance de filigrane de texte
            Font font = new Font("Arial", 19, FontStyle.Bold | FontStyle.Italic);
            TextWatermark watermark = new TextWatermark("my watermark", font);
            watermark.ForegroundColor = Color.Red;
            watermark.BackgroundColor = Color.Blue;
            watermarker.Add(watermark);

            // Enregistrer le résultat WORD
            watermarker.Save("output.docx");
        }
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "En savoir plus sur l'ajout de filigranes"
  description: "Tirez parti de notre puissante API pour afficher, convertir et gérer des documents, des diapositives, des diagrammes et divers autres types de documents dans .NET applications. GroupDocs.Watermark intègre de manière fluide des fonctionnalités de filigrane pour améliorer la sécurité des documents et la protection des droits d'auteur."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Ajouter un filigrane"
  features:
    # feature loop
    - title: "Ajoutez des filigranes à vos documents sans effort."
      content: "GroupDocs.Watermark permet à .NET développeurs d'intégrer facilement le filigrane dans leurs applications. Ajoutez sans effort du texte, des images ou des filigranes dynamiques à des documents et fichiers professionnels populaires, afin de garantir la sécurité de votre contenu et la cohérence de votre marque sur toutes les plateformes."

    # feature loop
    - title: "Personnalisez les filigranes en fonction de vos besoins."
      content: "Personnalisez les filigranes en fonction de vos besoins spécifiques grâce aux fonctionnalités étendues prises en charge par GroupDocs.Watermark. Ajustez la taille, la rotation, la transparence, la couleur et la police pour que votre filigrane soit non seulement parfait, mais renforce également la sécurité des documents sans obstruer les informations importantes."

    # feature loop
    - title: "Exploitez les fonctionnalités natives des documents pour le filigrane"
      content: "Utilisez les caractéristiques inhérentes aux formats de documents pour un filigrane sophistiqué. Qu'il s'agisse d'utiliser des annotations natives PDF, des arrière-plans MS Word ou des en-têtes et pieds de page Excel, GroupDocs.Watermark s'intègre parfaitement aux structures des documents pour appliquer des filigranes à la fois efficaces et peu invasifs."
      
  code_samples:
    # code sample loop
    - title: "Générer un filigrane d'image pour DOCX"
      content: |
        Cet exemple montre comment appliquer des effets d'image aux filigranes de forme.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Charger le document Word
            var loadOptions = new WordProcessingLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.docx", loadOptions))
            {
                //  Configurer les options de filigrane
                using (ImageWatermark watermark = new ImageWatermark("logo.png"))
                {
                    WordProcessingImageEffects effects = new WordProcessingImageEffects();
                    effects.Brightness = 0.7;
                    effects.Contrast = 0.6;
                    effects.ChromaKey = Color.Red;
                    effects.BorderLineFormat.Enabled = true;
                    effects.BorderLineFormat.Weight = 1;

                    WordProcessingWatermarkSectionOptions options = new WordProcessingWatermarkSectionOptions();
                    options.Effects = effects;

                    //  Générer un filigrane
                    watermarker.Add(watermark, options);
                }

                //  Enregistrer le document mis à jour
                watermarker.save("result.docx");
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
    title: "Filigrane alimenté par C# dans Word et OpenOffice via C#"
    exclude: "WORD"
    description: "Maximisez l'impact de vos documents MS Word et OpenOffice grâce à des filigranes personnalisés qui offrent à la fois protection et professionnalisme. Notre API C# facilite l'application de filigranes précis et attrayants."
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