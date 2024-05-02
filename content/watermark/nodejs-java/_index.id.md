---
############################# Static ############################
layout: "landing"
date: 2024-04-29T14:27:13
draft: false

lang: id
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js Watermarking Library | tanda air dokumen"
head_description: "Solusi Node.js melindungi dokumen bisnis dengan tanda air teks dan gambar. Format populer seperti PDF, Word, Excel, PowerPoint didukung."

############################# Header ############################
title: "Akses ke teknologi watermarking di Node.js melalui solusi Java"
description: "Lindungi kekayaan intelektual Anda dan cegah penyalinan yang tidak sah dengan solusi Node.js ini. Hal ini memungkinkan pengguna untuk dengan mudah menambahkan tanda air ke dokumen bisnis dalam berbagai format, termasuk PDF, Word, Excel, PowerPoint, gambar dll."
words:
  for: "untuk"

actions:
  main: "Gunakan NPM untuk mengunduh secara gratis"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.watermark"
  alt: "Perizinan"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Watermark secara gratis atau minta lisensi"

release:
  title: "Versi {0} dirilis"
  notes: "Lihat apa yang baru"
  downloads: "Unduhan"
  link: "https://releases.groupdocs.com/watermark/nodejs-java/"

code:
  title: "Tambahkan watermark ke PDF dengan TypeScript"
  more: "Lebih banyak contoh"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.watermarker"
  content: |
    ```javascript {style=abap}

    // Instantiate Watermarker melewati jalur PDF
    let loadOptions = new PdfLoadOptions();
    let watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // Sesuaikan opsi tanda air
    let textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // Terapkan tanda air ke dokumen PDF
    watermarker.add(textWatermark);

    // Simpan dokumen hasil
    watermarker.save("result.pdf");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Sekilas tentang GroupDocs.Watermark"
  description: "Pustaka TypeScript Node.js untuk watermarking"
  features:
    # feature loop
    - title: "Tanda Air File Node.js"
      content: "Lindungi dokumen bisnis Anda dengan GroupDocs.Watermark for Node.js via Java. Tambahkan teks, gambar, diagram, atau lampiran email sebagai tanda air ke berbagai format file."

    # feature loop
    - title: "Sesuaikan Watermark untuk Kebutuhan Anda"
      content: "GroupDocs.Watermark for Node.js via Java menyediakan opsi penyesuaian ekstensif untuk tanda air. Gaya teks yang disempurnakan (tebal, miring, font) dan properti gambar (rotasi, dll.) memungkinkan untuk menyesuaikan pemrosesan dokumen."

    # feature loop
    - title: "Dukungan Format Komprehensif"
      content: "GroupDocs.Watermark for Node.js via Java terintegrasi secara mulus dengan berbagai format file, termasuk: PDF, MS Office seperti Word, Excel, PowerPoint, gambar seperti JPEG, PNG, GIF, BMP, Visio, Visio diagram, email dll. Berdayakan pemrosesan dokumen untuk mencapai tujuan bisnis."

    # feature loop
    - title: "Pencarian dan Pembaruan Tanda Air yang Kuat"
      content: "Dapatkan dan perbarui tanda air yang ada di dokumen yang diberi tanda air. Ubah teks, gaya, konten gambar, atau hapus seluruhnya. GroupDocs.Watermark for Node.js via Java menyediakan berbagai pemrosesan tanda air."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independensi platform"
  description: "GroupDocs.Watermark for Node.js via Java mudah terintegrasi dengan berbagai sistem operasi dan manajer paket."
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
    GroupDocs.Watermark for Node.js via Java memberdayakan Anda untuk memproses beragam format file. [Jelajahi daftar lengkapnya](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Node.js via Java: Set Fitur"
  description: "Berdayakan keamanan dokumen yang kuat melalui watermarking terprogram. Mendukung beragam format file termasuk: PDF, DOCX, XLSX, PPTX, dan format gambar (PNG, JPG, dll.)."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Kontrol Watermarking yang Tepat"
      content: "Manipulasi tanda air secara tepat dengan menambahkan atau menghapusnya dari bagian tertentu, seluruh dokumen, atau lampiran dan bentuk individu dalam format file yang berbeda."

    # feature loop
    - icon: "watermark_style"
      title: "Kustomisasi Penampilan Watermark"
      content: "Berikan kontrol halus atas estetika tanda air dengan memodifikasi atribut seperti warna, font, opacity, rotasi, dan posisi di dalam dokumen."

    # feature loop
    - icon: "hidden_print"
      title: "Cetak PDF Watermarking"
      content: "Gunakan tanda air tersembunyi yang tetap tidak terlihat selama tampilan dokumen biasa tetapi menjadi jelas hanya selama proses pencetakan, meningkatkan keamanan dokumen secara diam-diam."

    # feature loop
    - icon: "image_only"
      title: "Watermarking Gambar Khusus"
      content: "Tandai gambar tertentu dalam dokumen menggunakan solusi kami. Pilih untuk menyematkan tanda air di bagian yang ditentukan (misalnya, halaman, slide) atau di seluruh dokumen."

    # feature loop
    - icon: "image_frame"
      title: "Watermarking Gambar Multi-Bingkai"
      content: "Terapkan tanda air secara selektif ke bingkai tertentu dalam format gambar multi-bingkai, memastikan kontrol granular atas penempatan tanda air."

    # feature loop
    - icon: "attachments"
      title: "Perlindungan Konten Komprehensif"
      content: "Perluas perlindungan ke berbagai elemen dokumen seperti lampiran dalam Excel dokumen dan bentuk gambar dalam Presentasi, memberikan lapisan keamanan tambahan."

    # feature loop
    - icon: "pdf_objects"
      title: "Watermarking Tingkat Lanjut di PDF"
      content: "Tandai area yang berbeda dari PDF s, termasuk Bleed Box, Art Box, Crop Box, Trim Box dll."

    # feature loop
    - icon: "doc_background"
      title: "Watermarking Gambar Latar Belakang"
      content: "Kelola tanda air dalam gambar latar belakang Spreadsheet dan Presentasi, menawarkan opsi penyesuaian tambahan untuk langkah-langkah keamanan visual."

    # feature loop
    - icon: "unreadable_characters"
      title: "Tanda Air Teks dengan Karakter yang Tidak Dapat Dibaca"
      content: "Gunakan karakter yang tidak dapat dibaca dalam tanda air teks yang tertanam dalam Presentasi, meningkatkan keamanan dengan membuat ekstraksi tanda air yang tidak sah secara signifikan lebih menantang."

    # feature loop
    - icon: "watermark_text_search"
      title: "Pencarian Watermark Tingkat Lanjut"
      content: "Manfaatkan kemampuan pencarian komprehensif untuk menemukan tanda air dalam dokumen berdasarkan parameter tertentu atau dengan menggabungkan berbagai kriteria, memungkinkan pengambilan dan manajemen yang efisien."

    # feature loop
    - icon: "watermark_image_search"
      title: "Deteksi Watermark Gambar Mirip"
      content: "Temukan gambar tanda air serupa di dalam dokumen yang secara visual menyerupai gambar sumber."

    # feature loop
    - icon: "document_info"
      title: "Ekstraksi Informasi Dokumen Terprogram"
      content: "Ekstrak metadata berharga secara terprogram, termasuk detail pengaturan halaman dan informasi dokumen lainnya untuk format file yang didukung."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Contoh kode"
  description: "Selami contoh kode yang menampilkan fungsi GroupDocs.Watermark for Node.js via Java umum"
  items:
    # code sample loop
    - title: "Tandai Dokumen dengan Gambar"
      content: |
        Manfaatkan GroupDocs.Watermark for Node.js via Java untuk meningkatkan keamanan dokumen dengan menambahkan tanda air gambar. Pelajari lebih lanjut: [Tanda air gambar](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="Cara melindungi file dengan tanda air gambar.">}}
        ```javascript {style=abap}
        // Muat dokumen sumber ke Watermarker
        let watermarker = new Watermarker("document.pdf");
        
        // Tentukan jalur ke gambar tanda air
        let watermark = new ImageWatermark("watermark.jpg");

        // Lindungi file dan simpan
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Cari dan Ubah Watermark yang Ada"
      content: |
        GroupDocs.Watermark for Node.js via Java memberdayakan Anda untuk mengelola tanda air dokumen. Pilih tanda air, ubah propertinya. Temukan caranya: [Ubah tanda air](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="Pencarian & modifikasi tanda air.">}}
        ```javascript {style=abap}   
        // Muat dokumen sumber
        let watermarker = new Watermarker("document.pdf");

        // Cari tanda air yang akan diperbarui
        let searchCriteria = new TextSearchCriteria("test", false);                               
        let watermarks = watermarker.search(searchCriteria); 

        // Perbarui properti yang diinginkan
        watermarks.forEach((watermark)
        {  
            watermark.setText("New Text");
        }

        // Simpan dokumen yang dimodifikasi ke jalur yang ditentukan
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
