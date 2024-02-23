---
layout: "autogen"
draft: false
path: "watermark/java/remove/text/txt/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "JavaのTXTから透かしを削除する"
head_description: "GroupDocs.Watermark APIforJavaを使用したJavaアプリケーション内のスマート検索を使用してTXTドキュメントから透かしを検索して削除するJavaライブラリ."

title: "JavaのTXTから透かしを削除する"
description: "スマート検索を使用して、JavaおよびJ2SEアプリケーション内からテキスト形式のTXTドキュメントから透かしを見つけて削除します。特定のフォント名、色、サイズ、およびその他の一致するプロパティに基づいて透かしを検索および削除するための検索基準を定義します."

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
    title_left: "JavaのTXTファイルから透かしを削除する"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/)を使用すると、Java開発者は、いくつかの簡単な手順を実装することで、アプリケーションからテキスト形式の透かしを簡単に検索して削除できます。

        * 力TXTドキュメントを使用して* Watermarker* をインスタンス化します。
        * かしを見つけて削除するには、定義された検索条件を初期化します。
        * 更したドキュメントを保存します。
        
    title_right: "システム要求"
    content_right: |
        以下のコード例を実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * ペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 発環境: NetBeans、IntelliJ IDEA、Eclipse
        * レームワーク: Java 7（1.7）以降
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)から最新バージョンのGroupDocs.WatermarkforJavaをダウンロードします。
        
    code: |
        ```cs
        //JavaアプリケーションでTXTドキュメントから透かしを検索して削除します
        //入力TXTドキュメントを使用してウォーターマーカーをインスタンス化します
        Watermarker watermarker = new Watermarker(input.txt))

        PossibleWatermarkCollection possibleWatermarks = watermarker.search();

        //指定されたインデックスで可能な透かしをドキュメントから削除します
        possibleWatermarks.removeAt(0);

        //指定された可能性のある透かしをドキュメントから削除します
        possibleWatermarks.remove(possibleWatermarks.get_Item(0));

        //変更したドキュメントを保存します
        watermarker.save(output.txt);

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
