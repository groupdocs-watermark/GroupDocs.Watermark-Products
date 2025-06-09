
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: id
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Tambahkan Watermark ke File Excel"
head_description: "Tambahkan watermark gambar secara otomatis ke file Excel dengan Python. Proses banyak file sekaligus untuk perlindungan yang konsisten."

############################# Header ############################
title: "Tambahkan Watermark ke Excel dengan Python" 
description: "Tambahkan dengan cepat watermark teks atau gambar ke file Excel menggunakan Python. Panduan kami menunjukkan cara menjaga spreadsheet Anda tetap profesional dan aman dengan sedikit pekerjaan manual."
subtitle: "API GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh PyPi secara gratis"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Pustaka GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "Pelajari selengkapnya"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET memungkinkan Anda menambahkan watermark ke spreadsheet Excel di Python. Anda bisa menggunakan berbagai jenis watermark dan menyesuaikan opasitas, rotasi, dan penempatan. Pustaka ini juga membantu Anda menemukan dan mengelola watermark yang sudah ada untuk menjaga file Anda aman dari perubahan.

############################# Steps ############################
steps:
    enable: true
    title: "Tambahkan Watermark: Watermarking Python untuk Excel"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** adalah pustaka yang memungkinkan Anda menambahkan watermark ke banyak jenis file bisnis. Ikuti langkah-langkah berikut untuk cepat menambahkan watermark ke dokumen Anda di Python:
      
      1. **Mulai dengan Watermarking:** Mulailah dengan membuat instance dari kelas **Watermarker**. Berikan file Excel Anda (sebagai jalur atau aliran) ke konstruktor untuk membukanya agar dapat diberi watermark.
      2. **Buat Watermark Anda:** Buat objek **Watermark** dengan teks dan pengaturan yang diinginkan. Anda dapat menambahkan watermark ke halaman mana pun atau bahkan ke elemen dokumen seperti header atau lampiran.
      3. **Sesuaikan Watermark:** Sesuaikan ukuran, posisi, font, warna, dan penempatan watermark agar sesuai dengan kebutuhan Anda. Ini membantu watermark Anda terlihat tepat di dokumen Anda.
      4. **Terapkan dan Simpan:** Gunakan metode **Watermarker** untuk menambahkan watermark Anda ke dokumen. Simpan hasilnya, idealnya ke file baru untuk keamanan.
   
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
        # Tambahkan watermark teks ke file EXCEL
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # Pilih file yang ingin Anda tambahkan watermark
        with gw.Watermarker("input.xslx") as watermarker:

            # Buat objek watermark teks
            font = gww.Font("Arial", 36.0)
            watermark = gww.TextWatermark("top secret", font)
            watermark.foreground_color = gww.Color.red
            watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
            watermark.opacity = 0.4

            watermarker.add(watermark)

            # Simpan file EXCEL yang telah diperbarui
            watermarker.save("output.xslx")
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Jelajahi Fitur Watermarking Lainnya"
  description: "Gunakan API Python kami untuk menambahkan, melihat, mengonversi, dan mengelola watermark dalam dokumen, slide, diagram, dan lainnya. GroupDocs.Watermark for Python via .NET membantu Anda melindungi file Anda dan menambahkan informasi hak cipta dengan mudah."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Tambahkan Watermark"
  features:
    # feature loop
    - title: "Tambahkan Watermark dengan Mudah"
      content: "GroupDocs.Watermark memungkinkan pengembang Python dengan cepat menambahkan watermark teks, gambar, atau dinamis ke dokumen bisnis. Jaga keamanan dan merek file Anda dengan upaya minimal."

    # feature loop
    - title: "Watermark yang Sepenuhnya Dapat Disesuaikan"
      content: "Ubah ukuran, rotasi, transparansi, warna, dan font watermark menggunakan GroupDocs.Watermark. Buat watermark Anda sesuai dengan dokumen dengan sempurna sambil menjaga konten penting tetap terlihat."

    # feature loop
    - title: "Gunakan Fitur Dokumen untuk Watermarking"
      content: "Manfaatkan fitur dokumen yang sudah ada seperti anotasi PDF, latar belakang Word, atau header Excel untuk menambahkan watermark. GroupDocs.Watermark bekerja dengan struktur dokumen untuk watermarking yang efektif dan tidak mengganggu."
      
  code_samples:
    # code sample loop
    - title: "Tambahkan Watermark Gambar ke DOCX"
      content: |
        Contoh ini menunjukkan cara menerapkan efek gambar pada watermark bentuk.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.wordprocessing as gwow

        # Buka dokumen Word
        load_options = gwow.WordProcessingLoadOptions()
        with gw.Watermarker("source.docx", load_options) as watermarker:

            # Atur opsi watermark
            with gww.ImageWatermark("logo.png") as watermark:

                effects = gwow.WordProcessingImageEffects()
                effects.brightness = 0.7
                effects.contrast = 0.6
                effects.chroma_key = gww.Color.red

                options = gwow.WordProcessingWatermarkSectionOptions()
                options.Effects = effects;

                # Buat watermark
                watermarker.add(watermark, options)

                # Simpan dokumen dengan watermark
                watermarker.save("result.docx")
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
    title: "Tambahkan Watermark Teks dan Gambar ke Excel dengan Python"
    exclude: "EXCEL"
    description: "Gunakan GroupDocs.Watermark untuk dengan cepat menambahkan watermark kustom ke file Excel. Tingkatkan keamanan dokumen dan branding dengan alat watermarking yang fleksibel."
    items: 
        # format loop 1
        - name: "Tanda air PDF"
          format: "PDF"
          link: "/watermark/python-net/add//pdf/"
          description: "Adobe Portable Format Dokumen"

        # format loop 2
        - name: "Tanda air Word"
          format: "WORD"
          link: "/watermark/python-net/add//word/"
          description: "MS Word dan dokumen Open Office"
          
        # format loop 3
        - name: "Tanda air Excel"
          format: "EXCEL"
          link: "/watermark/python-net/add//excel/"
          description: "MS Excel dan spreadsheet Open Office"

        # format loop 4
        - name: "Gambar Tanda Air"
          format: "IMAGE"
          link: "/watermark/python-net/add//image/"
          description: "Format gambar populer"

        # format loop 5
        - name: "Foto Tanda Air"
          format: "PHOTO"
          link: "/watermark/python-net/add//photo/"
          description: "Format foto"

        # format loop 6
        - name: "Tanda air PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/add//powerpoint/"
          description: "MS PowerPoint dan presentasi Open Office"

        # format loop 7
        - name: "Tanda air DOCX"
          format: "DOCX"
          link: "/watermark/python-net/add//docx/"
          description: "Microsoft Word Buka Dokumen XML"
          
        # format loop 8
        - name: "Tanda air PPTX"
          format: "PPTX"
          link: "/watermark/python-net/add//pptx/"
          description: "PowerPoint Presentasi XML Terbuka"
          
        # format loop 9
        - name: "Tanda air XLSX"
          format: "XLSX"
          link: "/watermark/python-net/add//xlsx/"
          description: "Microsoft Excel Buka Spreadsheet XML"

        # format loop 10
        - name: "Tanda air JPEG"
          format: "JPEG"
          link: "/watermark/python-net/add//jpeg/"
          description: "JPEG Gambar"

        # format loop 11
        - name: "Tanda air PNG"
          format: "PNG"
          link: "/watermark/python-net/add//png/"
          description: "Portable Grafik Jaringan"

        # format loop 12
        - name: "Tanda air TIFF"
          format: "TIFF"
          link: "/watermark/python-net/add//tiff/"
          description: "Tag Format File Gambar"

        # format loop 13
        - name: "Tanda Air WEBP"
          format: "WEBP"
          link: "/watermark/python-net/add//webp/"
          description: "Gambar WEB"

        # format loop 14
        - name: "Tanda air DOC"
          format: "DOC"
          link: "/watermark/python-net/add//doc/"
          description: "Microsoft Word 97 - 2007 Dokumen"

        # format loop 15
        - name: "Tanda air XLS"
          format: "XLS"
          link: "/watermark/python-net/add//xls/"
          description: "Microsoft Excel Buku Kerja 97-2003"

        # format loop 16
        - name: "Tanda air PPT"
          format: "PPT"
          link: "/watermark/python-net/add//ppt/"
          description: "PowerPoint Presentasi 97-2003"

        # format loop 17
        - name: "Tanda air RTF"
          format: "RTF"
          link: "/watermark/python-net/add//rtf/"
          description: "Format Teks Kaya"

---