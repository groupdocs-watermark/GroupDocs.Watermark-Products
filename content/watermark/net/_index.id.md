---
############################# Static ############################
layout: "landing"
date: 2024-04-29T14:27:13
draft: false

lang: id
product: "Watermark"
product_tag: "watermark"
platform: "Net"
platform_tag: "net"

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

############################# Head ############################
head_title: "C# .NET Perangkat Lunak Watermark Dokumen | tambahkan tanda air"
head_description: "C# .NET Library untuk menambahkan, mencari, dan menghapus tanda air dalam dokumen: PDF, Word, Excel, presentasi, diagram Visio, email dan format file gambar."

############################# Header ############################
title: "Tanda air dokumen dengan mudah di aplikasi C # .NET Anda"
description: "Berdayakan solusi C# Anda dengan API watermarking dokumen fleksibel yang menyediakan penambahan tanda air yang dapat disesuaikan ke semua format dokumen populer."
words:
  for: "untuk"

actions:
  main: "Gratis NuGet Unduh"
  main_link: "https://www.nuget.org/packages/GroupDocs.Watermark"
  alt: "Perizinan"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/net/"
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Watermark secara gratis atau minta lisensi"

release:
  title: "Versi {0} dirilis"
  notes: "Lihat apa yang baru"
  downloads: "Unduhan"

code:
  title: "Tanda air PDF file dalam C #"
  more: "Lebih banyak contoh"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
  install: "dotnet add package GroupDocs.Watermark"
  content: |
    ```csharp {style=abap}   
    // Instantiate Watermarker melewati jalur PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    using (Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions))
    {
        // Sesuaikan opsi tanda air
        TextWatermark textWatermark = 
            new TextWatermark("Approved", new Font("Arial", 8));
        
        // Terapkan tanda air ke dokumen PDF
        watermarker.Add(textWatermark);

        // Simpan dokumen hasil
        watermarker.Save("result.pdf");
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Sekilas tentang GroupDocs.Watermark"
  description: "API untuk menempatkan tanda air pada dokumen melalui .NET"
  features:
    # feature loop
    - title: "Tanda air file C#"
      content: "Tambahkan tanda air ke file bisnis Anda menggunakan GroupDocs.Watermark. Gunakan teks, gambar, diagram atau lampiran email."

    # feature loop
    - title: "Sesuaikan tanda air dengan tujuan Anda"
      content: "GroupDocs.Watermark for .NET perangkat lunak memungkinkan untuk menyesuaikan tanda air dengan berbagai cara. Gaya teks seperti tebal, miring, jenis font bersama dengan properti gambar seperti rotasi dll memperkaya proses watermarking."

    # feature loop
    - title: "Semua format file populer didukung"
      content: "Banyak format file dan dokumen didukung oleh solusi GroupDocs.Watermark. PDF, Microsoft Office Word, Excel, PowerPoint, gambar seperti JPEG, PNG, GIF, BMP, Visio diagram, email dll dapat dilindungi dengan tanda air kami."

    # feature loop
    - title: "Cari dan perbarui tanda air"
      content: "Watermark yang sudah disajikan dalam dokumen dapat ditemukan dan diproses lagi. Ubah teks, gaya, gambar, atau hapus tanda air yang terungkap tanpa upaya ekstra."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independensi platform"
  description: "GroupDocs.Watermark for .NET mendukung sistem operasi, kerangka kerja dan manajer paket yang tercantum di bawah ini"
  items:
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
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Format file yang didukung"
  description: |
    GroupDocs.Watermark for .NET menyediakan pemrosesan [format file] berikut (https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark fitur"
  description: "Lindungi PDF, Office, Gambar, dan format lainnya dengan watermark"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Watermarking dokumen"
      content: "Tambahkan atau Hapus Watermark dari Bagian Tertentu atau seluruh Dokumen Berbagai Format File."

    # feature loop
    - icon: "watermark_style"
      title: "Tata tanda air Anda"
      content: "Sesuaikan berbagai properti watermark seperti warna, font, rotasi dll."

    # feature loop
    - icon: "hidden_print"
      title: "PDF tanda air cetak tersembunyi"
      content: "Alokasikan Tanda Air Tersembunyi ke PDF yang hanya Muncul saat Mencetak Dokumen."

    # feature loop
    - icon: "image_only"
      title: "Tanda air hanya gambar dalam dokumen"
      content: "Tandai semua Gambar di Bagian, Halaman, Slide, atau Dokumen Tertentu."

    # feature loop
    - icon: "image_frame"
      title: "Memproses bingkai gambar yang dipilih"
      content: "Tetapkan Tanda Air hanya untuk Bingkai Khusus dari Gambar Multi-Bingkai."

    # feature loop
    - icon: "attachments"
      title: "Lampiran & bentuk"
      content: "Atur Watermark ke semua Lampiran dalam Dokumen Excel & semua Bentuk Gambar di Slide."

    # feature loop
    - icon: "pdf_objects"
      title: "PDF objek"
      content: "Sejajarkan Watermark ke Bleed Box, Art Box, Crop Box, atau Trim Box di Dokumen PDF."

    # feature loop
    - icon: "doc_background"
      title: "Latar belakang dokumen"
      content: "Tempatkan Watermark atau Hapus dari Gambar Latar Belakang Spreadsheet atau Slide."

    # feature loop
    - icon: "unreadable_characters"
      title: "Perlindungan Karakter yang Tidak Dapat Dibaca"
      content: "Lindungi Tanda Air Teks menggunakan Karakter yang Tidak Dapat Dibaca dalam Presentasi."

    # feature loop
    - icon: "watermark_text_search"
      title: "Cari Watermark di Dokumen"
      content: "Cari Watermark Berdasarkan Parameter Tertentu atau dengan Menggabungkan Beberapa Kriteria."

    # feature loop
    - icon: "watermark_image_search"
      title: "Cari tanda air gambar serupa"
      content: "Cari Watermark Gambar yang menyerupai gambar tertentu."

    # feature loop
    - icon: "document_info"
      title: "Dapatkan informasi dokumen"
      content: "Ekstrak Pengaturan Halaman & Informasi Lainnya secara Terprogram untuk Format yang Didukung."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Contoh kode"
  description: "Beberapa kasus penggunaan operasi GroupDocs.Watermark for .NET tipikal"
  items:
    # code sample loop
    - title: "Watermark dengan menambahkan gambar ke dokumen."
      content: |
        Untuk melindungi dokumen apa pun, Anda dapat menggunakan [image watermarks](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/):
        {{< landing/code title="Cara melindungi file dengan tanda air gambar.">}}
        ```csharp {style=abap}
        // Muat dokumen sumber ke Watermarker
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Tentukan jalur ke gambar tanda air
            using (ImageWatermark watermark = new ImageWatermark("watermark.jpg"))
            {
                // Lindungi file dan simpan
                watermarker.Add(watermark);

                watermarker.Save("result.pdf");
            }
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Cari dan ubah tanda air yang ada."
      content: |
        GroupDocs.Watermark mampu [memodifikasi tanda air](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/) yang sudah disajikan dalam dokumen. Cari item yang diinginkan dan perbarui propertinya.
        {{< landing/code title="Pencarian & modifikasi tanda air.">}}
        ```csharp {style=abap}   
        // Muat dokumen sumber
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // Cari tanda air yang akan diperbarui
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                // Perbarui properti yang diinginkan
                watermark.Text = "New Text";
            }

            // Simpan dokumen yang dimodifikasi ke jalur yang ditentukan
            watermarker.Save("document.pdf");
        }
        ```
        {{< /landing/code >}}

---
