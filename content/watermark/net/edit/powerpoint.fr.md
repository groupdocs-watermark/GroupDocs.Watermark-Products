
---
############################# Static ############################
layout: "format"
date:  2024-05-07T12:13:17
draft: false
lang: fr
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Modifier les filigranes dans Powerpoint documents"
head_description: "Simplifiez l'édition des filigranes Powerpoint et protégez vos documents avec GroupDocs.Watermark for .NET Library. Bénéficiez d'un contrôle précis et d'une grande polyvalence."

############################# Header ############################
title: "Modifier Powerpoint Placement des filigranes : .NET Précision" 
description: "Contrôlez avec précision le placement des filigranes et la sécurité des documents grâce à la solution GroupDocs.Watermark for .NET. Modifiez les filigranes Powerpoint avec précision."
subtitle: "GroupDocs.Watermark for .NET Bibliothèque" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Télécharger à Nuget"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET API"
    link: "/watermark/net/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Modifier le placement des filigranes Powerpoint :** Contrôlez avec précision le placement des filigranes et la sécurité des documents avec GroupDocs.Watermark for .NET développeurs. Simplifiez votre flux de travail et garantissez l'authenticité sans effort.

############################# Steps ############################
steps:
    enable: true
    title: "Modifiez les filigranes dans les documents Powerpoint à l'aide de .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** permet aux développeurs .NET de modifier sans effort les filigranes dans divers documents Powerpoint. Voici un guide simplifié sur la façon d'utiliser notre API dans votre application :
      
      1. Commencez par transmettre votre fichier Powerpoint en tant que paramètre au constructeur de classe **Watermarker**. Vous pouvez fournir le fichier sous forme de flux d'octets, de flux de fichiers ou de chemin d'accès au disque local.
      2. Ensuite, localisez les filigranes spécifiques qui nécessitent une modification. Utilisez le **SearchCriteria** pour identifier les filigranes avec les propriétés correspondantes précédemment ajoutées au document.
      3. Suite à la recherche, vous obtiendrez une liste de filigranes pertinents. Vous pouvez ensuite personnaliser leurs propriétés, telles que la taille, l'alignement des pages, le texte, la couleur, le contenu de l'image, etc. Cela vous accorde un contrôle étendu sur vos données.
      4. Une fois que vous avez terminé de modifier les filigranes, enregistrez le document mis à jour. Vous pouvez utiliser un chemin de fichier local ou un flux pour stocker le résultat final.
   
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
        // Modifier le filigrane de texte POWERPOINT

        // Créer Watermarker fournissant un fichier POWERPOINT
        using (Watermarker watermarker = new Watermarker("input.pptx"))
        {
            // Construisez le TextSearchCriteria et obtenez des filigranes de texte
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                 // Modifier le filigrane du texte
                 watermark.FormattedTextFragments.Clear();
                 watermark.FormattedTextFragments.Add("passed", 
                    new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
            }

            // Enregistrez le document
            watermarker.Save("output.pptx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "En savoir plus sur la modification des filigranes"
  description: "Renforcez vos applications .NET grâce à notre bibliothèque et ajoutez, modifiez, supprimez ou recherchez des filigranes dans différents formats de fichiers."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Modifier le filigrane"
  features:
    # feature loop
    - title: "Fichiers filigranes pour votre entreprise"
      content: "Utilisez GroupDocs.Watermark for .NET pour filigraner des fichiers et des documents. Ajoutez et gérez des filigranes sans effort supplémentaire en implémentant notre API dans vos applications. Recherchez, modifiez et supprimez les filigranes ajoutés précédemment."

    # feature loop
    - title: "Ajustez les filigranes en fonction de vos besoins"
      content: "Notre API propose un ensemble complet d'options de personnalisation. Modifiez sans effort des aspects tels que la taille, l'orientation, la palette de couleurs, la famille de polices, etc. pour créer le filigrane idéal."

    # feature loop
    - title: "Tirez parti des fonctionnalités spécifiques aux documents"
      content: "Selon le format de fichier que vous utilisez, vous pouvez intégrer des fonctionnalités intégrées. Il peut s'agir de l'arrière-plan du document, d'annotations, d'en-têtes ou d'autres éléments servant de conteneurs de filigranes."
      
  code_samples:
    # code sample loop
    - title: "Excel modification du texte du filigrane"
      content: |
        Cet exemple montre comment modifier le texte de certains filigranes dans Excel feuilles de travail
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Charger la feuille de calcul XLSX
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  Charger le contenu d'une feuille de calcul
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();

                //  Modifier le texte intérieur du filigrane
                foreach (SpreadsheetShape shape in content.Worksheets[0].Shapes)
                {
                    if (shape.Text == "GroupDocs 2016")
                    {
                        shape.Text = "GroupDocs 2017";
                    }
                }

                //  Enregistrer le résultat de sortie
                watermarker.save("result.xlsx");
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
    title: "Affiner les filigranes dans d'autres formats"
    exclude: "POWERPOINT"
    description: "Modifiez les filigranes dans différents formats de document avec GroupDocs.Watermark for .NET."
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