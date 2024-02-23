---
layout: "autogen"
draft: false
path: "watermark/java/add/text/vst/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLSB XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS

head_title: "JavaのVSTにテキスト透かしを追加する"
head_description: "GroupDocs.Watermark APIforJavaを使用してJavaおよびJ2SEアプリケーションのVSTファイルにテキスト透かしを追加するJavaライブラリ"

title: "JavaのVSTにテキスト透かしを追加する"
description: "JavaおよびJ2SEアプリケーションのVSTファイルにテキスト透かしを追加します。必要に応じて、透かしのサイズ、フォントタイプ、回転角度、およびドキュメントページ上の透かしの位置を管理します。"

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
    title_left: "JavaのVSTファイルにテキスト透かしを追加"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/)を使用すると、Java開発者は、いくつかの簡単な手順を実装することで、アプリケーションにテキスト透かしを簡単に追加できます。

        * 力VSTドキュメントで* Watermarker* をインスタンス化します。
        * かしテキスト、フォントサイズ、スタイルを使用して* TextWatermarker* を初期化します。
        * かしのプロパティ（配置、色など）を設定します。
        * かし入れに透かしを追加し、出力ドキュメントを生成します。
        
    title_right: "システム要求"
    content_right: |
        以下のコード例を実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * ペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 発環境: NetBeans、IntelliJ IDEA、Eclipse
        * レームワーク: Java 7（1.7）以降
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-watermark)から最新バージョンのGroupDocs.WatermarkforJavaをダウンロードします。
        
    code: |
        ```cs
        //JavaのVSTにテキスト透かしを追加します
        //入力VSTドキュメントでウォーターマーカーをインスタンス化します
        (Watermarker watermarker = new Watermarker(input.vst))
        
        //透かしテキスト、フォントサイズ、スタイルを使用してTextWatermarkerをインスタンス化します
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
            
        //透かしのプロパティを設定します
        watermark.setForegroundColor(Color.getRed());
        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
        watermark.setVerticalAlignment(VerticalAlignment.Center);

        //透かしを追加し、透かしを入れた画像を保存します
        watermarker.add(watermark);
        watermarker.save(output.vst);
        
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
