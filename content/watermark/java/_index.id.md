---
############################# Static ############################
layout: "landing"
date: 2024-05-06T23:13:47
draft: false

lang: id
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

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
head_title: "Java Perpustakaan Watermark | tambahkan tanda air ke dokumen"
head_description: "Perangkat lunak asli Java untuk menambahkan dan memanipulasi teks dan tanda air gambar di PDF, Word, Excel, Presentasi, Visio diagram, email dan file gambar."

############################# Header ############################
title: "Menerapkan watermark dokumen di Java proyek dengan mudah"
description: "Tingkatkan aplikasi Java Anda dengan kemampuan untuk menandai file menggunakan perpustakaan GroupDocs.Watermark. API kami menawarkan tanda air yang dapat disesuaikan untuk berbagai format file populer."
words:
  for: "untuk"

actions:
  main: "Download Gratis dari Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "Perizinan"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java/"
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Watermark secara gratis atau minta lisensi"

release:
  title: "Versi {0} dirilis"
  notes: "Lihat apa yang baru"
  downloads: "Unduhan"

code:
  title: "Tanda air PDF s melalui Java"
  more: "Lebih banyak contoh"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-watermark</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Instantiate Watermarker melewati jalur PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Sesuaikan opsi tanda air
    TextWatermark textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Terapkan tanda air ke dokumen PDF
    watermarker.add(textWatermark);

    // Simpan dokumen hasil
    watermarker.save("result.pdf");
    watermarker.close();
      
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Sekilas tentang GroupDocs.Watermark"
  description: "Perpustakaan yang dirancang untuk menambahkan tanda air menggunakan teknologi Java"
  features:
    # feature loop
    - title: "File Tanda Air melalui Java"
      content: "Lindungi dokumen bisnis Anda menggunakan GroupDocs.Watermark for Java. Tambahkan teks, gambar, diagram, atau lampiran email sebagai tanda air ke berbagai format file."

    # feature loop
    - title: "Sesuaikan Watermark untuk Kebutuhan Khusus"
      content: "GroupDocs.Watermark for Java menawarkan opsi penyesuaian ekstensif untuk tanda air. Sesuaikan gaya teks (tebal, miring, font) dan properti gambar (rotasi, dll.) Untuk menyesuaikan proses watermark dengan tujuan spesifik Anda."

    # feature loop
    - title: "Dukungan Format Luas"
      content: "GroupDocs.Watermark for Java terintegrasi dengan mulus dengan berbagai format file, termasuk: PDF, Microsoft Office (Word, Excel, PowerPoint), gambar (JPEG, PNG, GIF, BMP), Visio diagram, dan email. Tingkatkan keamanan dokumen di berbagai jenis file."

    # feature loop
    - title: "Pencarian dan Manajemen Tanda Air yang Mudah"
      content: "Kelola tanda air yang ada secara efisien dalam dokumen. Temukan tanda air tertentu, ubah teks, gaya, atau gambarnya, atau hapus seluruhnya. GroupDocs.Watermark for Java menyederhanakan alur kerja watermarking."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independensi platform"
  description: "GroupDocs.Watermark for Java mendukung berbagai sistem operasi dan manajer paket."
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Format file yang didukung"
  description: |
    GroupDocs.Watermark for Java memungkinkan pemrosesan berbagai format file. [Lihat daftar lengkapnya](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Java: Fitur"
  description: "Lindungi file Anda dengan menambahkan tanda air. Mendukung berbagai format termasuk PDF, dokumen Office, dan gambar."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "File Watermarking"
      content: "Tambahkan atau hapus tanda air dari bagian tertentu atau seluruh dokumen untuk berbagai format file yang didukung."

    # feature loop
    - icon: "watermark_style"
      title: "Kustomisasi Tanda Air"
      content: "Sesuaikan tampilan watermark Anda dengan opsi seperti warna, font, rotasi, dan banyak lagi."

    # feature loop
    - icon: "hidden_print"
      title: "Tanda Air Pencetakan Tersembunyi untuk PDF"
      content: "Tambahkan tanda air yang hanya muncul saat mencetak dokumen PDF."

    # feature loop
    - icon: "image_only"
      title: "Watermarking Gambar Selektif"
      content: "Tandai semua gambar dalam bagian, halaman, slide, atau seluruh dokumen tertentu."

    # feature loop
    - icon: "image_frame"
      title: "Watermarking Bingkai Gambar Khusus"
      content: "Terapkan tanda air ke bingkai tertentu dalam gambar multi-bingkai."

    # feature loop
    - icon: "attachments"
      title: "Lampiran dan Bentuk Watermarking"
      content: "Tambahkan tanda air ke semua lampiran di Excel dokumen atau semua bentuk gambar di Presentasi."

    # feature loop
    - icon: "pdf_objects"
      title: "Penyelarasan Tanda Air di PDF"
      content: "Sejajarkan tanda air ke berbagai area dokumen PDF, termasuk Bleed Box, Art Box, Crop Box, dan Trim Box."

    # feature loop
    - icon: "doc_background"
      title: "Watermark dengan Gambar Latar Belakang"
      content: "Tambahkan atau hapus tanda air gambar latar belakang ke Spreadsheet atau Presentasi."

    # feature loop
    - icon: "unreadable_characters"
      title: "Perlindungan dengan Karakter yang Tidak Dapat Dibaca"
      content: "Lindungi Presentasi menggunakan Tanda Air Teks dengan Karakter yang Tidak Dapat Dibaca."

    # feature loop
    - icon: "watermark_text_search"
      title: "Cari Watermark"
      content: "Dapatkan daftar tanda air yang disajikan dalam file, menggunakan berbagai parameter termasuk ekspresi reguler."

    # feature loop
    - icon: "watermark_image_search"
      title: "Temukan Tanda Air Gambar Serupa"
      content: "Temukan tanda air gambar yang terlihat seperti gambar tertentu."

    # feature loop
    - icon: "document_info"
      title: "Ekstrak Informasi Dokumen"
      content: "Dapatkan berbagai data dokumen seperti pengaturan halaman untuk format file yang didukung."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Contoh kode"
  description: "Jelajahi contoh kode yang menggambarkan fungsi GroupDocs.Watermark for Java tipikal"
  items:
    # code sample loop
    - title: "Tandai Dokumen Menggunakan Gambar"
      content: |
        Manfaatkan GroupDocs.Watermark for Java untuk meningkatkan keamanan dokumen dengan menambahkan tanda air gambar. Pelajari lebih lanjut: [Tanda air gambar](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Cara melindungi file dengan tanda air gambar.">}}
        ```csharp {style=abap}
        // Muat dokumen sumber ke Watermarker
        Watermarker watermarker = new Watermarker("document.pdf");
        
        // Tentukan jalur ke gambar tanda air
        ImageWatermark watermark = new ImageWatermark("watermark.jpg");

        // Lindungi file dan simpan
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Ubah Tanda Air"
      content: |
        GroupDocs.Watermark for Java memberdayakan Anda untuk mengelola tanda air yang ada di dalam dokumen. Temukan tanda air tertentu dan [ubah propertinya](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Pencarian & modifikasi tanda air.">}}
        ```csharp {style=abap}   
        // Muat dokumen sumber
        Watermarker watermarker = new Watermarker("document.pdf");

        // Cari tanda air yang akan diperbarui
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);                               
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);                             

        // Perbarui properti yang diinginkan
        for (PossibleWatermark watermark : watermarks)                                                           
        {  
            watermark.setText("New Text");
        }

        // Simpan dokumen yang dimodifikasi ke jalur yang ditentukan
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
