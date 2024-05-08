
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:19
draft: false
lang: id
format: Image
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Watermarking Dinamis untuk perlindungan Gambar"
head_description: "Amankan hak cipta gambar Anda dengan watermarking dinamis Node.js. Mendukung JPG, PNG, WEBP dan banyak lagi."

############################# Header ############################
title: "Watermarking Dinamis untuk Perlindungan Gambar dengan Node.js" 
description: "Gunakan toolkit Node.js kami untuk menghasilkan tanda air yang dinamis dan aman untuk gambar Anda, mendukung format seperti JPG, PNG, dan WEBP. Pastikan hak cipta gambar Anda dengan fitur perlindungan lanjutan."
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
       Dengan GroupDocs.Watermark for Node.js via Java, menerapkan tanda air ke gambar mudah dan dapat disesuaikan. Toolkit ini mendukung berbagai format gambar, termasuk gambar raster tradisional seperti JPG dan PNG, serta format yang lebih baru seperti WEBP. Ini memungkinkan pengembang untuk secara dinamis menambahkan tanda air yang tidak hanya aman tetapi juga menyatu secara alami dengan konten gambar, memberikan perlindungan yang kuat terhadap pelanggaran hak cipta tanpa mengurangi daya tarik asli gambar.

############################# Steps ############################
steps:
    enable: true
    title: "Dokumen Bisnis yang Aman: Hasilkan Tanda Air untuk Format Image"
    content: |
      Tingkatkan Keamanan Dokumen Anda dengan **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/):** Suntikkan API kami ke aplikasi Anda dan buat tanda air untuk banyak format file yang didukung.
      
      1. **Memulai Watermarking:** Mulai pemrosesan dokumen dengan kelas **Watermarker** yang menyediakan fitur utama kami. Buat instance dengan meneruskan file Image ke konstruktor yang seharusnya diamankan dengan tanda air yang dihasilkan.
      2. **Buat objek Tanda Air utama:** Sempurnakan dokumen Anda dengan membuat objek **Watermark** yang dipesan lebih dahulu. Lebih dari sekedar halaman, mereka terintegrasi dengan mulus ke dalam elemen asli seperti lampiran atau header, sehingga menambahkan lapisan keamanan dan profesionalisme.
      3. **Perbaiki Atribut Tanda Air:** Sempurnakan tanda air Anda dengan presisi, penyesuaian dimensi, perataan, dan skema warna. Setiap detail meningkatkan integritas dokumen, menjadikan file Anda benar-benar milik Anda.
      4. **Terapkan dengan Presisi:** Manfaatkan metode **Watermarker** untuk menerapkan tanda air khusus Anda dengan sempurna. Baik tunggal atau ganda, setiap tanda air menambahkan lapisan perlindungan ekstra. Untuk keamanan tambahan, pertimbangkan untuk menyimpan dokumen Anda yang sudah diproses di lokasi terpisah dan aman.
   
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

        // Buat tanda air teks untuk IMAGE

        // Teruskan file sumber ke instance Watermarker
        const watermarker = new groupdocs.watermark.Watermarker("input.jpeg");
        
        // Hasilkan tanda air teks dan atur opsinya
        const  watermark = new groupdocs.watermark.TextWatermark
            ("My Watermark", groupdocs.watermark.new Font("Arial", 36));

        // Dapatkan hasil IMAGE
        watermarker.add(watermark);
        watermarker.save("output.jpeg");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Teknik Watermarking Tingkat Lanjut"
  description: "Temukan teknik watermarking mutakhir dengan API kami yang kuat, dirancang untuk diintegrasikan dengan mulus ke lingkungan .NET. Sempurna untuk menambahkan tanda air canggih dan aman ke beragam jenis dokumen termasuk presentasi, dokumen hukum, dan diagram teknis."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Tanda Air yang Canggih"
  features:
    # feature loop
    - title: "Penempatan Tanda Air Dinamis"
      content: "API kami menawarkan opsi penempatan dinamis yang menyesuaikan posisi tanda air berdasarkan konten dokumen. Ideal untuk tata letak kompleks dalam presentasi dan diagram teknis, fitur ini memastikan bahwa tanda air selalu ditempatkan secara optimal tanpa mengganggu keterbacaan informasi yang mendasarinya."

    # feature loop
    - title: "Keamanan yang Ditingkatkan dengan Watermark Tak Terlihat"
      content: "Terapkan tanda air tak terlihat yang menawarkan perlindungan kuat tanpa mengubah tampilan dokumen Anda. Watermark ini dirancang untuk dideteksi hanya melalui alat perangkat lunak tertentu, menjadikannya sempurna untuk melindungi informasi sensitif dalam dokumen hukum dan keuangan."

    # feature loop
    - title: "Alur Kerja Watermarking Otomatis"
      content: "Sederhanakan proses keamanan dokumen Anda dengan alur kerja watermarking otomatis. Konfigurasikan aturan berdasarkan jenis dokumen, sensitivitas konten, dan tingkat akses pengguna untuk menerapkan tanda air secara otomatis, memastikan protokol keamanan yang konsisten dipertahankan di semua dokumen."
      
  code_samples:
    # code sample loop
    - title: "Hasilkan tanda air untuk lampiran PDF"
      content: |
        Contoh ini menunjukkan cara menghasilkan tanda air di semua lampiran PDF
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Muat dokumen PDF
            const loadOptions = new groupdocsWatermark.PdfLoadOptions();
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf", loadOptions);
            const pdfContent = watermarker.getContent(groupdocsWatermark.PdfContent.class);

            //  Hasilkan tanda air teks
            const watermark = new groupdocsWatermark.TextWatermark('WaterMark', new groupdocsWatermark.Font('Arial', 19));
  
            //  Tambahkan tanda air ke lampiran yang sesuai
            for (const attachment of pdfContent.getAttachments().getInnerList().toArray()) {
                const info = attachment.getDocumentInfo();
                if (info.getFileType() !== groupdocsWatermark.FileType.Unknown && !info.isEncrypted()) {
                    const attachedWatermarker = attachment.createWatermarker();
                    attachedWatermarker.add(watermark);
                    attachment.updateContent(attachedWatermarker);
                    attachedWatermarker.close();
                }
            }

            //  Simpan diproses PDF
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
    title: "Menerapkan Watermark yang menakjubkan dalam Gambar melalui JavaScript"
    exclude: "IMAGE"
    description: "Lindungi hak cipta gambar Anda secara efektif dengan API Node.js kami. Tambahkan tanda air secara dinamis ke file JPG, PNG, dan WEBP, memastikan setiap gambar ditandai untuk pemiliknya yang sah."
    items: 
        # format loop 1
        - name: "Tanda air PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/generate//pdf/"
          description: "Adobe Portable Format Dokumen"

        # format loop 2
        - name: "Tanda air Word"
          format: "WORD"
          link: "/watermark/nodejs-java/generate//word/"
          description: "MS Word dan dokumen Open Office"
          
        # format loop 3
        - name: "Tanda air Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/generate//excel/"
          description: "MS Excel dan spreadsheet Open Office"

        # format loop 4
        - name: "Gambar Tanda Air"
          format: "IMAGE"
          link: "/watermark/nodejs-java/generate//image/"
          description: "Format gambar populer"

        # format loop 5
        - name: "Foto Tanda Air"
          format: "PHOTO"
          link: "/watermark/nodejs-java/generate//photo/"
          description: "Format foto"

        # format loop 6
        - name: "Tanda air PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/generate//powerpoint/"
          description: "MS PowerPoint dan presentasi Open Office"

        # format loop 7
        - name: "Tanda air DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/generate//docx/"
          description: "Microsoft Word Buka Dokumen XML"
          
        # format loop 8
        - name: "Tanda air PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/generate//pptx/"
          description: "PowerPoint Presentasi XML Terbuka"
          
        # format loop 9
        - name: "Tanda air XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/generate//xlsx/"
          description: "Microsoft Excel Buka Spreadsheet XML"

        # format loop 10
        - name: "Tanda air JPEG"
          format: "JPEG"
          link: "/watermark/nodejs-java/generate//jpeg/"
          description: "JPEG Gambar"

        # format loop 11
        - name: "Tanda air PNG"
          format: "PNG"
          link: "/watermark/nodejs-java/generate//png/"
          description: "Portable Grafik Jaringan"

        # format loop 12
        - name: "Tanda air TIFF"
          format: "TIFF"
          link: "/watermark/nodejs-java/generate//tiff/"
          description: "Tag Format File Gambar"

        # format loop 13
        - name: "Tanda Air WEBP"
          format: "WEBP"
          link: "/watermark/nodejs-java/generate//webp/"
          description: "Gambar WEB"

        # format loop 14
        - name: "Tanda air DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/generate//doc/"
          description: "Microsoft Word 97 - 2007 Dokumen"

        # format loop 15
        - name: "Tanda air XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/generate//xls/"
          description: "Microsoft Excel Buku Kerja 97-2003"

        # format loop 16
        - name: "Tanda air PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/generate//ppt/"
          description: "PowerPoint Presentasi 97-2003"

        # format loop 17
        - name: "Tanda air RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/generate//rtf/"
          description: "Format Teks Kaya"

---