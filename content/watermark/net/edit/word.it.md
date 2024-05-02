
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:26:59
draft: false
lang: it
format: Word
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Modifica le filigrane nei documenti Word"
head_description: "Perfeziona il posizionamento delle filigrane e garantisci la sicurezza dei documenti con GroupDocs.Watermark for .NET. Personalizza le filigrane Word nelle tue soluzioni senza sforzo."

############################# Header ############################
title: "Migliora Word Watermark: .NET Confidenza" 
description: "Assicura l'autenticità dei documenti Word e l'integrità del marchio con GroupDocs.Watermark for .NET. Modifica le filigrane utilizzando la nostra soluzione in tutta sicurezza."
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica a Nuget gratuitamente"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "Scopri di più"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Enhance Word Document Security:** GroupDocs.Watermark for .NET consente agli sviluppatori di migliorare la sicurezza dei documenti con facilità. Modifica le filigrane per soddisfare i tuoi requisiti specifici in tutta sicurezza.

############################# Steps ############################
steps:
    enable: true
    title: "Modifica le filigrane nei documenti Word usando .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** consente agli .NET sviluppatori di modificare facilmente le filigrane all'interno di vari documenti Word. Ecco una guida semplificata su come utilizzare la nostra API nella tua applicazione:
      
      1. **Watermarker**. Puoi fornire il file come flusso di byte, flusso di file o percorso del disco locale.
      2. **criteri di ricerca** per identificare le filigrane con le proprietà corrispondenti precedentemente aggiunte al documento.
      3. Dopo la ricerca, otterrai un elenco di filigrane pertinenti. È quindi possibile personalizzare le loro proprietà, come dimensioni, allineamento della pagina, testo, colore, contenuto dell'immagine e altro ancora. Questo ti garantisce un ampio controllo sui tuoi dati.
      4. Una volta completata la modifica delle filigrane, salva il documento aggiornato. Puoi utilizzare un percorso di file locale o uno stream per memorizzare il risultato finale.
   
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
        // Modifica filigrana di testo WORD

        // Crea Watermarker fornendo il file WORD
        using (Watermarker watermarker = new Watermarker("input.docx"))
        {
            // Costruisci TextSearchCriteria e ottieni filigrane di testo
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                 // Modifica filigrana di testo
                 watermark.FormattedTextFragments.Clear();
                 watermark.FormattedTextFragments.Add("passed", 
                    new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
            }

            // Salva il documento
            watermarker.Save("output.docx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Scopri di più sulla modifica delle filigrane"
  description: "Potenzia le tue .NET applicazioni con la nostra libreria e aggiungi, modifica, rimuovi o cerca filigrane in vari formati di file."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Modifica filigrana"
  features:
    # feature loop
    - title: "File con filigrana per la tua azienda"
      content: "Usa GroupDocs.Watermark for .NET per aggiungere una filigrana a file e documenti. Aggiungi e gestisci le filigrane senza ulteriori sforzi implementando la nostra API nelle tue applicazioni. Cerca, modifica e rimuovi le filigrane aggiunte in precedenza."

    # feature loop
    - title: "Ottimizza le filigrane per le tue esigenze"
      content: "La nostra API offre una serie completa di opzioni di personalizzazione. Modifica facilmente aspetti come dimensioni, orientamento, combinazione di colori, famiglia di caratteri e altro per creare la filigrana ideale."

    # feature loop
    - title: "Sfrutta le funzionalità specifiche del documento"
      content: "A seconda del formato di file che stai utilizzando, puoi incorporare funzionalità integrate. Questi possono includere lo sfondo del documento, le annotazioni, le intestazioni o altri elementi che fungono da contenitori di filigrane."
      
  code_samples:
    # code sample loop
    - title: "Excel modifica del testo della filigrana"
      content: |
        Questo esempio mostra come modificare il testo per filigrane particolari in Excel Fogli di lavoro
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Carica il foglio di calcolo XLSX
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  Caricare il contenuto del foglio di calcolo
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();

                //  Modifica il testo interno della filigrana
                foreach (SpreadsheetShape shape in content.Worksheets[0].Shapes)
                {
                    if (shape.Text == "GroupDocs 2016")
                    {
                        shape.Text = "GroupDocs 2017";
                    }
                }

                //  Salva il risultato dell'output
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
    title: "Migliora la sicurezza di altri formati"
    exclude: "WORD"
    description: "GroupDocs.Watermark for .NET offre soluzioni efficienti per migliorare la sicurezza dei documenti in diversi formati."
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