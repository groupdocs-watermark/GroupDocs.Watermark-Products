
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:24
draft: false
lang: ja
format: Jpg
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "JPG 画像の C# ウォーターマーキング"
head_description: ".NET C# を使用して JPG ファイルにウォーターマークを統合し、デジタル画像を効果的に保護します。"

############################# Header ############################
title: ".NET C# で JPG 枚のイメージを保護する" 
description: ".NET C# を適用して JPG 枚の画像に強固なウォーターマークを作成してください。著作権保護と不正使用の防止に最適です。"
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
       GroupDocs.Watermark for .NET は .NET C# 開発者に JPG 個の画像にウォーターマークを追加するための高度なフレームワークを提供します。この API を使用すると、透明度、位置、サイズをカスタマイズできるテキスト、ロゴ、グラフィックウォーターマークを正確に埋め込むことができ、デジタルメディアやプロの写真撮影に最適です。元のアートワークの完全性を維持しながら著作権侵害を防止するウォーターマークを埋め込むように設計された機能により、品質を犠牲にすることなく画像のセキュリティを強化できます。GroupDocs.Watermark は、個人の写真保護から広告やメディアでの商用利用まで、幅広い用途に適しており、ビジュアルアセットに独自のマークを付けて法的に保護します。

############################# Steps ############################
steps:
    enable: true
    title: "Jpg ドキュメントのウォーターマークを簡単に生成"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/):** .NET アプリケーション用の高度な透かしライブラリ。ソリューションを強化し、ジャストインタイムでウォーターマークを使用してドキュメントを保護します。
      
      1. **コア クラス: Watermarker。** API のメイン クラスは **Watermarker** です。ドキュメントを処理する前にインスタンス化する必要があります。 Jpg ファイルをパスまたはストリーム オブジェクトとしてコンストラクターに渡すことを忘れないでください。
      2. **ウォーターマークの作成** 次のステップでは、目的のタイプのウォーターマーク オブジェクトを構築します。特定のドキュメント ページだけでなく、画像やヘッダーなどのネイティブ ドキュメント パーツにも配置できます。
      3. **外観の微調整。** 高さと幅、上、左、中央の配置、フォントと色などのウォーターマークのプロパティを設定します。
      4. **適用と保存。** 新しい透かしを追加するには、**Watermarker** メソッドを使用します。必要なだけ透かしを追加してください。透かし入りのドキュメントは任意の場所に保存できます。
   
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
        // JPG ファイルに画像ウォーターマークを生成します

        // ソース ファイル パスを Watermarker コンストラクターに提供します
        using (Watermarker watermarker = new Watermarker("input.jpg"))
        {
            // 画像ファイルを使用して画像透かしインスタンスを生成する
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // 透かし入りの JPG の結果を保存する
            watermarker.Save("output.jpg");
        }
        
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "ウォーターマーキングゲームをレベルアップ"
  description: ".NET 用の GroupDocs.Watermark API で高度なウォーターマーク機能を活用してください。この強力なツールを使用すると、さまざまな文書タイプにウォーターマークを正確にカスタマイズして適用できるため、視覚的な混乱を最小限に抑えながら、最大限のセキュリティと著作権遵守を確保できます。"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "包括的なウォーターマーキングソリューション"
  features:
    # feature loop
    - title: "洗練されたタイリングオプション"
      content: "タイリングオプションを使用して、透かしをドキュメント全体にシームレスに拡張できます。この機能により、ウォーターマークが文書領域全体に広がり、デザインや読みやすさを損なうことなく、削除を防ぎ、文書を完全に保護できます。"

    # feature loop
    - title: "鮮やかな色のカスタマイズ"
      content: "ウォーターマークに彩りを添えましょう！当社の API では色を全面的にカスタマイズできるため、企業のブランディングやドキュメントスタイルにぴったり合ったウォーターマークを適用できます。強固なセキュリティ機能を維持しつつ、視覚的な魅力を高めましょう。"

    # feature loop
    - title: "セキュリティ設定の強化"
      content: "高度なウォーターマーク設定で文書のセキュリティを次のレベルに引き上げましょう。可視要素と不可視要素の両方を組み込んだ多層ウォーターマークを設定することで、不正コピーを防ぎ、意図した受信者だけが重要な情報にアクセスできるようにします。"
      
  code_samples:
    # code sample loop
    - title: "PowerPoint ウォーターマークを生成"
      content: |
        この例は、PPTX 背景画像にウォーターマークを追加する方法を示しています
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  PPTX プレゼンテーションをロード
            var loadOptions = new PresentationLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pptx", loadOptions))
            {
                //  ウォーターマークプロパティの設定
                TextWatermark watermark = new TextWatermark("Protected image", new Font("Arial", 8));
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermark.RotateAngle = 45;
                watermark.SizingType = SizingType.ScaleToParentDimensions;
                watermark.ScaleFactor = 1;

                //  ウォーターマークスライドの背景
                PresentationContent content = watermarker.GetContent<PresentationContent>();
                foreach (PresentationSlide slide in content.Slides)
                {
                    if (slide.ImageFillFormat.BackgroundImage != null)
                    {
                        slide.ImageFillFormat.BackgroundImage.Add(watermark);
                    }
                }

                //  処理済みのプレゼンテーションを保存
                watermarker.save("result.pptx");
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
    title: "C# で JPG にウォーターマークを実装する"
    exclude: "JPG"
    description: ".NET C #を活用して、JPG ファイルに不可視または可視のウォーターマークを埋め込んでください。これは、安全で認識可能なデジタルコンテンツに不可欠です。"
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