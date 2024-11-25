---
############################# Static ############################
layout: "family"
date:  2024-11-25T09:49:28
draft: false

product: "Watermark"
product_tag: "watermark"

lang: fr

############################# Head ############################
head_title: "Filigrane de document C# Java Node.js Python | Ajouter un filigrane"
head_description: "Ajoutez un filigrane à PDF, à des images et à des documents. Solution de filigrane pour Microsoft Office, PDF, OpenDocument, images, etc."

############################# Header ############################
title: "Solution de filigrane pour documents"
description:  |
  Ajoutez des filigranes de texte et d'image à vos documents et images.

  Recherchez et modifiez les filigranes des documents de manière pratique.

  Obtenez des informations sur les filigranes présentés dans vos documents.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Choisissez votre plateforme"
  title: "Indépendance de la plateforme"
  description: "La bibliothèque GroupDocs.Watermark prend en charge les systèmes d'exploitation et les frameworks suivants :"
  details_link_title: "En savoir plus"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Watermark .NET 
      color: "blue"
      tag: "net"
      link: "/watermark/net/"
      features_link: "https://docs.groupdocs.com/watermark/net/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    .NET Framework 4.5 or higher <br> .NET Core 3.0 or higher <br> .NET 5.0 or higher
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Watermark Java
      color: "red"
      tag: "java"
      link: "/watermark/java/"
      features_link: "https://docs.groupdocs.com/watermark/java/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    Java 8 or higher <br> Kotlin
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Watermark Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/watermark/nodejs-java/"
      features_link: "https://docs.groupdocs.com/watermark/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Tout autre éditeur de texte
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Python"
      description: GroupDocs.Watermark Python
      color: "yellow"
      tag: "python-net"
      link: "/watermark/python-net/"
      features_link: "https://docs.groupdocs.com/watermark/python-net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Python 3.9+ and .Net 6+
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "4"
            content: |
                    IDLE <br> PyCharm <br> Visual Studio Code
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Watermark revue des fonctionnalités"
  description: "La bibliothèque conçue pour ajouter, rechercher et mettre à jour différents types de filigranes pour les formats de documents courants."

  items:
    # items loop
    - icon: "protect"
      title: "Protégez les fichiers avec des filigranes"
      content: "Ajoutez des filigranes de texte et d'image à vos documents professionnels."

    # items loop
    - icon: "search"
      title: "Rechercher des filigranes existants"
      content: "Obtenez des informations détaillées sur les filigranes placés dans le document précédemment."

    # items loop
    - icon: "manipulate"
      title: "Manipuler les filigranes des documents"
      content: "Contrôlez le texte, le style, l'image et les autres fonctionnalités du filigrane."

    # items loop
    - icon: "additional"
      title: "Diverses fonctionnalités supplémentaires"
      content: "Obtenez des informations sur le document, mettez à jour les hyperliens ou l'arrière-plan des pages, etc."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Protégez les documents par des filigranes"
  description: "GroupDocs.Watermark exemples de code d'opérations typiques."
  items:
    # code sample loop
    - title: "Création d'un filigrane."
      content: |
       Pour ajouter un filigrane à un document, indiquez le chemin du fichier cible. Vous avez le choix entre de nombreuses options pour obtenir un filigrane personnalisé sur une page spécifique.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Spécifiez le document à filigraner
            using (Watermarker watermarker = new Watermarker("source.docx"))
            {
                // Créer un objet en filigrane
                TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                // Définir les options de filigrane
                watermark.ForegroundColor = Color.Red;
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;

                // Ajouter un filigrane et enregistrer le fichier traité
                watermarker.Add(watermark);
                watermarker.Save("result.docx");
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Spécifiez le document à filigraner
            Watermarker watermarker = new Watermarker("source.docx");

            // Créer un objet en filigrane
            TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

            // Définir les options de filigrane
            watermark.setForegroundColor(Color.getRed());
            watermark.setHorizontalAlignment(HorizontalAlignment.Center);
            watermark.setVerticalAlignment(VerticalAlignment.Center);

            // Ajouter un filigrane et enregistrer le fichier traité
            watermarker.add(watermark);
            watermarker.save("result.docx");
            watermarker.close();
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            // Spécifiez le document à filigraner
            const watermarker = new Watermarker("source.docx");

            // Créer un objet en filigrane
            const watermark = new TextWatermark("top secret", new Font("Arial", 36));

            // Définir les options de filigrane
            watermark.setForegroundColor(Color.getRed());
            watermark.setHorizontalAlignment(HorizontalAlignment.Center);
            watermark.setVerticalAlignment(VerticalAlignment.Center);

            // Ajouter un filigrane et enregistrer le fichier traité
            watermarker.add(watermark);
            watermarker.save("result.docx");
            ```
        - language: "Python"
          color: "yellow"
          content: |
            ```python {style=abap}  
            def run():
                # Spécifiez le document à filigraner
                with groupdocs.watermark.Watermarker("source.docx") as watermarker:
                    font = groupdocs.watermark.watermarks.Font("Arial", 36.0)

                    # Créer un objet en filigrane
                    watermark = groupdocs.watermark.watermarks.TextWatermark("top secret", font)

                    # Définir les options de filigrane
                    watermark.foreground_color = groupdocs.watermark.watermarks.Color.red;
                    watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
                    watermark.vertical_alignment = groupdocs.watermark.common.VerticalAlignment.CENTER

                    # Ajouter un filigrane et enregistrer le fichier traité
                    watermarker.add(watermark)
                    watermarker.save("result.docx")
            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "Plus de 50 formats de fichiers pris en charge"
  description: "GroupDocs.Watermark fournit un filigrane pour les formats de documents et de fichiers courants."

############################# Metrics ###############################
metrics:
  enable: true
  title: "Données statistiques de notre bibliothèque"
  description: "Explorez en profondeur les indicateurs clés et découvrez un aperçu de nos réalisations, de notre impact et de notre croissance."

  items:
    # items loop
    - number: "50+"
      title: "Formats pris en charge"
      content: "La bibliothèque est capable de traiter plus de 50 des formats de fichiers les plus populaires."

    # items loop
    - number: "500k"
      title: "NuGet téléchargements"
      content: "GroupDocs.Watermark pour .NET est une bibliothèque populaire qui compte plus de 500 000 téléchargements sur NuGet."

    # items loop
    - number: "15k"
      title: "Téléchargements de Maven"
      content: "Avec plus de 15 000 téléchargements sur Maven, GroupDocs.Watermark est un choix populaire pour Java développeurs."

    # items loop
    - number: "140+"
      title: "Des clients satisfaits"
      content: "Les développeurs individuels et les plus grandes entreprises du monde entier préfèrent nos bibliothèques pour créer des solutions innovantes."


############################# Customers ###############################
customers:
  enable: true
  title: "Nos clients satisfaits"
  description: "GroupDocs bibliothèques sont utilisées par des marques renommées et distinguées à travers le monde."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Prêt à démarrer ?"
  description: "Essayez GroupDocs.Watermark fonctionnalités gratuitement sur votre plateforme"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/watermark/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/watermark/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/watermark/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "Questions fréquemment posées"
  description: "Consultez nos questions fréquemment posées"

  items:
    # items loop
    - question: "Des bibliothèques externes sont-elles requises par GroupDocs.Watermark pour manipuler des documents ?"
      answer: "GroupDocs.Watermark fonctionne indépendamment, aucun logiciel tiers comme Adobe Acrobat, Microsoft Office, etc. n'est nécessaire."

    # items loop
    - question: "Puis-je tester les fonctionnalités de GroupDocs.Watermark avant d'acheter ?"
      answer: "Oui, GroupDocs.Watermark propose un essai gratuit ! Installez-le et essayez-le, mais n'oubliez pas : les versions d'essai ajoutent des « badges d'essai » à vos documents, seules les 3 premières pages sont traitées. Vous voulez vivre une expérience complète ? Obtenez une licence temporaire gratuite de 30 jours pour bénéficier de toutes les fonctionnalités. Voir les détails sous [licence temporaire](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Quels sont les types de licences proposés ?"
      answer: "Vous avez besoin d'une licence GroupDocs.Watermark ? Nous avons des options ! Choisissez parmi les licences proposées parmi de nombreuses options. Nombre de développeurs dans votre équipe. Lieux de déploiement tels que des bureaux uniques ou des lieux de travail distants. La distribution destinée aux clients finaux doit-elle partager le SDK/API avec les clients ? Il existe également une licence pour une utilisation mensuelle : ne payez que pour ce que vous utilisez avec les forfaits payants. Approfondissez vos connaissances et trouvez le [prix idéal](https://purchase.groupdocs.com/pricing/watermark/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Watermark API à faible code"
  description: "Ajoutez des filigranes aux fichiers par votre application à l'aide de notre API REST basée sur le cloud."
  
  items:
    # items loop
    - title: "GroupDocs.Watermark Cloud for cURL"
      content: "Utilisez l'API complète cURL REST pour filigraner PDF, Word, Excel, PowerPoint, JPEG et d'autres formats de fichiers courants."
      icon: "groupdocs_watermark-for-curl"
      link: "https://products.groupdocs.cloud/watermark/curl"

    # items loop
    - title: "GroupDocs.Watermark Cloud for .NET"
      content: "Renforcez vos applications .NET grâce aux fonctionnalités de filigrane des documents proposées par Cloud SDK pour .NET. Protégez vous-même vos documents commerciaux."
      icon: "groupdocs_watermark-for-net"
      link: "https://products.groupdocs.cloud/watermark/net"

    # items loop
    - title: "GroupDocs.Watermark Cloud for Java"
      content: "Le SDK GroupDocs.Watermark conçu pour Java offre de nouvelles possibilités pour vos Java applications et fichiers professionnels."
      icon: "groupdocs_watermark-for-java"
      link: "https://products.groupdocs.cloud/watermark/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Watermark Applications Web"
  description: "GroupDocs donne accès à une application Web permettant d'ajouter des filigranes à vos documents. Plus de 50 formats de fichiers populaires peuvent être filigranés GRATUITEMENT dans votre navigateur préféré."

  items:
    # items loop
    - title: "GroupDocs.Watermark Total"
      content: "Outil en ligne pour ajouter des filigranes à des documents depuis n'importe quel appareil."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/watermark/total"

    # items loop
    - title: "GroupDocs.Watermark DOCX"
      content: "Filigrane MS Word DOCX en ligne."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/watermark/docx"

    # items loop
    - title: "GroupDocs.Watermark PDF"
      content: "Protégez PDF documents en ligne."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/watermark/pdf"


      


---