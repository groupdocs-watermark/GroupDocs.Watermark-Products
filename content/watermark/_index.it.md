---
############################# Static ############################
layout: "family"
date:  2024-06-26T07:20:48
draft: false

product: "Watermark"
product_tag: "watermark"

lang: it

############################# Head ############################
head_title: "Documento Filigrana C# Java Node.js Python | aggiungi filigrana"
head_description: "Aggiungi filigrana a PDF, immagini e documenti. Soluzione di filigrana per Microsoft Office, PDF, OpenDocument, immagini e così via."

############################# Header ############################
title: "Soluzione Documents Watermark"
description:  |
  Aggiungi filigrane di testo e immagini per i tuoi documenti e immagini.

  Cerca e modifica le filigrane dei documenti in modo conveniente.

  Ottieni informazioni sulle filigrane presenti nei tuoi documenti.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Scegli la tua piattaforma"
  title: "Indipendenza dalla piattaforma"
  description: "La libreria GroupDocs.Watermark supporta i seguenti sistemi operativi e framework:"
  details_link_title: "Scopri di più"

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
      features_link: "https://docs.groupdocs.com/watermark/"
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
                    Atom <br> Visual Studio Code <br> Qualsiasi altro editor di testo
      
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
      features_link: "https://docs.groupdocs.com/watermark/net/system-requirements/"
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
  title: "Recensione delle caratteristiche di GroupDocs.Watermark"
  description: "La libreria progettata per aggiungere, cercare e aggiornare vari tipi di filigrana per i formati di documento più diffusi."

  items:
    # items loop
    - icon: "protect"
      title: "Proteggi i file con filigrane"
      content: "Aggiungi filigrane di testo e immagini ai tuoi documenti aziendali."

    # items loop
    - icon: "search"
      title: "Cerca filigrane esistenti"
      content: "Ottieni informazioni dettagliate sulle filigrane inserite in precedenza nel documento."

    # items loop
    - icon: "manipulate"
      title: "Manipolare le filigrane dei documenti"
      content: "Controlla testo, stile, immagine e altre funzionalità della filigrana."

    # items loop
    - icon: "additional"
      title: "Diverse funzionalità aggiuntive"
      content: "Ottieni informazioni sui documenti, aggiorna i collegamenti ipertestuali o lo sfondo delle pagine, ecc."

############################# Code Samples ###############################
code_samples:
  enable: true
  title: "Proteggi i documenti con filigrane"
  description: "GroupDocs.Watermark esempi di codice operativo tipico."

  items:
    # items loop
    - title: "Creare una filigrana."
      content: "Per aggiungere una filigrana a un documento, fornisci il percorso del file di destinazione. Hai molte opzioni tra cui scegliere per ottenere una filigrana personalizzata su una pagina specifica."
      samples:
          # samples loop
          - language: "C#"
            color: "blue"
            content: |
                    <code class="language-csharp" data-lang="csharp">
                        // Specifica il documento da filigranare

                        using (Watermarker watermarker = new Watermarker("source.docx"))
                        {
                          // Crea un oggetto filigrana
                          TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                          // Imposta le opzioni della filigrana
                          watermark.ForegroundColor = Color.Red;
                          watermark.HorizontalAlignment = HorizontalAlignment.Center;
                          watermark.VerticalAlignment = VerticalAlignment.Center;

                          // Aggiungi filigrana e salva il file elaborato
                          watermarker.Add(watermark);
                          watermarker.Save("result.docx");
                        }                    
                    </code>

          # samples loop
          - language: "Java"
            color: "red"
            content: |
                    <code class="language-java" data-lang="java">
                        // Specifica il documento da filigranare

                        Watermarker watermarker = new Watermarker("source.docx");

                        // Crea un oggetto filigrana
                        TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // Imposta le opzioni della filigrana
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // Aggiungi filigrana e salva il file elaborato
                        watermarker.add(watermark);
                        watermarker.save("result.docx");
                        watermarker.close();

                    </code>

          # samples loop
          - language: "TypeScript"
            color: "green"
            content: |
                    <code class="language-java" data-lang="javascript">
                        // Specifica il documento da filigranare

                        const watermarker = new Watermarker("source.docx");
    
                        // Crea un oggetto filigrana
                        const watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // Imposta le opzioni della filigrana
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // Aggiungi filigrana e salva il file elaborato
                        watermarker.add(watermark);
                        watermarker.save("result.docx");                        

                    </code>

          # samples loop
          - language: "Python"
            color: "yellow"
            content: |
                    <code class="python-net" data-lang="python">
                        def run():

                            # Specifica il documento da filigranare
                            with groupdocs.watermark.Watermarker("source.docx") as watermarker:
                                font = groupdocs.watermark.watermarks.Font("Arial", 36.0)

                                # Crea un oggetto filigrana
                                watermark = groupdocs.watermark.watermarks.TextWatermark("top secret", font)

                                # Imposta le opzioni della filigrana
                                watermark.foreground_color = groupdocs.watermark.watermarks.Color.red;
                                watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
                                watermark.vertical_alignment = groupdocs.watermark.common.VerticalAlignment.CENTER

                                # Aggiungi filigrana e salva il file elaborato
                                watermarker.add(watermark)
                                watermarker.save("result.docx")

                    </code>

############################# Supported Formats ###############################
formats:
  enable: true
  title: "Oltre 50 formati di file supportati"
  description: "GroupDocs.Watermark fornisce una filigrana per i formati di documenti e file più diffusi."

############################# Metrics ###############################
metrics:
  enable: true
  title: "I dati statistici della nostra biblioteca"
  description: "Approfondisci le metriche chiave, rivelando informazioni sui nostri risultati, impatto e crescita."

  items:
    # items loop
    - number: "50+"
      title: "Formati supportati"
      content: "La libreria è in grado di elaborare più di 50 dei formati di file più diffusi."

    # items loop
    - number: "500k"
      title: "NuGet download"
      content: "GroupDocs.Watermark for .NET è una libreria popolare con oltre 500.000 download su NuGet."

    # items loop
    - number: "15k"
      title: "Download Maven"
      content: "Con oltre 15.000 download su Maven, GroupDocs.Watermark è una scelta popolare per Java sviluppatori."

    # items loop
    - number: "140+"
      title: "Clienti soddisfatti"
      content: "I singoli sviluppatori e le migliori aziende di tutto il mondo preferiscono le nostre librerie per creare soluzioni innovative."


############################# Customers ###############################
customers:
  enable: true
  title: "I nostri clienti soddisfatti"
  description: "GroupDocs le biblioteche sono impiegate da marchi rinomati e illustri in tutto il mondo."

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
  title: "Pronto per iniziare?"
  description: "Prova le GroupDocs.Watermark funzionalità gratuitamente sulla tua piattaforma"

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
  title: "Domande frequenti"
  description: "Consulta le nostre domande frequenti"

  items:
    # items loop
    - question: "Le librerie esterne sono richieste da GroupDocs.Watermark per la manipolazione dei documenti?"
      answer: "GroupDocs.Watermark funziona in modo indipendente, senza bisogno di software di terze parti come Adobe Acrobat, Microsoft Office, ecc."

    # items loop
    - question: "Posso testare le funzioni di GroupDocs.Watermark prima dell'acquisto?"
      answer: "Sì, GroupDocs.Watermark offre una prova gratuita! Installalo e provalo, ma tieni presente: le versioni di prova aggiungono «badge di prova» ai tuoi documenti, vengono elaborate solo le prime 3 pagine. Vuoi un'esperienza completa? Ottieni una licenza temporanea gratuita di 30 giorni per una funzionalità completa. Vedi i dettagli nella sezione [licenza temporanea](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Quali tipi di licenza vengono forniti?"
      answer: "Hai bisogno di una licenza GroupDocs.Watermark? Abbiamo delle opzioni! Scegli tra le licenze in base a molte opzioni. Numero di sviluppatori nel tuo team. Luoghi di distribuzione come uffici singoli o postazioni di lavoro remote. La distribuzione dei clienti finali deve condividere l'SDK/API con i clienti? In alternativa, è disponibile una licenza per l'utilizzo mensile: paghi solo ciò che usi con i piani a consumo. Approfondisci e trova il [prezzo perfetto](https://purchase.groupdocs.com/pricing/watermark/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Watermark API low code"
  description: "Aggiungi filigrane ai file tramite la tua applicazione utilizzando la nostra API REST basata su cloud."
  
  items:
    # items loop
    - title: "GroupDocs.Watermark Cloud for cURL"
      content: "Usa l'API cURL REST ful per aggiungere un watermark a PDF, Word, Excel, PowerPoint, JPEG e altri formati di file popolari."
      icon: "groupdocs_watermark-for-curl"
      link: "https://products.groupdocs.cloud/watermark/curl"

    # items loop
    - title: "GroupDocs.Watermark Cloud for .NET"
      content: "Potenzia le tue .NET applicazioni con le funzionalità di filigrana dei documenti di Cloud SDK per .NET. Proteggi i documenti aziendali per conto tuo."
      icon: "groupdocs_watermark-for-net"
      link: "https://products.groupdocs.cloud/watermark/net"

    # items loop
    - title: "GroupDocs.Watermark Cloud for Java"
      content: "L'SDK GroupDocs.Watermark progettato per Java offre nuove possibilità per le tue Java applicazioni e file aziendali."
      icon: "groupdocs_watermark-for-java"
      link: "https://products.groupdocs.cloud/watermark/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Watermark App Web"
  description: "GroupDocs consente l'accesso all'applicazione web per aggiungere filigrane ai documenti. Puoi aggiungere una filigrana a più di 50 formati di file popolari nel tuo browser preferito GRATUITAMENTE."

  items:
    # items loop
    - title: "GroupDocs.Watermark Total"
      content: "Strumento online per aggiungere filigrane ai documenti da qualsiasi dispositivo."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/watermark/total"

    # items loop
    - title: "GroupDocs.Watermark DOCX"
      content: "Filigrana MS Word DOCX on-line."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/watermark/docx"

    # items loop
    - title: "GroupDocs.Watermark PDF"
      content: "Proteggi PDF documenti online."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/watermark/pdf"


      


---