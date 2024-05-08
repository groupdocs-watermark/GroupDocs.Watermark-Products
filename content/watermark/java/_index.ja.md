---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:29
draft: false

lang: ja
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

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

############################# Head ############################
head_title: "Java ウォーターマークライブラリ | ドキュメントにウォーターマークを追加"
head_description: "PDF、Word、Excel、プレゼンテーション、Visio の図、電子メール、画像ファイルにテキストと画像のウォーターマークを追加および操作するためのネイティブ Java ソフトウェア。"

############################# Header ############################
title: "Java 件のプロジェクトに文書ウォーターマークを簡単に実装"
description: "GroupDocs.Watermark ライブラリを使用してファイルにウォーターマークを付ける機能で Java アプリケーションを強化してください。当社の API では、一般的なさまざまなファイル形式のウォーターマークをカスタマイズできます。"
words:
  for: "にとって"

actions:
  main: "Mavenから無料でダウンロード"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "ライセンス"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java/"
  title: "始める準備はできましたか?"
  description: "GroupDocs.Watermark の機能を無料で試すか、ライセンスをリクエストしてください"

release:
  title: "バージョン {0} がリリースされました"
  notes: "新機能を見る"
  downloads: "ダウンロード"

code:
  title: "Java 経由で PDF のウォーターマーク"
  more: "その他の例"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-watermark</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // PDF パスを渡すウォーターマーカーをインスタンス化
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // ウォーターマークオプションのカスタマイズ
    TextWatermark textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // PDF ドキュメントにウォーターマークを適用
    watermarker.add(textWatermark);

    // 結果文書を保存
    watermarker.save("result.pdf");
    watermarker.close();
      
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark 一目でわかる"
  description: "Java テクノロジーを使用してウォーターマークを追加するために設計されたライブラリ"
  features:
    # feature loop
    - title: "Java 経由でファイルにウォーターマークを付ける"
      content: "GroupDocs.Watermark for Java を使用してビジネス文書を保護してください。テキスト、画像、図、メールの添付ファイルをウォーターマークとしてさまざまなファイル形式に追加できます。"

    # feature loop
    - title: "特定のニーズに合わせてウォーターマークをカスタマイズ"
      content: "GroupDocs.Watermark for Java には、ウォーターマークの幅広いカスタマイズオプションが用意されています。テキストスタイル (太字、斜体、フォント) と画像プロパティ (回転など) を調整して、ウォーターマークのプロセスを特定の目的に合わせて調整できます。"

    # feature loop
    - title: "幅広いフォーマットのサポート"
      content: "GroupDocs.Watermark for Java は、PDF、Microsoft Office (Word、Excel、PowerPoint)、画像 (JPEG、PNG、GIF、BMP)、Visio 図、電子メールなど、さまざまなファイル形式とシームレスに統合されます。多様なファイルタイプにわたる文書セキュリティを強化します。"

    # feature loop
    - title: "簡単なウォーターマーク検索と管理"
      content: "文書内の既存のウォーターマークを効率的に管理します。特定のウォーターマークを検索したり、テキスト、スタイル、画像を変更したり、完全に削除したりできます。GroupDocs.Watermark for Java を使うと、ウォーターマークのワークフローが簡単になります。"

############################# Platforms ############################
platforms:
  enable: true
  title: "プラットフォーム独立性"
  description: "GroupDocs.Watermark for Java は、さまざまなオペレーティングシステムとパッケージマネージャーをサポートしています。"
  items:
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "対応ファイル形式"
  description: |
    GroupDocs.Watermark for Java は幅広いファイル形式の処理を可能にします。[全リストを見る](https://docs.groupdocs.com/watermark/net/supported-document-formats/)。
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
  title: "GroupDocs.Watermark for Java: 機能"
  description: "ウォーターマークを追加してファイルを保護します。PDF、Office ドキュメント、画像など、さまざまな形式をサポートします。"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "ファイルウォーターマーク"
      content: "サポートされているさまざまなファイル形式の特定のセクションまたはドキュメント全体にウォーターマークを追加または削除します。"

    # feature loop
    - icon: "watermark_style"
      title: "ウォーターマークのカスタマイズ"
      content: "色、フォント、回転などのオプションを使用してウォーターマークの外観をカスタマイズします。"

    # feature loop
    - icon: "hidden_print"
      title: "PDF の隠し印刷ウォーターマーク"
      content: "PDF ドキュメントを印刷するときにのみ表示されるウォーターマークを追加します。"

    # feature loop
    - icon: "image_only"
      title: "選択的画像ウォーターマーキング"
      content: "特定のセクション、ページ、スライド、またはドキュメント全体内のすべての画像に透かしを入れます。"

    # feature loop
    - icon: "image_frame"
      title: "特定の画像フレームにウォーターマークを付ける"
      content: "マルチフレーム画像内の特定のフレームにウォーターマークを適用します。"

    # feature loop
    - icon: "attachments"
      title: "ウォーターマークアタッチメントとシェイプ"
      content: "Excel ドキュメントのすべての添付ファイル、またはプレゼンテーションのすべての画像シェイプにウォーターマークを追加します。"

    # feature loop
    - icon: "pdf_objects"
      title: "PDF のウォーターマーク配置"
      content: "ブリードボックス、アートボックス、クロップボックス、トリムボックスなど、PDF ドキュメントのさまざまな領域にウォーターマークを揃えます。"

    # feature loop
    - icon: "doc_background"
      title: "背景画像によるウォーターマーク"
      content: "スプレッドシートまたはプレゼンテーションに背景画像のウォーターマークを追加または削除します。"

    # feature loop
    - icon: "unreadable_characters"
      title: "読めない文字による保護"
      content: "読めない文字を含むテキストウォーターマークを使用してプレゼンテーションを保護します。"

    # feature loop
    - icon: "watermark_text_search"
      title: "ウォーターマークを検索する"
      content: "正規表現を含むさまざまなパラメータを使用して、ファイルに表示されているウォーターマークのリストを取得します。"

    # feature loop
    - icon: "watermark_image_search"
      title: "類似画像のウォーターマークを検索"
      content: "特定の画像のように見える画像ウォーターマークを探します。"

    # feature loop
    - icon: "document_info"
      title: "文書情報を抽出"
      content: "サポートされているファイル形式のページ設定など、さまざまなドキュメントデータを取得します。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "コードサンプル"
  description: "一般的な GroupDocs.Watermark for Java の機能を説明するコード例をご覧ください"
  items:
    # code sample loop
    - title: "画像を使用して文書にウォーターマークを付ける"
      content: |
        GroupDocs.Watermark for Java を活用して、画像ウォーターマークを追加してドキュメントのセキュリティを強化してください。詳細:[画像透かし](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/)
        {{< landing/code title="画像ウォーターマークでファイルを保護する方法">}}
        ```csharp {style=abap}
        // ソースドキュメントをウォーターマーカーに読み込み
        Watermarker watermarker = new Watermarker("document.pdf");
        
        // ウォーターマーク画像へのパスを指定
        ImageWatermark watermark = new ImageWatermark("watermark.jpg");

        // ファイルを保護して保存する
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "ウォーターマークを修正"
      content: |
        GroupDocs.Watermark for Java を使用すると、ドキュメント内の既存のウォーターマークを管理できます。特定のウォーターマークを検索して [プロパティを変更](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/)。
        {{< landing/code title="ウォーターマークの検索と変更。">}}
        ```csharp {style=abap}   
        // ソースドキュメントをロード
        Watermarker watermarker = new Watermarker("document.pdf");

        // 更新するウォーターマークを検索する
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);                               
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);                             

        // 必要なプロパティを更新
        for (PossibleWatermark watermark : watermarks)                                                           
        {  
            watermark.setText("New Text");
        }

        // 変更したドキュメントを指定したパスに保存
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
