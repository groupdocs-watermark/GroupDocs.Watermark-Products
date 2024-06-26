---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:48
draft: false

lang: it
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
head_title: "C# .NET Document Watermark Software | aggiungi filigrana"
head_description: "Libreria C# .NET per aggiungere, cercare e rimuovere filigrane nei documenti: PDF, Word, Excel, presentazioni, diagrammi Visio, e-mail e formati di file di immagine."

############################# Header ############################
title: "Aggiungi facilmente la filigrana ai documenti nelle tue applicazioni C# .NET"
description: "Potenzia le tue soluzioni C# con un'API flessibile per la filigrana dei documenti che consente di aggiungere filigrane personalizzabili a tutti i formati di documento più diffusi."
words:
  for: "per"

actions:
  main: "Scarica NuGet gratis"
  main_link: "https://www.nuget.org/packages/GroupDocs.Watermark"
  alt: "Licenze"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/net/"
  title: "Pronto per iniziare?"
  description: "Prova le funzioni GroupDocs.Watermark gratuitamente o richiedi una licenza"

release:
  title: "Rilasciata la versione {0}"
  notes: "Scopri cosa c'è di nuovo"
  downloads: "Download"

code:
  title: "Filigrana PDF per i file in C#"
  more: "Altri esempi"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
  install: "dotnet add package GroupDocs.Watermark"
  content: |
    ```csharp {style=abap}   
    // Istanzia Watermarker passando il percorso PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    using (Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions))
    {
        // Personalizza le opzioni della filigrana
        TextWatermark textWatermark = 
            new TextWatermark("Approved", new Font("Arial", 8));
        
        // Applica filigrana al documento PDF
        watermarker.Add(textWatermark);

        // Salva il documento dei risultati
        watermarker.Save("result.pdf");
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark a colpo d'occhio"
  description: "API per inserire filigrane sui documenti tramite .NET"
  features:
    # feature loop
    - title: "Filigrana dei file C#"
      content: "Aggiungi filigrane ai tuoi file aziendali utilizzando GroupDocs.Watermark. Usa testo, immagini, diagrammi o allegati e-mail."

    # feature loop
    - title: "Personalizza le filigrane in base ai tuoi obiettivi"
      content: "Il software GroupDocs.Watermark for .NET consente di personalizzare le filigrane in vari modi. Stili di testo come grassetto, corsivo, tipi di carattere insieme alle proprietà dell'immagine come la rotazione ecc. arricchiscono il processo di filigrana."

    # feature loop
    - title: "Sono supportati tutti i formati di file più diffusi"
      content: "Molti formati di file e documenti sono supportati dalla soluzione GroupDocs.Watermark. PDF, Microsoft Office Word, Excel, PowerPoint, immagini come JPEG, PNG, GIF, BMP, Visio, Visio, diagrammi, email ecc. potrebbero essere protetti con le nostre filigrane."

    # feature loop
    - title: "Cerca e aggiorna le filigrane"
      content: "Le filigrane già presenti in un documento possono essere trovate ed elaborate nuovamente. Modifica testo, stile, immagini o rimuovi le filigrane visualizzate senza ulteriori sforzi."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indipendenza dalla piattaforma"
  description: "GroupDocs.Watermark for .NET supporta i sistemi operativi, i framework e i gestori di pacchetti elencati di seguito"
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
  title: "Formati di file supportati"
  description: |
    GroupDocs.Watermark for .NET fornisce l'elaborazione dei seguenti [formati di file](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formati Microsoft Office e OpenDocument
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### Immagini e grafica
        * **Formati di immagine più diffusi:** BMP, JPG, JPEG, PNG
        * **Immagini multipagina:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### Altro
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark caratteristiche"
  description: "Proteggi PDF, Office, Immagini e altri formati con una filigrana"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Filigrana dei documenti"
      content: "Aggiungi o rimuovi filigrane da una sezione particolare o da un intero documento di vari formati di file."

    # feature loop
    - icon: "watermark_style"
      title: "Personalizza la tua filigrana"
      content: "Personalizza varie proprietà della filigrana come colore, carattere, rotazione ecc."

    # feature loop
    - icon: "hidden_print"
      title: "PDF filigrana di stampa nascosta"
      content: "Assegna una filigrana nascosta a PDF che appare solo durante la stampa del documento."

    # feature loop
    - icon: "image_only"
      title: "Filigrana solo le immagini nei documenti"
      content: "Filigrana tutte le immagini in una particolare sezione, pagina, diapositiva o documento."

    # feature loop
    - icon: "image_frame"
      title: "Elabora i fotogrammi delle immagini selezionati"
      content: "Assegna la filigrana solo a fotogrammi particolari di un'immagine con più fotogrammi."

    # feature loop
    - icon: "attachments"
      title: "Allegati e forme"
      content: "Imposta la filigrana su tutti gli allegati in un documento Excel e su tutte le forme delle immagini nelle diapositive."

    # feature loop
    - icon: "pdf_objects"
      title: "PDF oggetti"
      content: "Allinea la filigrana a Bleed Box, Art Box, Crop Box o Trim Box nel documento PDF."

    # feature loop
    - icon: "doc_background"
      title: "Sfondo dei documenti"
      content: "Inserisci la filigrana o rimuovila dalle immagini di sfondo del foglio di calcolo o delle diapositive."

    # feature loop
    - icon: "unreadable_characters"
      title: "Protezione dei caratteri illeggibili"
      content: "Proteggi la filigrana del testo utilizzando caratteri illeggibili nelle presentazioni."

    # feature loop
    - icon: "watermark_text_search"
      title: "Cerca filigrane nei documenti"
      content: "Cerca filigrane in base a parametri specifici o combinando più criteri."

    # feature loop
    - icon: "watermark_image_search"
      title: "Cerca filigrane di immagini simili"
      content: "Cerca filigrane di immagini che assomiglino a un'immagine particolare."

    # feature loop
    - icon: "document_info"
      title: "Ottieni informazioni sui documenti"
      content: "Estrai programmaticamente l'impostazione della pagina e altre informazioni per i formati supportati."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Esempi di codice"
  description: "Alcuni casi d'uso delle operazioni tipiche di GroupDocs.Watermark for .NET"
  items:
    # code sample loop
    - title: "Filigrana aggiungendo un'immagine a un documento."
      content: |
        Per proteggere qualsiasi documento puoi usare [filigrane dell'immagine](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/):
        {{< landing/code title="Come proteggere il file con la filigrana dell'immagine.">}}
        ```csharp {style=abap}
        // Carica il documento sorgente su Watermarker
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Specifica il percorso di un'immagine con filigrana
            using (ImageWatermark watermark = new ImageWatermark("watermark.jpg"))
            {
                // Proteggi il file e salvalo
                watermarker.Add(watermark);

                watermarker.Save("result.pdf");
            }
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Cerca e modifica le filigrane esistenti."
      content: |
        GroupDocs.Watermark è in grado di [modificare le filigrane](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/) che sono già presenti in un documento. Cerca gli elementi desiderati e aggiorna le loro proprietà.
        {{< landing/code title="Ricerca e modifica delle filigrane.">}}
        ```csharp {style=abap}   
        // Carica il documento sorgente
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Cerca filigrane da aggiornare
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                // Aggiornare le proprietà desiderate
                watermark.Text = "New Text";
            }

            // Salva il documento modificato in un percorso specificato
            watermarker.Save("document.pdf");
        }
        ```
        {{< /landing/code >}}

---
