
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:27:07
draft: false
lang: fr
format: Pptx
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "API C# .NET pour la suppression des filigranes PowerPoint"
head_description: "Supprimez efficacement les filigranes de PowerPoint diapositives à l'aide de notre API C# .NET, garantissant des présentations claires et professionnelles."

############################# Header ############################
title: "Supprimer PPTX filigranes en utilisant C# .NET" 
description: "Utilisez l'API GroupDocs.Watermark for .NET C# pour supprimer efficacement les filigranes des fichiers PPTX, ce qui est idéal pour préserver l'intégrité et l'attrait visuel de vos présentations."
subtitle: "GroupDocs.Watermark for .NET C# ET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Téléchargement gratuit Nuget"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "bibliothèque GroupDocs.Watermark for .NET C#"
    link: "/watermark/net/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       La bibliothèque GroupDocs.Watermark for .NET C# propose des outils complets pour gérer les filigranes dans PowerPoint présentations. Que vous ayez besoin de supprimer, modifier ou ajuster des filigranes, cette API permet de contrôler avec précision les éléments des diapositives, garantissant ainsi des présentations de qualité professionnelle pour les entreprises, l'enseignement, etc.

############################# Steps ############################
steps:
    enable: true
    title: "Supprimez les filigranes des documents Pptx par programmation à l'aide de .NET"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/)** permet à .NET développeurs de supprimer par programmation les filigranes de divers documents Pptx. Ce guide décrit le processus :
      
      1. **Watermarker**. Le fichier peut être fourni sous la forme d'un flux d'octets, d'un flux de fichiers ou d'une référence à un emplacement de disque local.
      2. **SearchCriteria** pour identifier les filigranes spécifiques à supprimer. Cet objet permet de filtrer les filigranes en fonction des propriétés précédemment intégrées dans le document. Vous pouvez utiliser une image comme paramètre de recherche à côté du texte ou des attributs de mise en forme pour une recherche très granulaire.
      3. Après une recherche réussie, vous recevrez une collection de filigranes pertinents. Ces filigranes offrent un contrôle granulaire, vous permettant d'effectuer l'opération de suppression.
      4. Une fois le filigrane supprimé, conservez le document modifié. L'API facilite le stockage à l'aide d'un chemin de fichier local ou d'un objet de flux.
   
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
        // Supprimer le filigrane de l'image dans le document PPTX

        // Instanciez un filigrane en transmettant le document PPTX
        using (Watermarker watermarker = new Watermarker("input.pptx"))
        {
            // Supprimer les filigranes trouvés dans le document
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria(logo.png);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            possibleWatermarks.Remove(watermarks[0]);

            // Enregistrez le document
            watermarker.Save("output.pptx");
        }
        
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "Suppression avancée des filigranes avec l'API C# .NET | GroupDocs.Watermark"
  description: "Débloquez des fonctionnalités avancées de suppression des filigranes grâce à notre API C# .NET. Conçue pour une intégration parfaite avec .NET applications, cette API facilite la suppression des filigranes des PDF s et des documents Office, garantissant ainsi des sorties non marquées de haute qualité destinées à un usage professionnel."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "Supprimer le filigrane"
  features:
    # feature loop
    - title: "Suppression précise des filigranes dans .NET"
      content: "Notre API C# est conçue pour permettre une suppression précise des filigranes, garantissant ainsi que vos documents conservent leur qualité et leur format d'origine. Idéal pour les documents juridiques, éducatifs et professionnels où la clarté et l'authenticité sont cruciales."

    # feature loop
    - title: "Automatisez la suppression des filigranes par C#"
      content: "Améliorez l'efficacité de votre application grâce à des fonctionnalités de suppression automatique des filigranes. Notre API permet de traiter de nombreux lots de documents, ce qui facilite les opérations à grande échelle sans compromettre les performances."

    # feature loop
    - title: "Modifier et effacer les filigranes de manière dynamique"
      content: "Bénéficiez de la flexibilité nécessaire pour modifier dynamiquement ou supprimer complètement les filigranes selon les besoins de votre application. Cette fonctionnalité prend en charge diverses options de personnalisation, permettant à .NET développeurs de préserver l'esthétique et l'intégrité des documents en fonction de leurs exigences."
      
  code_samples:
    # code sample loop
    - title: "Filigrane d'arrière-plan de la présentation supprimer"
      content: |
        Cet exemple montre comment supprimer l'image d'arrière-plan d'une diapositive particulière.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Charger la présentation
            var loadOptions = new PresentationLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pptx", loadOptions))
            {
                //  Obtenir le contenu de la présentation
                PresentationContent content = watermarker.GetContent<PresentationContent>();

                //  Supprimer le filigrane d'arrière-plan de la diapositive
                content.Slides[0].ImageFillFormat.BackgroundImage = null;

                //  Enregistrer le document
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
    title: "Améliorer PowerPoint présentations avec C# .NET"
    exclude: "PPTX"
    description: "Découvrez comment l'API GroupDocs.Watermark for .NET C# peut vous aider à gérer et à supprimer les filigranes des fichiers PPTX, garantissant ainsi des présentations professionnelles et percutantes."
    items: 
        # format loop 1
        - name: "Filigrane PDF"
          format: "PDF"
          link: "/watermark/net/remove//pdf/"
          description: "Format de document Adobe Portable"

        # format loop 2
        - name: "Filigrane Word"
          format: "WORD"
          link: "/watermark/net/remove//word/"
          description: "MS Word et documents Open Office"
          
        # format loop 3
        - name: "Filigrane Excel"
          format: "EXCEL"
          link: "/watermark/net/remove//excel/"
          description: "MS Excel et feuilles de calcul Open Office"

        # format loop 4
        - name: "Filigrane PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/remove//powerpoint/"
          description: "MS PowerPoint et présentations Open Office"

        # format loop 5
        - name: "Filigrane DOCX"
          format: "DOCX"
          link: "/watermark/net/remove//docx/"
          description: "Microsoft Word Ouvrir un document XML"
          
        # format loop 6
        - name: "Filigrane PPTX"
          format: "PPTX"
          link: "/watermark/net/remove//pptx/"
          description: "PowerPoint Présentation Open XML"
          
        # format loop 7
        - name: "Filigrane XLSX"
          format: "XLSX"
          link: "/watermark/net/remove//xlsx/"
          description: "Feuille de calcul Microsoft Excel Open XML"

        # format loop 8
        - name: "Filigrane DOC"
          format: "DOC"
          link: "/watermark/net/remove//doc/"
          description: "Microsoft Word 97 - 2007 Documento"

        # format loop 9
        - name: "Filigrane XLS"
          format: "XLS"
          link: "/watermark/net/remove//xls/"
          description: "Classeur Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrane PPT"
          format: "PPT"
          link: "/watermark/net/remove//ppt/"
          description: "PowerPoint Présentation 97-2003"

        # format loop 11
        - name: "Filigrane RTF"
          format: "RTF"
          link: "/watermark/net/remove//rtf/"
          description: "Format de texte enrichi"

---