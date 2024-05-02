---
############################# Static ############################
layout: "family"
date:  2024-04-29T14:27:12
draft: false

product: "Watermark"
product_tag: "watermark"

lang: de

############################# Head ############################
head_title: "Dokument Wasserzeichen C# Java Node.js | Wasserzeichen hinzufügen"
head_description: "Fügen Sie Wasserzeichen zu PDF, Bildern und Dokumenten hinzu. Wasserzeichen-Lösung für Microsoft Office, PDF, OpenDocument, Bilder usw."

############################# Header ############################
title: "Wasserzeichen-Lösung für Dokumente"
description:  |
  Fügen Sie Text- und Bildwasserzeichen für Ihre Dokumente und Bilder hinzu.

  Suchen und ändern Sie Dokumentwasserzeichen auf bequeme Weise.

  Informieren Sie sich über Wasserzeichen, die in Ihren Dokumenten enthalten sind.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Wähle deine Plattform"
  title: "Plattformunabhängigkeit"
  description: "Die GroupDocs.Watermark -Bibliothek unterstützt die folgenden Betriebssysteme und Frameworks:"
  details_link_title: "Erfahre mehr"

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
                    .NET Framework 4.6.2 or higher <br> .NET Core 2.0 or higher <br> .NET 6.0 or higher
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider
      
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
                    Atom <br> Visual Studio Code <br> Jeder andere Texteditor
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Watermark Funktionsüberprüfung"
  description: "Die Bibliothek wurde entwickelt, um verschiedene Wasserzeichentypen für gängige Dokumentformate hinzuzufügen, zu suchen und zu aktualisieren."

  items:
    # items loop
    - icon: "protect"
      title: "Dateien mit Wasserzeichen schützen"
      content: "Fügen Sie Text- und Bildwasserzeichen an Ihre Geschäftsdokumente an."

    # items loop
    - icon: "search"
      title: "Suchen Sie nach vorhandenen Wasserzeichen"
      content: "Holen Sie sich detaillierte Informationen zu Wasserzeichen, die zuvor in einem Dokument platziert wurden."

    # items loop
    - icon: "manipulate"
      title: "Bearbeiten Sie die Wasserzeichen von Dokumenten"
      content: "Steuern Sie Text, Stil, Bild und andere Wasserzeichenfunktionen."

    # items loop
    - icon: "additional"
      title: "Verschiedene zusätzliche Funktionen"
      content: "Holen Sie sich Dokumentinformationen, aktualisieren Sie Hyperlinks oder den Seitenhintergrund usw."

############################# Code Samples ###############################
code_samples:
  enable: true
  title: "Dokumente durch Wasserzeichen schützen"
  description: "GroupDocs.Watermark Codebeispiele für typische Operationen."

  items:
    # items loop
    - title: "Erstellen eines Wasserzeichens."
      content: "Um ein Wasserzeichen an ein Dokument anzuhängen, geben Sie den Pfad zur Zieldatei an. Sie haben viele Optionen zur Auswahl, um ein benutzerdefiniertes Wasserzeichen auf einer bestimmten Seite zu erhalten."
      samples:
          # samples loop
          - language: "C#"
            color: "blue"
            content: |
                    <code class="language-csharp" data-lang="csharp">
                        // Geben Sie das Dokument an, das mit einem Wasserzeichen versehen werden soll

                        using (Watermarker watermarker = new Watermarker("source.docx"))
                        {
                          // Wasserzeichen-Objekt erstellen
                          TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                          // Wasserzeichenoptionen festlegen
                          watermark.ForegroundColor = Color.Red;
                          watermark.HorizontalAlignment = HorizontalAlignment.Center;
                          watermark.VerticalAlignment = VerticalAlignment.Center;

                          // Wasserzeichen hinzufügen und verarbeitete Datei speichern
                          watermarker.Add(watermark);
                          watermarker.Save("result.docx");
                        }                    
                    </code>

          # samples loop
          - language: "Java"
            color: "red"
            content: |
                    <code class="language-java" data-lang="java">
                        // Geben Sie das Dokument an, das mit einem Wasserzeichen versehen werden soll

                        Watermarker watermarker = new Watermarker("source.docx");

                        // Wasserzeichen-Objekt erstellen
                        TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // Wasserzeichenoptionen festlegen
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // Wasserzeichen hinzufügen und verarbeitete Datei speichern
                        watermarker.add(watermark);
                        watermarker.save("result.docx");
                        watermarker.close();

                    </code>

          # samples loop
          - language: "TypeScript"
            color: "green"
            content: |
                    <code class="language-java" data-lang="javascript">
                        // Geben Sie das Dokument an, das mit einem Wasserzeichen versehen werden soll

                        const watermarker = new Watermarker("source.docx");
    
                        // Wasserzeichen-Objekt erstellen
                        const watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // Wasserzeichenoptionen festlegen
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // Wasserzeichen hinzufügen und verarbeitete Datei speichern
                        watermarker.add(watermark);
                        watermarker.save("result.docx");                        

                    </code>

############################# Supported Formats ###############################
formats:
  enable: true
  title: "Über 50 Dateiformate werden unterstützt"
  description: "GroupDocs.Watermark bietet Wasserzeichen für gängige Dokument- und Dateiformate."

############################# Metrics ###############################
metrics:
  enable: true
  title: "Statistische Daten unserer Bibliothek"
  description: "Tauchen Sie tief in die wichtigsten Kennzahlen ein und geben Sie Einblicke in unsere Erfolge, Auswirkungen und unser Wachstum."

  items:
    # items loop
    - number: "50+"
      title: "Unterstützte Formate"
      content: "Die Bibliothek ist in der Lage, mehr als 50 der gängigsten Dateiformate zu verarbeiten."

    # items loop
    - number: "800k"
      title: "NuGet herunterladen"
      content: "GroupDocs.Watermark for .NET ist eine beliebte Bibliothek mit über 800.000 Downloads auf NuGet."

    # items loop
    - number: "15k"
      title: "Maven lädt herunter"
      content: "Mit über 15.000 Downloads auf Maven ist GroupDocs.Watermark eine beliebte Wahl für Java Entwickler."

    # items loop
    - number: "140+"
      title: "Glückliche Kunden"
      content: "Einzelne Entwickler und Top-Unternehmen weltweit bevorzugen unsere Bibliotheken, um innovative Lösungen zu entwickeln."


############################# Customers ###############################
customers:
  enable: true
  title: "Unsere zufriedenen Kunden"
  description: "GroupDocs Bibliotheken sind für weltweit bekannte und angesehene Marken auf der ganzen Welt tätig."

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
  title: "Bereit loszulegen?"
  description: "Testen Sie GroupDocs.Watermark Funktionen kostenlos auf Ihrer Plattform"

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
  title: "Häufig gestellte Fragen"
  description: "Schauen Sie sich unsere häufig gestellten Fragen an"

  items:
    # items loop
    - question: "Werden von GroupDocs.Watermark externe Bibliotheken für die Bearbeitung von Dokumenten benötigt?"
      answer: "GroupDocs.Watermark funktioniert unabhängig, Software von Drittanbietern wie Adobe Acrobat, Microsoft Office usw. ist nicht erforderlich."

    # items loop
    - question: "Kann ich GroupDocs.Watermark Funktionen vor dem Kauf testen?"
      answer: "Ja, GroupDocs.Watermark bietet eine kostenlose Testversion an! Installieren Sie es und probieren Sie es aus, aber denken Sie daran: Testversionen fügen Ihren Dokumenten „Test-Badges“ hinzu, nur die ersten 3 Seiten werden verarbeitet. Willst du das volle Erlebnis? Holen Sie sich eine kostenlose temporäre 30-Tage-Lizenz für den vollen Funktionsumfang. Einzelheiten finden Sie unter [temporäre Lizenz](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Welche Lizenztypen werden angeboten?"
      answer: "Benötigen Sie eine GroupDocs.Watermark -Lizenz? Wir haben Optionen! Wählen Sie aus Lizenzen, die auf vielen Optionen basieren. Anzahl der Entwickler in Ihrem Team. Einsatzorte wie einzelne Büros oder entfernte Arbeitsplätze. Muss der Endkundenvertrieb das SDK/API mit den Kunden teilen? Alternativ gibt es eine Lizenz für die monatliche Nutzung: Bei kostenpflichtigen Tarifen zahlen Sie nur für das, was Sie nutzen. Tauchen Sie tiefer ein und finden Sie den perfekten [Preis](https://purchase.groupdocs.com/pricing/watermark/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Watermark Low-Code-APIs"
  description: "Fügen Sie mithilfe unserer cloudbasierten REST API mithilfe Ihrer Anwendung Wasserzeichen zu Dateien hinzu."
  
  items:
    # items loop
    - title: "GroupDocs.Watermark Cloud for cURL"
      content: "Verwenden Sie die cURL REST ful-API, um PDF, Word, Excel, PowerPoint, JPEG und andere beliebte Dateiformate mit Wasserzeichen zu versehen."
      icon: "groupdocs_watermark-for-curl"
      link: "https://products.groupdocs.cloud/watermark/curl"

    # items loop
    - title: "GroupDocs.Watermark Cloud for .NET"
      content: "Stärken Sie Ihre .NET Anwendungen mit Funktionen zum Wasserzeichen für Dokumente von Cloud SDK für .NET. Schützen Sie Geschäftsdokumente auf eigene Faust."
      icon: "groupdocs_watermark-for-net"
      link: "https://products.groupdocs.cloud/watermark/net"

    # items loop
    - title: "GroupDocs.Watermark Cloud for Java"
      content: "Das für Java entwickelte GroupDocs.Watermark SDK bietet neue Möglichkeiten für Ihre Java Anwendungen und Geschäftsdateien."
      icon: "groupdocs_watermark-for-java"
      link: "https://products.groupdocs.cloud/watermark/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Watermark Webanwendungen"
  description: "GroupDocs gewährt Zugriff auf eine Webanwendung zum Hinzufügen von Wasserzeichen zu Ihren Dokumenten. Mehr als 50 beliebte Dateiformate können in Ihrem Lieblingsbrowser KOSTENLOS mit einem Wasserzeichen versehen werden."

  items:
    # items loop
    - title: "GroupDocs.Watermark Total"
      content: "Online-Tool zum Hinzufügen von Wasserzeichen zu Dokumenten von jedem Gerät aus."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/watermark/total"

    # items loop
    - title: "GroupDocs.Watermark DOCX"
      content: "Wasserzeichen MS Word DOCX online."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/watermark/docx"

    # items loop
    - title: "GroupDocs.Watermark PDF"
      content: "Schützen Sie PDF Dokumente online."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/watermark/pdf"


      


---