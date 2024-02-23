---
layout: "autogen"
draft: false
path: "watermark/java/add/text/vsdx/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "Tambahkan Tanda Air Teks ke VSDX di Java"
head_description: "Pustaka Java untuk menambahkan tanda air teks ke file VSDX di aplikasi Java & J2SE menggunakan GroupDocs.Watermark API untuk Java"

title: "Tambahkan Tanda Air Teks ke VSDX di Java"
description: "Menambahkan watermark teks ke file VSDX di aplikasi Java & J2SE. Kelola ukuran tanda air, jenis font, sudut rotasi, dan posisi tanda air pada halaman dokumen, sesuai kebutuhan Anda."

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
    title_left: "Tambahkan Tanda Air Teks ke File VSDX di Java"
    content_left: |
        [GroupDocs.Watermark](/watermark/java/) memudahkan pengembang Java untuk menambahkan tanda air teks dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Instansiasi **Watermarker** dengan memasukkan dokumen VSDX.
        * Inisialisasi **TextWatermarker** dengan teks watermark, ukuran font dan gaya.
        * Atur properti tanda air (perataan, warna, dll).
        * Tambahkan tanda air ke penanda air dan hasilkan dokumen keluaran.
        
    title_right: "Persyaratan sistem"
    content_right: |
        Sebelum menjalankan contoh kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: NetBeans, IntelliJ IDEA, Eclipse
        * Kerangka: Java 7 (1.7) dan di atasnya
        * Unduh versi terbaru GroupDocs.Watermark untuk Java dari [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
        
    code: |
        ```cs
        // Tambahkan tanda air teks ke VSDX di Java
        // Instansiasi Watermarker dengan memasukkan dokumen VSDX
        (Watermarker watermarker = new Watermarker(input.vsdx))
        
        // Instansiasi TextWatermarker dengan teks watermark, ukuran font dan gaya
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
            
        // Setel properti tanda air
        watermark.setForegroundColor(Color.getRed());
        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
        watermark.setVerticalAlignment(VerticalAlignment.Center);

        // Tambahkan tanda air dan simpan gambar yang diberi tanda air
        watermarker.add(watermark);
        watermarker.save(output.vsdx);
        
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
