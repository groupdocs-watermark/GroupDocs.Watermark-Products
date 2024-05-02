
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:27:01
draft: false
lang: id
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Perbarui Watermark untuk Excel Spreadsheet"
head_description: "Perbarui tanda air dalam spreadsheet berbagai format menggunakan GroupDocs.Watermark for Node.js via Java. Perkaya Node.js via Java aplikasi Anda."

############################# Header ############################
title: "Merevolusi Spreadsheet Watermarking menggunakan Node.js via Java" 
description: "Rasakan kekuatan GroupDocs.Watermark for Node.js via Java. Amankan dokumen bisnis Anda dengan berbagai tanda air. Perbarui ukuran tanda air, penyelarasan, sudut rotasi, posisi, dll."
subtitle: "GroupDocs.Watermark for Node.js via Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduhan gratis NPM"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java perpustakaan"
    link: "/watermark/nodejs-java/"
    link_title: "Pelajari selengkapnya"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java adalah solusi komprehensif untuk mengelola tanda air menggunakan lingkungan Node.js via Java. Dengan alat ini, pengembang dapat dengan mudah melakukan operasi seperti menambahkan, mengedit, mencari, dan menghapus tanda air dari dokumen dalam berbagai format file, termasuk PDF, Microsoft Word, Excel, PowerPoint, Visio, email, dan format gambar. GroupDocs.Watermark mendukung semua sistem operasi utama dan versi Node.js.

############################# Steps ############################
steps:
    enable: true
    title: "Perbarui Watermark di EXCEL melalui Node.js via Java"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** melengkapi Node.js via Java pengembang dengan API yang kuat untuk memperbarui tanda air secara terprogram dalam berbagai dokumen EXCEL. Panduan ini menguraikan prosesnya:
      
      1. **Watermarker**. Bergantung pada permintaan Anda, file dapat disediakan sebagai aliran atau referensi ke lokasi disk lokal.
      2. **SearchCriteria** untuk mengidentifikasi tanda air tertentu yang memerlukan modifikasi. Objek ini memungkinkan penentuan tanda air berdasarkan properti yang diinginkan.
      3. Setelah keberhasilan pelaksanaan pencarian, Anda akan menerima kumpulan tanda air yang relevan. Watermark ini menawarkan kontrol granular, memungkinkan Anda memperbarui properti seperti dimensi, posisi halaman, konten teks, skema warna, data gambar, dan banyak lagi.
      4. Setelah penyelesaian pembaruan tanda air, pertahankan dokumen yang dimodifikasi. API memfasilitasi penyimpanan menggunakan jalur file lokal atau objek aliran.
   
    code:
      platform: "net"
      copy_title: "Salin"
      install:
        command: "npm i @groupdocs/groupdocs.watermark"
        copy_tip: "klik untuk menyalin"
        copy_done: "menyalin"
      links:
        #  loop
        - title: "Lebih banyak contoh"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/watermark/nodejs-java/"
          
      content: |
        ```javascript {style=abap}

        // Perbarui EXCEL tanda air teks

        // Menyediakan contoh Watermarker untuk file EXCEL
        const watermarker = new groupdocs.watermark.Watermarker("input.xslx");

        // Gunakan TextSearchCriteria untuk menemukan tanda air teks
        const searchCriteria = 
            new groupdocs.watermark.TextSearchCriteria("test", false);
        const watermarks = watermarker.search(searchCriteria);
        
        // Perbarui tanda air teks
        for (const watermark of watermarks.getInnerList().toArray())
        {
            watermark.setText("passed");
        }

        // Nikmati hasilnya
        watermarker.save("output.xslx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Menguasai Pengeditan Tanda Air dalam PDF detik dengan GroupDocs.Watermark"
  description: "Jelajahi fitur API komprehensif untuk menyesuaikan dan mengelola tanda air dalam PDF s dalam Node.js via Java aplikasi."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Edit Tanda Air"
  features:
    # feature loop
    - title: "Mengedit Watermark dengan mudah dalam PDF s"
      content: "GroupDocs.Watermark menawarkan alat yang kuat di Node.js via Java untuk mengedit tanda air yang ada dengan mulus di dokumen PDF. Sesuaikan posisi, transparansi, dan lainnya dengan mudah."

    # feature loop
    - title: "Sempurnakan Detail Tanda Air untuk Presisi"
      content: "Kendalikan detailnya. API kami memungkinkan Anda untuk menyempurnakan tampilan tanda air, memungkinkan modifikasi ukuran, opasitas, dan warna yang tepat di PDF s Anda."

    # feature loop
    - title: "Manajemen Watermark yang Efisien"
      content: "API kami menyederhanakan pengelolaan tanda air. Baik memperbarui atau menghapus, Anda dapat mengelola tanda air secara efisien, menjaga integritas dokumen sambil memenuhi kebutuhan branding Anda."
      
  code_samples:
    # code sample loop
    - title: "Java Contoh: Edit PDF Tanda Air"
      content: |
        Contoh Java ini menunjukkan cara mengedit tanda air yang ada di dokumen PDF, menampilkan cara menyesuaikan propertinya secara terprogram.
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Muat dokumen PDF untuk diproses
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  Cari tanda air tertentu yang memenuhi kriteria Anda
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria("test", false);
            const watermarks = watermarker.search(searchCriteria);
  
            //  Mengedit pengaturan tanda air, seperti ukuran, warna, dan posisi
            for (const watermark of watermarks.getInnerList().toArray()) {
                watermark.getFormattedTextFragments().clear();
                watermark.getFormattedTextFragments().add("passed", 
                    new groupdocsWatermark.Font("Calibri", 19, groupdocsWatermark.FontStyle.Bold), 
                    groupdocsWatermark.Color.getRed(), groupdocsWatermark.Color.getAqua());
            }

            //  Simpan dokumen yang diperbarui ke sistem lokal atau streaming langsung
            watermarker.save("result.pdf");
            watermarker.close();

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Watermark secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "NPM unduhan"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      color: "red"
        #  loop
    - title: "Perizinan"
      link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Perbarui Watermark Di Seluruh Format File yang Didukung"
    exclude: "EXCEL"
    description: "Perbarui tanda air secara efisien di PDF, Word, Excel, dan lainnya dengan GroupDocs.Watermark for Node.js via Java. Dokumen bertanda air dapat memperkaya proses bisnis Anda."
    items: 
        # format loop 1
        - name: "Tanda air PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/update//pdf/"
          description: "Adobe Portable Format Dokumen"

        # format loop 2
        - name: "Tanda air Word"
          format: "WORD"
          link: "/watermark/nodejs-java/update//word/"
          description: "MS Word dan dokumen Open Office"
          
        # format loop 3
        - name: "Tanda air Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/update//excel/"
          description: "MS Excel dan spreadsheet Open Office"

        # format loop 4
        - name: "Tanda air PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/update//powerpoint/"
          description: "MS PowerPoint dan presentasi Open Office"

        # format loop 5
        - name: "Tanda air DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/update//docx/"
          description: "Microsoft Word Buka Dokumen XML"
          
        # format loop 6
        - name: "Tanda air PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/update//pptx/"
          description: "PowerPoint Presentasi XML Terbuka"
          
        # format loop 7
        - name: "Tanda air XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/update//xlsx/"
          description: "Microsoft Excel Buka Spreadsheet XML"

        # format loop 8
        - name: "Tanda air DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/update//doc/"
          description: "Microsoft Word 97 - 2007 Dokumen"

        # format loop 9
        - name: "Tanda air XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/update//xls/"
          description: "Microsoft Excel Buku Kerja 97-2003"

        # format loop 10
        - name: "Tanda air PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/update//ppt/"
          description: "PowerPoint Presentasi 97-2003"

        # format loop 11
        - name: "Tanda air RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/update//rtf/"
          description: "Format Teks Kaya"

---