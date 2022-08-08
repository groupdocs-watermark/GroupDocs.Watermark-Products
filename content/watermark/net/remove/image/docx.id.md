---
layout: "autogen"
draft: false
path: "watermark/net/remove/image/docx/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "Hapus Tanda Air Gambar dari DOCX di C# .NET"
head_description: ".Pustaka .NET untuk menemukan dan menghapus tanda air gambar dari dokumen DOCX menggunakan pencarian cerdas dalam aplikasi C#, ASP.NET, VB.NET & .NET Core menggunakan API GroupDocs.Watermark untuk .NET."

title: "Hapus Tanda Air Gambar dari DOCX di C#"
description: "Gunakan pencarian cerdas untuk menemukan & menghapus tanda air gambar dari dokumen DOCX dari dalam aplikasi C#, ASP.NET, VB.NET & .NET Core. Tentukan kriteria pencarian untuk mencari & menghapus tanda air yang ditentukan dari dokumen."

submenu:
    enable: true

about:
    enable: true
    title: "GroupDocs.Watermark untuk .NET API"
    content: |
        GroupDocs.Watermark untuk .NET adalah solusi manajemen tanda air lengkap untuk aplikasi .NET. Pengembang dapat dengan cepat melakukan operasi manipulasi tanda air seperti; tambahkan, edit, cari, dan hapus berbagai jenis tanda air dari dalam dokumen semua format file populer. Mendukung bekerja dengan teks dan tanda air gambar dalam berbagai dokumen termasuk PDF, Microsoft Word, Excel, PowerPoint, Visio, Email dan format gambar.
        
        GroupDocs.Watermark API didukung dengan baik di semua sistem operasi dan platform utama termasuk .NET Framework, .NET Standard, .NET Core, Mono, dan Xamarin.

steps:
    enable: true
    title_left: "Hapus Tanda Air dari File DOCX di .NET"
    content_left: |
        [GroupDocs.Watermark](watermark/net/) memudahkan pengembang .NET untuk mencari dan menghapus tanda air dengan pemformatan teks dari aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Instansiasi **Watermarker** dengan memasukkan dokumen DOCX.
        * Inisialisasi **SearchCriteria** untuk menemukan watermark gambar.
        * Hapus tanda air yang ditentukan dari dokumen.
        * Simpan dokumen yang dimodifikasi.
        
    title_right: "Persyaratan sistem"
    content_right: |
        Sebelum menjalankan contoh kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: Visual Studio, Xamarin, MonoDevelop
        * Kerangka: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Watermark untuk .NET dari [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)
        
    code: |
        ```cs
        // Cari & hapus tanda air gambar dengan dari dokumen DOCX di aplikasi C#, ASP.NET, VB.NET & .NET Core
        // Instansiasi Watermarker dengan memasukkan dokumen DOCX
        using (Watermarker watermarker = new Watermarker(input.docx))
          {
            // Inisialisasi Kriteria Pencarian untuk mencocokkan gambar tertentu
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria(logo.png);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            // Hapus tanda air yang ditentukan dari dokumen
            possibleWatermarks.Remove(possibleWatermarks[0]);

            // Simpan dokumen yang dimodifikasi
            watermarker.Save(output.docx);
          }
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
