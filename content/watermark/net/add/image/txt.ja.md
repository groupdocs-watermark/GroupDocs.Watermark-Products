---
layout: "autogen"
draft: false
path: "watermark/net/add/image/txt/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "C＃、ASP.NET、VB.NETのTXTに画像透かしを追加する"
head_description: ".GroupDocs.Watermark API for .NETを使用して、C＃、ASP.NET、VB.NET、および.NETCoreアプリケーションのTXTファイルに画像透かしを追加するNETライブラリ."

title: "C＃.NETのTXTに画像透かしを追加する"
description: "C＃、ASP.NET、VB.NET、および.NETCoreアプリケーションのTXTファイルに画像透かしを追加します。ドキュメントにBMP、PNG、GIF、JPEG画像の透かしを追加します。また、必要に応じて、透かしのサイズ、配置、回転角度、およびドキュメントページ上の透かしの位置を管理します。"

submenu:
    enable: true

about:
    enable: true
    title: "GroupDocs.Watermark for .NET API"
    content: |
        GroupDocs.Watermark for .NETは、.NETアプリケーション用の完全な透かし管理ソリューションです。開発者は、次のような透かし操作操作をすばやく実行できます。すべての一般的なファイル形式のドキュメント内から、さまざまな種類の透かしを追加、編集、検索、および削除します。 PDF、Microsoft Word、Excel、PowerPoint、Visio、Eメール、画像形式など、さまざまなドキュメントのテキストと画像の透かしの操作をサポートしています。
        
        GroupDocs.Watermark APIは、.NET Framework、.NET Standard、.NET Core、Mono、Xamarinを含むすべての主要なオペレーティングシステムとプラットフォームで十分にサポートされています。

steps:
    enable: true
    title_left: ".NETのTXTファイルに画像透かしを追加"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/）を使用すると、.NET開発者は、いくつかの簡単な手順を実装することで、アプリケーションに画像（BMP、PNG、GIF、またはJPEG)の透かしを簡単に追加できます。 。

        * 力TXTドキュメントを使用して* Watermarker* をインスタンス化します。
        * * ImageWatermark* クラスのコンストラクターパラメーターとして画像透かしパスを使用します。
        * かしのプロパティ（サイズ、配置、色など）を設定します。
        * かし入れに透かしを追加し、出力ドキュメントを生成します。
        
    title_right: "システム要求"
    content_right: |
        以下のコード例を実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * ペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 発環境: Visual Studio、Xamarin、MonoDevelop
        * レームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        * [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)から最新バージョンのGroupDocs.Watermarkfor.NETをダウンロードします。
        
    code: |
        ```cs
        // C＃、ASP.NET、VB.NET、および.NETCoreアプリケーションのTXTに画像透かしを追加します
        //入力TXTドキュメントを使用してウォーターマーカーをインスタンス化します
        using (Watermarker watermarker = new Watermarker(input.txt))
          {
            //ImageWatermarkクラスのコンストラクターパラメーターとして画像透かしパスを使用します
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                //透かしのプロパティ（幅、高さ、配置）を設定します
                watermark.Width = 140;
                watermark.Height = 140;
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;

                //透かしを透かし入れに追加し、出力ドキュメントを生成します
                watermarker.Add(watermark);
                watermarker.Save(output.txt);
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
