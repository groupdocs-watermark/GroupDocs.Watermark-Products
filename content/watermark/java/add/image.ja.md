
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:26
draft: false
lang: ja
format: Image
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java で画像の効果的なウォーターマークを生成"
head_description: "Java を使って画像用の洗練されたウォーターマークを作成してください。文書を保護し、著作権を効果的に主張しましょう。"

############################# Header ############################
title: "Java で画像にシームレスに透かしを入れる" 
description: "Java を使用して画像ファイルに動的ウォーターマークを実装します。このツールを使用すると、ポジショニング、スケーラビリティ、透明性を正確に調整して、セキュリティとブランド認知度を高めることができます。"
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
       GroupDocs.Watermark for Java GroupDocs.Watermark for Java により、開発者は画像ファイルのウォーターマークを効果的に生成および管理できます。幅広い画像フォーマットをサポートしているため、位置、縮尺、透明度を自由にカスタマイズできるテキストウォーターマークとグラフィックウォーターマークの両方を実装できます。この機能は、ブランディングと著作権の完全性が最優先されるデジタルメディア、広告、オンラインコンテンツ配信のアプリケーションにとって非常に重要です。さらに、GroupDocs.Watermark には既存のウォーターマークを検索して削除する機能が含まれ、画像管理とセキュリティのための汎用性の高いツールとなっています。

############################# Steps ############################
steps:
    enable: true
    title: "Java 経由で Image ドキュメントにウォーターマークを追加します"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** を使用すると、Java の開発者は、一般的なビジネス ファイル形式にさまざまなタイプのウォーターマークを簡単に追加できます。以下に示すいくつかの簡単な手順で、ライブラリをアプリケーションに追加し、ドキュメントに透かしを入れます。
      
      1. API のメイン クラスは **Watermarker** です。ドキュメントを処理する前にインスタンス化する必要があります。 Image ファイルをパスまたはストリーム オブジェクトとしてコンストラクターに渡すことを忘れないでください。
      2. 次のステップでは、目的のタイプの **Watermark** オブジェクトを構築します。特定のドキュメント ページだけでなく、添付ファイルやヘッダーなどのネイティブ ドキュメント パーツにも配置できます。
      3. 高さと幅、ページ配置 (上、左、中央など)、フォント ファミリーと色、その他多くの透かしプロパティを設定します。
      4. **Watermarker** メソッドを呼び出して、新しいウォーターマークを追加します。必要なだけ透かしを追加できます。処理したドキュメントを別の場所に保存することをお勧めします。
   
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

        // テキストの透かしを IMAGE に追加します

        // 透かしを入れるファイルを Watermarker に渡します
        Watermarker watermarker = new Watermarker("input.JPEG");
        
        // テキストの透かしを作成し、プロパティを設定する
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        watermark.setForegroundColor(Color.getRed());

        // 透かし入りファイルを保存する
        watermarker.add(watermark);
        watermarker.save("output.JPEG");
        
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
    title: "Java のウォーターマークでセキュリティ画像を効率化"
    exclude: "IMAGE"
    description: "当社の Java ツールキットを使用すると、あらゆる画像形式に合わせてパーソナライズされたウォーターマークを生成でき、セキュリティとブランディングを強化できます。ウォーターマークをカスタマイズすることで、さまざまなメディアでビジュアルが認識され、保護されます。"
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