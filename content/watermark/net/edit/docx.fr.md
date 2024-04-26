
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:39:04
draft: false
lang: fr
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Modifier les filigranes dans Docx fichiers"
head_description: "Modifiez les filigranes dans Docx fichiers avec GroupDocs.Watermark for .NET Applications. Améliorez l'authenticité des documents sans effort."

############################# Header ############################
title: "Modifier Docx filigranes sur tous les fichiers : .NET Polyvalence" 
description: "Personnalisez vos documents en toute confiance à l'aide des applications GroupDocs.Watermark for .NET. Modifiez sans effort les filigranes dans différents formats de fichiers."
subtitle: "GroupDocs.Watermark for .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Téléchargement gratuit Nuget"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Modifier les filigranes dans Docx fichiers :** Modifiez facilement les filigranes dans différents formats de fichiers avec GroupDocs.Watermark for .NET Applications. Personnalisez vos documents en toute confiance et efficacité.

############################# Steps ############################
steps:
    enable: true
    title: "Modifiez par programmation les filigranes dans les documents Docx avec l'API .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** fournit à .NET développeurs une API robuste pour manipuler par programmation les filigranes dans divers Docx documents. Ce guide décrit le processus :
      
      1. **Watermarker**. Le fichier peut être fourni sous la forme d'un flux d'octets, d'un flux de fichiers ou d'une référence à un emplacement de disque local.
      2. **SearchCriteria** pour identifier les filigranes spécifiques nécessitant une modification. Cet objet permet d'identifier les filigranes précédemment incorporés dans le document.
      3. Une fois la recherche exécutée avec succès, vous recevrez une collection de filigranes pertinents. Ces filigranes offrent un contrôle granulaire, vous permettant de modifier des propriétés telles que les dimensions, le positionnement des pages, le contenu du texte, la palette de couleurs, les données d'image, etc.
      4. Une fois les modifications apportées au filigrane, conservez le document modifié. L'API facilite le stockage à l'aide d'un chemin de fichier local ou d'un objet de flux.
   
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
        // Modifier le filigrane de l'image dans DOCX doc

        // Initialiser Watermarker par fichier source
        using (Watermarker watermarker = new Watermarker("input.docx"))
        {
            // Créer des critères de recherche pour la recherche de filigranes d'images
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                // Modifier le filigrane de l'image
                watermark.ImageData = imageData;
            }

            // Enregistrer le résultat DOCX
            watermarker.Save("output.docx");
        }
        
        ```     

############################# More features ############################
more_features:
  enable: true
  title: "Boostez vos flux de travail grâce à la gestion des filigranes"
  description: "Simplifiez le filigrane dans divers formats de fichiers dans vos applications .NET grâce à notre bibliothèque robuste. Ajoutez, modifiez, recherchez ou supprimez facilement des filigranes pour améliorer la sécurité des documents et améliorer l'image de marque."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Édition fluide des filigranes"
  features:
    # feature loop
    - title: "Simplifiez le filigrane dans vos applications"
      content: "Tirez parti de la puissance de GroupDocs.Watermark for .NET pour intégrer de manière fluide la fonctionnalité de filigrane à vos .NET applications. Notre API intuitive simplifie la création, la gestion, la recherche et la modification de filigranes, éliminant ainsi le besoin de processus manuels complexes."

    # feature loop
    - title: "Personnalisation granulaire du filigrane"
      content: "Exploitez tout le potentiel de la personnalisation des filigranes grâce à notre API complète. Ajustez chaque détail, notamment la taille, l'orientation, la palette de couleurs et la sélection de la police, pour créer des filigranes parfaitement adaptés à votre image de marque et à vos exigences de sécurité."

    # feature loop
    - title: "Exploitez les fonctionnalités spécifiques aux documents pour un filigrane flexible"
      content: "Exploitez la puissance des fonctionnalités natives de différents formats de documents. Utilisez des éléments tels que l'arrière-plan du document, des annotations, des en-têtes ou d'autres objets en tant que conteneurs de filigranes uniques, répondant à divers types de documents et à des besoins de sécurité."
      
  code_samples:
    # code sample loop
    - title: "PDF modification du filigrane de l'image"
      content: |
        Cet exemple montre comment modifier le contenu d'un filigrane d'image
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Charger le document sous le nom PDF
            var loadOptions = new PdfLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pdf", loadOptions))
            {
                //  Charger du contenu
                PdfContent pdfContent = watermarker.GetContent<PdfContent>();

                //  Modifier le filigrane de l'image
                foreach (PdfArtifact artifact in pdfContent.Pages[0].Artifacts)
                {
                    if (artifact.Image != null)
                    {
                        artifact.Image = new PdfWatermarkableImage(File.ReadAllBytes("test.png"));
                    }
                }

                //  Profitez du résultat de sortie
                watermarker.save("result.pdf");
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
    title: "Modifier les filigranes d'un fichier à l'autre"
    exclude: "DOCX"
    description: "Modifiez facilement les filigranes dans de nombreux formats de fichiers grâce aux applications optimisées par GroupDocs.Watermark for .NET."
    items: 
        # format loop 1
        - name: "Filigrane PDF"
          format: "PDF"
          link: "/watermark/net/edit//pdf/"
          description: "Format de document Adobe Portable"

        # format loop 2
        - name: "Filigrane Word"
          format: "WORD"
          link: "/watermark/net/edit//word/"
          description: "MS Word et documents Open Office"
          
        # format loop 3
        - name: "Filigrane Excel"
          format: "EXCEL"
          link: "/watermark/net/edit//excel/"
          description: "MS Excel et feuilles de calcul Open Office"

        # format loop 4
        - name: "Filigrane PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/edit//powerpoint/"
          description: "MS PowerPoint et présentations Open Office"

        # format loop 5
        - name: "Filigrane DOCX"
          format: "DOCX"
          link: "/watermark/net/edit//docx/"
          description: "Microsoft Word Ouvrir un document XML"
          
        # format loop 6
        - name: "Filigrane PPTX"
          format: "PPTX"
          link: "/watermark/net/edit//pptx/"
          description: "PowerPoint Présentation Open XML"
          
        # format loop 7
        - name: "Filigrane XLSX"
          format: "XLSX"
          link: "/watermark/net/edit//xlsx/"
          description: "Feuille de calcul Microsoft Excel Open XML"

        # format loop 8
        - name: "Filigrane DOC"
          format: "DOC"
          link: "/watermark/net/edit//doc/"
          description: "Microsoft Word 97 - 2007 Documento"

        # format loop 9
        - name: "Filigrane XLS"
          format: "XLS"
          link: "/watermark/net/edit//xls/"
          description: "Classeur Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrane PPT"
          format: "PPT"
          link: "/watermark/net/edit//ppt/"
          description: "PowerPoint Présentation 97-2003"

        # format loop 11
        - name: "Filigrane RTF"
          format: "RTF"
          link: "/watermark/net/edit//rtf/"
          description: "Format de texte enrichi"

---