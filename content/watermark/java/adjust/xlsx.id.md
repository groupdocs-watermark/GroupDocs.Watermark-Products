
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:10
draft: false
lang: id
format: Xlsx
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Sesuaikan & Kelola XLSX Watermark - GroupDocs.Watermark"
head_description: "Sederhanakan proses pengelolaan tanda air Anda dengan GroupDocs.Watermark. Sederhanakan perlindungan dokumen dan branding."

############################# Header ############################
title: "Streamline XLSX Manajemen Tanda Air: Kontrol Sederhana" 
description: "Sederhanakan proses pengelolaan tanda air Anda dengan solusi efisien kami. Fokus pada konten Anda dengan mudah."
subtitle: "GroupDocs.Watermark for Java Perpustakaan" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh di Maven secara gratis"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java Perpustakaan"
    link: "/watermark/java/"
    link_title: "Pelajari selengkapnya"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Sesuaikan Opsi Watermark**: Pindahkan tanda air pada halaman menggunakan solusi presisi kami. GroupDocs.Watermark menawarkan banyak opsi untuk penyesuaian tanda air dan memastikan keamanan dokumen.

############################# Steps ############################
steps:
    enable: true
    title: "Sesuaikan tanda air dokumen Xlsx menggunakan Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** memungkinkan pengembang Java menyesuaikan tanda air di banyak dokumen dengan mudah menggunakan aplikasi mereka. Berikut panduan singkatnya:
      
      1. Pertama, Anda harus meneruskan file Xlsx sebagai parameter konstruktor kelas **Watermarker**. Menyediakan aliran byte atau file atau jalur disk lokal.
      2. Kedua, temukan tanda air yang perlu disesuaikan. Gunakan **SearchCriteria** untuk mengidentifikasi tanda air dengan properti spesifik yang sebelumnya ditambahkan ke dokumen.
      3. Setelah pencarian, Anda akan menerima daftar tanda air yang relevan. Anda kemudian dapat menyesuaikan propertinya, termasuk ukuran, perataan halaman, teks, warna, konten gambar, dan banyak lagi. Ini menawarkan penyesuaian tingkat tinggi untuk data Anda.
      4. Setelah Anda selesai menyesuaikan tanda air, simpan dokumen yang diperbarui. Anda dapat menggunakan jalur file lokal, atau streaming untuk menyimpan hasilnya.
   
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
        // Sesuaikan tanda air gambar XLSX

        // Buat instance Watermarker dengan XLSX
        Watermarker watermarker = new Watermarker("input.xlsx");
        
        // Inisialisasi SearchCriteria agar cocok dengan gambar tertentu
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);

        for (PossibleWatermark watermark : watermarks)
        {
            // Ganti gambar yang ditemukan
            watermark.setImageData(imageData);
        }

        // Simpan file yang disesuaikan
        watermarker.save("output.xlsx");
        
        ```
        
############################# More features ############################
more_features:
  enable: true
  title: "Manajemen Tanda Air Tingkat Lanjut XLSX untuk Aplikasi Java"
  description: "GroupDocs.Watermark API memberdayakan pengembang untuk mengintegrasikan fungsionalitas watermarking dengan mulus ke dalam aplikasi Java mereka. Ini mendukung penambahan, pengeditan, penghapusan, dan pencarian tanda air di berbagai format dokumen."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Penyesuaian Tanda Air"
  features:
    # feature loop
    - title: "Integrasi Watermark yang Mudah"
      content: "GroupDocs.Watermark menyederhanakan proses penambahan tanda air yang beragam ke berbagai dokumen bisnis dan file dalam Java aplikasi. Pengembang tidak hanya dapat menerapkan tanda air, tetapi juga memperbarui atau menghapus yang sudah ada secara terprogram."

    # feature loop
    - title: "Kustomisasi Tanda Air Granular"
      content: "API menyediakan opsi penyesuaian ekstensif untuk tanda air. Pengembang dapat dengan mudah menyesuaikan ukuran, rotasi, warna, font, gaya, dan properti lainnya untuk mencapai efek visual yang diinginkan."

    # feature loop
    - title: "Memanfaatkan XLSX Fitur Dokumen Asli"
      content: "Tergantung pada format dokumen target, pengembang dapat menggunakan fungsi asli untuk penempatan tanda air. Fungsionalitas ini mungkin termasuk latar belakang halaman dokumen, anotasi, header, atau objek lain sebagai wadah tanda air."
      
  code_samples:
    # code sample loop
    - title: "Sesuaikan tanda air gambar di Spreadsheets"
      content: |
        Contoh ini menunjukkan cara menyesuaikan gambar bentuk tertentu dalam Lembar Kerja Excel.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Muat dokumen sebagai Spreadsheet
        SpreadsheetLoadOptions loadOptions = new SpreadsheetLoadOptions();
        Watermarker watermarker = new Watermarker("source.xlsx", loadOptions);

        //  Dapatkan byte tanda air baru
        File file = new File("new_watermark.png");
        byte[] imageBytes = new byte[(int) file.length()];
        FileInputStream inputStream = new FileInputStream(file);
        inputStream.read(imageBytes);
        inputStream.close();

        //  Sesuaikan konten tanda air tertentu
        for (SpreadsheetShape shape : content.getWorksheets().get_Item(0).getShapes())
        {
            if (shape.getImage() != null)
            {
                shape.setImage(new SpreadsheetWatermarkableImage(imageBytes));
            }
        }

        //  Simpan dokumen hasil
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
    title: "Gunakan GroupDocs.Watermark for Java untuk mengedit tanda air dalam format file lain"
    exclude: "XLSX"
    description: "Sederhanakan proses pengelolaan tanda air Anda di berbagai format dokumen. Fokus pada konten Anda dengan mudah sambil memastikan perlindungan dan branding."
    items: 
        # format loop 1
        - name: "Tanda air PDF"
          format: "PDF"
          link: "/watermark/java/adjust//pdf/"
          description: "Adobe Portable Format Dokumen"

        # format loop 2
        - name: "Tanda air Word"
          format: "WORD"
          link: "/watermark/java/adjust//word/"
          description: "MS Word dan dokumen Open Office"
          
        # format loop 3
        - name: "Tanda air Excel"
          format: "EXCEL"
          link: "/watermark/java/adjust//excel/"
          description: "MS Excel dan spreadsheet Open Office"

        # format loop 4
        - name: "Tanda air PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/adjust//powerpoint/"
          description: "MS PowerPoint dan presentasi Open Office"

        # format loop 5
        - name: "Tanda air DOCX"
          format: "DOCX"
          link: "/watermark/java/adjust//docx/"
          description: "Microsoft Word Buka Dokumen XML"
          
        # format loop 6
        - name: "Tanda air PPTX"
          format: "PPTX"
          link: "/watermark/java/adjust//pptx/"
          description: "PowerPoint Presentasi XML Terbuka"
          
        # format loop 7
        - name: "Tanda air XLSX"
          format: "XLSX"
          link: "/watermark/java/adjust//xlsx/"
          description: "Microsoft Excel Buka Spreadsheet XML"

        # format loop 8
        - name: "Tanda air DOC"
          format: "DOC"
          link: "/watermark/java/adjust//doc/"
          description: "Microsoft Word 97 - 2007 Dokumen"

        # format loop 9
        - name: "Tanda air XLS"
          format: "XLS"
          link: "/watermark/java/adjust//xls/"
          description: "Microsoft Excel Buku Kerja 97-2003"

        # format loop 10
        - name: "Tanda air PPT"
          format: "PPT"
          link: "/watermark/java/adjust//ppt/"
          description: "PowerPoint Presentasi 97-2003"

        # format loop 11
        - name: "Tanda air RTF"
          format: "RTF"
          link: "/watermark/java/adjust//rtf/"
          description: "Format Teks Kaya"

---