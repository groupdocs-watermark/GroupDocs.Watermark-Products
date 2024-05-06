
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:29
draft: false
lang: it
format: Word
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "API C# .NET per la rimozione della filigrana Word"
head_description: "Cancella, elimina o modifica in modo efficiente le filigrane dai documenti Word utilizzando la nostra API C# .NET per una presentazione impeccabile dei documenti."

############################# Header ############################
title: "Word Watermark Remover per C# .NET" 
description: "Usa l'API GroupDocs.Watermark for .NET C# per rimuovere le filigrane dai documenti Word, perfetta per mantenere l'integrità e la pulizia dei documenti legali e aziendali."
subtitle: "GroupDocs.Watermark for .NET C# API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica a Nuget gratuitamente"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "libreria GroupDocs.Watermark for .NET C#"
    link: "/watermark/net/"
    link_title: "Scopri di più"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       Con la libreria GroupDocs.Watermark for .NET C# .NET, gli sviluppatori possono gestire e rimuovere facilmente le filigrane nei file Microsoft Word. Questo strumento supporta un'ampia gamma di operazioni sulle filigrane, tra cui il rilevamento, la modifica e la rimozione di filigrane di testo e immagini, garantendo che i documenti siano privi di segni indesiderati e preservando il layout e la formattazione.

############################# Steps ############################
steps:
    enable: true
    title: "Rimuovi filigrane dai documenti Word utilizzando .NET"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/)** semplifica l'attività di rimozione delle filigrane dai documenti aziendali. Potenzia la tua applicazione .NET integrando la nostra libreria e seguendo questi semplici passaggi:
      
      1. Inizia istanziando la classe principale, **Watermarker**, con il documento Word. La nostra API supporta l'elaborazione di documenti forniti come flusso o percorso locale.
      2. Utilizza **SearchCriteria** per restringere l'insieme di filigrane da elaborare. Puoi utilizzare vari parametri come immagini, testo o funzionalità di formattazione. Più specifici sono i parametri di ricerca forniti, più precisi saranno i risultati ottenuti.
      3. Elabora l'elenco delle filigrane del documento ottenuto come risultato della ricerca e rimuovile dal documento.
      4. Dopo aver rimosso le filigrane, salva il documento risultante come file locale o flusso di byte.
   
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
        // Rimuovi la filigrana di testo dal documento Word

        // Fornisci l'istanza di Watermarker per il documento di origine del documento Word
        using (Watermarker watermarker = new Watermarker("input.docx"))
        {
            // Rimuovi le filigrane selezionate dal documento
            TextFormattingSearchCriteria criteria = new TextFormattingSearchCriteria();
            criteria.ForegroundColorRange = new ColorRange();
            criteria.FontBold = true;
            PossibleWatermarkCollection watermarks = watermarker.Search(criteria);
            watermarks.Clear();

            // Salva il file nel percorso fornito
            watermarker.Save("output.docx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Semplifica la rimozione della filigrana con l'API C# .NET"
  description: "Scopri le potenti funzionalità di rimozione delle filigrane della nostra API C# .NET, progettata per integrarsi perfettamente con le tue applicazioni .NET. Rimuovi o cancella le filigrane dai PDF s e dai documenti Office in modo efficiente preservando la qualità del file originale."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "Rimuovi filigrana"
  features:
    # feature loop
    - title: "Liquidazione precisa della filigrana"
      content: "La nostra API .NET fornisce strumenti precisi per rimuovere in modo pulito le filigrane da qualsiasi documento. Progettata su misura per gli sviluppatori, questa funzionalità garantisce che la rimozione delle filigrane non comprometta la qualità o il layout del documento."

    # feature loop
    - title: "Rimozione automatica della filigrana in blocco"
      content: "Automatizza il processo di rimozione delle filigrane da set di documenti di grandi dimensioni con la nostra API .NET. Ideale per le aziende che gestiscono grandi volumi di documenti, migliorando sia l'efficienza che la sicurezza dei documenti."

    # feature loop
    - title: "Funzionalità avanzate di modifica della filigrana"
      content: "Sfrutta le funzionalità avanzate per modificare o modificare selettivamente le filigrane. La nostra API supporta regolazioni dettagliate per garantire che i tuoi documenti mantengano un aspetto professionale proteggendo al contempo le informazioni sensibili."
      
  code_samples:
    # code sample loop
    - title: "Rimuovi la filigrana di testo dai fogli di calcolo"
      content: |
        Come rimuovere le filigrane di testo con una formattazione speciale nei documenti Excel.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Carica la cartella di lavoro Excel
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  Ottieni contenuti e trova la filigrana appropriata
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();
                foreach (SpreadsheetWorksheet section in content.Worksheets)
                {
                    for (int i = section.Shapes.Count - 1; i >= 0; i--)
                    {
                        foreach (FormattedTextFragment fragment in section.Shapes[i].FormattedTextFragments)
                        {
                            if (fragment.ForegroundColor.Equals(Color.Red) && fragment.Font.FamilyName == "Arial")
                            {
                                //  Rimuovi la filigrana di testo
                                section.Shapes.RemoveAt(i);
                                break;
                            }
                        }
                    }
                }

                //  Salva elaborato XLSX
                watermarker.save("result.xlsx");
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
    title: "Gestione delle filigrane Word con .NET"
    exclude: "WORD"
    description: "Esplora le potenti funzionalità per la gestione delle filigrane nei documenti Word utilizzando la nostra API C# .NET, progettata per migliorare la sicurezza e la presentazione dei documenti senza compromettere la qualità."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/net/remove//pdf/"
          description: "Formato documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/net/remove//word/"
          description: "MS Word e documenti Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/net/remove//excel/"
          description: "MS Excel e fogli di calcolo Open Office"

        # format loop 4
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/remove//powerpoint/"
          description: "MS PowerPoint e presentazioni Open Office"

        # format loop 5
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/net/remove//docx/"
          description: "Documento XML aperto Microsoft Word"
          
        # format loop 6
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/net/remove//pptx/"
          description: "PowerPoint Presentazione XML aperta"
          
        # format loop 7
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/net/remove//xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"

        # format loop 8
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/net/remove//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/net/remove//xls/"
          description: "Cartella di lavoro Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/net/remove//ppt/"
          description: "PowerPoint Presentazione 97-2003"

        # format loop 11
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/net/remove//rtf/"
          description: "Formato RTF"

---