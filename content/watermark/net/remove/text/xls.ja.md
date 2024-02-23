---
layout: "autogen"
draft: false
path: "watermark/net/remove/text/xls/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "C＃、ASP.NET、VB.NETのXLSから透かしを削除します"
head_description: ".GroupDocs.Watermark API for .NETを使用したC＃、ASP.NET、VB.NET、および.NET Coreアプリケーション内のスマート検索を使用して、XLSドキュメントから透かしを検索して削除するNETライブラリ."

title: "C＃.NETのXLSから透かしを削除する"
description: "スマート検索を使用して、C＃、ASP.NET、VB.NET、および.NETCoreアプリケーション内からテキスト形式のXLSドキュメントから透かしを見つけて削除します。特定のフォント名、色、サイズ、およびその他の一致するプロパティに基づいて透かしを検索および削除するための検索基準を定義します."

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
    title_left: ".NETのXLSファイルから透かしを削除する"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実装することで、アプリケーションからテキスト形式の透かしを簡単に検索して削除できます。

        * 力XLSドキュメントを使用して* Watermarker* をインスタンス化します。
        * *  TextFormattingSearchCriteria * を初期化して、テキストの透かしを検索します。
        * かしを見つけて削除するには、定義された検索条件を初期化します。
        * 更したドキュメントを保存します。
        
    title_right: "システム要求"
    content_right: |
        以下のコード例を実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * ペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 発環境: Visual Studio、Xamarin、MonoDevelop
        * レームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        * [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)から最新バージョンのGroupDocs.Watermarkfor.NETをダウンロードします。
        
    code: |
        ```cs
        // C＃、ASP.NET、VB.NET、および.NET CoreアプリケーションのXLSドキュメントから、テキスト形式の透かしを検索して削除します
        //入力XLSドキュメントを使用してウォーターマーカーをインスタンス化します
        using (Watermarker watermarker = new Watermarker(input.xls))
          {
            // TextFormattingSearchCriteriaを初期化して、検索する透かしを定義します
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

            //変更したドキュメントを保存します
            watermarker.Save(output.xls);
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
