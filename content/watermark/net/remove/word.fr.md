
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:19
draft: false
lang: fr
format: Word
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "API C# .NET pour la suppression du filigrane Word"
head_description: "Effacez, supprimez ou modifiez efficacement les filigranes de Word documents à l'aide de notre API C# .NET pour une présentation parfaite des documents."

############################# Header ############################
title: "Word Suppresseur de filigrane pour C# .NET" 
description: "Utilisez l'API GroupDocs.Watermark for .NET C# pour supprimer les filigranes des documents Word, ce qui est idéal pour préserver l'intégrité et la propreté des documents juridiques et d'entreprise."
subtitle: "GroupDocs.Watermark for .NET C# ET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Téléchargez gratuitement sur Nuget"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "bibliothèque GroupDocs.Watermark for .NET C#"
    link: "/watermark/net/"
    link_title: "En savoir plus"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       Grâce à la bibliothèque GroupDocs.Watermark for .NET C# .NET, les développeurs peuvent facilement gérer et supprimer les filigranes dans les fichiers Microsoft Word. Cet outil prend en charge un large éventail d'opérations de filigrane, notamment la détection, la modification et la suppression des filigranes de texte et d'image, garantissant ainsi que les documents sont exempts de marques indésirables tout en préservant la mise en page et la mise en forme.

############################# Steps ############################
steps:
    enable: true
    title: "Supprimer les filigranes des documents Word à l'aide de .NET"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/)** simplifie la tâche de suppression des filigranes des documents professionnels. Renforcez votre application .NET en intégrant notre bibliothèque et suivez ces étapes simples :
      
      1. Commencez par instancier la classe principale, **Watermarker**, avec le document Word. Notre API prend en charge le traitement des documents fournis sous forme de flux ou de chemin local.
      2. Utilisez **SearchCriteria** pour affiner l'ensemble des filigranes à traiter. Vous pouvez utiliser divers paramètres tels que des images, du texte ou des fonctionnalités de formatage. Plus les paramètres de recherche que vous fournissez sont précis, plus les résultats que vous obtenez sont précis.
      3. Traitez la liste des filigranes de document obtenue en tant que résultat de recherche et supprimez-les du document.
      4. Après avoir supprimé les filigranes, enregistrez le document résultant en tant que fichier local ou flux d'octets.
   
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
        // Supprimer le filigrane de texte du document Word

        // Fournir une instance Watermarker pour le document Word document source
        using (Watermarker watermarker = new Watermarker("input.docx"))
        {
            // Supprimer les filigranes sélectionnés du document
            TextFormattingSearchCriteria criteria = new TextFormattingSearchCriteria();
            criteria.ForegroundColorRange = new ColorRange();
            criteria.FontBold = true;
            PossibleWatermarkCollection watermarks = watermarker.Search(criteria);
            watermarks.Clear();

            // Enregistrer le fichier dans le chemin fourni
            watermarker.Save("output.docx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Simplifiez la suppression des filigranes avec l'API C# .NET"
  description: "Découvrez les puissantes fonctionnalités de suppression des filigranes de notre API C# .NET, conçue pour s'intégrer parfaitement à vos applications .NET. Supprimez ou effacez les filigranes des PDF et des documents Office de manière efficace tout en préservant la qualité du fichier d'origine."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "Supprimer le filigrane"
  features:
    # feature loop
    - title: "Élimination précise des filigranes"
      content: "Notre API .NET fournit des outils précis pour supprimer proprement les filigranes de n'importe quel document. Conçue pour les développeurs, cette fonctionnalité garantit que la suppression des filigranes ne compromet pas la qualité ou la mise en page du document."

    # feature loop
    - title: "Automatisez la suppression en masse des filigranes"
      content: "Automatisez le processus de suppression des filigranes des grands ensembles de documents grâce à notre API .NET. Idéal pour les entreprises qui gèrent de gros volumes de documents, améliorant à la fois l'efficacité et la sécurité des documents."

    # feature loop
    - title: "Fonctionnalités avancées d'édition des filigranes"
      content: "Tirez parti des fonctionnalités avancées pour supprimer ou modifier les filigranes de manière sélective. Notre API prend en charge des ajustements détaillés pour garantir que vos documents conservent une apparence professionnelle tout en protégeant les informations sensibles."
      
  code_samples:
    # code sample loop
    - title: "Supprimer le filigrane de texte des feuilles de calcul"
      content: |
        Comment supprimer les filigranes de texte avec une mise en forme spéciale dans Excel docs.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Charger le classeur Excel
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  Accédez au contenu et trouvez le filigrane approprié
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();
                foreach (SpreadsheetWorksheet section in content.Worksheets)
                {
                    for (int i = section.Shapes.Count - 1; i >= 0; i--)
                    {
                        foreach (FormattedTextFragment fragment in section.Shapes[i].FormattedTextFragments)
                        {
                            if (fragment.ForegroundColor.Equals(Color.Red) && fragment.Font.FamilyName == "Arial")
                            {
                                //  Supprimer le filigrane de texte
                                section.Shapes.RemoveAt(i);
                                break;
                            }
                        }
                    }
                }

                //  Sauvegarde traitée XLSX
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
    title: "Gérer Word filigranes avec .NET"
    exclude: "WORD"
    description: "Explorez de puissantes fonctionnalités de gestion des filigranes dans Word documents à l'aide de notre API C# .NET, conçue pour améliorer la sécurité et la présentation des documents sans compromettre la qualité."
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