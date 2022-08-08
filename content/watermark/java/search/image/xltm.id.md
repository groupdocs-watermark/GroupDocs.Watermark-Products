---
layout: "autogen"
draft: false
path: "watermark/java/search/image/xltm/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "Cari Tanda Air Gambar dari XLTM di Jawa"
head_description: "Pustaka Java untuk mencari tanda air gambar dari dokumen XLTM menggunakan fitur pencarian cerdas dalam aplikasi Java & J2SE menggunakan GroupDocs.API Watermark untuk Java."

title: "Cari Tanda Air Gambar dari XLTM di Jawa"
description: "Gunakan pencarian cerdas untuk menemukan semua kemungkinan tanda air gambar dari file XLTM dari dalam aplikasi Java & J2SE. Tentukan kriteria pencarian untuk menemukan semua tanda air gambar yang cocok dari seluruh atau halaman tertentu dari dokumen sumber."

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
    title_left: "Cari Tanda Air dari XLTM di Jawa"
    content_left: |
        [GroupDocs.Watermark](watermark/java/) memudahkan pengembang Java untuk secara cerdas mencari tanda air gambar dari dalam dokumen mereka dengan menerapkan beberapa langkah mudah.

        * Instansiasi **Watermarker** dengan memasukkan dokumen XLTM.
        * Inisialisasi **ImageSearchCriteria** untuk melakukan pencarian tanda air.
        * Atur perbedaan maksimum yang diizinkan antara gambar.
        * Tampilkan kemungkinan tanda air yang cocok.
        
    title_right: "Persyaratan sistem"
    content_right: |
        Sebelum menjalankan contoh kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: NetBeans, IntelliJ IDEA, Eclipse
        * Kerangka: Java 7 (1.7) dan di atasnya
        * Unduh versi terbaru GroupDocs.Watermark untuk Java dari [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
        
    code: |
        ```cs
        // mencari kemungkinan tanda air GAMBAR dalam dokumen XLTM menggunakan Java.
        // Instansiasi Watermarker dengan memasukkan dokumen XLTM
        Watermarker watermarker = new Watermarker(input.xltm);
        
        // Inisialisasi ImageSearchCriteria untuk memulai pencarian tanda air
        ImageSearchCriteria imageSearchCriteria = new ImageDctHashSearchCriteria(watermark.jpeg);

        // Tetapkan perbedaan maksimum yang diizinkan antara gambar sampel dan kemungkinan tanda air
        imageSearchCriteria.setMaxDifference(0.9);
        PossibleWatermarkCollection possibleWatermarks = watermarker.search(imageSearchCriteria);
        System.out.println("Found " + possibleWatermarks.getCount() + " possible watermark(s).");

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
