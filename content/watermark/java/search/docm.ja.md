---
layout: "autogen"
draft: false
path: "watermark/java/search/docm/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "JavaでDOCMから透かしを検索する"
head_description: "GroupDocs.Watermark APIforJavaを使用してJavaアプリケーション内のスマート検索機能を使用してDOCMドキュメントから透かしを検索するJavaライブラリ."

title: "JavaでDOCMから透かしを検索する"
description: "スマート検索を使用して、JavaおよびJ2SEアプリケーション内のDOCMファイルから可能なすべての透かしを検索します。テキスト、正規表現（RegEx）、画像、ハイパーリンク、文字、およびさまざまな検索オブジェクトに基づいて検索条件を定義し、ソースドキュメントのページ全体または特定のページから透かしを検索します."

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
    title_left: "JavaでDOCMから透かしを検索する"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/)を使用すると、Java開発者は、いくつかの簡単な手順を実装することで、アプリケーション内から透かしをインテリジェントに検索できます。

        * 力DOCMドキュメントを使用して* Watermarker* をインスタンス化します。
        * ォーターマーク検索を実行するために* PossibleWatermarkCollection* を初期化します。
        * 能な透かしを見つけるための定義された検索基準。
        
    title_right: "システム要求"
    content_right: |
        以下のコード例を実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * ペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 発環境: NetBeans、IntelliJ IDEA、Eclipse
        * レームワーク: Java 7（1.7）以降
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)から最新バージョンのGroupDocs.WatermarkforJavaをダウンロードします。
        
    code: |
        ```cs
        //Javaを使用してDOCMドキュメントで可能な透かしを検索します。
        //入力DOCMドキュメントを使用してウォーターマーカーをインスタンス化します
        Watermarker watermarker = new Watermarker(input.docm))

        //PossibleWatermarkCollectionを初期化してウォーターマーク検索を開始します
        PossibleWatermarkCollection possibleWatermarks = watermarker.search();
        for (PossibleWatermark possibleWatermark : possibleWatermarks)
        {
            if (possibleWatermark.getImageData() != null)
            {
                System.out.println(possibleWatermark.getImageData().length);
            }

            //可能な透かしを見つけるための定義された検索条件
            System.out.println(possibleWatermark.getText());
            System.out.println(possibleWatermark.getX());
            System.out.println(possibleWatermark.getY());
            System.out.println(possibleWatermark.getRotateAngle());
            System.out.println(possibleWatermark.getWidth());
            System.out.println(possibleWatermark.getHeight());
        }

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
