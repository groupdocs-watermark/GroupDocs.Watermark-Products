---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:48
draft: false

lang: fr
product: "Watermark"
product_tag: "watermark"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"
    # supported_platforms loop
    - title: "Python"
      tag: "python-net"

############################# Head ############################
head_title: "Logiciel de filigrane de documents C# .NET | ajouter un filigrane"
head_description: "Bibliothèque C# .NET pour ajouter, rechercher et supprimer des filigranes dans les documents : PDF, Word, Excel, présentations, Visio diagrammes, e-mails et formats de fichiers image."

############################# Header ############################
title: "Ajoutez facilement des filigranes à vos documents dans vos applications C# .NET"
description: "Renforcez vos solutions C# grâce à une API flexible de filigrane de documents qui permet d'ajouter des filigranes personnalisables à tous les formats de documents courants."
words:
  for: "pour"

actions:
  main: "Télécharger gratuitement NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Watermark"
  alt: "Licences"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/net/"
  title: "Prêt à démarrer ?"
  description: "Essayez GroupDocs.Watermark fonctionnalités gratuitement ou demandez une licence"

release:
  title: "Version {0} publiée"
  notes: "Découvrez les nouveautés"
  downloads: "Téléchargements"

code:
  title: "Filigrane PDF fichiers en C#"
  more: "Plus d'exemples"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
  install: "dotnet add package GroupDocs.Watermark"
  content: |
    ```csharp {style=abap}   
    // Instanciez un filigrane en passant le chemin PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    using (Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions))
    {
        // Personnalisez les options de filigrane
        TextWatermark textWatermark = 
            new TextWatermark("Approved", new Font("Arial", 8));
        
        // Appliquer un filigrane au document PDF
        watermarker.Add(textWatermark);

        // Enregistrer le document de résultats
        watermarker.Save("result.pdf");
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark en un coup d'œil"
  description: "API pour mettre des filigranes sur les documents via .NET"
  features:
    # feature loop
    - title: "Filigrane de fichiers C#"
      content: "Ajoutez des filigranes à vos fichiers professionnels à l'aide de GroupDocs.Watermark. Utilisez du texte, des images, des diagrammes ou des pièces jointes à un e-mail."

    # feature loop
    - title: "Personnalisez les filigranes en fonction de vos objectifs"
      content: "Le logiciel GroupDocs.Watermark for .NET permet de personnaliser les filigranes de différentes manières. Les styles de texte tels que le gras, l'italique, les types de police ainsi que les propriétés de l'image telles que la rotation, etc. enrichissent le processus de filigrane."

    # feature loop
    - title: "Tous les formats de fichiers courants sont pris en charge"
      content: "De nombreux formats de fichiers et de documents sont pris en charge par la solution GroupDocs.Watermark. PDF, Microsoft Office Word, Excel, PowerPoint, les images telles que JPEG, PNG, GIF, BMP, Visio diagrammes, e-mails, etc. peuvent être protégés par nos filigranes."

    # feature loop
    - title: "Rechercher et mettre à jour des filigranes"
      content: "Les filigranes déjà présents dans un document peuvent être trouvés et traités à nouveau. Modifiez le texte, le style, les images ou supprimez les filigranes révélés sans effort supplémentaire."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indépendance de la plateforme"
  description: "GroupDocs.Watermark for .NET prend en charge les systèmes d'exploitation, les frameworks et les gestionnaires de packages répertoriés ci-dessous"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Formats de fichiers pris en charge"
  description: |
    GroupDocs.Watermark for .NET assure le traitement des [formats de fichiers suivants](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### formats Microsoft Office et OpenDocument
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### Images et graphiques
        * **Formats d'image populaires:** BMP, JPG, JPEG, PNG
        * **Images de plusieurs pages:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### Autres
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark fonctionnalités"
  description: "Protégez PDF, Office, Images et autres formats par un filigrane"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Filigrane de documents"
      content: "Ajoutez ou supprimez des filigranes d'une section particulière ou d'un document entier de différents formats de fichiers."

    # feature loop
    - icon: "watermark_style"
      title: "Personnalisez votre filigrane"
      content: "Personnalisez diverses propriétés du filigrane comme la couleur, la police, la rotation, etc."

    # feature loop
    - icon: "hidden_print"
      title: "PDF filigrane d'impression masqué"
      content: "Attribuez un filigrane masqué à PDF qui n'apparaît que lors de l'impression du document."

    # feature loop
    - icon: "image_only"
      title: "Filigrane uniquement les images dans les documents"
      content: "Ajoutez un filigrane à toutes les images d'une section, d'une page, d'une diapositive ou d'un document en particulier."

    # feature loop
    - icon: "image_frame"
      title: "Traiter les images sélectionnées"
      content: "Attribuez un filigrane uniquement à certains cadres d'une image comportant plusieurs cadres."

    # feature loop
    - icon: "attachments"
      title: "Pièces jointes et formes"
      content: "Définissez un filigrane sur toutes les pièces jointes d'un document Excel et sur toutes les formes d'image des diapositives."

    # feature loop
    - icon: "pdf_objects"
      title: "PDF objets"
      content: "Alignez le filigrane sur la zone de fond, la zone artistique, la zone de recadrage ou la zone de découpe dans le document PDF."

    # feature loop
    - icon: "doc_background"
      title: "Contexte des documents"
      content: "Placez un filigrane ou supprimez-le des images d'arrière-plan d'une feuille de calcul ou de diapositives."

    # feature loop
    - icon: "unreadable_characters"
      title: "Protection contre les caractères illisibles"
      content: "Protégez le filigrane de texte à l'aide de caractères illisibles dans les présentations."

    # feature loop
    - icon: "watermark_text_search"
      title: "Rechercher des filigranes dans les documents"
      content: "Recherchez des filigranes en fonction de paramètres spécifiques ou en combinant plusieurs critères."

    # feature loop
    - icon: "watermark_image_search"
      title: "Rechercher des filigranes d'images similaires"
      content: "Recherchez les filigranes qui ressemblent à une image en particulier."

    # feature loop
    - icon: "document_info"
      title: "Obtenir des informations sur le document"
      content: "Extrayez par programmation la mise en page et d'autres informations pour les formats pris en charge."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de code"
  description: "Quelques cas d'utilisation d'opérations typiques de GroupDocs.Watermark for .NET"
  items:
    # code sample loop
    - title: "Filigrane en ajoutant une image à un document."
      content: |
        Pour protéger n'importe quel document, vous pouvez utiliser [filigranes d'image](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/) :
        {{< landing/code title="Comment protéger un fichier par filigrane d'image.">}}
        ```csharp {style=abap}
        // Charger le document source dans Watermarker
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Spécifier le chemin d'accès à une image en filigrane
            using (ImageWatermark watermark = new ImageWatermark("watermark.jpg"))
            {
                // Protégez le fichier et enregistrez-le
                watermarker.Add(watermark);

                watermarker.Save("result.pdf");
            }
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Recherchez et modifiez les filigranes existants."
      content: |
        GroupDocs.Watermark est capable de [modifier les filigranes](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/) qui sont déjà présentés dans un document. Recherchez les articles souhaités et mettez à jour leurs propriétés.
        {{< landing/code title="Recherche et modification de filigranes.">}}
        ```csharp {style=abap}   
        // Charger le document source
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Rechercher les filigranes à mettre à jour
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                // Mettre à jour les propriétés souhaitées
                watermark.Text = "New Text";
            }

            // Enregistrer le document modifié dans un chemin spécifié
            watermarker.Save("document.pdf");
        }
        ```
        {{< /landing/code >}}

---
