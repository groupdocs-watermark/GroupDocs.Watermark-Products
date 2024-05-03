
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:04
draft: false
lang: id
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Hasilkan Watermark di Excel Spreadsheet untuk Java"
head_description: "Mudah menerapkan pembuatan watermark teks dan gambar di Excel dengan Java untuk melindungi spreadsheet data Excel Anda"

############################# Header ############################
title: "Otomatis Excel Watermarking dengan Java Code" 
description: "Terapkan teks kustom atau tanda air gambar di lembar bentang Excel menggunakan Java. Panduan ini menawarkan petunjuk langkah demi langkah untuk meningkatkan keamanan dokumen dan branding, yang disesuaikan untuk berbagai kebutuhan profesional."
subtitle: "GroupDocs.Watermark for Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduhan gratis Maven"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java perpustakaan"
    link: "/watermark/java/"
    link_title: "Pelajari selengkapnya"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java menawarkan manajemen tanda air yang komprehensif dalam spreadsheet Excel, memungkinkan pengembang untuk dengan mudah membuat, menyesuaikan, dan menghapus tanda air. Ini mendukung semua format file Excel populer, memungkinkan penyematan tanda air teks dan gambar yang dapat disesuaikan dalam font, warna, ukuran, dan posisi. GroupDocs.Watermark juga menyertakan fitur untuk pencarian tanda air, memastikan bahwa tanda air Anda utuh dan tahan rusak. Ideal untuk aplikasi yang membutuhkan peningkatan keamanan dokumen dalam lingkungan Java.

############################# Steps ############################
steps:
    enable: true
    title: "Tambahkan Tanda Air ke Dokumen Excel melalui Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** memudahkan pengembang Java untuk menambahkan berbagai jenis tanda air ke format file bisnis populer. Tambahkan perpustakaan kami ke aplikasi Anda dan beri tanda air pada dokumen Anda dalam beberapa langkah mudah seperti yang tercantum di bawah ini.
      
      1. Kelas utama API kami adalah **Watermarker**. Anda perlu membuat instance sebelum pemrosesan dokumen. Jangan lupa meneruskan file Excel ke konstruktor sebagai jalur atau objek aliran.
      2. Langkah selanjutnya adalah membuat objek **Watermark** dengan tipe yang diinginkan. Itu dapat ditempatkan tidak hanya pada halaman dokumen tertentu tetapi juga di bagian dokumen asli seperti lampiran atau header.
      3. Atur properti tanda air seperti tinggi dan lebar, perataan halaman (atas, kiri, tengah, dll.), jenis dan warna font, dan banyak lainnya.
      4. Panggil metode **Watermarker** untuk menambahkan tanda air baru. Anda dapat menambahkan tanda air sebanyak yang Anda perlukan. Disarankan untuk menyimpan dokumen yang diproses ke lokasi lain.
   
    code:
      platform: "net"
      copy_title: "Salin"
      install:
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-watermark</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "klik untuk menyalin"
        copy_done: "menyalin"
      links:
        #  loop
        - title: "Lebih banyak contoh"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/watermark/java/"
          
      content: |
        ```java {style=abap}

        // Tambahkan tanda air teks ke EXCEL

        // Berikan file yang akan diberi watermark ke Watermarker
        Watermarker watermarker = new Watermarker("input.xslx");
        
        // Buat tanda air teks dan atur properti
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        watermark.setForegroundColor(Color.getRed());

        // Simpan file yang diberi tanda air
        watermarker.add(watermark);
        watermarker.save("output.xslx");
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "Tingkatkan Watermark Anda dengan Mudah"
  description: "Manfaatkan kekuatan GroupDocs.Watermark untuk menghasilkan, menyusun, dan menambahkan tanda air di berbagai format dokumen. API ini tidak hanya meningkatkan keamanan dokumen tetapi juga melindungi kekayaan intelektual Anda dengan menyematkan tanda air yang dapat disesuaikan yang serbaguna dan kuat."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Tambahkan Watermark"
  features:
    # feature loop
    - title: "Opsi Tanda Air Serbaguna."
      content: "Jelajahi berbagai pilihan watermarking dengan GroupDocs.Watermark. Dari menyesuaikan opasitas dan rotasi hingga ukuran penskalaan secara proporsional, API kami memungkinkan Anda menyesuaikan tanda air dengan tepat sesuai kebutuhan Anda, memastikan bahwa tanda air tersebut menyatu dengan mulus dengan dokumen Anda sambil mempertahankan integritas konten."

    # feature loop
    - title: "Penataan Tanda Air Tingkat Lanjut."
      content: "GroupDocs.Watermark memungkinkan Anda untuk menata tanda air Anda dengan berbagai font, warna, dan bayangan, membuatnya khas dan lebih sulit untuk dihapus. Tingkatkan daya tarik estetika dokumen dan gambar Anda yang dilindungi dengan tanda air bergaya yang mencerminkan identitas dan profesionalisme merek Anda."

    # feature loop
    - title: "Ubin & Pemosisian Tanda Air"
      content: "Dengan GroupDocs.Watermark, terapkan efek ubin untuk menutupi seluruh dokumen Anda, memastikan perlindungan lengkap. Posisikan tanda air tepat di tempat yang Anda butuhkan — lokasi tengah, sudut, atau kustom. Opsi penentuan posisi fleksibel kami membantu melindungi dokumen Anda dari penggunaan dan duplikasi yang tidak sah."
      
  code_samples:
    # code sample loop
    - title: "PDF tanda air anotasi"
      content: |
        Contoh ini menunjukkan cara menambahkan anotasi tanda air ke dokumen PDF
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Muat dokumen sebagai PDF
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Buat tanda air berdasarkan anotasi PDF
        PdfAnnotationWatermarkOptions options = new PdfAnnotationWatermarkOptions();
        TextWatermark textWatermark = new TextWatermark("Annotation watermark", new Font("Arial", 8));

        //  Menyiapkan opsi tanda air
        textWatermark.setHorizontalAlignment(HorizontalAlignment.Left);
        textWatermark.setVerticalAlignment(VerticalAlignment.Top);

        //  Tambahkan tanda air teks ke dokumen hasil
        watermarker.add(textWatermark, options);
        watermarker.save("result.pdf");

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Watermark secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "Maven unduhan"
      link: "https://releases.groupdocs.com/watermark/java/"
      color: "red"
        #  loop
    - title: "Perizinan"
      link: "https://purchase.groupdocs.com/pricing/watermark/java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Java Teknik untuk Excel Watermarking"
    exclude: "EXCEL"
    description: "Menggunakan GroupDocs.Watermark for Java, dengan mudah menerapkan tanda air berbasis teks atau gambar ke lembar bentang Excel, secara signifikan meningkatkan keamanan dokumen dan branding sebagai bagian dari alur kerja bisnis Anda."
    items: 
        # format loop 1
        - name: "Tanda air PDF"
          format: "PDF"
          link: "/watermark/java/add//pdf/"
          description: "Adobe Portable Format Dokumen"

        # format loop 2
        - name: "Tanda air Word"
          format: "WORD"
          link: "/watermark/java/add//word/"
          description: "MS Word dan dokumen Open Office"
          
        # format loop 3
        - name: "Tanda air Excel"
          format: "EXCEL"
          link: "/watermark/java/add//excel/"
          description: "MS Excel dan spreadsheet Open Office"

        # format loop 4
        - name: "Gambar Tanda Air"
          format: "IMAGE"
          link: "/watermark/java/add//image/"
          description: "Format gambar populer"

        # format loop 5
        - name: "Foto Tanda Air"
          format: "PHOTO"
          link: "/watermark/java/add//photo/"
          description: "Format foto"

        # format loop 6
        - name: "Tanda air PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/add//powerpoint/"
          description: "MS PowerPoint dan presentasi Open Office"

        # format loop 7
        - name: "Tanda air DOCX"
          format: "DOCX"
          link: "/watermark/java/add//docx/"
          description: "Microsoft Word Buka Dokumen XML"
          
        # format loop 8
        - name: "Tanda air PPTX"
          format: "PPTX"
          link: "/watermark/java/add//pptx/"
          description: "PowerPoint Presentasi XML Terbuka"
          
        # format loop 9
        - name: "Tanda air XLSX"
          format: "XLSX"
          link: "/watermark/java/add//xlsx/"
          description: "Microsoft Excel Buka Spreadsheet XML"

        # format loop 10
        - name: "Tanda air JPEG"
          format: "JPEG"
          link: "/watermark/java/add//jpeg/"
          description: "JPEG Gambar"

        # format loop 11
        - name: "Tanda air PNG"
          format: "PNG"
          link: "/watermark/java/add//png/"
          description: "Portable Grafik Jaringan"

        # format loop 12
        - name: "Tanda air TIFF"
          format: "TIFF"
          link: "/watermark/java/add//tiff/"
          description: "Tag Format File Gambar"

        # format loop 13
        - name: "Tanda Air WEBP"
          format: "WEBP"
          link: "/watermark/java/add//webp/"
          description: "Gambar WEB"

        # format loop 14
        - name: "Tanda air DOC"
          format: "DOC"
          link: "/watermark/java/add//doc/"
          description: "Microsoft Word 97 - 2007 Dokumen"

        # format loop 15
        - name: "Tanda air XLS"
          format: "XLS"
          link: "/watermark/java/add//xls/"
          description: "Microsoft Excel Buku Kerja 97-2003"

        # format loop 16
        - name: "Tanda air PPT"
          format: "PPT"
          link: "/watermark/java/add//ppt/"
          description: "PowerPoint Presentasi 97-2003"

        # format loop 17
        - name: "Tanda air RTF"
          format: "RTF"
          link: "/watermark/java/add//rtf/"
          description: "Format Teks Kaya"

---