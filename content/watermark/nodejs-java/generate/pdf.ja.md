
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:26
draft: false
lang: ja
format: Pdf
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Node.js ウォーターマークで PDF を保護"
head_description: "Node.js を使用して PDF にウォーターマークを組み込むことで、公式文書や契約書を保護できます。"

############################# Header ############################
title: "Node.js を使用して PDF ドキュメント用のウォーターマークを作成" 
description: "Node.js を使用して PDF ファイルに高度なウォーターマークを追加し、公式文書、契約書、機密情報を保護します。"
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "NPM で無料でダウンロード"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "さらに詳しく"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java は、Node.js 開発者に PDF ファイル用に特別に設計されたウォーターマークを生成、作成、管理するための強力なツールを提供します。この API により、ウォーターマークを公式文書、契約書、および追加のセキュリティレイヤーが必要な PDF の機密ファイルに正確に統合できます。ウォーターマークを表示または非表示にカスタマイズして、コンテンツの読みやすさを妨げないようにすると同時に、著作権保護と不正防止を効果的に行えます。文書の完全性が最優先される法律、金融、政府機関での使用に最適な GroupDocs.Watermark は、大規模文書セットのウォーターマークのバッチ処理もサポートしており、最新の Node.js 環境と完全に互換性があります。

############################# Steps ############################
steps:
    enable: true
    title: "ビジネス ドキュメントの保護: Pdf ウォーターマークを生成"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/):** でドキュメントのセキュリティを強化 - Node.js via Java 用の強力なウォーターマーク生成ソリューション。
      
      1. **Node.js via Java アプリケーションでの安全なウォーターマークの効率化:** **Watermarker** クラスは、GroupDocs.Watermark API のコア コンポーネントとして機能します。このライブラリは、Pdf を含むさまざまなドキュメント形式のウォーターマークの生成を簡素化します。まず、ドキュメントを処理する前にウォーターマーカー インスタンスを作成します。初期化中に、Pdf ファイル パスまたはストリーム オブジェクトをコンストラクターに提供します。
      2. **保護を強化するためのウォーターマークの生成:** セキュリティのニーズに完全に適合するウォーターマークを強化します。目的のタイプを指定して **Watermark** オブジェクトを構築します。従来のページ配置とは異なり、ヘッダーや添付ファイルなどのネイティブ ドキュメント要素内に透かしを埋め込むことができ、ドキュメントのセキュリティを強化し、プロフェッショナルな雰囲気を加えることができます。
      3. **透かしの外観を微調整して効果を最適化:** 透かしの視覚的な側面を制御します。高さ、幅、配置 (上、左、中央など)、フォント ファミリ、色などのプロパティをカスタマイズして、文書の正当性を強化する視覚的に効果的で一貫した結果を実現します。
      4. **ウォーターマーク アプリケーションと安全なストレージ**: **Watermarker** メソッドを使用してウォーターマークを組み込みます。このライブラリでは、保護を強化するために必要に応じて複数のウォーターマークを追加できます。元のファイルを保存し、透かし入りのドキュメントを保護するために、変更した Pdf ドキュメントを別の安全な場所に保存することをお勧めします。
   
    code:
      platform: "net"
      copy_title: "[コピー]"
      install:
        command: "npm i @groupdocs/groupdocs.watermark"
        copy_tip: "クリックしてコピー"
        copy_done: "コピーされました"
      links:
        #  loop
        - title: "その他の例"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
        #  loop
        - title: "ドキュメンテーション"
          link: "https://docs.groupdocs.com/watermark/nodejs-java/"
          
      content: |
        ```javascript {style=abap}

        // PDF の画像ウォーターマークを生成します

        // ソース ファイルを渡して Watermarker をインスタンス化します
        const watermarker = new groupdocs.watermark.Watermarker("input.pdf");
        
        // 画像ファイルを提供してウォーターマークを生成
        const watermark = new groupdocs.watermark.ImageWatermark("watermark.png");

        // PDF の結果を取得する
        watermarker.add(watermark);
        watermarker.save("output.pdf");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "洗練されたウォーターマーク統合"
  description: ".NET 開発者向けの GroupDocs.Watermark API は、ウォーターマークをあらゆるドキュメントにシームレスに統合するための洗練されたソリューションを提供します。このツールは、文書の美観を保ちながら著作権を確実に保護する、洗練された控えめなウォーターマークを作成するように設計されています。"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "高精度ウォーターマーク統合"
  features:
    # feature loop
    - title: "グラデーションウォーターマークエフェクト"
      content: "ドキュメント全体にスムーズに溶け込むグラデーションウォーターマークを実装します。この機能により、線状または放射状のグラデーションが可能になり、セキュリティ機能にモダンな外観が加わり、コンテンツを圧迫することなく保護と視覚的エンゲージメントの両方が強化されます。"

    # feature loop
    - title: "セキュリティを強化するためのパターンウォーターマーク"
      content: "パターンベースのウォーターマークを使用して、セキュリティをさらに強化します。当社の API は、複雑な設計や文書全体で繰り返し使用できるさまざまなパターンをサポートしているため、ウォーターマークの改ざんや削除に対する耐性が高まります。"

    # feature loop
    - title: "文書固有のウォーターマーク"
      content: "ウォーターマークは、さまざまなドキュメントタイプに合わせてカスタマイズできます。法的契約、事業計画、科学レポートのいずれであっても、文書の目的や読者のアクセシビリティに合わせてウォーターマークをカスタマイズすることで、最適な統合とセキュリティを確保できます。"
      
  code_samples:
    # code sample loop
    - title: "PDF 画像ウォーターマークを生成"
      content: |
        PDF ドキュメント内にあるすべての画像に画像ウォーターマークを生成
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  PDF としてドキュメントをロード
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  PDF アノテーションに基づいてウォーターマークを作成
            const imageWatermark = new groupdocsWatermark.ImageWatermark("watermark.jpg");
            imageWatermark.setHorizontalAlignment(groupdocsWatermark.HorizontalAlignment.Center);
            imageWatermark.setVerticalAlignment(groupdocsWatermark.VerticalAlignment.Center);
            imageWatermark.setRotateAngle(-45);
            imageWatermark.setSizingType(groupdocsWatermark.SizingType.ScaleToParentDimensions);
            imageWatermark.setScaleFactor(1);
  
            //  ウォーターマークオプションを設定する
            const images = watermarker.getImages();
            for (let i = 0; i < images.getCount(); i++) {
                if (images.get_Item(i).getWidth() > 100 && images.get_Item(i).getHeight() > 100) {
                    images.get_Item(i).add(imageWatermark);
                }
            }

            //  結果文書にテキストウォーターマークを追加
            watermarker.save("result.pdf");
            watermarker.close();

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか?"
  description: "GroupDocs.Watermark の機能を無料で試すか、ライセンスをリクエストしてください"
  items:
    #  loop
    - title: "NPM ダウンロード"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      color: "red"
        #  loop
    - title: "ライセンス"
      link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Node.js を使用して PDF にウォーターマークを実装してください"
    exclude: "PDF"
    description: "Node.js を活用すると、法的コンテンツや公式コンテンツの保護に不可欠な PDF 件の文書にウォーターマークを動的に作成して適用できます。"
    items: 
        # format loop 1
        - name: "ウォーターマーク PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/generate//pdf/"
          description: "アドビ Portable ドキュメントフォーマット"

        # format loop 2
        - name: "ウォーターマーク Word"
          format: "WORD"
          link: "/watermark/nodejs-java/generate//word/"
          description: "MS Word とオープンオフィス文書"
          
        # format loop 3
        - name: "ウォーターマーク Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/generate//excel/"
          description: "MS Excel とオープンオフィススプレッドシート"

        # format loop 4
        - name: "ウォーターマーク画像"
          format: "IMAGE"
          link: "/watermark/nodejs-java/generate//image/"
          description: "人気の画像フォーマット"

        # format loop 5
        - name: "ウォーターマーク写真"
          format: "PHOTO"
          link: "/watermark/nodejs-java/generate//photo/"
          description: "写真フォーマット"

        # format loop 6
        - name: "ウォーターマーク PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/generate//powerpoint/"
          description: "MS PowerPoint とオープンオフィスプレゼンテーション"

        # format loop 7
        - name: "ウォーターマーク DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/generate//docx/"
          description: "マイクロソフト Word XML ドキュメントを開く"
          
        # format loop 8
        - name: "ウォーターマーク PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/generate//pptx/"
          description: "PowerPoint XML プレゼンテーションを開く"
          
        # format loop 9
        - name: "ウォーターマーク XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/generate//xlsx/"
          description: "マイクロソフト Excel オープン XML スプレッドシート"

        # format loop 10
        - name: "ウォーターマーク JPEG"
          format: "JPEG"
          link: "/watermark/nodejs-java/generate//jpeg/"
          description: "JPEG イメージ"

        # format loop 11
        - name: "ウォーターマーク PNG"
          format: "PNG"
          link: "/watermark/nodejs-java/generate//png/"
          description: "Portable ネットワークグラフィック"

        # format loop 12
        - name: "ウォーターマーク TIFF"
          format: "TIFF"
          link: "/watermark/nodejs-java/generate//tiff/"
          description: "タグ画像ファイル形式"

        # format loop 13
        - name: "ウォーターマーク WEBP"
          format: "WEBP"
          link: "/watermark/nodejs-java/generate//webp/"
          description: "ウェブ画像"

        # format loop 14
        - name: "ウォーターマーク DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/generate//doc/"
          description: "マイクロソフト Word 97-2007 ドキュメント"

        # format loop 15
        - name: "ウォーターマーク XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/generate//xls/"
          description: "マイクロソフト Excel ワークブック 97-2003"

        # format loop 16
        - name: "ウォーターマーク PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/generate//ppt/"
          description: "PowerPoint プレゼンテーション 97-2003"

        # format loop 17
        - name: "ウォーターマーク RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/generate//rtf/"
          description: "リッチテキスト形式"

---