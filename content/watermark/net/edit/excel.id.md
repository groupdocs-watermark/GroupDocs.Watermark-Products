
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:26:59
draft: false
lang: id
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Edit Watermark dalam format Excel"
head_description: "Sesuaikan dan amankan dokumen Anda dengan mudah dengan GroupDocs.Watermark for .NET. Tingkatkan integritas dokumen dan edit Excel tanda air dengan mudah."

############################# Header ############################
title: "Edit Tanda Air Spreadsheet Excel Anda: Efisiensi .NET" 
description: "Tingkatkan keamanan dokumen Anda dengan alat watermarking kami yang dapat disesuaikan yang dirancang untuk efisiensi .NET. Edit tanda air Excel dengan mudah."
subtitle: "GroupDocs.Watermark for .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduhan gratis Nuget"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET Perpustakaan"
    link: "/watermark/net/"
    link_title: "Pelajari selengkapnya"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Edit Excel Tanda Air Dengan Alat Kami:** Alat GroupDocs.Watermark for .NET kami menawarkan strategi yang efisien untuk meningkatkan dan melindungi dokumen Anda. Dengan berbagai fitur untuk .NET pengembang, mengelola tanda air menjadi mudah, memastikan keamanan dan keaslian dokumen.

############################# Steps ############################
steps:
    enable: true
    title: "Edit tanda air di dokumen Excel menggunakan .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** memberdayakan .NET pengembang untuk mengedit tanda air dengan mudah dalam berbagai dokumen Excel. Berikut panduan sederhana cara menggunakan API kami di aplikasi Anda:
      
      1. **Watermarker**. Anda dapat menyediakan file baik sebagai aliran byte, aliran file, atau jalur disk lokal.
      2. **Kriteria pencari** untuk mengidentifikasi tanda air dengan properti terkait yang sebelumnya ditambahkan ke dokumen.
      3. Setelah pencarian, Anda akan mendapatkan daftar tanda air yang relevan. Anda kemudian dapat menyesuaikan propertinya, seperti ukuran, penyelarasan halaman, teks, warna, konten gambar, dan banyak lagi. Ini memberi Anda kontrol yang luas atas data Anda.
      4. Setelah Anda selesai mengedit tanda air, simpan dokumen yang diperbarui. Anda dapat menggunakan jalur file lokal atau aliran untuk menyimpan hasil akhir.
   
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
        // Mengedit EXCEL tanda air teks

        // Buat Watermarker menyediakan file EXCEL
        using (Watermarker watermarker = new Watermarker("input.xslx"))
        {
            // Bangun TextSearchCriteria dan dapatkan tanda air teks
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                 // Edit tanda air teks
                 watermark.FormattedTextFragments.Clear();
                 watermark.FormattedTextFragments.Add("passed", 
                    new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
            }

            // Simpan dokumen
            watermarker.Save("output.xslx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Pelajari lebih lanjut tentang modifikasi tanda air"
  description: "Berdayakan aplikasi .NET Anda dengan perpustakaan kami dan tambahkan, edit, hapus, atau cari tanda air dalam berbagai format file."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "Edit Tanda Air"
  features:
    # feature loop
    - title: "File Watermark untuk Bisnis Anda"
      content: "Gunakan GroupDocs.Watermark for .NET untuk menandai file dan dokumen. Tambahkan dan kelola tanda air tanpa upaya ekstra menerapkan API kami di aplikasi Anda. Cari, edit, dan hapus tanda air yang ditambahkan sebelumnya."

    # feature loop
    - title: "Sempurnakan Watermark untuk Kebutuhan Anda"
      content: "API kami menawarkan serangkaian opsi penyesuaian yang komprehensif. Ubah aspek seperti ukuran, orientasi, skema warna, keluarga font, dan banyak lagi dengan mudah untuk membuat tanda air yang ideal."

    # feature loop
    - title: "Manfaatkan Fitur Khusus Dokumen"
      content: "Tergantung pada format file yang Anda gunakan, Anda dapat memasukkan fungsionalitas bawaan. Ini mungkin termasuk latar belakang dokumen, anotasi, header, atau elemen lain untuk berfungsi sebagai wadah tanda air."
      
  code_samples:
    # code sample loop
    - title: "Excel pengeditan teks tanda air"
      content: |
        Contoh ini menunjukkan cara mengedit teks untuk tanda air tertentu di Excel Lembar Kerja
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Muat lembar bentang XLSX
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  Muat konten spreadsheet
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();

                //  Edit teks bagian dalam tanda air
                foreach (SpreadsheetShape shape in content.Worksheets[0].Shapes)
                {
                    if (shape.Text == "GroupDocs 2016")
                    {
                        shape.Text = "GroupDocs 2017";
                    }
                }

                //  Simpan hasil keluaran
                watermarker.save("result.xlsx");
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
    title: "Sesuaikan Watermark Anda dalam Format Lain"
    exclude: "EXCEL"
    description: "Tandai berbagai format dokumen sesuai kebutuhan Anda dengan GroupDocs.Watermark for .NET."
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