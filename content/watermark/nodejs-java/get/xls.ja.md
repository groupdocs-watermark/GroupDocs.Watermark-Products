
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:27:12
draft: false
lang: ja
format: Xls
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "どの XLS 文書からでも簡単にウォーターマークを取得"
head_description: "GroupDocs.Watermark で XLS スプレッドシートからウォーターマークをすばやく取得できます。"

############################# Header ############################
title: "XLS スプレッドシートへのアクセスとウォーターマークの取得" 
description: "GroupDocs.Watermark for Node.js via Java を使用すると、XLS ドキュメント内のウォーターマークを簡単に取得して取得できます。"
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "NPM で GroupDocs.Watermark for Node.js via Java を無料でゲット"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java でパワフルなウォーターマーク管理をアンロック"
    link: "/watermark/nodejs-java/"
    link_title: "さらに詳しく"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       Node.js via Java ワークフロー内のウォーターマーク管理に革命をもたらします。GroupDocs.Watermark for Node.js via Java を使用すると、さまざまなファイル形式のウォーターマークを簡単に生成、更新、取得 (取得)、削除できるため、ドキュメント処理が合理化されます。

############################# Steps ############################
steps:
    enable: true
    title: "GroupDocs.Watermark を使用して Xls ファイルからウォーターマークを取得"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)**は、一般的なビジネス文書形式にウォーターマークを付けるための包括的なソリューションを提供します。当社のライブラリを Node.js via Java アプリケーションに統合することで、強力なウォーターマーク検索機能を搭載できます。
      
      1. **Watermarker** クラスをインスタンス化し、Xls ファイルパスを指定します。また、バイトストリームとして保存されたファイルを使用することもできます。このアクションでは、基本的にターゲットドキュメントが読み込まれ、包括的なウォーターマーク分析が可能になります。
      2. **SearchCriteria** オブジェクトを作成します。画像を指定して類似の画像ウォーターマークを検索できます。また、テキストウォーターマークの場合は、テキストコンテンツ、フォントプロパティ、色属性、その他の関連パラメーターを定義して検索条件を絞り込み、より正確な結果を得ることもできます。
      3. **Watermarker**オブジェクトの**Get**メソッド (または同様の命名規則) を呼び出して、ロードされたドキュメント内でウォーターマーク取得プロセスを開始します。この関数はウォーターマークになりそうなオブジェクトのコレクションを返すので、特定の要件に基づいてさらに処理を進めることができます。
      4. ウォーターマークの結果コレクションでは、ドキュメント内で識別されるウォーターマークを制御できます。不要なウォーターマークを削除したり、必要に応じてウォーターマークのサイズ、位置、テキストの内容を調整するなど、ウォーターマークのプロパティを動的に変更したりできます。
   
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

        // XLS に配置された画像のウォーターマークを取得

        // ソースパスを持つウォーターマーカーオブジェクトを作成
        const watermarker = new groupdocs.watermark.Watermarker("input.xls");
        
        // 類似の画像ハッシュでウォーターマークを取得
        const imageSearchCriteria = 
            new groupdocs.watermark.ImageDctHashSearchCriteria("watermark.jpg");
        imageSearchCriteria.setMaxDifference(0.9);
        const possibleWatermarks = watermarker.search(imageSearchCriteria);

        // ウォーターマークを好きなように処理
        console.log(`Found ${possibleWatermarks.getCount()} possible watermark(s).`);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "GroupDocs.Watermark でのウォーターマーク検索に Node.js を活用してください"
  description: "Node.js via Java プラットフォーム内の GroupDocs.Watermark を使用して、Node.js アプリケーションに動的で効率的なウォーターマーク検索機能を実装します。"
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "Node.js ウォーターマーク検索"
  features:
    # feature loop
    - title: "フレキシブルウォーターマーク検索のための Node.js API"
      content: "Node.js と GroupDocs.Watermark の柔軟性を活用して、複数のドキュメント形式のウォーターマークを検索できます。サイズ、タイプ、内容などの特定の要件に合わせて簡単に検索を設定できます。"

    # feature loop
    - title: "Node.js によるウォーターマーク識別の強化"
      content: "Node.js を使用してウォーターマークを正確に識別することで、文書処理を改善できます。GroupDocs.Watermark の API を利用すると、複雑な文書構造内でもウォーターマークを検出できます。"

    # feature loop
    - title: "スケーラブルなウォーターマーク検索ソリューション"
      content: "Node.js を使用してドキュメントセキュリティソリューションを拡張してください。GroupDocs.Watermark は大規模なドキュメントバッチを効率的に処理できるため、エンタープライズレベルのアプリケーションに最適です。"
      
  code_samples:
    # code sample loop
    - title: "Node.js の例:ウォーターマークの検索と取得"
      content: |
        この Node.js の例は、GroupDocs.Watermark を使用してウォーターマークを検索および取得する方法を示し、効率的でスケーラブルな検索操作を示しています。
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            const files = ["source.docx", "source.xlsx", "source.pptx", "source.vsdx"];
            for (const file of files) {
                //  Node.js 環境をセットアップし、必要なドキュメントをロードします
                const settings = new groupdocsWatermark.WatermarkerSettings();
                settings.setSearchableObjects(new groupdocsWatermark.SearchableObjects());
                settings.getSearchableObjects().setWordProcessingSearchableObjects(
                    groupdocsWatermark.WordProcessingSearchableObjects.Hyperlinks | 
                    groupdocsWatermark.WordProcessingSearchableObjects.Text
                );
                settings.getSearchableObjects().setSpreadsheetSearchableObjects(
                    groupdocsWatermark.SpreadsheetSearchableObjects.HeadersFooters
                );
                settings.getSearchableObjects().setPresentationSearchableObjects(
                    groupdocsWatermark.PresentationSearchableObjects.SlidesBackgrounds |
                    groupdocsWatermark.PresentationSearchableObjects.Shapes
                );
                settings.getSearchableObjects().setDiagramSearchableObjects(groupdocsWatermark.DiagramSearchableObjects.None);
                settings.getSearchableObjects().setPdfSearchableObjects(groupdocsWatermark.PdfSearchableObjects.All);

                //  さまざまな基準に基づいてウォーターマークを識別するように検索を設定します
                const watermarker = new groupdocsWatermark.Watermarker(file, settings);

                //  ウォーターマーク検索を実行し、特定されたウォーターマークに関するデータを収集します
                const watermarks = watermarker.search();

                //  結果を処理して、ビジネスニーズに応じてウォーターマークを変更または削除します。
                console.log(`In ${documentPath} found ${watermarks.getCount()} possible watermark(s).`);
                watermarker.close();
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
    title: "どのファイル形式からでも簡単にウォーターマークを取得"
    exclude: "XLS"
    description: "GroupDocs.Watermark for Node.js via Java の機能により、あらゆるファイル形式のウォーターマークの取得（取得）が簡単になります。"
    items: 
        # format loop 1
        - name: "ウォーターマーク PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/get//pdf/"
          description: "アドビ Portable ドキュメントフォーマット"

        # format loop 2
        - name: "ウォーターマーク Word"
          format: "WORD"
          link: "/watermark/nodejs-java/get//word/"
          description: "MS Word とオープンオフィス文書"
          
        # format loop 3
        - name: "ウォーターマーク Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/get//excel/"
          description: "MS Excel とオープンオフィススプレッドシート"

        # format loop 4
        - name: "ウォーターマーク PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/get//powerpoint/"
          description: "MS PowerPoint とオープンオフィスプレゼンテーション"

        # format loop 5
        - name: "ウォーターマーク DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/get//docx/"
          description: "マイクロソフト Word XML ドキュメントを開く"
          
        # format loop 6
        - name: "ウォーターマーク PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/get//pptx/"
          description: "PowerPoint XML プレゼンテーションを開く"
          
        # format loop 7
        - name: "ウォーターマーク XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/get//xlsx/"
          description: "マイクロソフト Excel オープン XML スプレッドシート"

        # format loop 8
        - name: "ウォーターマーク DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/get//doc/"
          description: "マイクロソフト Word 97-2007 ドキュメント"

        # format loop 9
        - name: "ウォーターマーク XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/get//xls/"
          description: "マイクロソフト Excel ワークブック 97-2003"

        # format loop 10
        - name: "ウォーターマーク PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/get//ppt/"
          description: "PowerPoint プレゼンテーション 97-2003"

        # format loop 11
        - name: "ウォーターマーク RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/get//rtf/"
          description: "リッチテキスト形式"

---