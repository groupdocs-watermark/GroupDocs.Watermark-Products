---
layout: "autogen"
draft: false
path: "watermark/net/add/text/vstm/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VTX VDW VSS VST

head_title: "C＃、ASP.NET、VB.NETのVSTMにテキスト透かしを追加する"
head_description: ".GroupDocs.Watermark API for .NETを使用して、C＃、ASP.NET、VB.NET、および.NETCoreアプリケーションのVSTMファイルにテキスト透かしを追加するNETライブラリ."

title: "C＃.NETのVSTMにテキスト透かしを追加する"
description: "C＃、ASP.NET、VB.NET、および.NETCoreアプリケーションのVSTMファイルにテキスト透かしを追加します。必要に応じて、透かしのサイズ、フォントタイプ、回転角度、およびドキュメントページ上の透かしの位置を管理します。"

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
    title_left: ".NETのVSTMファイルにテキスト透かしを追加する"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーションにテキスト透かしを簡単に追加できます。

        * 力VSTMドキュメントを使用して* Watermarker* をインスタンス化します。
        * かしに使用する* フォント* を初期化します。
        * * TextWatermark* オブジェクトを作成します。
        * かしのプロパティ（配置、色など）を設定します。
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
        // C＃、ASP.NET、VB.NET、および.NETCoreアプリケーションのVSTMにテキスト透かしを追加します
        //入力VSTMドキュメントを使用してウォーターマーカーをインスタンス化します
        using (Watermarker watermarker = new Watermarker(input.vstm))
          {
            //透かしに使用するフォントを初期化します
            Font font = new Font("Arial", 19, FontStyle.Bold | FontStyle.Italic);
            
            //TextWatermarkオブジェクトを作成します
            TextWatermark watermark = new TextWatermark("my watermark", font);

            //透かしのプロパティを設定します
            watermark.ForegroundColor = Color.Red;
            watermark.BackgroundColor = Color.Blue;
            watermark.TextAlignment = TextAlignment.Right;
            watermark.Opacity = 0.5;

            //透かしを追加し、透かしを入れた画像を保存します
            watermarker.Add(watermark);
            watermarker.Save(output.vstm);
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
