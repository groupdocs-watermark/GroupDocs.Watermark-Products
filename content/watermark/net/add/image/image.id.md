---
layout: "autogen"
draft: false
path: "watermark/net/add/image/image/"
otherformats: PDF WORD EXCEL VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "Tambahkan IMAGE Watermark ke IMAGE di C#, ASP.NET, VB.NET"
head_description: ".Pustaka .NET untuk menambahkan tanda air IMAGE ke file IMAGE di aplikasi C#, ASP.NET, VB.NET & .NET Core menggunakan API GroupDocs.Watermark untuk .NET."

title: "Tambahkan IMAGE Watermark ke IMAGE di C# .NET"
description: "Menambahkan tanda air IMAGE ke file IMAGE di aplikasi C#, ASP.NET, VB.NET & .NET Core. Tambahkan tanda air BMP, PNG, GIF & JPEG IMAGE ke dokumen. Kelola juga ukuran tanda air, perataan, sudut rotasi, dan posisi tanda air pada halaman dokumen, sesuai kebutuhan Anda."

submenu:
    enable: true

about:
    enable: true
    title: "GroupDocs.Watermark untuk .NET API"
    content: |
        GroupDocs.Watermark untuk .NET adalah solusi manajemen tanda air lengkap untuk aplikasi .NET. Pengembang dapat dengan cepat melakukan operasi manipulasi tanda air seperti; tambahkan, edit, cari, dan hapus berbagai jenis tanda air dari dalam dokumen semua format file populer. Mendukung bekerja dengan teks dan IMAGE watermark dalam berbagai dokumen termasuk PDF, Microsoft Word, Excel, PowerPoint, Visio, Email dan format IMAGE.
        
        GroupDocs.Watermark API didukung dengan baik di semua sistem operasi dan platform utama termasuk .NET Framework, .NET Standard, .NET Core, Mono, dan Xamarin.

steps:
    enable: true
    title_left: "Tambahkan IMAGE Watermark ke IMAGE File di .NET"
    content_left: |
        [GroupDocs.Watermark](watermark/net/) memudahkan pengembang .NET untuk menambahkan tanda air IMAGE (BMP, PNG, GIF, atau JPEG) dalam aplikasi mereka dengan menerapkan beberapa langkah mudah .

        * Instansiasi **Watermarker** dengan memasukkan dokumen IMAGE.
        * Gunakan jalur tanda air IMAGE sebagai parameter konstruktor kelas **ImageWatermark**.
        * Atur properti tanda air (ukuran, perataan, warna, dll).
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
        // Tambahkan tanda air IMAGE ke IMAGE di aplikasi C#, ASP.NET, VB.NET & .NET Core
        // Instansiasi Watermarker dengan memasukkan dokumen IMAGE
        using (Watermarker watermarker = new Watermarker(input.image))
          {
            // Gunakan jalur tanda air IMAGE sebagai parameter konstruktor kelas ImageWatermark
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                // Setel properti tanda air (lebar, tinggi, perataan)
                watermark.Width = 140;
                watermark.Height = 140;
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;

                //Tambahkan tanda air ke penanda air dan hasilkan dokumen keluaran
                watermarker.Add(watermark);
                watermarker.Save(output.image);
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
