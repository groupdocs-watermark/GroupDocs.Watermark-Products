
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:19
draft: false
lang: ja
format: Image
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET C# で画像にウォーターマークを付ける"
head_description: ".NET C# を使用して画像にシームレスなウォーターマークを適用する方法を学びましょう。品質を損なうことなく資産を保護しましょう。"

############################# Header ############################
title: ".NET を使用した画像のラピッドカスタムウォーターマーキング" 
description: ".NET C# ツールは、ウォーターマークを画像に埋め込むための迅速なソリューションを提供します。幅広い画像フォーマットをサポートしているため、写真からデジタルアートワークまですべてカバーできます。"
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Nuget で無料でダウンロード"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "さらに詳しく"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET は画像の透かし処理を自動化するように設計されており、JPEG、PNG、BMP、TIFF などのさまざまな形式をサポートしています。この堅牢な API により、特定の要件に合わせて不透明度、サイズ、位置を調整できるテキストや画像のウォーターマークをすばやく挿入できます。著作権保護の目的であれ、マーケティング資料の強化であれ、当社のツールキットを使用すれば、元の画質への影響を最小限に抑えながら、高い忠実度でウォーターマークを適用できます。

############################# Steps ############################
steps:
    enable: true
    title: "ドキュメントを強化: .NET を使用して Image のウォーターマークを生成"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** は、.NET 開発者向けにさまざまなビジネス ファイル形式にウォーターマークを簡単に追加できるライブラリです。私たちのライブラリをアプリケーションに統合し、次の手順を使用してドキュメントに簡単に透かしを入れます。
      
      1. **ウォーターマークの開始:** まず、API の基礎である **Watermarker** クラスを理解することから始めます。プロセスを開始するには、ドキュメント処理の前にプロセスをインスタンス化してください。パスであれストリーム オブジェクトであれ、Image ファイルをコンストラクターに提供することの重要性を見落とさないでください。
      2. **カスタム ウォーターマークの作成:** 仕様に合わせた **Watermark** オブジェクトを作成して、次のフェーズに進みます。この多用途ツールは、特定のドキュメント ページに限定されません。また、添付ファイルやヘッダーなどのネイティブのドキュメント要素にシームレスに統合することもできます。
      3. **透かし属性の微調整:** 高さ、幅、ページ配置、フォント ファミリー、色などのプロパティを調整して、透かしのエクスペリエンスを調整します。このレベルのカスタマイズにより、透かしがドキュメントにシームレスに溶け込むことが保証されます。
      4. **透かしの適用:** **Watermarker** メソッドを利用して、カスタム透かしをドキュメントに簡単に適用します。 1 つまたは複数の透かしを追加する必要がある場合でも、このプロセスには柔軟性があります。セキュリティを強化するには、処理したドキュメントを別の場所に保存することを検討してください。
   
    code:
      platform: "net"
      copy_title: "[コピー]"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "クリックしてコピー"
        copy_done: "コピーされました"
      links:
        #  loop
        - title: "その他の例"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "ドキュメンテーション"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // IMAGE ファイルにテキスト透かしを生成します

        // 透かしを入れるファイルを提供する
        using (Watermarker watermarker = new Watermarker("input.JPEG"))
        {
            // テキスト透かしインスタンスを生成する
            Font font = new Font("Arial", 19, FontStyle.Bold | FontStyle.Italic);
            TextWatermark watermark = new TextWatermark("my watermark", font);
            watermark.ForegroundColor = Color.Red;
            watermark.BackgroundColor = Color.Blue;
            watermarker.Add(watermark);

            // IMAGE の結果を保存
            watermarker.Save("output.JPEG");
        }
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "ウォーターマークの追加について詳しく調べる"
  description: "当社の強力なAPIを活用して、.NET アプリケーション内の文書、スライド、図、その他のさまざまな文書タイプをレンダリング、表示、変換、管理できます。GroupDocs.Watermark は透かし機能をシームレスに統合して、文書のセキュリティと著作権保護を強化します。"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "ウォーターマークを追加"
  features:
    # feature loop
    - title: "ドキュメントに簡単に透かしを入れます。"
      content: "GroupDocs.Watermark は .NET 人の開発者がウォーターマークをアプリケーションに簡単に統合できるようにします。人気のビジネス文書やファイルにテキスト、画像、動的ウォーターマークを簡単に追加できるため、コンテンツが安全に保たれ、すべてのプラットフォームで一貫したブランド化が保証されます。"

    # feature loop
    - title: "ニーズに合わせてウォーターマークをカスタマイズできます。"
      content: "GroupDocs.Watermark がサポートする豊富な機能を使用して、特定の要件に合わせてウォーターマークをカスタマイズできます。サイズ、回転、透明度、色、フォントを調整して、ウォーターマークが完璧に見えるようにするだけでなく、重要な情報を邪魔することなく文書のセキュリティを強化できます。"

    # feature loop
    - title: "ネイティブドキュメント機能をウォーターマークに活用"
      content: "文書フォーマット固有の機能を活用して、高度なウォーターマークを作成できます。ネイティブの PDF 注釈、MS Word 背景、Excel ヘッダーとフッターのいずれを使用する場合でも、GroupDocs.Watermark は文書構造と緊密に統合して、効果的で侵襲性の低いウォーターマークを適用します。"
      
  code_samples:
    # code sample loop
    - title: "DOCX の画像ウォーターマークを生成"
      content: |
        この例は、図形の透かしにイメージ効果を適用する方法を示します。
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  Word ドキュメントをロード
            var loadOptions = new WordProcessingLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.docx", loadOptions))
            {
                //  ウォーターマークオプションを設定する
                using (ImageWatermark watermark = new ImageWatermark("logo.png"))
                {
                    WordProcessingImageEffects effects = new WordProcessingImageEffects();
                    effects.Brightness = 0.7;
                    effects.Contrast = 0.6;
                    effects.ChromaKey = Color.Red;
                    effects.BorderLineFormat.Enabled = true;
                    effects.BorderLineFormat.Weight = 1;

                    WordProcessingWatermarkSectionOptions options = new WordProcessingWatermarkSectionOptions();
                    options.Effects = effects;

                    //  ウォーターマークを生成
                    watermarker.Add(watermark, options);
                }

                //  更新した文書を保存
                watermarker.save("result.docx");
            }

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか?"
  description: "GroupDocs.Watermark の機能を無料で試すか、ライセンスをリクエストしてください"
  items:
    #  loop
    - title: "Nuget ダウンロード"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "ライセンス"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "C# を使用して画像フォーマット全体でウォーターマークをすばやく実装"
    exclude: "IMAGE"
    description: "さまざまな画像形式を迅速かつ効率的に処理できる .NET C# ツールキットで画像保護を強化してください。ウォーターマークはビジュアルコンテンツと完璧に調和するようにカスタマイズできます。"
    items: 
        # format loop 1
        - name: "ウォーターマーク PDF"
          format: "PDF"
          link: "/watermark/net/generate//pdf/"
          description: "アドビ Portable ドキュメントフォーマット"

        # format loop 2
        - name: "ウォーターマーク Word"
          format: "WORD"
          link: "/watermark/net/generate//word/"
          description: "MS Word とオープンオフィス文書"
          
        # format loop 3
        - name: "ウォーターマーク Excel"
          format: "EXCEL"
          link: "/watermark/net/generate//excel/"
          description: "MS Excel とオープンオフィススプレッドシート"

        # format loop 4
        - name: "ウォーターマーク画像"
          format: "IMAGE"
          link: "/watermark/net/generate//image/"
          description: "人気の画像フォーマット"

        # format loop 5
        - name: "ウォーターマーク写真"
          format: "PHOTO"
          link: "/watermark/net/generate//photo/"
          description: "写真フォーマット"

        # format loop 6
        - name: "ウォーターマーク PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/generate//powerpoint/"
          description: "MS PowerPoint とオープンオフィスプレゼンテーション"

        # format loop 7
        - name: "ウォーターマーク DOCX"
          format: "DOCX"
          link: "/watermark/net/generate//docx/"
          description: "マイクロソフト Word XML ドキュメントを開く"
          
        # format loop 8
        - name: "ウォーターマーク PPTX"
          format: "PPTX"
          link: "/watermark/net/generate//pptx/"
          description: "PowerPoint XML プレゼンテーションを開く"
          
        # format loop 9
        - name: "ウォーターマーク XLSX"
          format: "XLSX"
          link: "/watermark/net/generate//xlsx/"
          description: "マイクロソフト Excel オープン XML スプレッドシート"

        # format loop 10
        - name: "ウォーターマーク JPEG"
          format: "JPEG"
          link: "/watermark/net/generate//jpeg/"
          description: "JPEG イメージ"

        # format loop 11
        - name: "ウォーターマーク PNG"
          format: "PNG"
          link: "/watermark/net/generate//png/"
          description: "Portable ネットワークグラフィック"

        # format loop 12
        - name: "ウォーターマーク TIFF"
          format: "TIFF"
          link: "/watermark/net/generate//tiff/"
          description: "タグ画像ファイル形式"

        # format loop 13
        - name: "ウォーターマーク WEBP"
          format: "WEBP"
          link: "/watermark/net/generate//webp/"
          description: "ウェブ画像"

        # format loop 14
        - name: "ウォーターマーク DOC"
          format: "DOC"
          link: "/watermark/net/generate//doc/"
          description: "マイクロソフト Word 97-2007 ドキュメント"

        # format loop 15
        - name: "ウォーターマーク XLS"
          format: "XLS"
          link: "/watermark/net/generate//xls/"
          description: "マイクロソフト Excel ワークブック 97-2003"

        # format loop 16
        - name: "ウォーターマーク PPT"
          format: "PPT"
          link: "/watermark/net/generate//ppt/"
          description: "PowerPoint プレゼンテーション 97-2003"

        # format loop 17
        - name: "ウォーターマーク RTF"
          format: "RTF"
          link: "/watermark/net/generate//rtf/"
          description: "リッチテキスト形式"

---