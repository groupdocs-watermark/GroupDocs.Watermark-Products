
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: id
format: Word
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Edit Watermark di file Word"
head_description: "Sesuaikan pengaturan watermark dan tingkatkan perlindungan dokumen menggunakan GroupDocs.Watermark for Python via .NET untuk Word."

############################# Header ############################
title: "Perbarui Watermark Word dengan Mudah Menggunakan Python" 
description: "Lindungi merek dan dokumen Anda dengan GroupDocs.Watermark for Python via .NET. Cepat ubah watermark di file Word."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh gratis di PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "Pelajari selengkapnya"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Amankan Dokumen Word Anda:** Gunakan GroupDocs.Watermark for Python via .NET untuk cepat memperbarui dan mengelola watermark yang sesuai dengan kebutuhan dokumen dan branding Anda.

############################# Steps ############################
steps:
    enable: true
    title: "Modifikasi watermark di dokumen Word dengan Python"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** membantu pengembang Python untuk memperbarui watermark di berbagai file Word. Berikut adalah cara menggunakannya dalam proyek Anda:
      
      1. Pertama, buka file Word Anda dengan meneruskannya ke konstruktor **Watermarker**. Anda dapat menggunakan jalur file, stream byte, atau stream file.
      2. Kemudian, temukan watermark yang ingin Anda ubah menggunakan **SearchCriteria**, yang memungkinkan Anda mencari teks atau properti watermark.
      3. Setelah ditemukan, Anda dapat mengubah detail seperti teks, font, ukuran, posisi, warna, dan banyak lagi. Ini memberi Anda kontrol penuh atas tampilan watermark.
      4. Setelah melakukan perubahan, simpan dokumen. Anda dapat menulis hasilnya ke stream atau jalur file.
   
    code:
      platform: "python-net"
      copy_title: "Salin"
      install:
        command: |
        command: "pip install groupdocs-watermark-net"
        copy_tip: "klik untuk menyalin"
        copy_done: "menyalin"
      links:
        #  loop
        - title: "Lebih banyak contoh"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/watermark/python-net/"
          
      content: |
        ```python {style=abap}
        # Perbarui teks watermark di WORD
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Buat Watermarker menggunakan file WORD
        with gw.Watermarker("input.docx") as watermarker:

            # Atur TextSearchCriteria untuk menemukan teks watermark
            search_criteria = gwss.TextSearchCriteria("test", False)

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # Modifikasi teks watermark
                        watermark.text = "passed"
                    except Exception as e:
                        pass
            
            watermarker.save("output.docx")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Temukan lebih banyak cara untuk memperbarui watermark"
  description: "Dengan pustaka kami, aplikasi Python dapat menambah, menemukan, mengedit, atau menghapus watermark di banyak tipe file."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Pengeditan Watermark"
  features:
    # feature loop
    - title: "Watermark File Anda dengan Mudah"
      content: "Gunakan GroupDocs.Watermark for Python via .NET untuk menambah dan mengelola watermark di dokumen Anda. Cari, perbarui, atau hapus watermark sesuai kebutuhan menggunakan API yang sederhana."

    # feature loop
    - title: "Kustomisasi Watermark Sesuai Kebutuhan Anda"
      content: "Sesuaikan pengaturan watermark seperti font, ukuran, orientasi, dan warna menggunakan API kami yang fleksibel untuk mendapatkan hasil yang Anda inginkan."

    # feature loop
    - title: "Gunakan Fitur Spesifik Format"
      content: "Bergantung pada format file, Anda dapat menggunakan fitur asli seperti header, footer, anotasi, atau latar belakang sebagai area watermark."
      
  code_samples:
    # code sample loop
    - title: "Edit Watermark Teks di Excel"
      content: |
        Kode ini menunjukkan cara mengubah teks watermark di spreadsheet Excel.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # Buka file XLSX
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # Baca data spreadsheet
        with gw.Watermarker("source.xlsx") as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,3]

            # Ubah teks watermark
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
        
            # Simpan hasil
            watermarker.save("output.xlsx")
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Watermark secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "PyPi unduhan"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      color: "red"
        #  loop
    - title: "Perizinan"
      link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Watermark Format File Lain"
    exclude: "WORD"
    description: "GroupDocs.Watermark for Python via .NET membantu Anda melindungi beberapa tipe file dengan alat watermark yang fleksibel."
    items: 
        # format loop 1
        - name: "Tanda air PDF"
          format: "PDF"
          link: "/watermark/python-net/edit//pdf/"
          description: "Adobe Portable Format Dokumen"

        # format loop 2
        - name: "Tanda air Word"
          format: "WORD"
          link: "/watermark/python-net/edit//word/"
          description: "MS Word dan dokumen Open Office"
          
        # format loop 3
        - name: "Tanda air Excel"
          format: "EXCEL"
          link: "/watermark/python-net/edit//excel/"
          description: "MS Excel dan spreadsheet Open Office"

        # format loop 4
        - name: "Tanda air PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/edit//powerpoint/"
          description: "MS PowerPoint dan presentasi Open Office"

        # format loop 5
        - name: "Tanda air DOCX"
          format: "DOCX"
          link: "/watermark/python-net/edit//docx/"
          description: "Microsoft Word Buka Dokumen XML"
          
        # format loop 6
        - name: "Tanda air PPTX"
          format: "PPTX"
          link: "/watermark/python-net/edit//pptx/"
          description: "PowerPoint Presentasi XML Terbuka"
          
        # format loop 7
        - name: "Tanda air XLSX"
          format: "XLSX"
          link: "/watermark/python-net/edit//xlsx/"
          description: "Microsoft Excel Buka Spreadsheet XML"

        # format loop 8
        - name: "Tanda air DOC"
          format: "DOC"
          link: "/watermark/python-net/edit//doc/"
          description: "Microsoft Word 97 - 2007 Dokumen"

        # format loop 9
        - name: "Tanda air XLS"
          format: "XLS"
          link: "/watermark/python-net/edit//xls/"
          description: "Microsoft Excel Buku Kerja 97-2003"

        # format loop 10
        - name: "Tanda air PPT"
          format: "PPT"
          link: "/watermark/python-net/edit//ppt/"
          description: "PowerPoint Presentasi 97-2003"

        # format loop 11
        - name: "Tanda air RTF"
          format: "RTF"
          link: "/watermark/python-net/edit//rtf/"
          description: "Format Teks Kaya"

---