---
############################# Static ############################
layout: "landing"
date: 2024-05-06T23:13:47
draft: false

lang: ja
product: "Watermark"
product_tag: "watermark"
platform: "Net"
platform_tag: "net"

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
head_title: "C# .NET ドキュメントウォーターマークソフトウェア | ウォーターマークを追加"
head_description: "ドキュメント内のウォーターマークを追加、検索、削除するためのC# .NET ライブラリ:PDF、Word、Excel、プレゼンテーション、Visio の図、電子メール、画像ファイル形式。"

############################# Header ############################
title: "C# .NET アプリケーションでドキュメントに簡単にウォーターマークを付ける"
description: "すべての一般的な文書形式にカスタマイズ可能な透かしを追加できる柔軟な文書透かし API で C# ソリューションを強化しましょう。"
words:
  for: "にとって"

actions:
  main: "無料 NuGet ダウンロード"
  main_link: "https://www.nuget.org/packages/GroupDocs.Watermark"
  alt: "ライセンス"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/net/"
  title: "始める準備はできましたか?"
  description: "GroupDocs.Watermark の機能を無料で試すか、ライセンスをリクエストしてください"

release:
  title: "バージョン {0} がリリースされました"
  notes: "新機能を見る"
  downloads: "ダウンロード"

code:
  title: "C# で PDF ファイルにウォーターマークを付ける"
  more: "その他の例"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
  install: "dotnet add package GroupDocs.Watermark"
  content: |
    ```csharp {style=abap}   
    // PDF パスを渡すウォーターマーカーをインスタンス化
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    using (Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions))
    {
        // ウォーターマークオプションのカスタマイズ
        TextWatermark textWatermark = 
            new TextWatermark("Approved", new Font("Arial", 8));
        
        // PDF ドキュメントにウォーターマークを適用
        watermarker.Add(textWatermark);

        // 結果文書を保存
        watermarker.Save("result.pdf");
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark 一目でわかる"
  description: ".NET 経由でドキュメントにウォーターマークを付けるためのAPI"
  features:
    # feature loop
    - title: "C# ファイルのウォーターマーク"
      content: "GroupDocs.Watermark を使用してビジネスファイルにウォーターマークを追加します。テキスト、画像、図、または電子メールの添付ファイルを使用してください。"

    # feature loop
    - title: "ウォーターマークを目的に合わせてカスタマイズ"
      content: "GroupDocs.Watermark for .NET ソフトウェアでは、ウォーターマークをさまざまな方法でカスタマイズできます。太字、斜体、フォントタイプなどのテキストスタイルと、回転などの画像プロパティにより、透かし処理が強化されます。"

    # feature loop
    - title: "すべての一般的なファイル形式がサポートされています"
      content: "GroupDocs.Watermark ソリューションでは、多くのファイルおよびドキュメント形式がサポートされています。PDF、Microsoft Office Word、Excel、PowerPoint、JPEG、PNG、GIF、BMP、Visio 図、電子メールなどの画像は、ウォーターマークで保護できます。"

    # feature loop
    - title: "ウォーターマークの検索と更新"
      content: "文書に既に表示されているウォーターマークは、検索して再度処理できます。余分な手間をかけずに、テキスト、スタイル、画像を変更したり、表示されているウォーターマークを削除したりできます。"

############################# Platforms ############################
platforms:
  enable: true
  title: "プラットフォーム独立性"
  description: "GroupDocs.Watermark for .NET は下記のオペレーティングシステム、フレームワーク、パッケージマネージャーをサポートしています"
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "対応ファイル形式"
  description: |
    GroupDocs.Watermark for .NET は次の [ファイル形式](https://docs.groupdocs.com/watermark/net/supported-document-formats/) の処理を提供します。
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
  title: "GroupDocs.Watermark の機能"
  description: "PDF、Office、画像、その他のフォーマットをウォーターマークで保護"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "ドキュメントウォーターマーキング"
      content: "さまざまなファイル形式の特定のセクションまたはドキュメント全体に透かしを追加または削除します。"

    # feature loop
    - icon: "watermark_style"
      title: "ウォーターマークのスタイルを設定する"
      content: "色、フォント、回転などのさまざまなウォーターマークプロパティをカスタマイズします。"

    # feature loop
    - icon: "hidden_print"
      title: "PDF 非表示の印刷ウォーターマーク"
      content: "文書の印刷時にのみ表示される PDF に隠しウォーターマークを割り当てます。"

    # feature loop
    - icon: "image_only"
      title: "文書内の画像のみにウォーターマークを付ける"
      content: "特定のセクション、ページ、スライド、またはドキュメントのすべての画像に透かしを入れます。"

    # feature loop
    - icon: "image_frame"
      title: "選択した画像フレームを処理"
      content: "マルチフレーム画像の特定のフレームにのみウォーターマークを割り当てます。"

    # feature loop
    - icon: "attachments"
      title: "アタッチメントとシェイプ"
      content: "Excel ドキュメントのすべての添付ファイルと、スライドのすべての画像シェイプにウォーターマークを設定します。"

    # feature loop
    - icon: "pdf_objects"
      title: "PDF オブジェクト"
      content: "ウォーターマークを PDF ドキュメントのブリードボックス、アートボックス、クロップボックス、またはトリムボックスに合わせます。"

    # feature loop
    - icon: "doc_background"
      title: "文書の背景"
      content: "透かしを入れるか、スプレッドシートやスライドの背景画像から削除します。"

    # feature loop
    - icon: "unreadable_characters"
      title: "読めない文字保護"
      content: "プレゼンテーションで判読できない文字を使用してテキストウォーターマークを保護します。"

    # feature loop
    - icon: "watermark_text_search"
      title: "ドキュメント内のウォーターマークを検索する"
      content: "特定のパラメータに基づいてウォーターマークを検索するか、複数の条件を組み合わせてウォーターマークを検索します。"

    # feature loop
    - icon: "watermark_image_search"
      title: "類似画像のウォーターマークを検索"
      content: "特定の画像に似ている画像ウォーターマークを探してください。"

    # feature loop
    - icon: "document_info"
      title: "文書情報を取得"
      content: "サポートされている形式のページ設定やその他の情報をプログラムで抽出します。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "コードサンプル"
  description: "一般的な GroupDocs.Watermark for .NET 操作のいくつかのユースケース"
  items:
    # code sample loop
    - title: "文書に画像を追加して透かしを入れます。"
      content: |
        どんなドキュメントでも保護するには、[画像の透かし](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/) を使用できます。
        {{< landing/code title="画像ウォーターマークでファイルを保護する方法">}}
        ```csharp {style=abap}
        // ソースドキュメントをウォーターマーカーに読み込み
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // ウォーターマーク画像へのパスを指定
            using (ImageWatermark watermark = new ImageWatermark("watermark.jpg"))
            {
                // ファイルを保護して保存する
                watermarker.Add(watermark);

                watermarker.Save("result.pdf");
            }
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "既存のウォーターマークを検索して変更します。"
      content: |
        GroupDocs.Watermark では、ドキュメントに既に表示されている [ウォーターマークの変更](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/) が可能です。必要なアイテムを検索し、そのプロパティを更新してください。
        {{< landing/code title="ウォーターマークの検索と変更。">}}
        ```csharp {style=abap}   
        // ソースドキュメントをロード
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // 更新するウォーターマークを検索する
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                // 必要なプロパティを更新
                watermark.Text = "New Text";
            }

            // 変更したドキュメントを指定したパスに保存
            watermarker.Save("document.pdf");
        }
        ```
        {{< /landing/code >}}

---
