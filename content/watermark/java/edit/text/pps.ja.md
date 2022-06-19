---
layout: "autogen"
draft: false
path: "watermark/java/edit/text/pps/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "JavaのPPSでテキスト透かしを編集する"
head_description: "GroupDocs.Watermark API for Javaを使用して、JavaアプリケーションのPPSファイルで見つかったテキスト透かしを編集するJavaライブラリ."

title: "JavaのPPSでテキスト透かしを編集する"
description: "JavaおよびJ2SEアプリケーション内でフォーマットを使用して、PPSドキュメントで見つかったテキスト透かしを検索および変更します。必要に応じて、透かしのサイズ、フォントタイプ、回転角度、およびドキュメントページ上の透かしの位置を管理します。"

submenu:
    enable: true

about:
    enable: true
    title: "GroupDocs.Watermark for Java API"
    content: |
        GroupDocs.Watermark for Javaは、Javaアプリケーション用の完全な透かし管理ソリューションです。開発者は、次のような透かし操作操作をすばやく実行できます。すべての一般的なファイル形式のドキュメント内から、さまざまな種類の透かしを追加、編集、検索、および削除します。 PDF、Microsoft Word、Excel、PowerPoint、Visio、Eメール、画像形式など、さまざまなドキュメントのテキストと画像の透かしの操作をサポートしています。
        
        GroupDocs.Watermark APIは、J2SE 7.0（1.7）、J2SE 8.0（1.8）、Java10を含むすべての主要なオペレーティングシステムとJavaバージョンで十分にサポートされています。

steps:
    enable: true
    title_left: "JavaのPPSファイルでテキスト透かしを編集する"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/)を使用すると、Java開発者は、いくつかの簡単な手順を実装することで、アプリケーションのテキスト透かしを簡単に編集できます。

        * 力PPSドキュメントを使用して* Watermarker* をインスタンス化します。
        * *  TextSearchCriteria * を初期化して、テキストの透かしを検索します。
        * つかった透かしのテキストを編集します。
        * かしのプロパティ（フォントスタイル、色など）を設定します。
        * しく透かしを入れたドキュメントを保存します。
        
    title_right: "システム要求"
    content_right: |
        以下のコード例を実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * ペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 発環境: NetBeans、IntelliJ IDEA、Eclipse
        * レームワーク: Java 7（1.7）以降
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)から最新バージョンのGroupDocs.WatermarkforJavaをダウンロードします。
        
    code: |
        ```cs
        //JavaアプリケーションのPPSでフォーマットされたテキスト透かしを検索して更新します
        //入力PPSドキュメントを使用してウォーターマーカーをインスタンス化します
        Watermarker watermarker = new Watermarker(input.pps))
        
        // TextSearchCriteriaを初期化して、テキストの透かしを検索します
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        for (PossibleWatermark watermark : watermarks)
        {
            try
            {
                //テキストを編集し、透かしのプロパティを設定します
                watermark.getFormattedTextFragments().clear();
                watermark.getFormattedTextFragments().add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
            }
            catch (Exception e)
            {
                //見つかったエンティティはテキスト編集をサポートしていない可能性があります
                //渡された引数は不適切な値を持つ可能性があります
                //このようなケースをここで処理します
            }
        }
            
        //透かし入りのドキュメントを保存します
        watermarker.save(output.pps);

        watermarker.close();
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
