---
layout: "autogen"
draft: false
path: "watermark/net/edit/image/vdx/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "Edit Tanda Air Gambar dalam VDX di C#, ASP.NET, VB.NET"
head_description: ".Pustaka .NET untuk mengedit tanda air gambar yang ditemukan dalam file VDX di aplikasi C#, ASP.NET, VB.NET & .NET Core menggunakan API GroupDocs.Watermark untuk .NET."

title: "Edit Tanda Air Gambar dalam VDX di C# .NET"
description: "Temukan & ubah tanda air gambar yang ditemukan dalam dokumen VDX dalam aplikasi C#, ASP.NET, VB.NET & .NET Core. Tambahkan tanda air gambar BMP, PNG, GIF & JPEG ke dokumen. Juga kelola ukuran tanda air, jenis font, sudut rotasi, dan posisi tanda air pada halaman dokumen, sesuai kebutuhan Anda."

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
    title_left: "Edit Tanda Air Gambar dalam File VDX di .NET"
    content_left: |
        [GroupDocs.Watermark](/watermark/net/) memudahkan pengembang .NET untuk mengedit tanda air gambar (BMP, PNG, GIF, atau JPEG) dalam aplikasi mereka dengan menerapkan beberapa langkah mudah .

        * Instansiasi **Watermarker** dengan memasukkan dokumen VDX.
        * Inisialisasi **SearchCriteria** untuk menemukan watermark gambar.
        * Ganti tanda air yang ditemukan.
        * Simpan dokumen yang baru diberi watermark.
        
    title_right: "Persyaratan sistem"
    content_right: |
        Sebelum menjalankan contoh kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: Visual Studio, Xamarin, MonoDevelop
        * Kerangka: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Watermark untuk .NET dari [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)
        
    code: |
        ```cs
        // Temukan & ganti tanda air gambar dalam VDX di aplikasi C#, ASP.NET, VB.NET & .NET Core
        // Instansiasi Watermarker dengan memasukkan dokumen VDX
        using (Watermarker watermarker = new Watermarker(input.vdx))
          {
            // Inisialisasi Kriteria Pencarian untuk mencocokkan gambar tertentu
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria(logo.png);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
                {
                    try
                        {
                            // Ganti gambar yang ditemukan
                            watermark.ImageData = imageData;
                        }
                    catch (Exception e)
                    {
                        // Entitas yang ditemukan mungkin tidak mendukung pengeditan teks
                        // Argumen yang diteruskan dapat memiliki nilai yang tidak sesuai
                        // Proses kasus seperti itu di sini
                    }
                }
            
            // Simpan dokumen yang diberi watermark
            watermarker.Save(output.vdx);
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
