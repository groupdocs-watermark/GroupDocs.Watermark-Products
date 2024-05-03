
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:14
draft: false
lang: it
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Modifica le filigrane nei file Docx"
head_description: "Modifica le filigrane nei file Docx con GroupDocs.Watermark for .NET Applicazioni. Migliora l'autenticità dei documenti senza sforzo."

############################# Header ############################
title: "Modifica Docx filigrane tra i file: .NET Versatilità" 
description: "Personalizza i tuoi documenti con sicurezza utilizzando GroupDocs.Watermark for .NET Applications. Modifica le filigrane in vari formati di file senza sforzo."
subtitle: "GroupDocs.Watermark for .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download gratuito di Nuget"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "Scopri di più"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Modifica filigrane su Docx file:** Modifica facilmente le filigrane in vari formati di file con GroupDocs.Watermark for .NET Applications. Personalizza i tuoi documenti con sicurezza ed efficienza.

############################# Steps ############################
steps:
    enable: true
    title: "Modifica a livello di codice le filigrane nei documenti Docx con l'API .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** fornisce agli sviluppatori di .NET una solida API per manipolare a livello di codice le filigrane all'interno di diversi documenti Docx. Questa guida descrive il processo:
      
      1. Avvia il flusso di lavoro fornendo il tuo file Docx come argomento al costruttore della classe **Watermarker**. Il file può essere fornito come flusso di byte, flusso di file o riferimento a una posizione del disco locale.
      2. Successivamente, sfrutta l'oggetto **SearchCriteria** per individuare le filigrane specifiche che richiedono la modifica. Questo oggetto permette di identificare filigrane precedentemente incorporate nel documento.
      3. Una volta eseguita con successo la ricerca, riceverai una raccolta di filigrane pertinenti. Queste filigrane offrono un controllo granulare, consentendoti di modificare proprietà quali dimensioni, posizionamento della pagina, contenuto del testo, combinazione di colori, dati di immagine e altro ancora.
      4. Una volta completate le modifiche alla filigrana, rendere persistente il documento modificato. L'API facilita l'archiviazione utilizzando un percorso file locale o un oggetto flusso.
   
    code:
      platform: "net"
      copy_title: "Copia"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "clicca per copiare"
        copy_done: "copiato"
      links:
        #  loop
        - title: "Altri esempi"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "Documentazione"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // Modifica la filigrana dell'immagine nel documento DOCX

        // Inizializza Watermarker per file sorgente
        using (Watermarker watermarker = new Watermarker("input.docx"))
        {
            // Crea SearchCriteria per la ricerca delle filigrane delle immagini
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                // Modifica la filigrana dell'immagine
                watermark.ImageData = imageData;
            }

            // Salva risultato DOCX
            watermarker.Save("output.docx");
        }
        
        ```     

############################# More features ############################
more_features:
  enable: true
  title: "Potenzia i tuoi flussi di lavoro con la gestione delle filigrane"
  description: "Semplifica la filigrana in diversi formati di file nelle tue applicazioni .NET con la nostra solida libreria. Aggiungi, modifica, cerca o rimuovi filigrane con facilità per migliorare la sicurezza e il branding dei documenti."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Modifica della filigrana senza interruzioni"
  features:
    # feature loop
    - title: "Semplifica la filigrana nelle tue applicazioni"
      content: "Sfrutta la potenza di GroupDocs.Watermark for .NET per integrare perfettamente la funzionalità di watermarking nelle tue applicazioni .NET. La nostra API intuitiva semplifica la creazione, la gestione, la ricerca e la modifica delle filigrane, eliminando la necessità di processi manuali complessi."

    # feature loop
    - title: "Personalizzazione granulare della filigrana"
      content: "Sfrutta tutto il potenziale della personalizzazione delle filigrane con la nostra API completa. Ottimizza ogni dettaglio, tra cui dimensione, orientamento, combinazione di colori e selezione dei caratteri, per creare filigrane perfettamente in linea con i tuoi requisiti di branding e sicurezza."

    # feature loop
    - title: "Sfrutta le funzionalità specifiche dei documenti per una filigrana flessibile"
      content: "Sblocca la potenza delle funzionalità native all'interno di vari formati di documenti. Utilizza elementi come lo sfondo del documento, le annotazioni, le intestazioni o altri oggetti come contenitori di filigrana unici, in grado di soddisfare diversi tipi di documenti ed esigenze di sicurezza."
      
  code_samples:
    # code sample loop
    - title: "PDF modifica della filigrana dell'immagine"
      content: |
        Questo esempio mostra come modificare il contenuto della filigrana dell'immagine
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Carica documento come PDF
            var loadOptions = new PdfLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pdf", loadOptions))
            {
                //  Carica contenuto
                PdfContent pdfContent = watermarker.GetContent<PdfContent>();

                //  Modifica filigrana dell'immagine
                foreach (PdfArtifact artifact in pdfContent.Pages[0].Artifacts)
                {
                    if (artifact.Image != null)
                    {
                        artifact.Image = new PdfWatermarkableImage(File.ReadAllBytes("test.png"));
                    }
                }

                //  Goditi il risultato in uscita
                watermarker.save("result.pdf");
            }

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Pronto per iniziare?"
  description: "Prova le funzioni GroupDocs.Watermark gratuitamente o richiedi una licenza"
  items:
    #  loop
    - title: "Nuget scarica"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "Licenze"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Modifica filigrane tra i file"
    exclude: "DOCX"
    description: "Modifica facilmente le filigrane in più formati di file con applicazioni basate su GroupDocs.Watermark for .NET."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/net/edit//pdf/"
          description: "Formato documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/net/edit//word/"
          description: "MS Word e documenti Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/net/edit//excel/"
          description: "MS Excel e fogli di calcolo Open Office"

        # format loop 4
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/edit//powerpoint/"
          description: "MS PowerPoint e presentazioni Open Office"

        # format loop 5
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/net/edit//docx/"
          description: "Documento XML aperto Microsoft Word"
          
        # format loop 6
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/net/edit//pptx/"
          description: "PowerPoint Presentazione XML aperta"
          
        # format loop 7
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/net/edit//xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"

        # format loop 8
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/net/edit//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/net/edit//xls/"
          description: "Cartella di lavoro Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/net/edit//ppt/"
          description: "PowerPoint Presentazione 97-2003"

        # format loop 11
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/net/edit//rtf/"
          description: "Formato RTF"

---