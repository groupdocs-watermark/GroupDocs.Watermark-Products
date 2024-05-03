
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:12
draft: false
lang: id
format: Png
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Amankan PNG dengan .NET C# Watermark"
head_description: "Sematkan tanda air ke file PNG menggunakan .NET C #, sempurna untuk hak cipta gambar dan keamanan."

############################# Header ############################
title: "C# Watermarking untuk PNG File" 
description: "Gunakan .NET C# untuk menerapkan tanda air tingkat lanjut ke PNG gambar, menjaga konten artistik dan digital secara efektif."
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
       GroupDocs.Watermark for .NET menyediakan toolkit khusus .NET C# untuk menyematkan tanda air di file PNG, melayani seniman, desainer, dan pembuat konten yang perlu melindungi aset visual mereka. API ini memungkinkan penambahan tanda air transparan dan buram tanpa batas yang dapat diposisikan dan diskalakan secara rumit untuk menjaga integritas gambar asli sambil memastikan perlindungan hukum. Fitur termasuk teks kustom dan tanda air gambar, kontrol yang tepat atas opacity watermark, dan kemampuan untuk menambahkan tanda air multi-layer untuk meningkatkan keamanan. Baik untuk penggunaan pribadi atau portofolio profesional, GroupDocs.Watermark memastikan PNG gambar Anda dilindungi dari reproduksi dan penggunaan yang tidak sah, didukung sepenuhnya di lingkungan .NET.

############################# Steps ############################
steps:
    enable: true
    title: "Menghasilkan Tanda Air dengan Mudah untuk Dokumen Png"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/):** Pustaka Watermarking tingkat lanjut untuk aplikasi .NET. Berdayakan solusi Anda dan amankan dokumen dengan tanda air tepat pada waktunya.
      
      1. **Kelas Inti: Watermarker.** Kelas utama API kami adalah **Watermarker**. Anda perlu membuat instance sebelum pemrosesan dokumen. Jangan lupa meneruskan file Png ke konstruktor sebagai jalur atau objek aliran.
      2. **Membuat Tanda Air Anda.** Langkah selanjutnya adalah membuat objek Tanda Air dengan jenis yang diinginkan. Itu dapat ditempatkan tidak hanya pada halaman dokumen tertentu tetapi juga di bagian dokumen asli seperti gambar atau header.
      3. **Penyempurnaan Tampilan.** Mengatur properti tanda air seperti tinggi dan lebar, perataan atas, kiri, tengah, font dan warna, dll.
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
        // Hasilkan tanda air gambar dalam file PNG

        // Berikan jalur file sumber ke konstruktor Watermarker
        using (Watermarker watermarker = new Watermarker("input.png"))
        {
            // Hasilkan contoh tanda air gambar dengan file gambar
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // Simpan hasil PNG yang diberi watermark
            watermarker.Save("output.png");
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
    title: "Menerapkan Watermark di PNG dengan C #"
    exclude: "PNG"
    description: "Terapkan .NET C# untuk membuat tanda air yang tersembunyi atau tebal dalam gambar PNG, memastikan fleksibilitas estetika dan perlindungan hak cipta yang kuat."
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