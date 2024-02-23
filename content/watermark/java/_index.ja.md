---
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

head_title: "検索を追加するJavaAPIPDFWordExcel画像に透かしを削除"
head_description: "Javaドキュメント透かしAPI–ドキュメントから透かしを生成、検索、削除します：PDF、Word、Excel、プレゼンテーション、Visio、電子メール、画像ファイル形式."

title: "透かしを操作するためのJavaAPI"
description: "スマート検索と堅牢なセキュリティを備えた画像とテキストの透かし操作を実行するJavaアプリケーションを開発する."
button:
    enable: true

submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Watermark for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-watermark-java.png"
        product: "GroupDocs.Watermark"
        platform: "Java"

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

            - link: "https://purchase.groupdocs.com/pricing/watermark/java"
              text: "価格設定"

    right:
        link_download: "https://downloads.groupdocs.com/watermark"
        link_learn: "https://docs.groupdocs.com/watermark/java/"
        link_buy: "https://purchase.groupdocs.com"

overview:
    enable: true
    content: |
      GroupDocs.Watermark for Javaを使用すると、エンドユーザーが新しい透かしを適用したり、サポートされている形式のファイル内の既存の透かしを検索および削除したりできるビジネスアプリケーションを作成できます。プログラムで多くのファイル形式に電子透かしを割り当て、その強力なスマート検索機能を利用できます。 GroupDocs.Watermark for Javaは、機密情報や知的財産コンテンツを含むデジタルドキュメントの誤用を回避するために使用できるさまざまな組み込みのセキュリティ対策を提供します。
    tabs:
      enable: true     
      
      tab_one:
        description: |
          以下は、Java用のGroupDocs.Watermarkの概要です。

        rright:
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
          各形式でサポートされている[ドキュメント形式と透かしの種類]（https://docs.groupdocs.com/watermark/java/supported-document-formats/）を以下に示します。

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
          GroupDocs.Watermark for Javaは、次のオペレーティングシステム、フレームワーク、パッケージマネージャーをサポートしています。
        
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "オペレーティングシステム"
              content: |
                *MicrosoftWindowsデスクトップ
                * Microsoft Windows Server
                * Linux
                * マックOS

            - icon: "fas fa-code"
              title: "サポートされているフレームワーク"
              content: |
                * Java 7（1.7）以降

        right:
          enable: true
          table:
            - icon: "fas fa-cogs"
              title: "開発環境"
              content: |
                * NetBeans
                * IntelliJ IDEA
                *Eclipse
            - icon: "fas fa-tools"
              title: "ビルド自動化ツール"
              content: |
                * Maven

features:
    enable: true
    title: "GroupDocs.Watermark for Java Features"

    feature:
      - icon: "fas fa-copy"
        content: "フォルダからさまざまな形式のすべてのドキュメントをプルし、透かしを適用または削除します"

      - icon: "fas fa-eye"
        content: "特定のセクションまたは完全なドキュメントから透かしを使用または削除する"

      - icon: "fas fa-bolt"
        content: "特定のセクション、ページ、スライド、またはドキュメント内のすべての画像に透かしを適用する"
      
      - icon: "fas fa-file-powerpoint"
        content: "マルチフレーム画像の選択したフレームに透かしを付ける"

      - icon: "fas fa-code"
        content: "隠し透かしをPDFに適用して、ドキュメントの印刷時に表示する"

      - icon: "fas fa-cloud"
        content: "Excelドキュメントの添付ファイルとスライドのすべての画像形状に透かしを使用する"

      - icon: "fas fa-remove-format"
        content: "透かしを配置するか、スライドまたはExcelシートの背景画像から透かしを削除します"

      - icon: "fas fa-comment-slash"
        content: "電子メールまたはPDFファイルの添付ファイルでサポートされているファイルに透かしを設定する"

      - icon: "fas fa-location-arrow"
        content: "PDFファイルのXObject、アーティファクト、および注釈として透かしを追加または削除します"

      - icon: "fas fa-border-all"
        content: "特定のフォーマットで透かし一致テキストを削除する"

      - icon: "fas fa-wrench"
        content: "特定の画像に似た画像透かしを見つける"

      - icon: "fas fa-columns"
        content: "文字の間に判読できない文字がある場合でも、テキストの透かしを識別します"

      - icon: "fas fa-file-word"
        content: "特定のパラメータに基づいて、または複数の基準を割り当てて透かしを探します"

      - icon: "fas fa-envelope"
        content: "フォントの書式設定を指定して、一致するテキストの透かしを見つけます"

      - icon: "fas fa-print"
        content: "透かしの絶対サイズと位置のページ、スライド、セルの寸法を取得"

      - icon: "fas fa-file-archive"
        content: "サポートされているドキュメント形式のヘッダーとフッター内の画像に透かしを適用する"

      - icon: "fas fa-lock"
        content: "Word文書の画像形状に透かしを追加し、透かしの編集を制限する"

      - icon: "fas fa-file-code"
        content: "判読不能な文字を使用したプレゼンテーションの安全なテキスト透かし"
      
      - icon: "fas fa-fill-drip"
        content: "単一ページまたはドキュメント全体をラスター化することにより、PDFドキュメントの透かしを保護します"

      - icon: "fas fa-file-excel"
        content: "現在のテキスト透かしを置き換えるときにテキストの書式を変更する"

      - icon: "fas fa-heading"
        content: "PDFファイルのブリードボックス、アートボックス、クロップボックス、またはトリムボックスに透かしを配置します"

    more_feature:
      - title: "透かしを使用する"
        content: |
          GroupDocs.Watermark for Javaを使用すると、さまざまな種類の透かしを操作できます。任意のタイプの透かしを追加するのは、ほんの数行のコードの問題です。以下の共有例では、Javaを使用してWord文書に画像透かしを追加する方法を示します。
          
          ```java
          Document doc = Document.load(Common.mapSourceFilePath("D://test.docx"));
          Font font = new Font("Times New Roman", 12);
          TextWatermark watermark = new TextWatermark("Test watermark", font);

          //サイズタイプを設定します
          watermark.setSizingType(SizingType.ScaleToParentDimensions);

          //透かしスケールを設定します
          watermark.setScaleFactor(0.5);

          doc.addWatermark(watermark);
          doc.save(Common.mapOutputFilePath("D://test.docx"));
          doc.close();
          ```
      - title: "外出先でさまざまな形式のファイルに透かしを追加する"
        content: "GroupDocs.Watermark for Java APIを使用すると、バッチモードで特定のフォルダーに存在するすべてのドキュメントの透かしを追加または削除できます。ドキュメントの形式が異なる場合でも、GroupDocs.WatermarkforJavaはすべてのファイルに透かしを正確に適用します。."

      - title: "透かしに絶対確実なセキュリティを割り当てる"
        content: "最小限のコードで、透かしに絶対確実なセキュリティを割り当てることができ、サードパーティのツールが割り当てられた透かしをPDFファイルから変更または削除することを非常に困難にすることができます。これは、GroupDocs.Watermark for Javaを使用すると、PDFファイルのすべてのページをラスター化された画像に変換できるためです。このアプローチにより、デジタル透かしを安全に保ちながら、元の品質に近づけることができます。"

support:
    enable: true

solutions:
    enable: true
    title: "GroupDocs.Watermarkは、他の一般的な開発環境向けのドキュメント表示APIを提供します"

    solution:
        - img_alt: "GroupDocs.Watermark for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-watermark-net.png"
          product: "GroupDocs.Watermark"
          platform: ".NET"
          link: "/watermark/net/"

back_to_top:
  enable: true
---
