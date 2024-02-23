---
layout: "autogen"
draft: false
path: "watermark/java/edit/text/pps/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "Edit Tanda Air Teks di PPS di Jawa"
head_description: "Pustaka Java untuk mengedit tanda air teks yang ditemukan dalam file PPS di aplikasi Java menggunakan GroupDocs.Watermark API untuk Java."

title: "Edit Tanda Air Teks di PPS di Jawa"
description: "Cari & ubah tanda air teks yang ditemukan dalam dokumen PPS dengan pemformatan dalam aplikasi Java & J2SE. Kelola ukuran tanda air, jenis font, sudut rotasi, dan posisi tanda air pada halaman dokumen, sesuai kebutuhan Anda."

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
    title_left: "Edit Tanda Air Teks dalam File PPS di Jawa"
    content_left: |
        [GroupDocs.Watermark](/watermark/java/) memudahkan pengembang Java untuk mengedit tanda air teks dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Instansiasi **Watermarker** dengan memasukkan dokumen PPS.
        * Inisialisasi **TextSearchCriteria** untuk mencari tanda air teks.
        * Edit teks tanda air yang ditemukan.
        * Atur properti tanda air (gaya font, warna, dll).
        * Simpan dokumen yang baru diberi watermark.
        
    title_right: "Persyaratan sistem"
    content_right: |
        Sebelum menjalankan contoh kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: NetBeans, IntelliJ IDEA, Eclipse
        * Kerangka: Java 7 (1.7) dan di atasnya
        * Unduh versi terbaru GroupDocs.Watermark untuk Java dari [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)
        
    code: |
        ```cs
        // Temukan & perbarui tanda air teks dengan pemformatan dalam PPS di aplikasi Java
        // Instansiasi Watermarker dengan memasukkan dokumen PPS
        Watermarker watermarker = new Watermarker(input.pps))
        
        // Inisialisasi TextSearchCriteria untuk menemukan teks watermark
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        for (PossibleWatermark watermark : watermarks)
        {
            try
            {
                // Edit teks dan atur properti tanda air
                watermark.getFormattedTextFragments().clear();
                watermark.getFormattedTextFragments().add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
            }
            catch (Exception e)
            {
                // Entitas yang ditemukan mungkin tidak mendukung pengeditan teks
                // Argumen yang diteruskan dapat memiliki nilai yang tidak sesuai
                // Proses kasus seperti itu di sini
            }
        }
            
        // Simpan dokumen yang diberi watermark
        watermarker.save(output.pps);

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
