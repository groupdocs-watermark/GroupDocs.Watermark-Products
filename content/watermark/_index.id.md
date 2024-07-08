---
############################# Static ############################
layout: "family"
date:  2024-07-08T16:36:26
draft: false

product: "Watermark"
product_tag: "watermark"

lang: id

############################# Head ############################
head_title: "Tanda Air Dokumen C# Java Node.js Python | tambahkan tanda air"
head_description: "Tambahkan watermark ke PDF, gambar dan dokumen. Solusi Watermarking untuk Microsoft Office, PDF, OpenDocument, Gambar dan lain-lain."

############################# Header ############################
title: "Solusi Watermark Dokumen"
description:  |
  Tambahkan tanda air teks dan gambar untuk dokumen dan gambar Anda.

  Cari dan ubah tanda air dokumen dengan cara yang nyaman.

  Dapatkan info tentang tanda air yang disajikan dalam dokumen Anda.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Pilih platform Anda"
  title: "Independensi platform"
  description: "GroupDocs.Watermark library mendukung sistem operasi dan kerangka kerja berikut:"
  details_link_title: "Pelajari selengkapnya"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Watermark .NET 
      color: "blue"
      tag: "net"
      link: "/watermark/net/"
      features_link: "https://docs.groupdocs.com/watermark/net/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    .NET Framework 4.5 or higher <br> .NET Core 3.0 or higher <br> .NET 5.0 or higher
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Watermark Java
      color: "red"
      tag: "java"
      link: "/watermark/java/"
      features_link: "https://docs.groupdocs.com/watermark/java/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    Java 8 or higher <br> Kotlin
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Watermark Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/watermark/nodejs-java/"
      features_link: "https://docs.groupdocs.com/watermark/"
      features:
          # features loop
          - rows: "4"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Editor teks lainnya
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Python"
      description: GroupDocs.Watermark Python
      color: "yellow"
      tag: "python-net"
      link: "/watermark/python-net/"
      features_link: "https://docs.groupdocs.com/watermark/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Python 3.9+ and .Net 6+
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "4"
            content: |
                    IDLE <br> PyCharm <br> Visual Studio Code
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Watermark ulasan fitur"
  description: "Perpustakaan dirancang untuk menambah, mencari, dan memperbarui berbagai jenis tanda air untuk format dokumen populer."

  items:
    # items loop
    - icon: "protect"
      title: "Lindungi file dengan tanda air"
      content: "Tambahkan tanda air teks dan gambar ke dokumen bisnis Anda."

    # items loop
    - icon: "search"
      title: "Cari tanda air yang ada"
      content: "Dapatkan informasi terperinci tentang tanda air yang ditempatkan dalam dokumen sebelumnya."

    # items loop
    - icon: "manipulate"
      title: "Memanipulasi tanda air dokumen"
      content: "Kontrol teks, gaya, gambar, dan fitur tanda air lainnya."

    # items loop
    - icon: "additional"
      title: "Berbagai fitur tambahan"
      content: "Dapatkan info dokumen, perbarui tautan hiper-atau halaman latar belakang dll."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Lindungi dokumen dengan tanda air"
  description: "GroupDocs.Watermark contoh kode operasi tipikal."
  items:
    # code sample loop
    - title: "Membuat tanda air."
      content: |
       Untuk menambahkan tanda air ke dokumen, berikan jalur ke file target. Anda memiliki banyak opsi untuk dipilih untuk mendapatkan tanda air yang disesuaikan pada halaman tertentu.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Tentukan dokumen yang akan diberi tanda air
            using (Watermarker watermarker = new Watermarker("source.docx"))
            {
                // Buat objek watermark
                TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                // Mengatur opsi tanda air
                watermark.ForegroundColor = Color.Red;
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;

                // Tambahkan watermark dan simpan file yang diproses
                watermarker.Add(watermark);
                watermarker.Save("result.docx");
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Tentukan dokumen yang akan diberi tanda air
            Watermarker watermarker = new Watermarker("source.docx");

            // Buat objek watermark
            TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

            // Mengatur opsi tanda air
            watermark.setForegroundColor(Color.getRed());
            watermark.setHorizontalAlignment(HorizontalAlignment.Center);
            watermark.setVerticalAlignment(VerticalAlignment.Center);

            // Tambahkan watermark dan simpan file yang diproses
            watermarker.add(watermark);
            watermarker.save("result.docx");
            watermarker.close();
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            // Tentukan dokumen yang akan diberi tanda air
            const watermarker = new Watermarker("source.docx");

            // Buat objek watermark
            const watermark = new TextWatermark("top secret", new Font("Arial", 36));

            // Mengatur opsi tanda air
            watermark.setForegroundColor(Color.getRed());
            watermark.setHorizontalAlignment(HorizontalAlignment.Center);
            watermark.setVerticalAlignment(VerticalAlignment.Center);

            // Tambahkan watermark dan simpan file yang diproses
            watermarker.add(watermark);
            watermarker.save("result.docx");
            ```
        - language: "Python"
          color: "yellow"
          content: |
            ```python {style=abap}  
            def run():
                # Tentukan dokumen yang akan diberi tanda air
                with groupdocs.watermark.Watermarker("source.docx") as watermarker:
                    font = groupdocs.watermark.watermarks.Font("Arial", 36.0)

                    # Buat objek watermark
                    watermark = groupdocs.watermark.watermarks.TextWatermark("top secret", font)

                    # Mengatur opsi tanda air
                    watermark.foreground_color = groupdocs.watermark.watermarks.Color.red;
                    watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
                    watermark.vertical_alignment = groupdocs.watermark.common.VerticalAlignment.CENTER

                    # Tambahkan watermark dan simpan file yang diproses
                    watermarker.add(watermark)
                    watermarker.save("result.docx")
            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "50+ format file didukung"
  description: "GroupDocs.Watermark menyediakan watermarking untuk dokumen populer dan format file."

############################# Metrics ###############################
metrics:
  enable: true
  title: "Data statistik perpustakaan kami"
  description: "Selami metrik utama, ungkapkan wawasan tentang pencapaian, dampak, dan pertumbuhan kami."

  items:
    # items loop
    - number: "50+"
      title: "Format yang didukung"
      content: "Perpustakaan dapat memproses lebih dari 50 format file paling populer."

    # items loop
    - number: "500k"
      title: "NuGet unduhan"
      content: "GroupDocs.Watermark untuk .NET adalah perpustakaan populer dengan lebih dari 500.000 unduhan di NuGet."

    # items loop
    - number: "15k"
      title: "Unduhan Maven"
      content: "Dengan lebih dari 15K unduhan di Maven, GroupDocs.Watermark adalah pilihan populer bagi Java pengembang."

    # items loop
    - number: "140+"
      title: "Pelanggan yang bahagia"
      content: "Pengembang individu dan perusahaan top di seluruh dunia lebih memilih perpustakaan kami untuk membangun solusi inovatif."


############################# Customers ###############################
customers:
  enable: true
  title: "Pelanggan kami yang bahagia"
  description: "GroupDocs perpustakaan dipekerjakan oleh merek-merek terkenal dan terkemuka di seluruh dunia."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Watermark secara gratis di platform Anda"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/watermark/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/watermark/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/watermark/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "Pertanyaan yang sering diajukan"
  description: "Lihat Pertanyaan yang Sering Diajukan"

  items:
    # items loop
    - question: "Apakah perpustakaan eksternal diperlukan oleh GroupDocs.Watermark untuk manipulasi dokumen?"
      answer: "GroupDocs.Watermark bekerja secara independen, tidak perlu perangkat lunak pihak ketiga seperti Adobe Acrobat, Microsoft Office, dll."

    # items loop
    - question: "Dapatkah saya menguji fitur GroupDocs.Watermark sebelum membeli?"
      answer: "Ya, GroupDocs.Watermark menawarkan uji coba gratis! Instal dan coba, tetapi perlu diingat: Versi uji coba menambahkan 'lencana percoba' ke dokumen Anda, hanya 3 halaman pertama yang diproses. Ingin pengalaman penuh? Dapatkan lisensi sementara 30 hari gratis untuk fungsionalitas penuh. Lihat detail di bawah [lisensi sementara](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Jenis lisensi apa yang disediakan?"
      answer: "Butuh lisensi GroupDocs.Watermark? Kami punya pilihan! Pilih dari lisensi berdasarkan banyak opsi. Jumlah pengembang dalam tim Anda. Lokasi penyebaran seperti kantor tunggal atau tempat kerja jarak jauh. Apakah distribusi pelanggan akhir perlu berbagi SDK/API dengan klien? Atau, ada lisensi untuk penggunaan bulanan: Bayar hanya untuk apa yang Anda gunakan dengan paket terukur. Selami lebih dalam dan temukan [harga](https://purchase.groupdocs.com/pricing/watermark/net/) yang sempurna."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Watermark API kode rendah"
  description: "Tambahkan tanda air ke file oleh aplikasi Anda menggunakan REST API berbasis cloud kami."
  
  items:
    # items loop
    - title: "GroupDocs.Watermark Cloud for cURL"
      content: "Gunakan cURL REST ful API untuk menandai PDF, Word, Excel, PowerPoint, JPEG dan format file populer lainnya."
      icon: "groupdocs_watermark-for-curl"
      link: "https://products.groupdocs.cloud/watermark/curl"

    # items loop
    - title: "GroupDocs.Watermark Cloud for .NET"
      content: "Berdayakan aplikasi .NET Anda dengan fitur watermarking dokumen oleh Cloud SDK untuk .NET. Lindungi dokumen bisnis Anda sendiri."
      icon: "groupdocs_watermark-for-net"
      link: "https://products.groupdocs.cloud/watermark/net"

    # items loop
    - title: "GroupDocs.Watermark Cloud for Java"
      content: "GroupDocs.Watermark SDK yang dirancang untuk Java memberikan kemungkinan baru untuk aplikasi Java dan file bisnis Anda."
      icon: "groupdocs_watermark-for-java"
      link: "https://products.groupdocs.cloud/watermark/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Watermark Aplikasi web"
  description: "GroupDocs memberikan akses ke aplikasi web untuk menambahkan tanda air ke dokumen Anda. Lebih dari 50 format file populer dapat diberi tanda air di browser favorit Anda SECARA GRATIS."

  items:
    # items loop
    - title: "GroupDocs.Watermark Total"
      content: "Alat online untuk menambahkan tanda air ke dokumen dari perangkat apa pun."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/watermark/total"

    # items loop
    - title: "GroupDocs.Watermark DOCX"
      content: "Watermark MS Word DOCX online."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/watermark/docx"

    # items loop
    - title: "GroupDocs.Watermark PDF"
      content: "Lindungi PDF dokumen secara online."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/watermark/pdf"


      


---