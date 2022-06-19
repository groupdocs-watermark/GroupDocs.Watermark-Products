---
layout: "autogen"
draft: false
path: "watermark/java/search/image/dot/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "JavaでDOTから画像透かしを検索"
head_description: "Java用のGroupDocs.WatermarkAPIを使用してJavaおよびJ2SEアプリケーション内のスマート検索機能を使用してDOTドキュメントから画像透かしを検索するJavaライブラリ."

title: "JavaでDOTから画像透かしを検索"
description: "スマート検索を使用して、JavaおよびJ2SEアプリケーション内のDOTファイルから可能なすべての画像透かしを検索します。ソースドキュメントのページ全体または特定のページから一致するすべての画像透かしを検索するための検索条件を定義します."

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
    title_left: "JavaでDOTから透かしを検索"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/)を使用すると、Java開発者は、いくつかの簡単な手順を実装することで、ドキュメント内から画像の透かしをインテリジェントに検索できます。

        * 力DOTドキュメントを使用して* Watermarker* をインスタンス化します。
        * ォーターマーク検索を実行するには、* ImageSearchCriteria* を初期化します。
        * 像間の最大許容差を設定します。
        * 致する可能性のある透かしを表示します。
        
    title_right: "システム要求"
    content_right: |
        以下のコード例を実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * ペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 発環境: NetBeans、IntelliJ IDEA、Eclipse
        * レームワーク: Java 7（1.7）以降
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)から最新バージョンのGroupDocs.WatermarkforJavaをダウンロードします。
        
    code: |
        ```cs
        //Javaを使用してDOTドキュメントで可能なIMAGE透かしを検索します。
        //入力DOTドキュメントを使用してウォーターマーカーをインスタンス化します
        Watermarker watermarker = new Watermarker(input.dot);
        
        // ImageSearchCriteriaを初期化して、透かし検索を開始します
        ImageSearchCriteria imageSearchCriteria = new ImageDctHashSearchCriteria(watermark.jpeg);

        //サンプル画像と可能な透かしの間の最大許容差を設定します
        imageSearchCriteria.setMaxDifference(0.9);
        PossibleWatermarkCollection possibleWatermarks = watermarker.search(imageSearchCriteria);
        System.out.println("Found " + possibleWatermarks.getCount() + " possible watermark(s).");

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
