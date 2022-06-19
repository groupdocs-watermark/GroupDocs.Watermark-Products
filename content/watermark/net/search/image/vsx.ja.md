---
layout: "autogen"
draft: false
path: "watermark/net/search/image/vsx/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "C＃ASP.NETVB.NETでVSXから画像透かしを検索"
head_description: ".GroupDocs.Watermark API for .NETを使用してC＃、ASP.NET、VB.NET、および.NETCoreアプリケーション内のスマート検索機能を使用してVSXドキュメントから画像透かしを検索するNETライブラリ."

title: "C＃でVSXから画像透かしを検索"
description: "スマート検索を使用して、C＃、ASP.NET、VB.NET、および.NETCoreアプリケーション内からVSXファイルから可能なすべての画像透かしを検索します。検索基準を定義し、ソースドキュメントのページ全体または特定のページから一致するすべての画像透かしを検索します."

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
    title_left: ".NETでVSXから透かしを検索"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、ドキュメント内から画像の透かしをインテリジェントに検索できます。

        * 力VSXドキュメントを使用して* Watermarker* をインスタンス化します。
        * ォーターマーク検索を実行するには、* ImageSearchCriteria* を初期化します。
        * 像間の最大許容差を設定します。
        * 致する可能性のある透かしを表示します。
        
    title_right: "システム要求"
    content_right: |
        以下のコード例を実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * ペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 発環境: Visual Studio、Xamarin、MonoDevelop
        * レームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        * [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)から最新バージョンのGroupDocs.Watermarkfor.NETをダウンロードします。
        
    code: |
        ```cs
        // C＃、ASP.NET、VB.NET、および.NET Coreを使用して、VSXドキュメントで可能なIMAGE透かしを検索します。
        //入力VSXドキュメントを使用してウォーターマーカーをインスタンス化します
        using (Watermarker watermarker = new Watermarker(input.vsx))
          {
            // ImageSearchCriteriaを初期化して、透かし検索を開始します
            ImageSearchCriteria imageSearchCriteria = new ImageDctHashSearchCriteria(watermark.jpeg);

            //サンプル画像と可能な透かしの間の最大許容差を設定します
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
