---
layout: "autogen"
draft: false
path: "watermark/net/edit/image/dotm/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "C＃、ASP.NET、VB.NETのDOTMで画像透かしを編集する"
head_description: ".GroupDocs.Watermark API for .NETを使用して、C＃、ASP.NET、VB.NET、および.NETCoreアプリケーションのDOTMファイルで見つかった画像透かしを編集するためのNETライブラリ."

title: "C＃.NETのDOTMで画像透かしを編集する"
description: "C＃、ASP.NET、VB.NET、および.NET Coreアプリケーション内のDOTMドキュメントで見つかった画像の透かしを検索し、変更します。ドキュメントにBMP、PNG、GIF、JPEG画像の透かしを追加します。また、必要に応じて、透かしのサイズ、フォントタイプ、回転角度、およびドキュメントページ上の透かしの位置を管理します。"

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
    title_left: ".NETのDOTMファイルで画像透かしを編集する"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/）を使用すると、.NET開発者は、いくつかの簡単な手順を実装することで、アプリケーションの画像（BMP、PNG、GIF、またはJPEG)透かしを簡単に編集できます。 。

        * 力DOTMドキュメントを使用して* Watermarker* をインスタンス化します。
        * 像の透かしを見つけるために* SearchCriteria* を初期化します。
        * つかった透かしを置き換えます。
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
        // C＃、ASP.NET、VB.NET、および.NETCoreアプリケーションのDOTMで画像透かしを検索して置換します
        //入力DOTMドキュメントを使用してウォーターマーカーをインスタンス化します
        using (Watermarker watermarker = new Watermarker(input.dotm))
          {
            //特定の画像に一致するようにSearchCriteriaを初期化します
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria(logo.png);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
                {
                    try
                        {
                            //見つかった画像を置き換えます
                            watermark.ImageData = imageData;
                        }
                    catch (Exception e)
                    {
                        //見つかったエンティティはテキスト編集をサポートしていない可能性があります
                        //渡された引数は不適切な値を持つ可能性があります
                        //このようなケースをここで処理します
                    }
                }
            
            //透かし入りのドキュメントを保存します
            watermarker.Save(output.dotm);
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
