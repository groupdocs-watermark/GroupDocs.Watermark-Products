---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:49
draft: false

lang: ja
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"
    # supported_platforms loop
    - title: "Python"
      tag: "python-net"

############################# Head ############################
head_title: "Node.js ウォーターマークライブラリ | ドキュメントウォーターマーク"
head_description: "Node.js ソリューションは、テキストと画像のウォーターマークでビジネス文書を保護します。PDF、Word、Excel、PowerPoint などの一般的な形式がサポートされています。"

############################# Header ############################
title: "Java ソリューションによる Node.js のウォーターマーキングテクノロジーへのアクセス"
description: "この Node.js ソリューションで知的財産を保護し、不正コピーを防止してください。これにより、ユーザーは PDF、Word、Excel、PowerPoint、画像など、さまざまな形式のビジネス文書にウォーターマークを簡単に追加できます。"
words:
  for: "にとって"

actions:
  main: "NPM を使用して無料でダウンロードする"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.watermark"
  alt: "ライセンス"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
  title: "始める準備はできましたか?"
  description: "GroupDocs.Watermark の機能を無料で試すか、ライセンスをリクエストしてください"

release:
  title: "バージョン {0} がリリースされました"
  notes: "新機能を見る"
  downloads: "ダウンロード"
  link: "https://releases.groupdocs.com/watermark/nodejs-java/"

code:
  title: "タイプスクリプトで PDF にウォーターマークを追加"
  more: "その他の例"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.watermark"
  content: |
    ```javascript {style=abap}

    // PDF パスを渡すウォーターマーカーをインスタンス化
    let loadOptions = new PdfLoadOptions();
    let watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // ウォーターマークオプションのカスタマイズ
    let textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // PDF ドキュメントにウォーターマークを適用
    watermarker.add(textWatermark);

    // 結果文書を保存
    watermarker.save("result.pdf");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark 一目でわかる"
  description: "ウォーターマーク用 Node.js タイプスクリプトライブラリ"
  features:
    # feature loop
    - title: "Node.js ファイルウォーターマーキング"
      content: "GroupDocs.Watermark for Node.js via Java でビジネス文書を保護してください。テキスト、画像、図、メールの添付ファイルをウォーターマークとしてさまざまなファイル形式に追加できます。"

    # feature loop
    - title: "必要に応じてウォーターマークをカスタマイズ"
      content: "GroupDocs.Watermark for Node.js via Java には、ウォーターマークの幅広いカスタマイズオプションが用意されています。テキストスタイル (太字、斜体、フォント) と画像プロパティ (回転など) を微調整することで、文書処理をカスタマイズできます。"

    # feature loop
    - title: "包括的なフォーマットサポート"
      content: "GroupDocs.Watermark for Node.js via Java は、Word、Excel、PowerPoint などの PDF、MS Office、JPEG、PNG、GIF、BMP、Visio 図などの画像、電子メールなどを含む幅広いファイル形式とシームレスに統合し、ビジネス目標を達成するための文書処理を強化します。"

    # feature loop
    - title: "強力なウォーターマーク検索と更新"
      content: "ウォーターマークの付いたドキュメント内の既存のウォーターマークを取得して更新します。テキスト、スタイル、画像コンテンツを変更したり、完全に削除したりできます。GroupDocs.Watermark for Node.js via Java は幅広いウォーターマーク処理を提供します。"

############################# Platforms ############################
platforms:
  enable: true
  title: "プラットフォーム独立性"
  description: "GroupDocs.Watermark for Node.js via Java は、さまざまなオペレーティングシステムやパッケージマネージャーと簡単に統合できます。"
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "対応ファイル形式"
  description: |
    GroupDocs.Watermark for Node.js via Java を使用すると、さまざまなファイル形式を処理できます。[全リストを見る](https://docs.groupdocs.com/watermark/java/supported-document-formats/)。
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office および OpenDocument フォーマット
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### イメージとグラフィックス
        * **人気の画像フォーマット:** BMP, JPG, JPEG, PNG
        * **複数ページの画像:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### その他
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark for Node.js via Java: フィーチャセット"
  description: "プログラムによるウォーターマーキングにより、強固な文書セキュリティを強化します。PDF、DOCX、XLSX、PPTX、および画像形式 (PNG、JPG など) を含むさまざまなファイル形式をサポートします。"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "正確なウォーターマーク制御"
      content: "ウォーターマークを特定のセクション、ドキュメント全体、またはさまざまなファイル形式内の個々の添付ファイルや図形に追加したり削除したりすることで、ウォーターマークを正確に操作できます。"

    # feature loop
    - icon: "watermark_style"
      title: "ウォーターマークの外観のカスタマイズ"
      content: "ドキュメント内の色、フォント、不透明度、回転、位置などの属性を変更することで、ウォーターマークの美観をきめ細かく制御できます。"

    # feature loop
    - icon: "hidden_print"
      title: "PDF ウォーターマークを印刷"
      content: "通常の文書表示では見えず、印刷プロセス中にのみ表示されるステルスウォーターマークを導入することで、文書のセキュリティを目立たなく強化できます。"

    # feature loop
    - icon: "image_only"
      title: "特定の画像ウォーターマーキング"
      content: "当社のソリューションを使用して、文書内の特定の画像に透かしを入れます。ウォーターマークを指定のセクション (ページ、スライドなど) に埋め込むか、ドキュメント全体に埋め込むかを選択できます。"

    # feature loop
    - icon: "image_frame"
      title: "マルチフレーム画像の透かし"
      content: "マルチフレーム画像フォーマット内の特定のフレームにウォーターマークを選択的に適用することで、ウォーターマークの配置をきめ細かく制御できます。"

    # feature loop
    - icon: "attachments"
      title: "包括的なコンテンツ保護"
      content: "Excel 文書内の添付ファイルやプレゼンテーション内の画像図形など、さまざまな文書要素に保護を拡張し、セキュリティをさらに強化します。"

    # feature loop
    - icon: "pdf_objects"
      title: "PDF の高度なウォーターマーキング"
      content: "ブリードボックス、アートボックス、クロップボックス、トリムボックスなど、PDF のさまざまな領域に透かしを入れます。"

    # feature loop
    - icon: "doc_background"
      title: "背景画像のウォーターマーク"
      content: "スプレッドシートとプレゼンテーションの背景画像内のウォーターマークを管理し、視覚的なセキュリティ対策のための追加のカスタマイズオプションを提供します。"

    # feature loop
    - icon: "unreadable_characters"
      title: "読めない文字を含むテキストウォーターマーク"
      content: "プレゼンテーションに埋め込まれたテキストウォーターマークに判読できない文字を使用することにより、不正なウォーターマーク抽出がはるかに困難になるため、セキュリティが強化されます。"

    # feature loop
    - icon: "watermark_text_search"
      title: "高度なウォーターマーク検索"
      content: "包括的な検索機能を活用して、特定のパラメータに基づいて、またはさまざまな基準を組み合わせて文書内のウォーターマークを検索し、効率的な検索と管理を可能にします。"

    # feature loop
    - icon: "watermark_image_search"
      title: "類似画像ウォーターマーク検出"
      content: "ソース画像と視覚的に似ている文書内の類似のウォーターマーク画像を検索します。"

    # feature loop
    - icon: "document_info"
      title: "プログラムによる文書情報抽出"
      content: "サポートされているファイル形式のページ設定の詳細やその他の文書情報など、貴重なメタデータをプログラムで抽出します。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "コードサンプル"
  description: "一般的な GroupDocs.Watermark for Node.js via Java の機能を紹介するコード例を見てみましょう"
  items:
    # code sample loop
    - title: "画像で文書にウォーターマークを付ける"
      content: |
        GroupDocs.Watermark for Node.js via Java を活用して、画像ウォーターマークを追加してドキュメントのセキュリティを強化してください。詳細:[画像透かし](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/)
        {{< landing/code title="画像ウォーターマークでファイルを保護する方法">}}
        ```javascript {style=abap}
        // ソースドキュメントをウォーターマーカーに読み込み
        let watermarker = new Watermarker("document.pdf");
        
        // ウォーターマーク画像へのパスを指定
        let watermark = new ImageWatermark("watermark.jpg");

        // ファイルを保護して保存する
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "既存のウォーターマークの検索と変更"
      content: |
        GroupDocs.Watermark for Node.js via Java ではドキュメントのウォーターマークを管理できます。ウォーターマークを選択し、そのプロパティを変更します。その方法をご覧ください:[ウォーターマークの変更](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/)
        {{< landing/code title="ウォーターマークの検索と変更。">}}
        ```javascript {style=abap}   
        // ソースドキュメントをロード
        let watermarker = new Watermarker("document.pdf");

        // 更新するウォーターマークを検索する
        let searchCriteria = new TextSearchCriteria("test", false);                               
        let watermarks = watermarker.search(searchCriteria); 

        // 必要なプロパティを更新
        watermarks.forEach((watermark)
        {  
            watermark.setText("New Text");
        }

        // 変更したドキュメントを指定したパスに保存
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
