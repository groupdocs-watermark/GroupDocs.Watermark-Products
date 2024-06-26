
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:24
draft: false
lang: ja
format: Xls
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C# で XLS にウォーターマークを作成"
head_description: ".NET C# を使用して XLS ファイルにウォーターマークを追加および管理し、Excel ドキュメントのセキュリティを強化します。"

############################# Header ############################
title: "XLS ファイルの C# ウォーターマークを生成" 
description: "Excel の財務データおよび個人データを保護するためにカスタマイズされた .NET C# を使用して XLS スプレッドシートに堅牢なウォーターマークを実装します。"
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
       GroupDocs.Watermark for .NET は .NET C# 開発者に XLS ファイルにウォーターマークを効果的に作成、作成、埋め込むためのツールを提供します。この API は Excel ワークフローへのシームレスな統合を目的として設計されており、透明度、テキスト、画像をカスタマイズできる可視ウォーターマークと不可視ウォーターマークの両方を簡単に追加できます。財務スプレッドシート、クライアントレポート、または機密保持を必要とするあらゆる Excel 文書内の機密情報の保護に最適な GroupDocs.Watermark には、内容分析に基づく条件付きウォーターマークの配置などの高度な機能が備わっています。このソリューションはすべての .NET 環境をサポートしているため、文書が不正使用や配布から確実に保護されます。

############################# Steps ############################
steps:
    enable: true
    title: "Xls ドキュメントのウォーターマークを簡単に生成"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/):** .NET アプリケーション用の高度な透かしライブラリ。ソリューションを強化し、ジャストインタイムでウォーターマークを使用してドキュメントを保護します。
      
      1. **コア クラス: Watermarker。** API のメイン クラスは **Watermarker** です。ドキュメントを処理する前にインスタンス化する必要があります。 Xls ファイルをパスまたはストリーム オブジェクトとしてコンストラクターに渡すことを忘れないでください。
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
        // XLS ファイルに画像ウォーターマークを生成します

        // ソース ファイル パスを Watermarker コンストラクターに提供します
        using (Watermarker watermarker = new Watermarker("input.xls"))
        {
            // 画像ファイルを使用して画像透かしインスタンスを生成する
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // 透かし入りの XLS の結果を保存する
            watermarker.Save("output.xls");
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
    title: "C# で XLS にウォーターマークを適用する"
    exclude: "XLS"
    description: ".NET C# を利用してカスタムウォーターマークを動的に生成して XLS ファイルに統合し、Excel データを効果的に保護します。"
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