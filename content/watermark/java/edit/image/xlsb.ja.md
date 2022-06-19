---
layout: "autogen"
draft: false
path: "watermark/java/edit/image/xlsb/"
otherformats: PDF WORD EXCEL IMAGE VISIO DOC DOT DOCX DOCM DOTX DOTM RTF TXT XLSX XLSM XLTM XLT XLTX XLS XLAM SXC PPTX PPTM PPSX PPSM POTM POT POTX PPT PPS ODT BMP GIF JPEG JP2 PNG TIFF WEBP VSD VDX VSDX VSTX VSX VSSX VSDM VSSM VSTM VTX VDW VSS VST

head_title: "JavaのXLSBで画像透かしを編集する"
head_description: "Java用のGroupDocs.WatermarkAPIを使用して、JavaおよびJ2SEアプリケーションのXLSBファイルで見つかった画像透かしを編集するJavaライブラリ."

title: "JavaのXLSBで画像透かしを編集する"
description: "JavaおよびJ2SEアプリケーション内のXLSBドキュメントで見つかった画像透かしを検索して変更します。ドキュメントにBMP、PNG、GIF、JPEG画像の透かしを追加します。また、必要に応じて、透かしのサイズ、フォントタイプ、回転角度、およびドキュメントページ上の透かしの位置を管理します。"

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
    title_left: "JavaでXLSBファイルの画像透かしを編集する"
    content_left: |
        [GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/）を使用すると、Java開発者は、いくつかの簡単な手順を実行することで、アプリケーションの画像（BMP、PNG、GIF、またはJPEG)透かしを簡単に編集できます。

        * 力XLSBドキュメントを使用して* Watermarker* をインスタンス化します。
        * 像の透かしを見つけるために* SearchCriteria* を初期化します。
        * つかった透かしを置き換えます。
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
        //JavaアプリケーションのXLSBで画像透かしを検索して置換します
        //入力XLSBドキュメントを使用してウォーターマーカーをインスタンス化します
        Watermarker watermarker = new Watermarker(input.xlsb)
        
        //特定の画像に一致するようにSearchCriteriaを初期化します
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria(logo.png);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        for (PossibleWatermark watermark : watermarks)
            {
                try
                {
                    //見つかった画像を置き換えます
                    watermark.setImageData(imageData);
                }
                
                catch (Exception e)
                {
                    //見つかったエンティティはテキスト編集をサポートしていない可能性があります
                    //渡された引数は不適切な値を持つ可能性があります
                    //このようなケースをここで処理します
                }
            }
            
            //透かし入りのドキュメントを保存します
            watermarker.save(output.xlsb);

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
