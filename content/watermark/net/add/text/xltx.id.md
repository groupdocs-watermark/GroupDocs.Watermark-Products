---
layout: "autogen"
draft: false
path: "watermark/net/add/text/xltx/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "Tambahkan Tanda Air Teks ke XLTX di C#, ASP.NET, VB.NET"
head_description: ".Pustaka .NET untuk menambahkan tanda air teks ke file XLTX di aplikasi C#, ASP.NET, VB.NET & .NET Core menggunakan API GroupDocs.Watermark untuk .NET."

title: "Tambahkan Tanda Air Teks ke XLTX di C# .NET"
description: "Menambahkan watermark teks ke file XLTX di aplikasi C#, ASP.NET, VB.NET & .NET Core. Kelola ukuran tanda air, jenis font, sudut rotasi, dan posisi tanda air pada halaman dokumen, sesuai kebutuhan Anda."

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
    title_left: "Tambahkan Tanda Air Teks ke File XLTX di .NET"
    content_left: |
        [GroupDocs.Watermark](/watermark/net/) memudahkan pengembang .NET untuk menambahkan tanda air teks dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Instansiasi **Watermarker** dengan memasukkan dokumen XLTX.
        * Inisialisasi **Font** yang akan digunakan untuk tanda air.
        * Buat objek **TextWatermark**.
        * Atur properti tanda air (perataan, warna, dll).
        * Tambahkan tanda air ke penanda air dan hasilkan dokumen keluaran.
        
    title_right: "Persyaratan sistem"
    content_right: |
        Sebelum menjalankan contoh kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: Visual Studio, Xamarin, MonoDevelop
        * Kerangka: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Watermark untuk .NET dari [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)
        
    code: |
        ```cs
        // Tambahkan tanda air teks ke XLTX di aplikasi C#, ASP.NET, VB.NET & .NET Core
        // Instansiasi Watermarker dengan memasukkan dokumen XLTX
        using (Watermarker watermarker = new Watermarker(input.xltx))
          {
            // Inisialisasi Font yang akan digunakan untuk watermark
            Font font = new Font("Arial", 19, FontStyle.Bold | FontStyle.Italic);
            
            // Buat objek TextWatermark
            TextWatermark watermark = new TextWatermark("my watermark", font);

            // Setel properti tanda air
            watermark.ForegroundColor = Color.Red;
            watermark.BackgroundColor = Color.Blue;
            watermark.TextAlignment = TextAlignment.Right;
            watermark.Opacity = 0.5;

            // Tambahkan tanda air dan simpan gambar yang diberi tanda air
            watermarker.Add(watermark);
            watermarker.Save(output.xltx);
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
