---
layout: "autogen"
draft: false
path: "watermark/net/search/visio/"
otherformats: PDF WORD EXCEL IMAGE DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "Cari Tanda Air dari VISIO di C#, ASP.NET, VB.NET"
head_description: ".Pustaka .NET untuk mencari tanda air dari dokumen VISIO menggunakan fitur pencarian pintar dalam aplikasi C#, ASP.NET, VB.NET & .NET Core menggunakan API GroupDocs.Watermark untuk .NET."

title: "Cari Tanda Air dari VISIO di C# .NET"
description: "Gunakan pencarian cerdas untuk menemukan semua kemungkinan tanda air dari file VISIO dari dalam aplikasi C#, ASP.NET, VB.NET & .NET Core. Tentukan kriteria pencarian berdasarkan teks, ekspresi reguler (RegEx), gambar, hyperlink, karakter, dan objek pencarian yang berbeda untuk menemukan tanda air dari seluruh atau halaman tertentu dari dokumen sumber."

submenu:
    enable: true

about:
    enable: true
    title: "GroupDocs.Watermark untuk .NET API"
    content: |
        GroupDocs.Watermark untuk .NET adalah solusi manajemen tanda air lengkap untuk aplikasi .NET. Pengembang dapat dengan cepat melakukan operasi manipulasi tanda air seperti; tambahkan, edit, cari, dan hapus berbagai jenis tanda air dari dalam dokumen semua format file populer. Mendukung bekerja dengan teks dan tanda air gambar dalam berbagai dokumen termasuk PDF, Microsoft Word, Excel, PowerPoint, VISIO, Email dan format gambar.
        
        GroupDocs.Watermark API didukung dengan baik di semua sistem operasi dan platform utama termasuk .NET Framework, .NET Standard, .NET Core, Mono, dan Xamarin.

steps:
    enable: true
    title_left: "Cari Tanda Air dari VISIO di .NET"
    content_left: |
        [GroupDocs.Watermark](/watermark/net/) memudahkan pengembang .NET untuk mencari tanda air secara cerdas dari dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Instansiasi **Watermarker** dengan memasukkan dokumen VISIO.
        * Inisialisasi **PossibleWatermarkCollection** untuk melakukan pencarian tanda air.
        * Kriteria pencarian yang ditentukan untuk menemukan kemungkinan tanda air.
        
    title_right: "Persyaratan sistem"
    content_right: |
        Sebelum menjalankan contoh kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: Visual Studio, Xamarin, MonoDevelop
        * Kerangka: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Watermark untuk .NET dari [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)
        
    code: |
        ```cs
        // mencari kemungkinan tanda air dalam dokumen VISIO menggunakan C#, ASP.NET, VB.NET & .NET Core.
        // Instansiasi Watermarker dengan memasukkan dokumen VISIO
        using (Watermarker watermarker = new Watermarker(input.vdx))
          {
            // Inisialisasi KemungkinanWatermarkCollection untuk memulai pencarian tanda air
            PossibleWatermarkCollection possibleWatermarks = watermarker.Search();
            foreach (PossibleWatermark possibleWatermark in possibleWatermarks)
            {
                if (possibleWatermark.ImageData != null)
                {
                    Console.WriteLine(possibleWatermark.ImageData.Length);
                }

                // Kriteria pencarian yang ditentukan untuk menemukan kemungkinan tanda air
                Console.WriteLine(possibleWatermark.Text);
                Console.WriteLine(possibleWatermark.X);
                Console.WriteLine(possibleWatermark.Y);
                Console.WriteLine(possibleWatermark.RotateAngle);
                Console.WriteLine(possibleWatermark.Width);
                Console.WriteLine(possibleWatermark.Height);
            }
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
