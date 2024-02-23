---
layout: "autogen"
draft: false
path: "watermark/net/remove/text/sxc/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "Hapus Tanda Air dari SXC di C#, ASP.NET, VB.NET"
head_description: ".Pustaka .NET untuk menemukan dan menghapus tanda air dari dokumen SXC menggunakan pencarian cerdas dalam aplikasi C#, ASP.NET, VB.NET & .NET Core menggunakan API GroupDocs.Watermark untuk .NET."

title: "Hapus Tanda Air dari SXC di C# .NET"
description: "Gunakan pencarian cerdas untuk menemukan & menghapus tanda air dari dokumen SXC dengan pemformatan teks dari dalam aplikasi C#, ASP.NET, VB.NET & .NET Core. Tentukan kriteria pencarian untuk mencari & menghapus tanda air berdasarkan nama font tertentu, warna, ukuran dan properti lain yang cocok."

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
    title_left: "Hapus Tanda Air dari File SXC di .NET"
    content_left: |
        [GroupDocs.Watermark](/watermark/net/) memudahkan pengembang .NET untuk mencari dan menghapus tanda air dengan pemformatan teks dari aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Instansiasi **Watermarker** dengan memasukkan dokumen SXC.
        * Inisialisasi **TextFormattingSearchCriteria** untuk menemukan tanda air teks.
        * Inisialisasi kriteria pencarian yang ditentukan untuk menemukan & menghapus tanda air.
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
        // Cari & hapus tanda air dengan pemformatan teks dari dokumen SXC di aplikasi C#, ASP.NET, VB.NET & .NET Core
        // Instansiasi Watermarker dengan memasukkan dokumen SXC
        using (Watermarker watermarker = new Watermarker(input.sxc))
          {
            // Inisialisasi TextFormattingSearchCriteria untuk menentukan tanda air yang akan dicari
            TextFormattingSearchCriteria criteria = new TextFormattingSearchCriteria();
            criteria.ForegroundColorRange = new ColorRange();
            criteria.ForegroundColorRange.MinHue = -5;
            criteria.ForegroundColorRange.MaxHue = 10;
            criteria.ForegroundColorRange.MinBrightness = 0.01f;
            criteria.ForegroundColorRange.MaxBrightness = 0.99f;
            criteria.BackgroundColorRange = new ColorRange();
            criteria.BackgroundColorRange.IsEmpty = true;
            criteria.FontName = "Arial";
            criteria.MinFontSize = 19;
            criteria.MaxFontSize = 42;
            criteria.FontBold = true;

            PossibleWatermarkCollection watermarks = watermarker.Search(criteria);
            watermarks.Clear();

            // Simpan dokumen yang dimodifikasi
            watermarker.Save(output.sxc);
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
