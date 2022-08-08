---
layout: "autogen"
draft: false
path: "watermark/java/edit/image/docm/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "Edit Tanda Air Gambar di DOCM di Jawa"
head_description: "Pustaka Java untuk mengedit tanda air gambar yang ditemukan dalam file DOCM di aplikasi Java & J2SE menggunakan GroupDocs.Watermark API untuk Java."

title: "Edit Tanda Air Gambar di DOCM di Jawa"
description: "Temukan & ubah tanda air gambar yang ditemukan dalam dokumen DOCM dalam aplikasi Java & J2SE. Tambahkan tanda air gambar BMP, PNG, GIF & JPEG ke dokumen. Juga kelola ukuran tanda air, jenis font, sudut rotasi, dan posisi tanda air pada halaman dokumen, sesuai kebutuhan Anda."

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
    title_left: "Edit Tanda Air Gambar dalam File DOCM di Jawa"
    content_left: |
        [GroupDocs.Watermark](watermark/java/) memudahkan pengembang Java untuk mengedit tanda air gambar (BMP, PNG, GIF, atau JPEG) dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Instansiasi **Watermarker** dengan memasukkan dokumen DOCM.
        * Inisialisasi **SearchCriteria** untuk menemukan watermark gambar.
        * Ganti tanda air yang ditemukan.
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
        // Temukan & ganti tanda air gambar dalam DOCM di aplikasi Java
        // Instansiasi Watermarker dengan memasukkan dokumen DOCM
        Watermarker watermarker = new Watermarker(input.docm)
        
        // Inisialisasi Kriteria Pencarian untuk mencocokkan gambar tertentu
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria(logo.png);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        for (PossibleWatermark watermark : watermarks)
            {
                try
                {
                    // Ganti gambar yang ditemukan
                    watermark.setImageData(imageData);
                }
                
                catch (Exception e)
                {
                    // Entitas yang ditemukan mungkin tidak mendukung pengeditan teks
                    // Argumen yang diteruskan dapat memiliki nilai yang tidak sesuai
                    // Proses kasus seperti itu di sini
                }
            }
            
            // Simpan dokumen yang diberi watermark
            watermarker.save(output.docm);

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
