
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:26:57
draft: false
lang: ja
format: Photo
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java で写真のウォーターマークをすばやく簡単に行えるようになりました"
head_description: "ウォーターマークで写真の保護を効率化しましょう。高速で信頼性が高い。"

############################# Header ############################
title: "写真透かし用の効率的な Java ツール" 
description: "Java APIを使用して、写真にウォーターマークをすばやく効率的に追加できます。最小限の労力でデジタル画像を保護し、ブランドの認知度を高めるのに最適です。"
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
       GroupDocs.Watermark for Java は、写真ファイルにすばやく効果的にウォーターマークを付けることができるように最適化されています。このツールを使用すると、JPEG、PNG、BMP など、さまざまな写真形式にテキストや画像のウォーターマークをすばやく統合できます。スタイル、透明度、配置の幅広いオプションを使用してウォーターマークをカスタマイズし、写真の品質を損なうことなくシームレスに溶け込むようにします。大量の処理に適しており、複数の写真にウォーターマークを一度に適用するバッチ処理をサポートしているため、ビジュアルアセットを効率的に保護してブランド化する必要がある企業やデジタルコンテンツクリエーターに最適です。

############################# Steps ############################
steps:
    enable: true
    title: "Java 経由で Photo ドキュメントにウォーターマークを追加"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** を使用すると、Java 開発者は一般的なビジネスファイル形式にさまざまなタイプのウォーターマークを簡単に追加できます。下記の簡単な手順で当社のライブラリをアプリケーションに追加し、ドキュメントにウォーターマークを付けてください。
      
      1. **ウォーターマーカー** です。文書処理の前にインスタンス化する必要があります。Photo ファイルをパスまたはストリームオブジェクトとしてコンストラクターに渡すことを忘れないでください。
      2. **Watermark** オブジェクトを作成することです。特定の文書ページだけでなく、添付ファイルやヘッダーなどのネイティブ文書パーツにも配置できます。
      3. 高さと幅、ページの配置 (上、左、中央など)、フォントファミリーと色などのウォーターマークプロパティを設定します。
      4. **Watermarker** メソッドを呼び出して、新しいウォーターマークを追加します。ウォーターマークは必要な数だけ追加できます。処理した文書は別の場所に保存することをお勧めします。
   
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

        // PHOTO にテキストウォーターマークを追加

        // ウォーターマークを付けるファイルをウォーターマーカーに渡す
        Watermarker watermarker = new Watermarker("input.png");
        
        // テキストウォーターマークの作成とプロパティの設定
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        watermark.setForegroundColor(Color.getRed());

        // ウォーターマーク付きファイルを保存
        watermarker.add(watermark);
        watermarker.save("output.png");
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "ウォーターマークを簡単に補正"
  description: "GroupDocs.Watermark の機能を活用して、複数のドキュメントフォーマットでウォーターマークを生成、作成、追加できます。この API は、文書のセキュリティを強化するだけでなく、用途が広く堅牢なカスタマイズ可能なウォーターマークを埋め込むことで知的財産を保護します。"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "ウォーターマークを追加"
  features:
    # feature loop
    - title: "多彩なウォーターマークオプション。"
      content: "GroupDocs.Watermark でさまざまなウォーターマークオプションを試してみてください。透明度や回転の調整からサイズの比例スケーリングまで、当社の API ではウォーターマークをニーズに合わせて正確にカスタマイズできるため、コンテンツの整合性を保ちながらドキュメントとシームレスに調和させることができます。"

    # feature loop
    - title: "高度なウォーターマークスタイリング。"
      content: "GroupDocs.Watermark を使用すると、ウォーターマークをさまざまなフォント、色、シャドウでスタイル設定できるため、ウォーターマークが目立つようになり、削除が難しくなります。ブランドのアイデンティティとプロ意識を反映したスタイリッシュなウォーターマークを使って、保護された文書や画像の美的魅力を高めましょう。"

    # feature loop
    - title: "ウォーターマークのタイリングと配置"
      content: "GroupDocs.Watermark を使用すると、ドキュメント全体にタイル効果を適用して、完全な保護を確保できます。ウォーターマークは、中央、コーナー、カスタム位置など、必要な場所に正確に配置できます。当社のフレキシブルなポジショニングオプションにより、不正使用や複製から文書を保護できます。"
      
  code_samples:
    # code sample loop
    - title: "PDF アノテーションウォーターマーク"
      content: |
        この例は、PDF ドキュメントにウォーターマーク注釈を追加する方法を示しています
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  PDF としてドキュメントをロード
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  PDF アノテーションに基づいてウォーターマークを作成
        PdfAnnotationWatermarkOptions options = new PdfAnnotationWatermarkOptions();
        TextWatermark textWatermark = new TextWatermark("Annotation watermark", new Font("Arial", 8));

        //  ウォーターマークオプションを設定する
        textWatermark.setHorizontalAlignment(HorizontalAlignment.Left);
        textWatermark.setVerticalAlignment(VerticalAlignment.Top);

        //  結果文書にテキストウォーターマークを追加
        watermarker.add(textWatermark, options);
        watermarker.save("result.pdf");

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
    title: "Java による写真の高速ウォーターマーク統合"
    exclude: "PHOTO"
    description: "Java APIを活用して写真にウォーターマークをすばやく適用し、セキュリティとブランドアイデンティティを強化します。自動化プロセスにより大量適用が可能になり、一貫性のあるプロフェッショナルな仕上がりが保証されます。"
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