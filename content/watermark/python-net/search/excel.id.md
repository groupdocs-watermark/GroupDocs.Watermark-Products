
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:16
draft: false
lang: id
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Mendeteksi Watermark Tersembunyi dalam Spreadsheet Excel"
head_description: "Ungkap tanda tersembunyi dalam file spreadsheet dengan GroupDocs.Watermark secara cepat dan akurat."

############################# Header ############################
title: "Segera Identifikasi Watermark dalam Spreadsheet Excel" 
description: "Temukan dan kelola watermark tanpa hambatan menggunakan GroupDocs.Watermark for Python via .NET."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download PyPi Sekarang – Gratis"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Ikhtisar GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "Pelajari selengkapnya"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET memberikan toolkit watermark fitur lengkap untuk pengembang Python. Buat, ubah, temukan, dan hapus konten watermark dari dokumen seperti Excel, Word, PDF, dan banyak lagi dengan sedikit usaha.

############################# Steps ############################
steps:
    enable: true
    title: "Cara Mendeteksi Watermark dalam Berkas Excel Melalui Python"
    content: |
      Dengan **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/python-net/)**, mengidentifikasi watermark yang tertanam dalam dokumen bisnis Anda menjadi lebih sederhana. Integrasikan kemampuannya ke dalam alur kerja Python Anda untuk deteksi yang tanpa hambatan.
      
      1. Mulai dengan memuat dokumen Excel ke dalam instance kelas **Watermarker**. Menerima input sebagai jalur, stream, atau array byte.
      2. Persempit pencarian Anda menggunakan objek **SearchCriteria**. Untuk menemukan tanda berbasis gambar, gunakan gambar contoh. Untuk yang berbasis teks, tetapkan karakteristik seperti konten, gaya, atau warna.
      3. Panggil metode **Search** dari objek **Watermarker** untuk mengekstrak data watermark. Sebuah koleksi instance watermark akan dikembalikan untuk diteliti.
      4. Setelah pengambilan, Anda dapat mengelola hasilnya: menghapus tanda yang tidak diinginkan, atau memperbarui detail seperti dimensi atau konten pesan.
   
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
        # Mendeteksi watermark teks dalam format EXCEL
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Inisialisasi Watermarker dengan file EXCEL
        with gw.Watermarker("input.xslx") as watermarker:

            # Eksekusi pencarian watermark
            search_criteria = gwss.TextSearchCriteria("test", False)
            possible_watermarks = watermarker.search(search_criteria)

            # Proses daftar watermark yang terdeteksi
            print("\nFound {0} possible watermark(s).".format(len(possible_watermarks)))
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Deteksi Watermark yang Kuat dengan GroupDocs.Watermark"
  description: "Gunakan GroupDocs.Watermark dalam proyek Python Anda untuk secara efisien memindai dan menemukan elemen watermark dalam berbagai jenis dokumen."
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "Mendeteksi Watermark"
  features:
    # feature loop
    - title: "Deteksi Lanjutan dengan Filter Cerdas"
      content: "Identifikasi watermark dengan mudah dalam berbagai format dokumen. GroupDocs.Watermark mendukung penyaringan berdasarkan sifat visual dan tekstual termasuk bentuk, transparansi, dan lainnya."

    # feature loop
    - title: "Kriteria Fleksibel untuk Pencarian"
      content: "Tentukan parameter pencarian watermark yang dipersonalisasi dengan GroupDocs.Watermark. Presisi ini memungkinkan pengambilan data watermark yang tersembunyi atau dikustomisasi."

    # feature loop
    - title: "Akses dan Atur Watermark yang Terdeteksi"
      content: "Permudah audit dokumen dengan mengambil semua watermark yang tertanam. Alat kami memungkinkan ekstraksi, tampilan, dan pengelolaan item yang ditemukan dengan efisien."
      
  code_samples:
    # code sample loop
    - title: "Contoh Kode: Mendeteksi Watermark"
      content: |
        Lihat cara menggunakan GroupDocs.Watermark untuk mencari dokumen yang berisi konten watermark menggunakan aturan deteksi yang fleksibel.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # Buka dokumen target dari disk atau stream
        load_options = gwos.SpreadsheetLoadOptions()
        with gw.Watermarker("source.xlsx", load_options) as watermarker:

            # Tentukan propertis watermark khusus yang akan digunakan dalam pencarian
            criteria = gwss.TextFormattingSearchCriteria()
            criteria.foreground_color_range = gwss.ColorRange()
            criteria.foreground_color_range.min_hue = -5.0
            criteria.foreground_color_range.max_hue = 10.0
            criteria.foreground_color_range.min_brightness = 0.01
            criteria.foreground_color_range.max_brightness = 0.99
            criteria.background_color_range = gwss.ColorRange()
            criteria.background_color_range.is_empty = True
            criteria.font_name = "Arial"
            criteria.min_font_size = 19.0
            criteria.max_font_size = 42.0
            criteria.font_bold = True

            # Lakukan pencarian dan kumpulkan hasilnya
            possible_watermarks = watermarker.search(criteria)

            # Bekerja dengan hasil yang ditemukan untuk tindakan lebih lanjut
            print("Found {0} possible watermark(s).".format(len(possible_watermarks)))
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
    title: "Pencarian Watermark Multi-Format"
    exclude: "EXCEL"
    description: "Temukan konten watermark di semua jenis file yang didukung oleh GroupDocs.Watermark."
    items: 
        # format loop 1
        - name: "Tanda air PDF"
          format: "PDF"
          link: "/watermark/python-net/search//pdf/"
          description: "Adobe Portable Format Dokumen"

        # format loop 2
        - name: "Tanda air Word"
          format: "WORD"
          link: "/watermark/python-net/search//word/"
          description: "MS Word dan dokumen Open Office"
          
        # format loop 3
        - name: "Tanda air Excel"
          format: "EXCEL"
          link: "/watermark/python-net/search//excel/"
          description: "MS Excel dan spreadsheet Open Office"

        # format loop 4
        - name: "Tanda air PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/search//powerpoint/"
          description: "MS PowerPoint dan presentasi Open Office"

        # format loop 5
        - name: "Tanda air DOCX"
          format: "DOCX"
          link: "/watermark/python-net/search//docx/"
          description: "Microsoft Word Buka Dokumen XML"
          
        # format loop 6
        - name: "Tanda air PPTX"
          format: "PPTX"
          link: "/watermark/python-net/search//pptx/"
          description: "PowerPoint Presentasi XML Terbuka"
          
        # format loop 7
        - name: "Tanda air XLSX"
          format: "XLSX"
          link: "/watermark/python-net/search//xlsx/"
          description: "Microsoft Excel Buka Spreadsheet XML"

        # format loop 8
        - name: "Tanda air DOC"
          format: "DOC"
          link: "/watermark/python-net/search//doc/"
          description: "Microsoft Word 97 - 2007 Dokumen"

        # format loop 9
        - name: "Tanda air XLS"
          format: "XLS"
          link: "/watermark/python-net/search//xls/"
          description: "Microsoft Excel Buku Kerja 97-2003"

        # format loop 10
        - name: "Tanda air PPT"
          format: "PPT"
          link: "/watermark/python-net/search//ppt/"
          description: "PowerPoint Presentasi 97-2003"

        # format loop 11
        - name: "Tanda air RTF"
          format: "RTF"
          link: "/watermark/python-net/search//rtf/"
          description: "Format Teks Kaya"

---