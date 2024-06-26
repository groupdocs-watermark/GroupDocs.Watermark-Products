---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:49
draft: false

lang: id
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

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
head_title: "Python Pustaka Tanda Air | Tanda Air Dokumen"
head_description: "Python melindungi dokumen bisnis dengan tanda air teks dan gambar. Format file seperti PDF, Word, Excel, dan PowerPoint didukung."

############################# Header ############################
title: "Akses Teknologi Watermarking Python via .NET"
description: "Lindungi data Anda dan cegah penyalinan tanpa izin dengan solusi Python ini. Tambahkan tanda air dengan mudah ke dokumen bisnis dalam berbagai format, termasuk PDF, Word, Excel, PowerPoint, gambar, dll."
words:
  for: "untuk"

actions:
  main: "PyPi unduh gratis"
  main_link: "https://pypi.org/project/groupdocs-watermark-net/"
  alt: "Perizinan"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Watermark secara gratis atau minta lisensi"

release:
  title: "Versi {0} dirilis"
  notes: "Lihat apa yang baru"
  downloads: "Unduhan"
  link: "https://releases.groupdocs.com/watermark/python-net/"

code:
  title: "Tambahkan Tanda Air ke PDF menggunakan Python"
  more: "Lebih banyak contoh"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
  install: "pip install groupdocs-watermark-net"
  content: |
    ```python {style=abap}

    import groupdocs.watermark as gw
    import groupdocs.watermark.watermarks as gww
    import groupdocs.watermark.options.pdf as gwop
    import groupdocs.watermark.common as gwc

    # Instantiate Watermarker melewati jalur PDF
    pdf_lo = gwop.PdfLoadOptions()
    with gw.Watermarker("source.pdf", pdf_lo) as watermarker:
        options = gwop.PdfArtifactWatermarkOptions()

        # Sesuaikan opsi tanda air
        text_watermark = 
            gww.TextWatermark("Approved", gww.Font("Arial", 8.0))
        text_watermark.horizontal_alignment = 
            gwc.HorizontalAlignment.RIGHT

        # Terapkan tanda air ke dokumen PDF
        watermarker.add(text_watermark, options)

        # Simpan dokumen hasil
        watermarker.save("result.pdf")

    ```

############################# Overview ############################
overview:
  enable: true
  title: "Sekilas tentang GroupDocs.Watermark"
  description: "Python Pustaka untuk Penandaan Air"
  features:
    # feature loop
    - title: "Python Penandaan Air Dokumen"
      content: "Amankan data sensitif Anda dengan GroupDocs.Watermark for Python via .NET. Letakkan teks atau gambar pada berbagai format file sebagai tanda air."

    # feature loop
    - title: "Sesuaikan Tanda Air"
      content: "Banyak opsi penyesuaian tersedia di GroupDocs.Watermark for Python via .NET. Atur gaya teks (tebal, miring, font) atau properti gambar seperti ukuran atau rotasi untuk menyempurnakan tanda air pada dokumen."

    # feature loop
    - title: "Dukungan Format File Populer"
      content: "GroupDocs.Watermark for Python via .NET mendukung berbagai format file, termasuk PDF, dokumen MS Office seperti Word, Excel, PowerPoint, dan gambar seperti JPEG, PNG, GIF, BMP, diagram Visio, email, dll. Tingkatkan pemrosesan dokumen untuk memenuhi kebutuhan bisnis sasaran."

    # feature loop
    - title: "Pencarian dan Pembaruan Tanda Air"
      content: "Ambil dan perbarui tanda air yang ditempatkan di dokumen. Ubah gaya teks, konten gambar, atau hapus seluruhnya. GroupDocs.Watermark for Python via .NET menawarkan beragam kemampuan pemrosesan tanda air."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independensi platform"
  description: "GroupDocs.Watermark for Python via .NET terintegrasi secara lancar dengan berbagai sistem operasi dan pengelola paket."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Format file yang didukung"
  description: |
    GroupDocs.Watermark for Python via .NET memberdayakan Anda untuk memproses beragam format file. [Jelajahi daftar lengkap](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office & OpenDocument format
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### Gambar & Grafik
        * **Format gambar populer:** BMP, JPG, JPEG, PNG
        * **Gambar multi-halaman:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### Lainnya
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "Fitur GroupDocs.Watermark for Python via .NET"
  description: "Perkuat keamanan dokumen melalui watermarking terprogram. Memproses beragam format file termasuk PDF, DOCX, XLSX, PPTX, dan format gambar (PNG, JPG, dll.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Kontrol Penandaan Air yang Tepat"
      content: "Kelola tanda air secara tepat dengan menambahkan atau menghapusnya dari bagian tertentu, seluruh dokumen, atau lampiran dan bentuk individual dalam format file berbeda."

    # feature loop
    - icon: "watermark_style"
      title: "Sesuaikan Tampilan Tanda Air"
      content: "Berikan kontrol menyeluruh terhadap estetika tanda air dengan memodifikasi atribut seperti warna, font, opacity, rotasi, dan posisi dalam dokumen."

    # feature loop
    - icon: "hidden_print"
      title: "Cetak Tanda Air PDF"
      content: "Tambahkan tanda air tersembunyi ke dalam dokumen biasa yang hanya terlihat selama proses pencetakan, sehingga meningkatkan keamanan dokumen secara diam-diam."

    # feature loop
    - icon: "image_only"
      title: "Tanda Air Gambar Tertentu"
      content: "Beri tanda air pada gambar tertentu dalam dokumen menggunakan solusi kami. Sematkan tanda air di bagian yang ditentukan (misalnya halaman, slide) atau di seluruh dokumen."

    # feature loop
    - icon: "image_frame"
      title: "Tanda Air Gambar Multi-Lapisan"
      content: "Tambahkan tanda air secara tepat ke bingkai tertentu dalam format gambar multi-bingkai, sehingga mencapai kontrol terperinci atas penempatan tanda air."

    # feature loop
    - icon: "attachments"
      title: "Perlindungan Konten Komprehensif"
      content: "Perluas perlindungan ke berbagai elemen dokumen seperti lampiran dalam dokumen Excel dan bentuk gambar dalam presentasi, sehingga memberikan lapisan keamanan tambahan."

    # feature loop
    - icon: "pdf_objects"
      title: "Penandaan Air PDF Tingkat Lanjut"
      content: "Beri tanda air pada berbagai area PDF, termasuk Bleed Box, Art Box, Crop Box, Trim Box, dll."

    # feature loop
    - icon: "doc_background"
      title: "Tanda Air Gambar Latar Belakang"
      content: "Kelola tanda air dalam gambar latar belakang spreadsheet dan presentasi, menawarkan opsi penyesuaian tambahan untuk tindakan keamanan visual."

    # feature loop
    - icon: "unreadable_characters"
      title: "Tanda Air Teks dengan Karakter Tidak Dapat Dibaca"
      content: "Gunakan karakter yang tidak dapat dibaca dalam tanda air teks yang tertanam dalam presentasi, tingkatkan keamanan dengan membuat ekstraksi tanda air tanpa izin jauh lebih menantang."

    # feature loop
    - icon: "watermark_text_search"
      title: "Pencarian Tanda Air Tingkat Lanjut"
      content: "Gunakan fitur pencarian komprehensif untuk menemukan tanda air pada dokumen berdasarkan parameter tertentu atau dengan menggabungkan berbagai kriteria."

    # feature loop
    - icon: "watermark_image_search"
      title: "Deteksi Tanda Air Gambar Serupa"
      content: "Temukan gambar tanda air serupa dalam dokumen yang secara visual menyerupai gambar sumber."

    # feature loop
    - icon: "document_info"
      title: "Analisis Informasi Dokumen"
      content: "Ekstrak data dokumen penting seperti pengaturan halaman untuk analisis lebih lanjut."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Contoh kode"
  description: "Jelajahi contoh kode yang menampilkan fungsi umum GroupDocs.Watermark for Python via .NET."
  items:
    # code sample loop
    - title: "Tandai Air pada Dokumen dengan Gambar"
      content: |
        Gunakan GroupDocs.Watermark for Python via .NET untuk melindungi dokumen dengan menambahkan tanda air gambar. [Pelajari lebih lanjut](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Cara melindungi file dengan tanda air gambar.">}}
        ```python {style=abap}

        # Muat dokumen sumber ke Watermarker
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Tentukan jalur ke gambar tanda air
            watermark = groupdocs.watermark.watermarks.ImageWatermark("watermark.jpg")
            watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwgroupdocs.watermark.common.VerticalAlignment.CENTER

            # Lindungi file dan simpan
            watermarker.add(watermark)
            watermarker.save("result.pdf")
       
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Cari dan Ubah Tanda Air yang Ada"
      content: |
        GroupDocs.Watermark for Python via .NET memberdayakan Anda untuk mengelola tanda air dokumen. Pilih tanda air dan ubah propertinya. [Temukan caranya](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Pencarian & modifikasi tanda air.">}}
        ```python {style=abap}

        # Muat dokumen sumber
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # Cari tanda air yang akan diperbarui
            search_criteria = groupdocs.watermark.search.searchcriteria.TextSearchCriteria("annotation", False)
            watermarks = watermarker.search(search_criteria)
            
            # Perbarui properti yang diinginkan
            for watermark in watermarks:
                watermark.text = "passed"

            # Simpan dokumen yang dimodifikasi ke jalur yang ditentukan
            watermarker.save("result.pdf")


        ```
        {{< /landing/code >}}

---
