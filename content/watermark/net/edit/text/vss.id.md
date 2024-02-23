---
layout: "autogen"
draft: false
path: "watermark/net/edit/text/vss/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VST

head_title: "Edit Tanda Air Teks dalam VSS di C#, ASP.NET, VB.NET"
head_description: ".Pustaka .NET untuk mengedit tanda air teks yang ditemukan dalam file VSS di aplikasi C#, ASP.NET, VB.NET & .NET Core menggunakan API GroupDocs.Watermark untuk .NET."

title: "Edit Tanda Air Teks dalam VSS di C# .NET"
description: "Temukan & ubah tanda air teks yang ditemukan dalam dokumen VSS dengan pemformatan dalam aplikasi C#, ASP.NET, VB.NET & .NET Core. Kelola ukuran tanda air, jenis font, sudut rotasi, dan posisi tanda air pada halaman dokumen, sesuai kebutuhan Anda."

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
    title_left: "Edit Tanda Air Teks dalam File VSS di .NET"
    content_left: |
        [GroupDocs.Watermark](/watermark/net/) memudahkan pengembang .NET untuk mengedit tanda air teks dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Instansiasi **Watermarker** dengan memasukkan dokumen VSS.
        * Inisialisasi **TextSearchCriteria** untuk menemukan tanda air teks.
        * Edit teks tanda air yang ditemukan
        * Edit dan atur properti tanda air (gaya font, warna, dll).
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
        // Temukan & ganti tanda air teks dengan memformat dalam VSS di aplikasi C#, ASP.NET, VB.NET & .NET Core
        // Instansiasi Watermarker dengan memasukkan dokumen VSS
        using (Watermarker watermarker = new Watermarker(input.vss))
          {
            // Inisialisasi TextSearchCriteria untuk menemukan watermark teks
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
                {
                    try
                        {
                            // Edit teks dan atur properti tanda air
                            watermark.FormattedTextFragments.Clear();
                            watermark.FormattedTextFragments.Add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
                        }
                    catch (Exception e)
                    {
                        // Entitas yang ditemukan mungkin tidak mendukung pengeditan teks
                        // Argumen yang diteruskan dapat memiliki nilai yang tidak sesuai
                        // Proses kasus seperti itu di sini
                    }
                }
            
            // Simpan dokumen yang diberi watermark
            watermarker.Save(output.vss);
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
