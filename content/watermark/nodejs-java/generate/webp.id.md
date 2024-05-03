
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:16
draft: false
lang: id
format: Webp
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Sematkan Watermark di WEBP dengan Node.js"
head_description: "Gunakan Node.js untuk menerapkan tanda air lanjutan ke gambar WEBP, meningkatkan perlindungan dan hak cipta."

############################# Header ############################
title: "Buat Watermark untuk WEBP Gambar melalui Node.js" 
description: "Terapkan Node.js untuk menghasilkan tanda air khusus dan aman untuk file WEBP, ideal untuk pembuat konten digital yang ingin melindungi visual mereka."
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
       GroupDocs.Watermark for Node.js via Java melengkapi pengembang Node.js dengan alat untuk menambahkan, mengelola, dan menyesuaikan tanda air dalam gambar WEBP. API ini memungkinkan integrasi tanda air transparan atau buram yang menyatu dengan sempurna dengan gambar, memastikan bahwa integritas karya seni dipertahankan sambil melindungi dari penggunaan yang tidak sah. Sesuaikan ukuran, opasitas, dan posisi tanda air untuk menonjolkan merek Anda atau mengamankan aset digital Anda secara diam-diam. Cocokan untuk fotografer, desainer grafis, dan setiap profesional yang berurusan dengan media digital, GroupDocs.Watermark meningkatkan keamanan gambar WEBP melalui antarmuka Node.js yang fleksibel dan kuat.

############################# Steps ############################
steps:
    enable: true
    title: "Lindungi Dokumen Bisnis: Hasilkan Tanda Air Webp"
    content: |
      Perkuat Keamanan Dokumen dengan **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/):** - Solusi Pembuatan Tanda Air yang Ampuh untuk Node.js via Java.
      
      1. **Sederhanakan Watermarking Aman di Aplikasi Node.js via Java Anda:** Kelas **Watermarker** bertindak sebagai komponen inti API GroupDocs.Watermark. Pustaka ini menyederhanakan pembuatan tanda air dalam berbagai format dokumen, termasuk Webp. Untuk memulai, buat instance Watermarker sebelum memproses dokumen Anda. Berikan jalur file Webp atau objek aliran ke konstruktor selama inisialisasi.
      2. **Hasilkan Tanda Air untuk Perlindungan yang Lebih Baik:** Berdayakan tanda air yang selaras dengan kebutuhan keamanan Anda. Buatlah objek **Watermark** yang menentukan tipe yang diinginkan. Tidak seperti penempatan halaman tradisional, Anda dapat menyematkan tanda air dalam elemen dokumen asli seperti header atau lampiran, memperkuat keamanan dokumen dan menambahkan sentuhan profesional.
      3. **Sempurnakan Tampilan Tanda Air untuk Dampak Optimal:** Kontrol aspek visual tanda air Anda. Sesuaikan properti seperti tinggi, lebar, perataan (atas, kiri, tengah, dll.), kelompok font, dan warna untuk mencapai hasil visual yang efektif dan konsisten yang memperkuat legitimasi dokumen.
      4. **Aplikasi Tanda Air dan Penyimpanan Aman**: Gabungkan tanda air Anda menggunakan metode **Watermarker**. Perpustakaan memungkinkan Anda menambahkan beberapa tanda air jika diperlukan untuk meningkatkan perlindungan. Sebaiknya simpan dokumen Webp yang telah diubah ke lokasi terpisah dan aman untuk menyimpan file asli dan mengamankan dokumen yang diberi watermark.
   
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

        // Buat tanda air gambar untuk WEBP

        // Buat instance Watermarker yang meneruskan file sumber
        const watermarker = new groupdocs.watermark.Watermarker("input.webp");
        
        // Hasilkan tanda air dengan menyediakan file gambar
        const watermark = new groupdocs.watermark.ImageWatermark("watermark.png");

        // Dapatkan hasil WEBP
        watermarker.add(watermark);
        watermarker.save("output.webp");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Integrasi Watermark yang Disempurnakan"
  description: "GroupDocs.Watermark API kami untuk .NET pengembang menawarkan solusi yang disempurnakan untuk mengintegrasikan tanda air secara mulus ke dalam dokumen apa pun. Alat ini dirancang untuk membuat tanda air canggih dan tidak mencolok yang memastikan perlindungan hak cipta sambil mempertahankan estetika dokumen."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Integrasi Tanda Air Presisi"
  features:
    # feature loop
    - title: "Efek Tanda Air Gradien"
      content: "Terapkan tanda air gradien yang menyatu dengan lancar di seluruh dokumen Anda. Fitur ini memungkinkan gradien linier atau radial, menambahkan tampilan modern ke fitur keamanan yang meningkatkan perlindungan dan keterlibatan visual tanpa mengalahkan konten."

    # feature loop
    - title: "Tanda Air Pola untuk Keamanan Ekstra"
      content: "Gunakan watermarking berbasis pola untuk menambahkan lapisan keamanan ekstra. API kami mendukung berbagai pola yang dapat dirancang dan diulang secara rumit di seluruh dokumen, membuat tanda air lebih tahan terhadap gangguan dan penghapusan."

    # feature loop
    - title: "Watermarking Khusus Dokumen"
      content: "Sesuaikan tanda air secara unik untuk berbagai jenis dokumen. Baik itu kontrak hukum, rencana bisnis, atau laporan ilmiah, sesuaikan tanda air agar sesuai dengan tujuan dokumen dan aksesibilitas pembaca, memastikan integrasi dan keamanan yang optimal."
      
  code_samples:
    # code sample loop
    - title: "Hasilkan tanda air gambar PDF"
      content: |
        Hasilkan tanda air gambar untuk semua gambar yang disajikan di dalam dokumen PDF
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  Muat dokumen sebagai PDF
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  Buat tanda air berdasarkan anotasi PDF
            const imageWatermark = new groupdocsWatermark.ImageWatermark("watermark.jpg");
            imageWatermark.setHorizontalAlignment(groupdocsWatermark.HorizontalAlignment.Center);
            imageWatermark.setVerticalAlignment(groupdocsWatermark.VerticalAlignment.Center);
            imageWatermark.setRotateAngle(-45);
            imageWatermark.setSizingType(groupdocsWatermark.SizingType.ScaleToParentDimensions);
            imageWatermark.setScaleFactor(1);
  
            //  Menyiapkan opsi tanda air
            const images = watermarker.getImages();
            for (let i = 0; i < images.getCount(); i++) {
                if (images.get_Item(i).getWidth() > 100 && images.get_Item(i).getHeight() > 100) {
                    images.get_Item(i).add(imageWatermark);
                }
            }

            //  Tambahkan tanda air teks ke dokumen hasil
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
    title: "Amankan WEBP File dengan Watermark Node.js"
    exclude: "WEBP"
    description: "Terapkan Node.js untuk menyisipkan tanda air yang dapat disesuaikan dan kuat ke gambar WEBP, memastikan hak cipta dan visibilitas merek dilindungi."
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