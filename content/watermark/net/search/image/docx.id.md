---
layout: "autogen"
draft: false
path: "watermark/net/search/image/docx/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "Cari Tanda Air Gambar dari DOCX di C# ASP.NET VB.NET"
head_description: ".Pustaka .NET untuk mencari tanda air gambar dari dokumen DOCX menggunakan fitur pencarian pintar dalam aplikasi C#, ASP.NET, VB.NET & .NET Core menggunakan API GroupDocs.Watermark untuk .NET."

title: "Cari Tanda Air Gambar dari DOCX di C#"
description: "Gunakan pencarian cerdas untuk menemukan semua kemungkinan tanda air gambar dari file DOCX dari dalam aplikasi C#, ASP.NET, VB.NET & .NET Core. Tentukan kriteria pencarian tp temukan semua tanda air gambar yang cocok dari seluruh atau halaman tertentu dari dokumen sumber."

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
    title_left: "Cari Tanda Air dari DOCX di .NET"
    content_left: |
        [GroupDocs.Watermark](/watermark/net/) memudahkan pengembang .NET untuk secara cerdas mencari tanda air gambar dari dalam dokumen mereka dengan menerapkan beberapa langkah mudah.

        * Instansiasi **Watermarker** dengan memasukkan dokumen DOCX.
        * Inisialisasi **ImageSearchCriteria** untuk melakukan pencarian tanda air.
        * Atur perbedaan maksimum yang diizinkan antara gambar.
        * Tampilkan kemungkinan tanda air yang cocok.
        
    title_right: "Persyaratan sistem"
    content_right: |
        Sebelum menjalankan contoh kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: Visual Studio, Xamarin, MonoDevelop
        * Kerangka: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Watermark untuk .NET dari [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)
        
    code: |
        ```cs
        // mencari kemungkinan tanda air GAMBAR dalam dokumen DOCX menggunakan C#, ASP.NET, VB.NET & .NET Core.
        // Instansiasi Watermarker dengan memasukkan dokumen DOCX
        using (Watermarker watermarker = new Watermarker(input.docx))
          {
            // Inisialisasi ImageSearchCriteria untuk memulai pencarian tanda air
            ImageSearchCriteria imageSearchCriteria = new ImageDctHashSearchCriteria(watermark.jpeg);

            // Tetapkan perbedaan maksimum yang diizinkan antara gambar sampel dan kemungkinan tanda air
            imageSearchCriteria.MaxDifference = 0.9;
            PossibleWatermarkCollection possibleWatermarks = watermarker.Search(imageSearchCriteria);
            Console.WriteLine("Found {0} possible watermark(s).", possibleWatermarks.Count);
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
