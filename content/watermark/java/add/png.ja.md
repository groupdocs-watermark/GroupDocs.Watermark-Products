
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:21
draft: false
lang: ja
format: Png
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java PNG ファイルの PNG ウォーターマークソリューション"
head_description: "Java を使用して PNG 枚の画像に動的ウォーターマークを適用して、デジタル資産を保護および認証します。"

############################# Header ############################
title: "Java で PNG を保護してカスタマイズしましょう" 
description: "Java を利用して、安全で適応性のあるウォーターマークを PNG ファイルに埋め込んでください。クリエイティブな作品を保護したい写真家やデザイナーに最適です。"
subtitle: "GroupDocs.Watermark for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Maven で無料でダウンロード"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java"
    link: "/watermark/java/"
    link_title: "さらに詳しく"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java は Java 人の開発者に PNG 枚の画像にウォーターマークを適用するための高度なフレームワークを提供します。この API は Java ベースのアプリケーションにシームレスに統合できるように設計されており、基になる画像と完全に調和する透明または不透明なウォーターマークを挿入できます。ウォーターマークをテキスト、ロゴ、または著作権記号でカスタマイズすると、画質を損なうことなくセキュリティを強化できます。GroupDocs.Watermark は、ピクセルパーフェクトなポジショニングや不透明度制御などの機能により、画像が視覚的に魅力的であると同時に法的に保護されていることを保証します。電子商取引サイトやオンラインポートフォリオなどでの使用に適しており、Java 8 以降と完全に互換性があります。

############################# Steps ############################
steps:
    enable: true
    title: "高度なテクニック: Java 経由で Png ドキュメントにウォーターマークを追加する"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** を使用して、Png ドキュメントの高度な透かし技術を探索する
      
      1. **Watermarker** クラスを初期化して、透かしプロセスを開始します。この基本的な手順により、Png ドキュメントをウォーターマークで強化するための準備が整います。 Png ファイルをパスまたはストリーム オブジェクトとしてコンストラクターに提供します。
      2. 仕様に合わせて **Watermark** オブジェクトを作成して、次のレベルに進みます。これらの多用途エンティティは、指定されたドキュメント ページだけでなく、添付ファイルやヘッダーなどのネイティブ要素内にも正確に配置できます。
      3. 寸法、配置、フォント スタイル、色などのプロパティを微調整して、透かしプロセスを改良します。このレベルのカスタマイズにより、文書の美しさを完全に補完する透かしを作成できるようになります。
      4. **Watermarker** メソッドを使用して、新しく作成したウォーターマークをドキュメントに適用します。要件に応じて複数の透かしを柔軟に追加できます。ドキュメントを保存するには、安全な場所に保存することを検討してください。
   
    code:
      platform: "net"
      copy_title: "[コピー]"
      install:
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-watermark</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "クリックしてコピー"
        copy_done: "コピーされました"
      links:
        #  loop
        - title: "その他の例"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
        #  loop
        - title: "ドキュメンテーション"
          link: "https://docs.groupdocs.com/watermark/java/"
          
      content: |
        ```java {style=abap}
        // 画像の透かしを PNG に追加します

        // 透かしを入れるファイルを Watermarker に渡します
        Watermarker watermarker = new Watermarker("input.png");
        
        // 透かしのある画像へのパスを提供します
        ImageWatermark watermark = new ImageWatermark("watermark.png");

        // 結果を保存する
        watermarker.add(watermark);
        watermarker.save("output.png");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ドキュメントウォーターマークのマスタリング"
  description: ".NET 人の開発者向けにカスタマイズされた高度なウォーターマークAPIで文書管理を強化しましょう。このツールでは、さまざまな文書フォーマットでウォーターマークを適用、カスタマイズ、管理するための包括的なソリューションが提供され、美的美的魅力とセキュリティ強化の両方を実現できます。"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "高度なドキュメントウォーターマーキング"
  features:
    # feature loop
    - title: "フレキシブルなウォーターマークローテーション"
      content: "柔軟な回転設定により、ウォーターマークを文書のどの向きにも合うように調整できます。文書が縦向きでも横向きでも、透かしの角度を簡単に調整して、文書のレイアウトに合う一貫した外観を保つことができます。"

    # feature loop
    - title: "パーフェクトな透明度コントロール"
      content: "透かしの透明度を正確に制御できるため、文書の内容を圧迫することなく、繊細ながらも安全なマーキングが可能になります。この機能は、セキュリティを強化しながら文書本来の美しさを保つのに理想的です。"

    # feature loop
    - title: "強調用のシャドウエフェクト"
      content: "カスタマイズ可能なシャドウ効果を使用して、透かしの視認性を高めたり、文書に微妙に組み込んだりできます。この機能により、さまざまなぼかし、広がり、色の影が可能になり、必要に応じて透かしをより際立たせたり、目立たなくしたりできます。"
      
  code_samples:
    # code sample loop
    - title: "MS Word ロックされたウォーターマーク"
      content: |
        この例は、DOCX 全ページのウォーターマークをロックする方法を示しています
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  ドキュメントを MS Word docとしてロード
        WordProcessingLoadOptions loadOptions = new WordProcessingLoadOptions();
        Watermarker watermarker = new Watermarker("source.docx", loadOptions);

        //  ウォーターマークの作成
        TextWatermark watermark = new TextWatermark("Watermark text", new Font("Arial", 19));
        watermark.setForegroundColor(Color.getRed());

        //  ネイティブ Word オプションのチューニング
        WordProcessingWatermarkPagesOptions options = new WordProcessingWatermarkPagesOptions();
        options.setLocked(true);
        options.setLockType(WordProcessingLockType.AllowOnlyFormFields);

        //  結果文書ページへのウォーターマークの追加
        watermarker.add(textWatermark, options);
        watermarker.save("result.docx");
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか?"
  description: "GroupDocs.Watermark の機能を無料で試すか、ライセンスをリクエストしてください"
  items:
    #  loop
    - title: "Maven ダウンロード"
      link: "https://releases.groupdocs.com/watermark/java/"
      color: "red"
        #  loop
    - title: "ライセンス"
      link: "https://purchase.groupdocs.com/pricing/watermark/java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Java による PNG イメージセキュリティの強化"
    exclude: "PNG"
    description: "Java を使用して PNG ファイルに堅牢なウォーターマークを埋め込みます。この機能は、画像の鮮明さを保ちながら、ビジュアルコンテンツを不正使用から保護するために不可欠です。"
    items: 
        # format loop 1
        - name: "ウォーターマーク PDF"
          format: "PDF"
          link: "/watermark/java/add//pdf/"
          description: "アドビ Portable ドキュメントフォーマット"

        # format loop 2
        - name: "ウォーターマーク Word"
          format: "WORD"
          link: "/watermark/java/add//word/"
          description: "MS Word とオープンオフィス文書"
          
        # format loop 3
        - name: "ウォーターマーク Excel"
          format: "EXCEL"
          link: "/watermark/java/add//excel/"
          description: "MS Excel とオープンオフィススプレッドシート"

        # format loop 4
        - name: "ウォーターマーク画像"
          format: "IMAGE"
          link: "/watermark/java/add//image/"
          description: "人気の画像フォーマット"

        # format loop 5
        - name: "ウォーターマーク写真"
          format: "PHOTO"
          link: "/watermark/java/add//photo/"
          description: "写真フォーマット"

        # format loop 6
        - name: "ウォーターマーク PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/add//powerpoint/"
          description: "MS PowerPoint とオープンオフィスプレゼンテーション"

        # format loop 7
        - name: "ウォーターマーク DOCX"
          format: "DOCX"
          link: "/watermark/java/add//docx/"
          description: "マイクロソフト Word XML ドキュメントを開く"
          
        # format loop 8
        - name: "ウォーターマーク PPTX"
          format: "PPTX"
          link: "/watermark/java/add//pptx/"
          description: "PowerPoint XML プレゼンテーションを開く"
          
        # format loop 9
        - name: "ウォーターマーク XLSX"
          format: "XLSX"
          link: "/watermark/java/add//xlsx/"
          description: "マイクロソフト Excel オープン XML スプレッドシート"

        # format loop 10
        - name: "ウォーターマーク JPEG"
          format: "JPEG"
          link: "/watermark/java/add//jpeg/"
          description: "JPEG イメージ"

        # format loop 11
        - name: "ウォーターマーク PNG"
          format: "PNG"
          link: "/watermark/java/add//png/"
          description: "Portable ネットワークグラフィック"

        # format loop 12
        - name: "ウォーターマーク TIFF"
          format: "TIFF"
          link: "/watermark/java/add//tiff/"
          description: "タグ画像ファイル形式"

        # format loop 13
        - name: "ウォーターマーク WEBP"
          format: "WEBP"
          link: "/watermark/java/add//webp/"
          description: "ウェブ画像"

        # format loop 14
        - name: "ウォーターマーク DOC"
          format: "DOC"
          link: "/watermark/java/add//doc/"
          description: "マイクロソフト Word 97-2007 ドキュメント"

        # format loop 15
        - name: "ウォーターマーク XLS"
          format: "XLS"
          link: "/watermark/java/add//xls/"
          description: "マイクロソフト Excel ワークブック 97-2003"

        # format loop 16
        - name: "ウォーターマーク PPT"
          format: "PPT"
          link: "/watermark/java/add//ppt/"
          description: "PowerPoint プレゼンテーション 97-2003"

        # format loop 17
        - name: "ウォーターマーク RTF"
          format: "RTF"
          link: "/watermark/java/add//rtf/"
          description: "リッチテキスト形式"

---