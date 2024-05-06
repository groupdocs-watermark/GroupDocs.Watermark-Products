
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:44
draft: false
lang: id
format: Xls
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Penghapusan Watermark yang Tepat di XLS Spreadsheet"
head_description: "GroupDocs.Watermark menawarkan kontrol granular atas penghapusan tanda air tertentu."

############################# Header ############################
title: "Tanda Air XLS Khusus Target" 
description: "Hapus tanda air yang tidak diinginkan secara selektif sambil mempertahankan yang diinginkan dengan GroupDocs.Watermark."
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh di NPM secara gratis"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "Pelajari selengkapnya"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark memberdayakan pengembang dengan kemampuan untuk menargetkan dan menghapus tanda air tertentu dalam dokumen. Kontrol granular ini memastikan pengeditan dokumen yang tepat, memungkinkan Anda untuk menghapus tanda air usang atau tidak relevan sambil mempertahankan informasi penting. GroupDocs.Watermark terintegrasi dengan mulus dengan lingkungan .NET, merampingkan penghapusan tanda air untuk berbagai format file.

############################# Steps ############################
steps:
    enable: true
    title: "Menghapus Tanda Air dengan Mudah dari Xls oleh Node.js via Java"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/nodejs-java/)** menyederhanakan proses penghapusan tanda air dari dokumen bisnis. Tingkatkan aplikasi Node.js via Java Anda dengan mengintegrasikan perpustakaan kami secara lancar dan mengikuti langkah-langkah mudah berikut:
      
      1. Mulai proses dengan membuat instance kelas inti, **Watermarker**, dengan dokumen Xls. API serbaguna kami memproses dokumen dengan lancar, baik yang disediakan sebagai aliran atau jalur lokal.
      2. Manfaatkan **SearchCriteria** untuk secara tepat menentukan tanda air yang ingin ditangani. Manfaatkan berbagai parameter seperti gambar, teks, atau fitur pemformatan untuk menyaring pencarian Anda. Semakin rinci kriteria Anda, semakin akurat hasil Anda.
      3. Jalankan proses penghapusan pada daftar tanda air dokumen yang diambil melalui pencarian Anda. Hapus dengan mudah dari dokumen.
      4. Setelah berhasil menghapus tanda air, simpan dokumen yang dihasilkan dengan aman sebagai file lokal atau aliran byte, dengan menjaga integritasnya.
   
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

        // Hapus tanda air gambar di dokumen XLS

        // Dapatkan Watermarker dengan meneruskan jalur XLS sebagai argumen
        const watermarker = new groupdocs.watermark.Watermarker("input.xls");
        
        // Hapus tanda air gambar berdasarkan kriteria pencarian
        const searchCriteria = 
            new groupdocs.watermark.ImageDctHashSearchCriteria("logo.png");
        const watermarks = watermarker.search(searchCriteria);
        watermarks.clear();

        // Simpan file yang diproses
        watermarker.save("output.xls");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Node.js via Java API untuk Penghapusan Tanda Air | GroupDocs.Watermark"
  description: "Integrasikan Node.js via Java API kami untuk menghapus tanda air dari dokumen dengan mudah, meningkatkan kejelasan dan estetika dokumen. Disesuaikan untuk lingkungan Node.js via Java, API ini sangat cocok untuk aplikasi yang perlu memproses dan menyajikan dokumen bersih yang bebas dari tanda air."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "Hapus Watermark"
  features:
    # feature loop
    - title: "Penghapusan Watermark yang Efisien untuk Node.js via Java"
      content: "API kami menawarkan alat penghapusan tanda air yang efisien yang dirancang khusus untuk Node.js via Java aplikasi, memungkinkan pengembang meningkatkan keterbacaan dokumen dan tampilan profesional tanpa pengkodean yang rumit."

    # feature loop
    - title: "Node.js via Java Pembersihan Tanda Air Batch"
      content: "Manfaatkan kemampuan untuk menghapus tanda air dari beberapa dokumen sekaligus dengan fitur pemrosesan batch kami. Ini sangat berguna untuk aplikasi yang perlu menangani aliran dokumen besar dengan cepat dan efisien."

    # feature loop
    - title: "Pengeditan Tanda Air Fleksibel melalui Node.js via Java"
      content: "Sesuaikan, ubah, atau hapus tanda air sepenuhnya menggunakan alat pengeditan fleksibel kami. Fitur ini memungkinkan Node.js via Java pengembang untuk menyesuaikan pemrosesan dokumen dengan kebutuhan bisnis tertentu atau permintaan klien, memastikan hasil yang optimal."
      
  code_samples:
    # code sample loop
    - title: "Hapus tanda air header spreadsheet"
      content: |
        Contoh ini menunjukkan cara menghapus tanda air yang dimasukkan ke dalam header XLSX
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Muat buku kerja Spreadsheet
            const loadOptions = new groupdocsWatermark.SpreadsheetLoadOptions();
            const watermarker = new groupdocsWatermark.Watermarker("source.xlsx", loadOptions);

            //  Dapatkan daftar bagian header
            const content = watermarker.getContent(groupdocsWatermark.SpreadsheetContent.class);
            const sections = content.getWorksheets().get_Item(0).getHeadersFooters()
                .getByOfficeHeaderFooterType(groupdocsWatermark.OfficeHeaderFooterType.HeaderPrimary).getSections();
  
            //  Hapus tanda air dari header
            for (const section of sections.getInnerList().toArray()) {
                section.setScript(null);
                section.setImage(null);
            }

            //  Simpan buku kerja yang sudah dibersihkan
            watermarker.save("result.xlsx");
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
    title: "Penghapusan Tepat di Seluruh Format"
    exclude: "XLS"
    description: "Targetkan tanda air tertentu di berbagai jenis dokumen dengan GroupDocs.Watermark."
    items: 
        # format loop 1
        - name: "Tanda air PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/delete//pdf/"
          description: "Adobe Portable Format Dokumen"

        # format loop 2
        - name: "Tanda air Word"
          format: "WORD"
          link: "/watermark/nodejs-java/delete//word/"
          description: "MS Word dan dokumen Open Office"
          
        # format loop 3
        - name: "Tanda air Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/delete//excel/"
          description: "MS Excel dan spreadsheet Open Office"

        # format loop 4
        - name: "Tanda air PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/delete//powerpoint/"
          description: "MS PowerPoint dan presentasi Open Office"

        # format loop 5
        - name: "Tanda air DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/delete//docx/"
          description: "Microsoft Word Buka Dokumen XML"
          
        # format loop 6
        - name: "Tanda air PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/delete//pptx/"
          description: "PowerPoint Presentasi XML Terbuka"
          
        # format loop 7
        - name: "Tanda air XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/delete//xlsx/"
          description: "Microsoft Excel Buka Spreadsheet XML"

        # format loop 8
        - name: "Tanda air DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/delete//doc/"
          description: "Microsoft Word 97 - 2007 Dokumen"

        # format loop 9
        - name: "Tanda air XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/delete//xls/"
          description: "Microsoft Excel Buku Kerja 97-2003"

        # format loop 10
        - name: "Tanda air PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/delete//ppt/"
          description: "PowerPoint Presentasi 97-2003"

        # format loop 11
        - name: "Tanda air RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/delete//rtf/"
          description: "Format Teks Kaya"

---