
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:24
draft: false
lang: id
format: Pdf
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Edit Pdf Watermark dengan GroupDocs.Watermark"
head_description: "Edit tanda air Pdf di Pdf file menggunakan GroupDocs.Watermark for .NET Framework. Beradaptasi dengan kebutuhan dokumen Anda dengan mudah."

############################# Header ############################
title: "Edit Watermark di Pdf: .NET Kemampuan Beradaptasi" 
description: "Beradaptasi dengan kebutuhan dokumen Anda dengan mulus dengan GroupDocs.Watermark for .NET Framework. Edit tanda air di berbagai format dengan mudah."
subtitle: "GroupDocs.Watermark for .NET Solusi" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Gratis Nuget paket"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET Solusi"
    link: "/watermark/net/"
    link_title: "Pelajari selengkapnya"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Edit Tanda Air dalam PDF s:** Lindungi konten Anda di berbagai format dengan GroupDocs.Watermark for .NET Framework. Beradaptasi dengan kebutuhan dokumen Anda dengan mulus dengan alat serbaguna kami.

############################# Steps ############################
steps:
    enable: true
    title: "Mengedit Tanda Air secara terprogram di Dokumen Pdf dengan API .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** melengkapi pengembang .NET dengan API yang kuat untuk memanipulasi tanda air secara terprogram dalam beragam dokumen Pdf. Panduan ini menguraikan prosesnya:
      
      1. Mulailah alur kerja dengan menyediakan file Pdf Anda sebagai argumen ke konstruktor kelas **Watermarker**. File dapat disediakan sebagai aliran byte, aliran file, atau referensi ke lokasi disk lokal.
      2. Selanjutnya, manfaatkan objek **SearchCriteria** untuk menentukan tanda air spesifik yang memerlukan modifikasi. Objek ini memungkinkan identifikasi tanda air yang sebelumnya tertanam dalam dokumen.
      3. Setelah pencarian berhasil, Anda akan menerima kumpulan tanda air yang relevan. Tanda air ini menawarkan kontrol terperinci, memungkinkan Anda mengubah properti seperti dimensi, posisi halaman, konten teks, skema warna, data gambar, dan banyak lagi.
      4. Setelah pengeditan tanda air selesai, pertahankan dokumen yang dimodifikasi. API memfasilitasi penyimpanan menggunakan jalur file lokal atau objek aliran.
   
    code:
      platform: "net"
      copy_title: "Salin"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "klik untuk menyalin"
        copy_done: "menyalin"
      links:
        #  loop
        - title: "Lebih banyak contoh"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // Edit tanda air gambar di dokumen PDF

        // Inisialisasi Watermarker berdasarkan file sumber
        using (Watermarker watermarker = new Watermarker("input.pdf"))
        {
            // Buat SearchCriteria untuk pencarian tanda air gambar
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                // Edit tanda air gambar
                watermark.ImageData = imageData;
            }

            // Simpan hasil PDF
            watermarker.Save("output.pdf");
        }
        
        ```     

############################# More features ############################
more_features:
  enable: true
  title: "Tingkatkan Alur Kerja Anda dengan Manajemen Watermark"
  description: "Sederhanakan watermarking di berbagai format file di aplikasi .NET Anda dengan perpustakaan kami yang kuat. Tambahkan, edit, cari, atau hapus tanda air dengan mudah untuk meningkatkan keamanan dokumen dan branding."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Pengeditan Tanda Air yang Mulus"
  features:
    # feature loop
    - title: "Merampingkan Watermarking di Aplikasi Anda"
      content: "Manfaatkan kekuatan GroupDocs.Watermark for .NET untuk mengintegrasikan fungsionalitas watermarking dengan mulus ke dalam aplikasi .NET Anda. API intuitif kami menyederhanakan pembuatan, pengelolaan, pencarian, dan pengeditan watermark, menghilangkan kebutuhan akan proses manual yang kompleks."

    # feature loop
    - title: "Kustomisasi Tanda Air Granular"
      content: "Bebaskan potensi penuh kustomisasi tanda air dengan API komprehensif kami. Sempurnakan setiap detail, termasuk ukuran, orientasi, skema warna, dan pemilihan font, untuk membuat tanda air yang selaras dengan persyaratan merek dan keamanan Anda."

    # feature loop
    - title: "Memanfaatkan Fitur Khusus Dokumen untuk Watermarking Fleksibel"
      content: "Buka kekuatan fungsionalitas asli dalam berbagai format dokumen. Manfaatkan elemen seperti latar belakang dokumen, anotasi, header, atau objek lain sebagai wadah tanda air unik, melayani beragam jenis dokumen dan kebutuhan keamanan."
      
  code_samples:
    # code sample loop
    - title: "PDF pengeditan tanda air gambar"
      content: |
        Contoh ini menunjukkan cara mengedit konten tanda air gambar
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Muat dokumen sebagai PDF
            var loadOptions = new PdfLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pdf", loadOptions))
            {
                //  Muat konten
                PdfContent pdfContent = watermarker.GetContent<PdfContent>();

                //  Edit tanda air gambar
                foreach (PdfArtifact artifact in pdfContent.Pages[0].Artifacts)
                {
                    if (artifact.Image != null)
                    {
                        artifact.Image = new PdfWatermarkableImage(File.ReadAllBytes("test.png"));
                    }
                }

                //  Nikmati hasil keluaran
                watermarker.save("result.pdf");
            }

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Watermark secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "Nuget unduhan"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "Perizinan"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Sesuaikan Watermark dalam Berbagai Format"
    exclude: "PDF"
    description: "Lindungi konten Anda di berbagai format dokumen dengan GroupDocs.Watermark for .NET Framework."
    items: 
        # format loop 1
        - name: "Tanda air PDF"
          format: "PDF"
          link: "/watermark/net/edit//pdf/"
          description: "Adobe Portable Format Dokumen"

        # format loop 2
        - name: "Tanda air Word"
          format: "WORD"
          link: "/watermark/net/edit//word/"
          description: "MS Word dan dokumen Open Office"
          
        # format loop 3
        - name: "Tanda air Excel"
          format: "EXCEL"
          link: "/watermark/net/edit//excel/"
          description: "MS Excel dan spreadsheet Open Office"

        # format loop 4
        - name: "Tanda air PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/edit//powerpoint/"
          description: "MS PowerPoint dan presentasi Open Office"

        # format loop 5
        - name: "Tanda air DOCX"
          format: "DOCX"
          link: "/watermark/net/edit//docx/"
          description: "Microsoft Word Buka Dokumen XML"
          
        # format loop 6
        - name: "Tanda air PPTX"
          format: "PPTX"
          link: "/watermark/net/edit//pptx/"
          description: "PowerPoint Presentasi XML Terbuka"
          
        # format loop 7
        - name: "Tanda air XLSX"
          format: "XLSX"
          link: "/watermark/net/edit//xlsx/"
          description: "Microsoft Excel Buka Spreadsheet XML"

        # format loop 8
        - name: "Tanda air DOC"
          format: "DOC"
          link: "/watermark/net/edit//doc/"
          description: "Microsoft Word 97 - 2007 Dokumen"

        # format loop 9
        - name: "Tanda air XLS"
          format: "XLS"
          link: "/watermark/net/edit//xls/"
          description: "Microsoft Excel Buku Kerja 97-2003"

        # format loop 10
        - name: "Tanda air PPT"
          format: "PPT"
          link: "/watermark/net/edit//ppt/"
          description: "PowerPoint Presentasi 97-2003"

        # format loop 11
        - name: "Tanda air RTF"
          format: "RTF"
          link: "/watermark/net/edit//rtf/"
          description: "Format Teks Kaya"

---