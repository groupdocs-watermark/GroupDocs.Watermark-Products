
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:26:57
draft: false
lang: id
format: Image
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Hasilkan Watermark Efektif untuk Gambar dengan Java"
head_description: "Gunakan Java untuk membuat tanda air canggih untuk Gambar. Lindungi dokumen Anda dan menegaskan hak cipta secara efektif."

############################# Header ############################
title: "Gambar Watermarking dengan mulus di Java" 
description: "Terapkan tanda air dinamis dalam file gambar Anda menggunakan Java. Alat ini memungkinkan penyesuaian posisi, skalabilitas, dan transparansi yang tepat untuk meningkatkan keamanan dan pengenalan merek."
subtitle: "GroupDocs.Watermark for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh di Maven secara gratis"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java"
    link: "/watermark/java/"
    link_title: "Pelajari selengkapnya"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java GroupDocs.Watermark for Java memungkinkan pengembang untuk secara efektif menghasilkan dan mengelola tanda air pada file gambar. Dengan dukungan untuk berbagai format gambar, pengguna dapat menerapkan tanda air teks dan grafik yang sepenuhnya dapat disesuaikan dalam posisi, skala, dan transparansi. Fungsi ini sangat penting untuk aplikasi di media digital, periklanan, dan distribusi konten online, di mana integritas branding dan hak cipta adalah yang terpenting. Selain itu, GroupDocs.Watermark menyertakan fitur untuk mencari dan menghapus tanda air yang ada, menyediakan alat serbaguna untuk manajemen dan keamanan gambar.

############################# Steps ############################
steps:
    enable: true
    title: "Tambahkan Watermark ke Dokumen Image melalui Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** memudahkan pengembang Java untuk menambahkan tanda air dari berbagai jenis ke format file bisnis populer. Tambahkan perpustakaan kami ke dokumen aplikasi dan tanda air Anda dalam beberapa langkah mudah seperti yang tercantum di bawah ini.
      
      1. **Watermarker**. Anda perlu membuat instansiasinya sebelum pemrosesan dokumen. Jangan lupa untuk meneruskan file Image ke konstruktor sebagai jalur atau objek aliran.
      2. **Watermark** dari jenis yang diinginkan. Itu dapat ditempatkan tidak hanya pada halaman dokumen tertentu tetapi juga di bagian dokumen asli seperti lampiran atau header.
      3. Tetapkan properti watermark seperti tinggi dan lebar, penyelarasan halaman (atas, kiri, tengah, dll.), Keluarga font dan warna, dan banyak lainnya.
      4. **Watermarker** untuk menambahkan tanda air baru. Anda dapat menambahkan tanda air sebanyak yang Anda butuhkan. Disarankan untuk menyimpan dokumen yang diproses ke lokasi lain.
   
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

        // Tambahkan tanda air teks ke IMAGE

        // Berikan file yang akan diberi tanda air ke Watermarker
        Watermarker watermarker = new Watermarker("input.jpeg");
        
        // Buat tanda air teks dan atur properti
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        watermark.setForegroundColor(Color.getRed());

        // Simpan file dengan tanda air
        watermarker.add(watermark);
        watermarker.save("output.jpeg");
        
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
    title: "Merampingkan keamanan Gambar dengan Watermarking di Java"
    exclude: "IMAGE"
    description: "Toolkit Java kami memungkinkan pembuatan tanda air yang dipersonalisasi untuk format gambar apa pun, meningkatkan keamanan dan branding. Watermark yang disesuaikan memastikan visual Anda dikenali dan dilindungi di berbagai media."
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