
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:24
draft: false
lang: fr
format: Doc
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Modifiez facilement les filigranes au format Doc"
head_description: "Modifiez facilement Doc filigranes avec l'API GroupDocs.Watermark for .NET. Personnalisez vos documents en toute confiance et efficacité."

############################# Header ############################
title: "Modifiez facilement Doc filigranes avec .NET" 
description: "Simplifiez la gestion des filigranes et protégez vos documents grâce à l'API GroupDocs.Watermark for .NET. Bénéficiez de la polyvalence et de l'efficacité de votre flux de travail."
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Téléchargez le package depuis Nuget"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET Cadre"
    link: "/watermark/net/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Modifiez facilement les filigranes :** Simplifiez la gestion des filigranes sur Doc documents grâce à notre solution conviviale .NET. Concentrez-vous sur votre contenu tout en garantissant la sécurité et l'intégrité des documents sans effort.

############################# Steps ############################
steps:
    enable: true
    title: "Modifiez par programme les filigranes dans les documents Doc avec l'API .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** fournit aux développeurs .NET une API robuste pour manipuler par programmation les filigranes dans divers documents Doc. Ce guide décrit le processus :
      
      1. Lancez le flux de travail en fournissant votre fichier Doc comme argument au constructeur de classe **Watermarker**. Le fichier peut être fourni sous forme de flux d'octets, de flux de fichiers ou de référence à un emplacement de disque local.
      2. Ensuite, exploitez l'objet **SearchCriteria** pour identifier les filigranes spécifiques nécessitant une modification. Cet objet permet d'identifier les filigranes préalablement incrustés dans le document.
      3. Une fois la recherche exécutée avec succès, vous recevrez une collection de filigranes pertinents. Ces filigranes offrent un contrôle granulaire, vous permettant de modifier des propriétés telles que les dimensions, le positionnement de la page, le contenu du texte, la palette de couleurs, les données d'image, etc.
      4. Une fois les modifications du filigrane terminées, conservez le document modifié. L'API facilite le stockage en utilisant soit un chemin de fichier local, soit un objet de flux.
   
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
        // Modifier le filigrane de l'image dans le document DOC

        // Initialiser Watermarker par fichier source
        using (Watermarker watermarker = new Watermarker("input.doc"))
        {
            // Créez SearchCriteria pour la recherche de filigranes d'images
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                // Modifier le filigrane de l'image
                watermark.ImageData = imageData;
            }

            // Enregistrer le résultat DOC
            watermarker.Save("output.doc");
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
    title: "Gérez facilement les filigranes dans d'autres formats"
    exclude: "DOC"
    description: "Simplifiez l'édition des filigranes dans divers formats de documents à l'aide de GroupDocs.Watermark for .NET."
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