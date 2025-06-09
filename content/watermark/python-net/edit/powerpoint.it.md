
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: it
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Modifica le filigrane nei file Powerpoint"
head_description: "Utilizza GroupDocs.Watermark for Python via .NET per cambiare rapidamente il contenuto della filigrana nelle presentazioni Powerpoint e mantenere i tuoi documenti sicuri."

############################# Header ############################
title: "Modifica precisa delle filigrane Powerpoint in Python" 
description: "Ottieni il pieno controllo sul layout e la visibilità della filigrana nelle tue presentazioni utilizzando GroupDocs.Watermark for Python via .NET."
subtitle: "GroupDocs.Watermark for Python via .NET Library" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download gratuito da PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET API"
    link: "/watermark/python-net/"
    link_title: "Scopri di più"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Controlla il layout della filigrana nei file Powerpoint:** Con GroupDocs.Watermark for Python via .NET, puoi posizionare le filigrane esattamente dove necessario e proteggere facilmente le tue presentazioni.

############################# Steps ############################
steps:
    enable: true
    title: "Modifica le filigrane nei documenti Powerpoint con Python"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** aiuta gli sviluppatori Python a aggiornare le filigrane in vari file Powerpoint. Ecco come utilizzarlo nel tuo progetto:
      
      1. Innanzitutto, apri il tuo file Powerpoint passando il percorso al costruttore **Watermarker**. Puoi utilizzare un percorso di file, uno stream di byte o uno stream di file.
      2. Quindi, trova le filigrane che desideri cambiare utilizzando **SearchCriteria**, che ti consente di cercare testo o proprietà della filigrana.
      3. Una volta trovate, puoi cambiare dettagli come testo, carattere, dimensione, posizione, colore e altro. Questo ti dà pieno controllo su come appare la filigrana.
      4. Dopo aver apportato le modifiche, salva il documento. Puoi scrivere il risultato in uno stream o in un percorso di file.
   
    code:
      platform: "python-net"
      copy_title: "Copia"
      install:
        command: |
        command: "pip install groupdocs-watermark-net"
        copy_tip: "clicca per copiare"
        copy_done: "copiato"
      links:
        #  loop
        - title: "Altri esempi"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
        #  loop
        - title: "Documentazione"
          link: "https://docs.groupdocs.com/watermark/python-net/"
          
      content: |
        ```python {style=abap}
        # Aggiornare il testo della filigrana in POWERPOINT
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Creare una Watermarker utilizzando un file POWERPOINT
        with gw.Watermarker("input.pptx") as watermarker:

            # Impostare TextSearchCriteria per trovare il testo della filigrana
            search_criteria = gwss.TextSearchCriteria("test", False)

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # Modificare il testo della filigrana
                        watermark.text = "passed"
                    except Exception as e:
                        pass
            
            watermarker.save("output.pptx")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Scopri altri modi per aggiornare le filigrane"
  description: "Con la nostra libreria, le app Python possono aggiungere, trovare, modificare o eliminare filigrane in molti tipi di file."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Modifica delle Filigrane"
  features:
    # feature loop
    - title: "Filigranare i tuoi file con semplicità"
      content: "Utilizza GroupDocs.Watermark for Python via .NET per aggiungere e gestire filigrane nei tuoi documenti. Cerca, aggiorna o rimuovi filigrane come necessario tramite un'API semplice."

    # feature loop
    - title: "Personalizza le filigrane per soddisfare le tue esigenze"
      content: "Regola le impostazioni delle filigrane come carattere, dimensione, orientamento e colore utilizzando la nostra API flessibile per ottenere esattamente il risultato desiderato."

    # feature loop
    - title: "Utilizza funzionalità specifiche del formato"
      content: "A seconda del formato del file, puoi utilizzare caratteristiche native come intestazioni, piè di pagina, annotazioni o sfondi come aree per la filigrana."
      
  code_samples:
    # code sample loop
    - title: "Modifica la filigrana di testo in Excel"
      content: |
        Questo codice mostra come cambiare il testo della filigrana nei fogli di calcolo Excel.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # Apri il file XLSX
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # Leggi i dati del foglio di calcolo
        with gw.Watermarker("source.xlsx") as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,3]

            # Cambia il testo della filigrana
            watermarks = watermarker.search(search_criteria)
            for watermark in watermarks:
                try:
                    watermark.formatted_text_fragments.clear()
                    watermark.formatted_text_fragments.add(
                       "passed", 
                        gww.Font("Calibri", 19.0, gww.FontStyle.bold), 
                        gww.Color.red, 
                        gww.Color.aqua
                    )
                except Exception as e:
                    pass
        
            # Salva il risultato
            watermarker.save("output.xlsx")
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Pronto per iniziare?"
  description: "Prova le funzioni GroupDocs.Watermark gratuitamente o richiedi una licenza"
  items:
    #  loop
    - title: "PyPi scarica"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      color: "red"
        #  loop
    - title: "Licenze"
      link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Modifica le filigrane in altri tipi di file"
    exclude: "POWERPOINT"
    description: "Utilizza GroupDocs.Watermark for Python via .NET per lavorare con le filigrane in diversi formati di documenti."
    items: 
        # format loop 1
        - name: "Filigrana PDF"
          format: "PDF"
          link: "/watermark/python-net/edit//pdf/"
          description: "Formato documento Adobe Portable"

        # format loop 2
        - name: "Filigrana Word"
          format: "WORD"
          link: "/watermark/python-net/edit//word/"
          description: "MS Word e documenti Open Office"
          
        # format loop 3
        - name: "Filigrana Excel"
          format: "EXCEL"
          link: "/watermark/python-net/edit//excel/"
          description: "MS Excel e fogli di calcolo Open Office"

        # format loop 4
        - name: "Filigrana PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/edit//powerpoint/"
          description: "MS PowerPoint e presentazioni Open Office"

        # format loop 5
        - name: "Filigrana DOCX"
          format: "DOCX"
          link: "/watermark/python-net/edit//docx/"
          description: "Documento XML aperto Microsoft Word"
          
        # format loop 6
        - name: "Filigrana PPTX"
          format: "PPTX"
          link: "/watermark/python-net/edit//pptx/"
          description: "PowerPoint Presentazione XML aperta"
          
        # format loop 7
        - name: "Filigrana XLSX"
          format: "XLSX"
          link: "/watermark/python-net/edit//xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"

        # format loop 8
        - name: "Filigrana DOC"
          format: "DOC"
          link: "/watermark/python-net/edit//doc/"
          description: "Documento Microsoft Word 97 - 2007"

        # format loop 9
        - name: "Filigrana XLS"
          format: "XLS"
          link: "/watermark/python-net/edit//xls/"
          description: "Cartella di lavoro Microsoft Excel 97-2003"

        # format loop 10
        - name: "Filigrana PPT"
          format: "PPT"
          link: "/watermark/python-net/edit//ppt/"
          description: "PowerPoint Presentazione 97-2003"

        # format loop 11
        - name: "Filigrana RTF"
          format: "RTF"
          link: "/watermark/python-net/edit//rtf/"
          description: "Formato RTF"

---