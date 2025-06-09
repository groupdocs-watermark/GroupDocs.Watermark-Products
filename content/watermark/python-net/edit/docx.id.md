
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:29
draft: false
lang: id
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Pengeditan Watermark Kustom dalam File Docx"
head_description: "Sesuaikan konten watermark dalam file Docx dengan alat GroupDocs.Watermark for Python via .NET untuk memenuhi kebutuhan branding."

############################# Header ############################
title: "Sesuaikan Watermark Docx dalam Proyek Python Anda" 
description: "Edit dan kelola watermark di berbagai jenis dokumen dengan mudah menggunakan GroupDocs.Watermark for Python via .NET."
subtitle: "GroupDocs.Watermark for Python via .NET API Suite" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Akses melalui PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "Pelajari selengkapnya"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Alat Watermark yang Fleksibel:** Sesuaikan dan personalkan watermark di berbagai format menggunakan GroupDocs.Watermark for Python via .NET dalam alur kerja Python Anda.

############################# Steps ############################
steps:
    enable: true
    title: "Gunakan API Python untuk Memodifikasi Watermark dalam Dokumen Docx"
    content: |
      Dengan **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)**, pengembang Python dapat memodifikasi konten watermark dalam berbagai dokumen Docx. Berikut adalah langkah cepat: 
      
      1. Mulailah dengan memuat dokumen Docx menggunakan kelas **Watermarker**, yang menerima jalur file, arus memori, atau array byte sebagai input.
      2. Buat objek **SearchCriteria** untuk mencari elemen watermark yang ada dalam dokumen Anda, baik yang bersifat tekstual maupun grafis.
      3. Setelah teridentifikasi, alat ini memberikan koleksi instansi watermark yang cocok untuk diperbarui—sesuaikan parameter seperti warna, penyelarasan, font, atau bahkan data gambar yang disematkan.
      4. Selesaikan proses dengan menyimpan dokumen yang telah direvisi ke disk atau arus output yang didukung menggunakan metode simpan bawaan.
   
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
        # Perbarui watermark gambar dalam file DOCX
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Buat instance Watermarker dengan file input
        with gw.Watermarker("input.docx") as watermarker:

            # Gunakan SearchCriteria untuk menemukan watermark berbasis gambar
            search_criteria = gwss.ImageDctHashSearchCriteria("logo.png")

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # Terapkan perubahan pada watermark gambar
                        watermark.ImageData = imageData
                    except Exception as e:
                        pass

            # Ekspor file DOCX yang telah diperbarui
            watermarker.save("output.docx")
        ```     

############################# More features ############################
more_features:
  enable: true
  title: "Tingkatkan Produktivitas dengan Alat Watermarking Lanjutan"
  description: "Percepat branding dan perlindungan dokumen dalam Python dengan API watermarking dinamis kami. Sisipkan, deteksi, modifikasi, atau hapus lapisan watermark dengan usaha minimal."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Alur Kerja Pengeditan Watermark Lanjutan"
  features:
    # feature loop
    - title: "Kontrol Watermark Terintegrasi"
      content: "Bawa kontrol siklus hidup watermark penuh ke aplikasi Python Anda menggunakan GroupDocs.Watermark for Python via .NET. Hindari tugas berulang dengan mengotomatiskan pengaturan, pembaruan, dan penghapusan watermark."

    # feature loop
    - title: "Penyetelan Presisi Atribut Watermark"
      content: "Ambil kontrol penuh atas estetika watermark—ubah ukuran, warna, putar, atau posisikan kembali sesuai kebutuhan visual menggunakan antarmuka API fleksibel kami."

    # feature loop
    - title: "Manfaatkan Fitur Format Asli"
      content: "Beradaptasi dengan format file apa pun dengan menyematkan watermark ke dalam header, footer, anotasi, atau latar belakang. API kami menghormati struktur asli untuk integrasi optimal."
      
  code_samples:
    # code sample loop
    - title: "Memodifikasi Watermark dalam File PDF"
      content: |
        Menunjukkan cara mengubah properti watermark dalam dokumen PDF.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # Buka file PDF
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.pdf as gwop

        # Baca konten watermark
        load_options = gwop.PdfLoadOptions()
        with gw.Watermarker("source.pdf", load_options) as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,5,8]

            # Terapkan pembaruan watermark
            watermarks = watermarker.search(search_criteria)
            for watermark in watermarks:
                try:
                    watermark.formatted_text_fragments.clear()
                    watermark.formatted_text_fragments.add(
                        "New text", 
                        gww.Font("Calibri", 5.0, gww.FontStyle.bold), 
                        gww.Color.white, 
                        gww.Color.aqua
                    )
                except Exception as e:
                    pass
        
            # Simpan hasil yang telah diedit
            watermarker.save("output.pdf")
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
    title: "Kontrol Watermark untuk Format Lain"
    exclude: "DOCX"
    description: "Manfaatkan alat pengeditan watermark yang konsisten di semua jenis file yang didukung menggunakan GroupDocs.Watermark for Python via .NET."
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