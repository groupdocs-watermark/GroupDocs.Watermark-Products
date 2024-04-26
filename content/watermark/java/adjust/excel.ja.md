
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:57
draft: false
lang: ja
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Excel ウォーターマーク調整ツール-GroupDocs.Watermark"
head_description: "GroupDocs.Watermark を使用すると、ウォーターマークを簡単に調整、更新、管理できます。文書を簡単にカスタマイズできます。"

############################# Header ############################
title: "スプレッドシートのウォーターマーク調整ツール:非常にシンプル" 
description: "直感的なウォーターマーク編集ツールで文書の質を高めましょう。ワークフローを簡単に簡素化できます。"
subtitle: "GroupDocs.Watermark for Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料 Maven ダウンロード"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java API"
    link: "/watermark/java/"
    link_title: "さらに詳しく"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **ウォーターマーク調整ツール**: 当社のウォーターマークツールは、ドキュメントを強化および保護するための使いやすいソリューションを提供します。直感的な編集機能により、ウォーターマークの管理が簡単になり、文書のセキュリティと信頼性が確保されます。

############################# Steps ############################
steps:
    enable: true
    title: "Excel ドキュメントのウォーターマークを Java で調整"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** では、Java 人の開発者がいくつかの簡単な手順を実行することで、アプリケーションのテキストウォーターマークを簡単に調整できます。
      
      1. **Watermarker**というAPIのメインオブジェクトにロードします。さらに処理するためのファイルを、ストリームまたはローカルディスク上のパスとして提供できます。
      2. **SearchCriteria** は、以前に文書に追加されたウォーターマークを適切なプロパティで識別するのに役立ちます。
      3. **検索**手順の結果として、適切なウォーターマークのリストを取得します。サイズ、ページの配置、テキスト、色、画像の内容など、見つかったウォーターマークのプロパティを調整するデータをカスタマイズする方法はたくさんあります。
      4. ウォーターマーク調整処理が完了したら、更新した文書を保存する必要があります。ローカルファイルパス、ファイル、またはバイトストリームを使用して結果を保存します。
   
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

        // EXCEL のテキストウォーターマークを調整

        // 入力 EXCEL ドキュメントでウォーターマーカーをインスタンス化
        Watermarker watermarker = new Watermarker("input.xslx");

        // テキスト検索条件を初期化し、テキストウォーターマークを検索する
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        
        // テキストウォーターマークのプロパティを調整
        for (PossibleWatermark watermark : watermarks)
        {
            watermark.getFormattedTextFragments().clear();
            watermark.getFormattedTextFragments().
                add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
        }

        // 更新した文書を保存する
        watermarker.save("output.xslx");
        
        ```            
        
############################# More features ############################
more_features:
  enable: true
  title: "EXCEL ウォーターマーク調整の詳細"
  description: "当社のAPIにより、Java 個のアプリケーションで、一般的なドキュメント形式のウォーターマークを追加、編集、削除、検索できます。"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "ウォーターマークを調整"
  features:
    # feature loop
    - title: "ドキュメントに簡単にウォーターマークを付ける"
      content: "GroupDocs.Watermark は Java 開発者のウォーターマークを簡素化します。さまざまなビジネス文書やファイルにさまざまなウォーターマークを追加できます。ウォーターマークを適用できるだけでなく、既存のウォーターマークを更新したり削除したりすることもできます。"

    # feature loop
    - title: "ウォーターマークをニーズに合わせてカスタマイズ"
      content: "当社の API は広範なカスタマイズオプションを提供します。サイズ、回転、色、フォント、スタイルなどを簡単に調整して、完璧なウォーターマークを作成できます。"

    # feature loop
    - title: "EXCEL のネイティブドキュメント機能を使用"
      content: "特定の文書形式によっては、ネイティブ機能を利用できます。これらには、ウォーターマークコンテナとしての文書ページの背景、注釈、ヘッダー、またはその他のオブジェクトが含まれる場合があります。"
      
  code_samples:
    # code sample loop
    - title: "PDF テキストウォーターマークの調整"
      content: |
        この例は、特定のアーティファクトのテキストを調整する方法を示しています。
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  PDF ドキュメントをロード
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  ドキュメントコンテンツを取得
        PdfContent pdfContent = watermarker.getContent(PdfContent.class);

        //  特定のウォーターマークテキストを調整
        for (PdfArtifact artifact : pdfContent.getPages().get_Item(0).getArtifacts())
        {
            if (artifact.getText().contains("Test"))
            {
                artifact.setText("Passed");
            }
        }

        //  文書を保存する
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
    title: "他の形式のウォーターマークを GroupDocs.Watermark for Java で調整"
    exclude: "EXCEL"
    description: "さまざまなドキュメント形式のウォーターマークを簡単にカスタマイズできます。文書のセキュリティと信頼性を簡単に強化できます。"
    items: 
        # format loop 1
        - name: "ウォーターマーク PDF"
          format: "PDF"
          link: "/watermark/java/adjust//pdf/"
          description: "アドビ Portable ドキュメントフォーマット"

        # format loop 2
        - name: "ウォーターマーク Word"
          format: "WORD"
          link: "/watermark/java/adjust//word/"
          description: "MS Word とオープンオフィス文書"
          
        # format loop 3
        - name: "ウォーターマーク Excel"
          format: "EXCEL"
          link: "/watermark/java/adjust//excel/"
          description: "MS Excel とオープンオフィススプレッドシート"

        # format loop 4
        - name: "ウォーターマーク PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/adjust//powerpoint/"
          description: "MS PowerPoint とオープンオフィスプレゼンテーション"

        # format loop 5
        - name: "ウォーターマーク DOCX"
          format: "DOCX"
          link: "/watermark/java/adjust//docx/"
          description: "マイクロソフト Word XML ドキュメントを開く"
          
        # format loop 6
        - name: "ウォーターマーク PPTX"
          format: "PPTX"
          link: "/watermark/java/adjust//pptx/"
          description: "PowerPoint XML プレゼンテーションを開く"
          
        # format loop 7
        - name: "ウォーターマーク XLSX"
          format: "XLSX"
          link: "/watermark/java/adjust//xlsx/"
          description: "マイクロソフト Excel オープン XML スプレッドシート"

        # format loop 8
        - name: "ウォーターマーク DOC"
          format: "DOC"
          link: "/watermark/java/adjust//doc/"
          description: "マイクロソフト Word 97-2007 ドキュメント"

        # format loop 9
        - name: "ウォーターマーク XLS"
          format: "XLS"
          link: "/watermark/java/adjust//xls/"
          description: "マイクロソフト Excel ワークブック 97-2003"

        # format loop 10
        - name: "ウォーターマーク PPT"
          format: "PPT"
          link: "/watermark/java/adjust//ppt/"
          description: "PowerPoint プレゼンテーション 97-2003"

        # format loop 11
        - name: "ウォーターマーク RTF"
          format: "RTF"
          link: "/watermark/java/adjust//rtf/"
          description: "リッチテキスト形式"

---