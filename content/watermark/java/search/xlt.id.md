---
layout: "autogen"
draft: false
path: "watermark/java/search/xlt/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "Cari Tanda Air dari XLT di Jawa"
head_description: "Pustaka Java untuk mencari tanda air dari dokumen XLT menggunakan fitur pencarian pintar dalam aplikasi Java menggunakan GroupDocs.API Watermark untuk Java."

title: "Cari Tanda Air dari XLT di Jawa"
description: "Gunakan pencarian cerdas untuk menemukan semua kemungkinan tanda air dari file XLT dari dalam aplikasi Java & J2SE. Tentukan kriteria pencarian berdasarkan teks, ekspresi reguler (RegEx), gambar, hyperlink, karakter, dan objek pencarian yang berbeda untuk menemukan tanda air dari seluruh atau halaman tertentu dari dokumen sumber."

submenu:
    enable: true

about:
    enable: true
    title: "GroupDocs.Watermark untuk Java API"
    content: |
        GroupDocs.Watermark for Java adalah solusi manajemen watermark lengkap untuk aplikasi Java. Pengembang dapat dengan cepat melakukan operasi manipulasi tanda air seperti; tambahkan, edit, cari, dan hapus berbagai jenis tanda air dari dalam dokumen semua format file populer. Mendukung bekerja dengan teks dan tanda air gambar dalam berbagai dokumen termasuk PDF, Microsoft Word, Excel, PowerPoint, Visio, Email dan format gambar.
        
        GroupDocs.Watermark API didukung dengan baik di semua sistem operasi utama dan versi Java termasuk J2SE 7.0 (1.7), J2SE 8.0 (1.8) dan Java 10.

steps:
    enable: true
    title_left: "Cari Tanda Air dari XLT di Jawa"
    content_left: |
        [GroupDocs.Watermark](/watermark/java/) memudahkan pengembang Java untuk mencari tanda air secara cerdas dari dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Instansiasi **Watermarker** dengan memasukkan dokumen XLT.
        * Inisialisasi **PossibleWatermarkCollection** untuk melakukan pencarian tanda air.
        * Kriteria pencarian yang ditentukan untuk menemukan kemungkinan tanda air.
        
    title_right: "Persyaratan sistem"
    content_right: |
        Sebelum menjalankan contoh kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: NetBeans, IntelliJ IDEA, Eclipse
        * Kerangka: Java 7 (1.7) dan di atasnya
        * Unduh versi terbaru GroupDocs.Watermark untuk Java dari [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
        
    code: |
        ```cs
        // mencari kemungkinan tanda air dalam dokumen XLT menggunakan Java.
        // Instansiasi Watermarker dengan memasukkan dokumen XLT
        Watermarker watermarker = new Watermarker(input.xlt))

        // Inisialisasi KemungkinanWatermarkCollection untuk memulai pencarian tanda air
        PossibleWatermarkCollection possibleWatermarks = watermarker.search();
        for (PossibleWatermark possibleWatermark : possibleWatermarks)
        {
            if (possibleWatermark.getImageData() != null)
            {
                System.out.println(possibleWatermark.getImageData().length);
            }

            // Kriteria pencarian yang ditentukan untuk menemukan kemungkinan tanda air
            System.out.println(possibleWatermark.getText());
            System.out.println(possibleWatermark.getX());
            System.out.println(possibleWatermark.getY());
            System.out.println(possibleWatermark.getRotateAngle());
            System.out.println(possibleWatermark.getWidth());
            System.out.println(possibleWatermark.getHeight());
        }

        watermarker.close();
        ```        

demos:
    enable: true
        

about_formats:
    enable: true


more_formats:
    enable: true


back_to_top:
    enable: true
---
