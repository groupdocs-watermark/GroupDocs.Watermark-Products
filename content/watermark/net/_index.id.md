---
layout: "product"
date: 2022-07-07T12:44:18+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

head_title: "..NET API untuk Menambahkan Pencarian Hapus Tanda Air ke Word Excel Gambar PDF"
head_description: "C# .NET API untuk menambahkan, mencari, dan menghapus gambar & tanda air berbasis teks dari dokumen: PDF, Word, Excel, presentasi, Visio, email, dan format file gambar."

title: ".NET API untuk Manipulasi Tanda Air"
description: "Bangun Aplikasi .NET untuk Mengoperasikan Tanda Air Berbasis Teks & Gambar dengan Pencarian Cerdas & Fitur Keamanan Kuat."
button:
    enable: true

submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Watermark for .NET"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-watermark-net.png"
        product: "GroupDocs.Watermark"
        platform: ".NET"

    middle:
        button:
            - link: "#overview"
              text: "Ringkasan"

            - link: "#features"
              text: "Fitur"

            - link: "#support"
              text: "Mendukung"

            - link: "https://products.groupdocs.app/watermark"
              text: "Demo Langsung"

            - link: "https://purchase.groupdocs.com/pricing/watermark/net"
              text: "Harga"

    right:
        link_download: "https://downloads.groupdocs.com/watermark"
        link_learn: "https://docs.groupdocs.com/watermark/net/"
        link_buy: "https://purchase.groupdocs.com"

overview:
    enable: true
    content: |
      GroupDocs.Watermark untuk .NET memungkinkan Anda membangun aplikasi bisnis yang siap dipasarkan di C#, ASP.NET dan teknologi terkait .NET lainnya, yang memungkinkan pengguna akhir Anda, menambahkan tanda air baru, mencari dan menghapus tanda air yang ada dalam format file yang didukung . Dengan menggunakan GroupDocs.Watermark untuk .NET, Anda dapat menerapkan tanda air digital secara terprogram ke banyak format file dan mencegah penggunaan kekayaan intelektual yang tidak sah dan secara aman memberi label dokumen yang bersifat sensitif dengan menggunakan berbagai langkah keamanan bawaan yang ditawarkan oleh API ini.
    tabs:
      enable: true
      
      tab_one:
        description: |
          Berikut ini adalah ikhtisar GroupDocs.Watermark untuk .NET:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Ringkasan"
          content: |
            * Tambah & Hapus Tanda Air
            * Cari & Ganti Tanda Air
            * Cari berdasarkan Format
            * Cari berdasarkan Perbandingan Gambar
            * Bekerja dengan Header & Footer
            * Bekerja dengan Gambar Latar Belakang
            * Bekerja dengan Lampiran
            * Rasterisasi Halaman
            * Terapkan Pembatasan Pengeditan
      
      tab_two:
        description: |
          [Format dokumen dan jenis tanda air](https://docs.groupdocs.com/watermark/net/supported-document-formats/) yang didukung untuk setiap format tercantum di bawah ini:

        left:
          enable: true
          table:
            - title: "Microsoft Office"
              content: |
                * **Kata:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
                * **Visi:** VSD, VDX, VSS, VSSX, VSX, VST, VSTX, VTX, VSDX, VDW, VSTM, VSSM, VSDM

            - title: "Menambahkan Tanda Air"
              content: |
                * **PDF**: XObject, Artefak, Anotasi
                * **Kata**: Bentuk
                * **Excel**: Bentuk, Header & Footer
                * **PowerPoint**: Bentuk
                * **Visio**: Bentuk
                * **Gambar Raster**: Teks, Gambar
                * **Tiff Multi-halaman**: Teks, Gambar
                * **Gif Animasi**: Teks, Gambar

        right:
          enable: true
          table:
            - title: "Dokumen PDF dan Gambar"
              content: |
                * **Format Dokumen Portabel**: PDF
                * **Buka Dokumen**: ODT
                * **Email**: EML, MSG, EMLX, OFT
                * **Gambar**: PNG, BMP, GIF, JPG, JPEG, JP2, TIF, TIFF, WebP

            - title: "Menghapus Tanda Air"
              content: |
                * **PDF**: XObject, Artefak, Anotasi, Teks Biasa
                * **Kata**: Bentuk, Teks Biasa
                * **Excel**: Bentuk, Header & Footer, Gambar Latar Belakang, Teks dan rumus dalam sel
                * **PowerPoint**: Bentuk
                * **Visio**: Bentuk, Diagram Komentar
                * **Email**: Gambar yang dilampirkan dan disematkan, Subjek dan fragmen teks isi

      tab_three:
        description: |
          GroupDocs.Watermark untuk .NET mendukung Sistem Operasi, Kerangka Kerja & Manajer Paket berikut:
        
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "Sistem operasi"
              content: |
                * Desktop Windows
                * Windows Server
                * Windows Azure
                * Linux

            - icon: "fas fa-code"
              title: "Kerangka yang Didukung"
              content: |
                * .NET Framework 2.0 atau lebih tinggi
                * Kerangka Mono 1.2 atau lebih tinggi
                * .NET Standar 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            - icon: "fas fa-box"
              title: "Manajer Paket"
              content: |
                * NuGet

            - icon: "fas fa-tools"
              title: "Lingkungan Pengembangan"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

features:
    enable: true
    title: "GroupDocs.Watermark untuk .NET Fitur"

    feature:
      - icon: "fas fa-copy"
        content: "Tambah atau Hapus Tanda Air dari Bagian Tertentu atau seluruh Dokumen dari Berbagai Format File"

      - icon: "fas fa-eye"
        content: "Lampirkan Tanda Air ke semua Gambar di Bagian, Halaman, Slide, atau Dokumen Tertentu"

      - icon: "fas fa-bolt"
        content: "Tetapkan Tanda Air hanya untuk Bingkai Tertentu dari Gambar Multi-Frame"
      
      - icon: "fas fa-file-powerpoint"
        content: "Alokasikan Tanda Air Tersembunyi ke PDF yang hanya Muncul saat Mencetak Dokumen"

      - icon: "fas fa-code"
        content: "Setel Tanda Air ke semua Lampiran dalam Dokumen Excel & semua Bentuk Gambar di Slide"

      - icon: "fas fa-cloud"
        content: "Tempatkan Tanda Air atau Hapus dari Gambar Latar Belakang Spreadsheet atau Slide"

      - icon: "fas fa-remove-format"
        content: "Gunakan Tanda Air ke File yang Didukung di semua Lampiran Email atau Dokumen PDF"

      - icon: "fas fa-comment-slash"
        content: "Terapkan atau Hapus Tanda Air sebagai XObjects, Artefak & Anotasi dalam Dokumen PDF"

      - icon: "fas fa-location-arrow"
        content: "Hilangkan Tanda Air yang Mengandung Teks dengan Pemformatan Tertentu"

      - icon: "fas fa-border-all"
        content: "Cari Tanda Air Gambar yang Menyerupai Gambar Tertentu"

      - icon: "fas fa-wrench"
        content: "Identifikasi Tanda Air Teks Bahkan jika ada Karakter yang Tidak Dapat Dibaca di antara Huruf"

      - icon: "fas fa-columns"
        content: "Cari Tanda Air Berdasarkan Parameter Tertentu atau dengan Menggabungkan Beberapa Kriteria"

      - icon: "fas fa-file-word"
        content: "Tentukan Pemformatan Font untuk Mencari Tanda Air Teks yang Cocok"

      - icon: "fas fa-envelope"
        content: "Ekstrak Pengaturan Halaman & Informasi Lain Secara Terprogram untuk Format yang Didukung"

      - icon: "fas fa-print"
        content: "Tambahkan Tanda Air ke Gambar di dalam Header & Footer mana pun dalam Format Dokumen yang Didukung"

      - icon: "fas fa-file-archive"
        content: "Tambahkan Tanda Air ke Bentuk Gambar di Dokumen Word & Kunci Tanda Air untuk Membatasi Pengeditan"

      - icon: "fas fa-lock"
        content: "Lindungi Tanda Air Teks menggunakan Karakter yang Tidak Dapat Dibaca dalam Presentasi"

      - icon: "fas fa-file-code"
        content: "Rasterisasi Halaman Tertentu atau Seluruh Dokumen PDF untuk Melindungi Tanda Air yang Ditambahkan"
      
      - icon: "fas fa-fill-drip"
        content: "Ubah Pemformatan Teks Saat Mengganti Tanda Air Teks Yang Ada"

      - icon: "fas fa-file-excel"
        content: "Sejajarkan Tanda Air ke Bleed Box, Art Box, Crop Box, atau Trim Box dalam Dokumen PDF"

      - icon: "fas fa-heading"
        content: "Edit Properti Bentuk di Dokumen Microsoft Visio"

    more_feature:
      - title: "Menambahkan Tanda Air"
        content: |
          GroupDocs.Watermark untuk .NET mendukung beberapa jenis tanda air. Menambahkan tanda air jenis apa pun hanya masalah beberapa baris kode. Contoh berikut menunjukkan, menerapkan tanda air gambar ke dokumen Word menggunakan C#:

          ```cs
          // Muat dokumen
          using (FileStream stream = File.Open("document.docx", FileMode.Open, FileAccess.ReadWrite))
          {
            using (Watermarker watermarker = new(Watermarker(stream))
            {
                    // Gunakan jalur ke gambar sebagai parameter konstruktor
                    using (ImageWatermark watermark = new ImageWatermark("logo.png"))
                      {
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermarker.Add(watermark);
                }
                // Simpan dokumen yang dihasilkan
                watermarker.Save("document_watermarked.docx");
                }
          }
          ```
      - title: "Terapkan Tanda Air ke File dengan Format Berbeda dalam Sekali Jalan"
        content: "GroupDocs.Watermark API memungkinkan Anda menerapkan tanda air atau menghapus tanda air semua file dalam folder tertentu sekaligus. File bahkan dapat memiliki format yang berbeda namun tanda air akan diterapkan ke semuanya secara akurat."

      - title: "Keamanan Sangat Mudah untuk Tanda Air"
        content: "Dengan hanya satu baris kode, Anda dapat mempersulit alat apa pun untuk menghapus tanda air Anda dari file PDF. Ini dicapai dengan mengonversi semua halaman dokumen PDF ke gambar raster sambil menjaga kualitas aslinya tetap utuh."

support:
    enable: true

solutions:
    enable: true
    title: "GroupDocs.Watermark menawarkan API tampilan dokumen untuk lingkungan pengembangan populer lainnya"

    solution:
        - img_alt: "GroupDocs.Watermark for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-watermark-java.png"
          product: "GroupDocs.Watermark"
          platform: "Java"
          link: "/watermark/java/"

back_to_top:
  enable: true
---
