---
layout: "autogen"
draft: false
path: "watermark/net/edit/text/vssx/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "C＃、ASP.NET、VB.NETのVSSXでテキスト透かしを編集する"
head_description: ".GroupDocs.Watermark API for .NETを使用して、C＃、ASP.NET、VB.NET、および.NETCoreアプリケーションのVSSXファイルで見つかったテキスト透かしを編集するためのNETライブラリ."

title: "C＃.NETのVSSXでテキスト透かしを編集する"
description: "C＃、ASP.NET、VB.NET、および.NET Coreアプリケーション内でフォーマットされた、VSSXドキュメントで見つかったテキスト透かしを検索して変更します。必要に応じて、透かしのサイズ、フォントタイプ、回転角度、およびドキュメントページ上の透かしの位置を管理します。"

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
    title_left: ".NETのVSSXファイルでテキスト透かしを編集する"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実装することで、アプリケーションのテキスト透かしを簡単に編集できます。

        * 力VSSXドキュメントを使用して* Watermarker* をインスタンス化します。
        * *  TextSearchCriteria * を初期化して、テキストの透かしを検索します。
        * つかった透かしのテキストを編集します
        * かしのプロパティ（フォントスタイル、色など）を編集および設定します。
        * しく透かしを入れたドキュメントを保存します。
        
    title_right: "システム要求"
    content_right: |
        以下のコード例を実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * ペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 発環境: Visual Studio、Xamarin、MonoDevelop
        * レームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        * [Nuget](https://www.nuget.org/packages/GroupDocs.Watermark)から最新バージョンのGroupDocs.Watermarkfor.NETをダウンロードします。
        
    code: |
        ```cs
        // C＃、ASP.NET、VB.NET、および.NET CoreアプリケーションのVSSXで、テキスト透かしを検索してフォーマットに置き換えます
        //入力VSSXドキュメントを使用してウォーターマーカーをインスタンス化します
        using (Watermarker watermarker = new Watermarker(input.vssx))
          {
            // TextSearchCriteriaを初期化して、テキストの透かしを検索します
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
                {
                    try
                        {
                            //テキストを編集し、透かしのプロパティを設定します
                            watermark.FormattedTextFragments.Clear();
                            watermark.FormattedTextFragments.Add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
                        }
                    catch (Exception e)
                    {
                        //見つかったエンティティはテキスト編集をサポートしていない可能性があります
                        //渡された引数は不適切な値を持つ可能性があります
                        //このようなケースをここで処理します
                    }
                }
            
            //透かし入りのドキュメントを保存します
            watermarker.Save(output.vssx);
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
