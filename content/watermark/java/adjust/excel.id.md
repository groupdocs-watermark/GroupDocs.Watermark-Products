
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:27
draft: false
lang: id
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Sesuaikan Alat Tanda Air Excel - GroupDocs.Watermark"
head_description: "Sesuaikan, perbarui, dan kelola tanda air dengan mudah dengan GroupDocs.Watermark. Sesuaikan dokumen Anda dengan mudah."

############################# Header ############################
title: "Sesuaikan Alat Watermark SpreadSheets: Sangat Sederhana" 
description: "Tingkatkan dokumen Anda dengan alat pengeditan tanda air intuitif kami. Sederhanakan alur kerja Anda dengan mudah."
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
    title: "GroupDocs.Watermark for Java API"
    link: "/watermark/java/"
    link_title: "Pelajari selengkapnya"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Alat Penyesuaian Watermark**: Alat watermarking kami menawarkan solusi yang mudah digunakan untuk meningkatkan dan melindungi dokumen Anda. Dengan fitur pengeditan intuitif, mengelola tanda air menjadi mudah, memastikan keamanan dan keaslian dokumen.

############################# Steps ############################
steps:
    enable: true
    title: "Sesuaikan tanda air pada dokumen Excel dengan Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** memudahkan pengembang Java untuk menyesuaikan tanda air teks di aplikasi mereka dengan menerapkan beberapa langkah mudah:
      
      1. Muat file Excel Anda ke objek utama API kami yang disebut **Watermarker**. Anda dapat menyediakan file untuk diproses lebih lanjut sebagai aliran atau sebagai jalur pada disk lokal.
      2. Langkah selanjutnya adalah mencari watermark yang harus disesuaikan. **SearchCriteria** membantu mengidentifikasi tanda air dengan properti yang tepat yang sebelumnya ditambahkan ke dokumen.
      3. Dapatkan daftar tanda air yang sesuai sebagai hasil dari prosedur **Search**. Sesuaikan properti tanda air yang ditemukan seperti ukuran, perataan halaman, teks, warna, konten gambar, dll. Ada banyak cara untuk menyesuaikan data Anda.
      4. Setelah menyelesaikan proses penyesuaian tanda air, Anda perlu menyimpan dokumen yang diperbarui. Gunakan jalur file lokal, aliran file atau byte untuk menyimpan hasil.
   
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

        // Sesuaikan tanda air teks EXCEL

        // Buat instance Watermarker dengan masukan dokumen EXCEL
        Watermarker watermarker = new Watermarker("input.xslx");

        // Inisialisasi TextSearchCriteria dan temukan tanda air teks
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        
        // Sesuaikan properti tanda air teks
        for (PossibleWatermark watermark : watermarks)
        {
            watermark.getFormattedTextFragments().clear();
            watermark.getFormattedTextFragments().
                add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
        }

        // Simpan dokumen yang diperbarui
        watermarker.save("output.xslx");
        
        ```            
        
############################# More features ############################
more_features:
  enable: true
  title: "Selami lebih dalam penyesuaian tanda air EXCEL"
  description: "API kami memberdayakan Java aplikasi untuk menambahkan, mengedit, menghapus, dan mencari tanda air di seluruh format dokumen populer."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Sesuaikan Tanda Air"
  features:
    # feature loop
    - title: "Tandai Dokumen Anda dengan Mudah"
      content: "GroupDocs.Watermark menyederhanakan watermarking untuk Java pengembang. Tambahkan tanda air yang beragam ke berbagai dokumen dan file bisnis. Anda tidak hanya dapat menerapkan tanda air, tetapi Anda juga dapat memperbarui atau menghapus yang sudah ada."

    # feature loop
    - title: "Sesuaikan Watermark dengan Kebutuhan Anda"
      content: "API kami menyediakan opsi penyesuaian yang luas. Sesuaikan ukuran, rotasi, warna, font, gaya, dan lainnya dengan mudah untuk mencapai tanda air yang sempurna."

    # feature loop
    - title: "Gunakan EXCEL Fitur Dokumen Asli"
      content: "Tergantung pada format dokumen tertentu, Anda dapat menggunakan fungsionalitas asli. Ini mungkin termasuk latar belakang halaman dokumen, anotasi, header, atau objek lain sebagai wadah tanda air."
      
  code_samples:
    # code sample loop
    - title: "PDF sesuaikan tanda air teks"
      content: |
        Contoh ini menunjukkan cara menyesuaikan teks artefak tertentu.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  Muat dokumen PDF
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  Dapatkan konten dokumen
        PdfContent pdfContent = watermarker.getContent(PdfContent.class);

        //  Sesuaikan teks tanda air tertentu
        for (PdfArtifact artifact : pdfContent.getPages().get_Item(0).getArtifacts())
        {
            if (artifact.getText().contains("Test"))
            {
                artifact.setText("Passed");
            }
        }

        //  Simpan dokumen
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
    title: "Sesuaikan Watermark melalui GroupDocs.Watermark for Java untuk format lain"
    exclude: "EXCEL"
    description: "Sesuaikan tanda air di berbagai format dokumen dengan mudah. Tingkatkan keamanan dan keaslian dokumen dengan mudah."
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