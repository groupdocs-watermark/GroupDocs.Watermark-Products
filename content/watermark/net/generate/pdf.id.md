
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:27:05
draft: false
lang: id
format: Pdf
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Tanda Air C# untuk Dokumen Aman PDF"
head_description: "Gunakan .NET C# untuk menyematkan tanda air di PDF, mengamankan dokumen resmi dan informasi sensitif."

############################# Header ############################
title: "Tingkatkan Keamanan PDF dengan Watermark C#" 
description: "Terapkan .NET C# untuk menerapkan tanda air di PDF dokumen, memastikan perlindungan untuk catatan hukum, keuangan, dan resmi."
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh di Nuget secara gratis"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "Pelajari selengkapnya"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET menawarkan .NET pengembang C# API yang kuat untuk memasukkan tanda air ke file PDF, alat penting untuk keamanan dokumen di sektor perusahaan, hukum, dan pemerintah. API ini mendukung opsi penyesuaian tanda air yang komprehensif termasuk pemformatan teks, integrasi gambar, dan penempatan dinamis untuk mengakomodasi berbagai tata letak dokumen. Baik mengamankan perjanjian rahasia, melindungi materi hak cipta, atau menandai informasi kepemilikan, GroupDocs.Watermark memastikan bahwa semua PDF menyampaikan kepemilikan secara jelas dan profesional. Fitur tambahan termasuk rotasi tanda air, kontrol transparansi, dan kemampuan layering, kompatibel dengan semua kerangka kerja .NET modern.

############################# Steps ############################
steps:
    enable: true
    title: "Menghasilkan Watermark dengan Mudah untuk Pdf Dokumen"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/) :** Pustaka Watermarking Tingkat Lanjut untuk aplikasi .NET. Berdayakan solusi Anda dan amankan dokumen dengan tanda air tepat waktu.
      
      1. **Kelas Inti: Watermarker.** Kelas utama API kami adalah **Watermarker**. Anda perlu membuat instansiasinya sebelum pemrosesan dokumen. Jangan lupa untuk meneruskan file Pdf ke konstruktor sebagai jalur atau objek aliran.
      2. **Membuat Watermark Anda.** Langkah selanjutnya adalah membangun objek Watermark dari jenis yang diinginkan. Hal ini dapat ditempatkan tidak hanya pada halaman dokumen tertentu tetapi juga di bagian dokumen asli seperti gambar atau header.
      3. **Penampilan Penyetelan Sempurna.** Atur properti tanda air seperti tinggi dan lebar, atas, kiri, keselarasan tengah, font dan warna, dll.
      4. **Menerapkan dan Menyimpan.** Gunakan metode **Watermarker** untuk menambahkan tanda air baru. Jangan ragu untuk menambahkan tanda air sebanyak yang Anda butuhkan. Anda dapat menyimpan dokumen yang diberi tanda air ke lokasi mana pun.
   
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
        // Hasilkan tanda air gambar dalam file PDF

        // Berikan jalur file sumber ke konstruktor Watermarker
        using (Watermarker watermarker = new Watermarker("input.pdf"))
        {
            // Hasilkan contoh tanda air gambar dengan file gambar
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // Simpan hasil PDF yang ditandai dengan tanda air
            watermarker.Save("output.pdf");
        }
        
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "Tingkatkan Game Watermarking Anda"
  description: "Buka kemampuan watermarking tingkat lanjut dengan GroupDocs.Watermark API kami untuk .NET. Alat canggih ini memungkinkan penyesuaian dan penerapan tanda air yang tepat di berbagai jenis dokumen untuk memastikan keamanan maksimum dan kepatuhan hak cipta dengan gangguan visual minimal."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "Solusi Watermarking Komprehensif"
  features:
    # feature loop
    - title: "Opsi Ubin Canggih"
      content: "Perluas tanda air Anda ke seluruh dokumen dengan mulus dengan opsi ubin kami. Fitur ini memungkinkan tanda air untuk menutupi area dokumen lengkap, mencegah penghapusan dan memastikan perlindungan dokumen lengkap tanpa mengorbankan desain atau keterbacaan."

    # feature loop
    - title: "Kustomisasi Warna Cerah"
      content: "Tambahkan percikan warna ke tanda air Anda! API kami memungkinkan kustomisasi warna spektrum penuh, memungkinkan Anda menerapkan tanda air yang sangat cocok dengan merek perusahaan atau gaya dokumen Anda. Tingkatkan daya tarik visual sambil mempertahankan fitur keamanan yang kuat."

    # feature loop
    - title: "Pengaturan Keamanan yang Ditingkatkan"
      content: "Tingkatkan keamanan dokumen dengan pengaturan watermark tingkat lanjut. Konfigurasikan tanda air multi-layer, menggabungkan elemen yang terlihat dan tidak terlihat, untuk melindungi dari penyalinan yang tidak sah dan memastikan hanya penerima yang dituju yang dapat mengakses informasi penting."
      
  code_samples:
    # code sample loop
    - title: "Hasilkan tanda air PowerPoint"
      content: |
        Contoh ini menunjukkan cara menambahkan watermark ke gambar latar belakang PPTX
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Muat presentasi PPTX
            var loadOptions = new PresentationLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pptx", loadOptions))
            {
                //  Menyiapkan properti tanda air
                TextWatermark watermark = new TextWatermark("Protected image", new Font("Arial", 8));
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermark.RotateAngle = 45;
                watermark.SizingType = SizingType.ScaleToParentDimensions;
                watermark.ScaleFactor = 1;

                //  Latar belakang slide tanda air
                PresentationContent content = watermarker.GetContent<PresentationContent>();
                foreach (PresentationSlide slide in content.Slides)
                {
                    if (slide.ImageFillFormat.BackgroundImage != null)
                    {
                        slide.ImageFillFormat.BackgroundImage.Add(watermark);
                    }
                }

                //  Simpan presentasi yang diproses
                watermarker.save("result.pptx");
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
    title: "Mengamankan PDF File dengan .NET C# Watermark"
    exclude: "PDF"
    description: "Gunakan .NET C# untuk menyematkan tanda air yang aman dan disesuaikan dalam dokumen PDF, ideal untuk melindungi informasi resmi dan sensitif."
    items: 
        # format loop 1
        - name: "Tanda air PDF"
          format: "PDF"
          link: "/watermark/net/generate//pdf/"
          description: "Adobe Portable Format Dokumen"

        # format loop 2
        - name: "Tanda air Word"
          format: "WORD"
          link: "/watermark/net/generate//word/"
          description: "MS Word dan dokumen Open Office"
          
        # format loop 3
        - name: "Tanda air Excel"
          format: "EXCEL"
          link: "/watermark/net/generate//excel/"
          description: "MS Excel dan spreadsheet Open Office"

        # format loop 4
        - name: "Gambar Tanda Air"
          format: "IMAGE"
          link: "/watermark/net/generate//image/"
          description: "Format gambar populer"

        # format loop 5
        - name: "Foto Tanda Air"
          format: "PHOTO"
          link: "/watermark/net/generate//photo/"
          description: "Format foto"

        # format loop 6
        - name: "Tanda air PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/generate//powerpoint/"
          description: "MS PowerPoint dan presentasi Open Office"

        # format loop 7
        - name: "Tanda air DOCX"
          format: "DOCX"
          link: "/watermark/net/generate//docx/"
          description: "Microsoft Word Buka Dokumen XML"
          
        # format loop 8
        - name: "Tanda air PPTX"
          format: "PPTX"
          link: "/watermark/net/generate//pptx/"
          description: "PowerPoint Presentasi XML Terbuka"
          
        # format loop 9
        - name: "Tanda air XLSX"
          format: "XLSX"
          link: "/watermark/net/generate//xlsx/"
          description: "Microsoft Excel Buka Spreadsheet XML"

        # format loop 10
        - name: "Tanda air JPEG"
          format: "JPEG"
          link: "/watermark/net/generate//jpeg/"
          description: "JPEG Gambar"

        # format loop 11
        - name: "Tanda air PNG"
          format: "PNG"
          link: "/watermark/net/generate//png/"
          description: "Portable Grafik Jaringan"

        # format loop 12
        - name: "Tanda air TIFF"
          format: "TIFF"
          link: "/watermark/net/generate//tiff/"
          description: "Tag Format File Gambar"

        # format loop 13
        - name: "Tanda Air WEBP"
          format: "WEBP"
          link: "/watermark/net/generate//webp/"
          description: "Gambar WEB"

        # format loop 14
        - name: "Tanda air DOC"
          format: "DOC"
          link: "/watermark/net/generate//doc/"
          description: "Microsoft Word 97 - 2007 Dokumen"

        # format loop 15
        - name: "Tanda air XLS"
          format: "XLS"
          link: "/watermark/net/generate//xls/"
          description: "Microsoft Excel Buku Kerja 97-2003"

        # format loop 16
        - name: "Tanda air PPT"
          format: "PPT"
          link: "/watermark/net/generate//ppt/"
          description: "PowerPoint Presentasi 97-2003"

        # format loop 17
        - name: "Tanda air RTF"
          format: "RTF"
          link: "/watermark/net/generate//rtf/"
          description: "Format Teks Kaya"

---