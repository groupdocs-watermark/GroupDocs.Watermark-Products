---
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

head_title: ".検索を追加するNETAPIWordExcelPDF画像に透かしを削除"
head_description: "ドキュメントから画像およびテキストベースの透かしを追加、検索、および削除するC＃.NET API：PDF、Word、Excel、プレゼンテーション、Visio、電子メール、および画像ファイル形式."

title: ".透かし操作用のNETAPI"
description: "スマート検索と強力なセキュリティ機能を備えたテキストおよび画像ベースの透かしを操作するための.NETアプリケーションを構築する."
button:
    enable: true

submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Watermark for .NET"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-watermark-net.png"
        product: "GroupDocs.Watermark"
        platform: ".NET"

    middle:
        button:
            - link: "#overview"
              text: "概要"

            - link: "#features"
              text: "特徴"

            - link: "#support"
              text: "サポート"

            - link: "https://products.groupdocs.app/watermark"
              text: "ライブデモ"

            - link: "https://purchase.groupdocs.com/pricing/watermark/net"
              text: "価格設定"

    right:
        link_download: "https://downloads.groupdocs.com/watermark"
        link_learn: "https://docs.groupdocs.com/watermark/net/"
        link_buy: "https://purchase.groupdocs.com"

overview:
    enable: true
    content: |
      GroupDocs.Watermark for .NETを使用すると、C＃、ASP.NET、およびその他の.NET関連テクノロジですぐに使用できるビジネスアプリケーションを構築できます。これにより、エンドユーザーは、サポートされているファイル形式で新しい透かしを追加したり、既存の透かしを検索および削除したりできます。 。 GroupDocs.Watermark for .NETを使用すると、このAPIが提供するさまざまな組み込みのセキュリティ対策を採用することで、プログラムで電子透かしを多数のファイル形式に適用し、知的財産の不正使用を阻止し、機密性の高いドキュメントに安全にラベルを付けることができます。
    tabs:
      enable: true
      
      tab_one:
        description: |
          以下は、GroupDocs.Watermarkfor.NETの概要です。
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "概要"
          content: |
            *透かしの追加と削除
            *透かしの検索と置換
            *フォーマットによる検索
            *画像比較による検索
            *ヘッダーとフッターを操作する
            *背景画像を操作する
            *添付ファイルを操作する
            *ページをラスタライズ
            *編集制限を適用する
      
      tab_two:
        description: |
          各形式でサポートされている[ドキュメント形式と透かしの種類]（https://docs.groupdocs.com/watermark/net/supported-document-formats/）を以下に示します。

        left:
          enable: true
          table:
            - title: "マイクロソフトオフィス"
              content: |
                * **ワード：** DOC、DOCX、DOCM、DOT、DOTX、DOTM、RTF、TXT
                * ** Excel：** XLS、XLSX、XLSM、XLSB、XLTM、XLT、XLTM、XLTX、XLAM、SXC、SpreadsheetML
                * ** PowerPoint：** PPT、PPTX、PPS、PPSX、PPSM、POT、POTM、POTX、PPTM
                * ** Visio：** VSD、VDX、VSS、VSSX、VSX、VST、VSTX、VTX、VSDX、VDW、VSTM、VSSM、VSDM

            - title: "透かしの追加"
              content: |
                * ** PDF **：XObject、Artifact、Annotation
                * **単語**：形
                * ** Excel **：形状、ヘッダー、フッター
                * ** PowerPoint **：形状
                * ** Visio **：形状
                * **ラスター画像**：テキスト、画像
                * **複数ページのTiff**：テキスト、画像
                * **アニメーションGIF**：テキスト、画像

        right:
          enable: true
          table:
            - title: "PDFおよび画像ドキュメント"
              content: |
                * **ポータブルドキュメントフォーマット**：PDF
                * **オープンドキュメント**：ODT
                * **メール**：EML、MSG、EMLX、OFT
                * **画像**：PNG、BMP、GIF、JPG、JPEG、JP2、TIF、TIFF、WebP

            - title: "透かしの削除"
              content: |
                * ** PDF **：XObject、アーティファクト、注釈、通常のテキスト
                * **単語**：形状、通常のテキスト
                * ** Excel **：セル内の形状、ヘッダーとフッター、背景画像、テキスト、数式
                * ** PowerPoint **：形状
                * ** Visio **：形状、図のコメント
                * **メール**：添付および埋め込み画像、件名と本文のテキストフラグメント

      tab_three:
        description: |
          GroupDocs.Watermark for .NETは、次のオペレーティングシステム、フレームワーク、およびパッケージマネージャーをサポートしています。
        
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "オペレーティングシステム"
              content: |
                *Windowsデスクトップ
                * WindowsServer
                * Windows Azure
                * Linux

            - icon: "fas fa-code"
              title: "サポートされているフレームワーク"
              content: |
                * .NETFramework2.0以降
                * MonoFramework1.2以降
                * .NET Standard 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            - icon: "fas fa-box"
              title: "パッケージマネージャー"
              content: |
                * NuGet

            - icon: "fas fa-tools"
              title: "開発環境"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

features:
    enable: true
    title: "GroupDocs.Watermarkfor.NET機能"

    feature:
      - icon: "fas fa-copy"
        content: "さまざまなファイル形式の特定のセクションまたはドキュメント全体から透かしを追加または削除する"

      - icon: "fas fa-eye"
        content: "特定のセクション、ページ、スライド、またはドキュメント内のすべての画像に透かしを添付する"

      - icon: "fas fa-bolt"
        content: "マルチフレーム画像の特定のフレームにのみ透かしを割り当てる"
      
      - icon: "fas fa-file-powerpoint"
        content: "ドキュメントの印刷時にのみ表示される隠し透かしをPDFに割り当てます"

      - icon: "fas fa-code"
        content: "Excelドキュメントのすべての添付ファイルとスライドのすべての画像形状に透かしを設定します"

      - icon: "fas fa-cloud"
        content: "透かしを配置するか、スプレッドシートまたはスライドの背景画像から透かしを削除します"

      - icon: "fas fa-remove-format"
        content: "電子メールまたはPDFドキュメントのすべての添付ファイルでサポートされているファイルに透かしを使用する"

      - icon: "fas fa-comment-slash"
        content: "PDFドキュメントのXObjects、Artifacts、Annotationsとして透かしを適用または削除する"

      - icon: "fas fa-location-arrow"
        content: "特定のフォーマットでテキストを含む透かしを削除します"

      - icon: "fas fa-border-all"
        content: "特定の画像に似た画像透かしを探す"

      - icon: "fas fa-wrench"
        content: "文字の間に判読できない文字がある場合でも、テキストの透かしを特定する"

      - icon: "fas fa-columns"
        content: "特定のパラメータに基づいて、または複数の基準を組み合わせて透かしを検索する"

      - icon: "fas fa-file-word"
        content: "一致するテキスト透かしを探すためのフォントフォーマットを指定する"

      - icon: "fas fa-envelope"
        content: "サポートされている形式のページ設定とその他の情報をプログラムで抽出します"

      - icon: "fas fa-print"
        content: "サポートされているドキュメント形式のヘッダーとフッター内の画像に透かしを追加する"

      - icon: "fas fa-file-archive"
        content: "Word文書の画像形状に透かしを追加し、透かしをロックして編集を制限する"

      - icon: "fas fa-lock"
        content: "プレゼンテーションで判読できない文字を使用してテキスト透かしを保護する"

      - icon: "fas fa-file-code"
        content: "追加された透かしを保護するために特定のページまたはPDFドキュメント全体をラスタライズする"
      
      - icon: "fas fa-fill-drip"
        content: "既存のテキスト透かしを置き換えながらテキストの書式を変更する"

      - icon: "fas fa-file-excel"
        content: "PDFドキュメントのブリードボックス、アートボックス、クロップボックス、またはトリムボックスに透かしを配置します"

      - icon: "fas fa-heading"
        content: "MicrosoftVisioドキュメントで図形のプロパティを編集する"

    more_feature:
      - title: "透かしの追加"
        content: |
          GroupDocs.Watermark for .NETは、複数のタイプの透かしをサポートしています。任意のタイプの透かしを追加するのは、数行のコードの問題です。次の例は、C＃を使用してWord文書に画像透かしを適用する方法を示しています。

          ```cs
          //ドキュメントをロードします
          using (FileStream stream = File.Open("document.docx", FileMode.Open, FileAccess.ReadWrite))
          {
            using (Watermarker watermarker = new(Watermarker(stream))
            {
                    //コンストラクタのパラメータとして画像へのパスを使用します
                    using (ImageWatermark watermark = new ImageWatermark("logo.png"))
                      {
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermarker.Add(watermark);
                }
                //結果のドキュメントを保存します
                watermarker.Save("document_watermarked.docx");
                }
          }
          ```
      - title: "外出先でさまざまな形式のファイルに透かしを適用する"
        content: "GroupDocs.Watermark APIを使用すると、特定のフォルダー内のすべてのファイルの透かしを一度に適用または削除できます。ファイルの形式を変えることもできますが、透かしはすべてのファイルに正確に適用されます。"

      - title: "透かしのための絶対確実なセキュリティ"
        content: "1行のコードだけで、どのツールでもPDFファイルから透かしを削除することを非常に困難にすることができます。これは、元の品質を維持したまま、PDFドキュメントのすべてのページをラスターイメージに変換することで実現されます。."

support:
    enable: true

solutions:
    enable: true
    title: "GroupDocs.Watermarkは、他の一般的な開発環境向けのドキュメント表示APIを提供します"

    solution:
        - img_alt: "GroupDocs.Watermark for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-watermark-java.png"
          product: "GroupDocs.Watermark"
          platform: "Java"
          link: "/watermark/java/"

back_to_top:
  enable: true
---
