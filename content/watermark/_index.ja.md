---
############################# Static ############################
layout: "family"
date:  2024-07-08T15:37:04
draft: false

product: "Watermark"
product_tag: "watermark"

lang: ja

############################# Head ############################
head_title: "ドキュメントのウォーターマーク C# Java Node.js Python |透かしを追加する"
head_description: "PDF、画像、文書にウォーターマークを追加します。Microsoft Office、PDF、OpenDocument、画像などのウォーターマークソリューション"

############################# Header ############################
title: "ドキュメントウォーターマークソリューション"
description:  |
  文書や画像にテキストや画像の透かしを追加します。

  便利な方法でドキュメントのウォーターマークを検索して変更します。

  ドキュメントに表示されるウォーターマークに関する情報を取得します。

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "プラットフォームを選択してください"
  title: "プラットフォーム独立性"
  description: "GroupDocs.Watermark ライブラリは、以下のオペレーティングシステムとフレームワークをサポートしています。"
  details_link_title: "さらに詳しく"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Watermark .NET 
      color: "blue"
      tag: "net"
      link: "/watermark/net/"
      features_link: "https://docs.groupdocs.com/watermark/net/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    .NET Framework 4.5 or higher <br> .NET Core 3.0 or higher <br> .NET 5.0 or higher
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Watermark Java
      color: "red"
      tag: "java"
      link: "/watermark/java/"
      features_link: "https://docs.groupdocs.com/watermark/java/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    Java 8 or higher <br> Kotlin
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Watermark Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/watermark/nodejs-java/"
      features_link: "https://docs.groupdocs.com/watermark/"
      features:
          # features loop
          - rows: "4"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> その他のテキストエディター
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Python"
      description: GroupDocs.Watermark Python
      color: "yellow"
      tag: "python-net"
      link: "/watermark/python-net/"
      features_link: "https://docs.groupdocs.com/watermark/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Python 3.9+ and .Net 6+
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "4"
            content: |
                    IDLE <br> PyCharm <br> Visual Studio Code
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Watermark 機能レビュー"
  description: "このライブラリは、一般的なドキュメント形式のさまざまなウォーターマークタイプを追加、検索、更新できるように設計されています。"

  items:
    # items loop
    - icon: "protect"
      title: "ウォーターマークでファイルを保護する"
      content: "ビジネス文書にテキストと画像のウォーターマークを追加します。"

    # items loop
    - icon: "search"
      title: "既存のウォーターマークを検索する"
      content: "以前にドキュメントに配置されたウォーターマークに関する詳細情報を取得します。"

    # items loop
    - icon: "manipulate"
      title: "ドキュメントウォーターマークの操作"
      content: "テキスト、スタイル、画像、その他のウォーターマーク機能を制御します。"

    # items loop
    - icon: "additional"
      title: "さまざまな追加機能"
      content: "ドキュメント情報の取得、ハイパーリンクやページの背景の更新など"

############################# Code samples ############################
code_samples:
  enable: true
  title: "ウォーターマークで文書を保護"
  description: "GroupDocs.Watermark 一般的な操作コードの例。"
  items:
    # code sample loop
    - title: "ウォーターマークの作成。"
      content: |
       "ドキュメントにウォーターマークを追加するには、ターゲットファイルへのパスを指定します。特定のページにカスタマイズしたウォーターマークを適用するには、さまざまな選択肢があります。"
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // 透かしを入れる文書を指定してください
            using (Watermarker watermarker = new Watermarker("source.docx"))
            {
                // ウォーターマークオブジェクトを作成
                TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                // ウォーターマークオプションを設定する
                watermark.ForegroundColor = Color.Red;
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;

                // ウォーターマークを追加して処理済みファイルを保存する
                watermarker.Add(watermark);
                watermarker.Save("result.docx");

            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // 透かしを入れる文書を指定してください
            Watermarker watermarker = new Watermarker("source.docx");

            // ウォーターマークオブジェクトを作成
            TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

            // ウォーターマークオプションを設定する
            watermark.setForegroundColor(Color.getRed());
            watermark.setHorizontalAlignment(HorizontalAlignment.Center);
            watermark.setVerticalAlignment(VerticalAlignment.Center);

            // ウォーターマークを追加して処理済みファイルを保存する
            watermarker.add(watermark);
            watermarker.save("result.docx");
            watermarker.close();
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            // 透かしを入れる文書を指定してください
            const watermarker = new Watermarker("source.docx");

            // ウォーターマークオブジェクトを作成
            const watermark = new TextWatermark("top secret", new Font("Arial", 36));

            // ウォーターマークオプションを設定する
            watermark.setForegroundColor(Color.getRed());
            watermark.setHorizontalAlignment(HorizontalAlignment.Center);
            watermark.setVerticalAlignment(VerticalAlignment.Center);

            // ウォーターマークを追加して処理済みファイルを保存する
            watermarker.add(watermark);
            watermarker.save("result.docx");
            ```
        - language: "Python"
          color: "yellow"
          content: |
            ```python {style=abap}  
            def run():
                # 透かしを入れる文書を指定してください
                with groupdocs.watermark.Watermarker("source.docx") as watermarker:
                    font = groupdocs.watermark.watermarks.Font("Arial", 36.0)

                    # ウォーターマークオブジェクトを作成
                    watermark = groupdocs.watermark.watermarks.TextWatermark("top secret", font)

                    # ウォーターマークオプションを設定する
                    watermark.foreground_color = groupdocs.watermark.watermarks.Color.red;
                    watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
                    watermark.vertical_alignment = groupdocs.watermark.common.VerticalAlignment.CENTER

                    # ウォーターマークを追加して処理済みファイルを保存する
                    watermarker.add(watermark)
                    watermarker.save("result.docx")
            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "50種類以上のファイルフォーマットに対応"
  description: "GroupDocs.Watermark は、一般的なドキュメントおよびファイル形式にウォーターマークを提供します。"

############################# Metrics ###############################
metrics:
  enable: true
  title: "当館統計データ"
  description: "主要な指標を深く掘り下げて、当社の業績、影響、成長に関する洞察を明らかにしてください。"

  items:
    # items loop
    - number: "50+"
      title: "対応フォーマット"
      content: "ライブラリは、50種類以上の最も一般的なファイル形式を処理できます。"

    # items loop
    - number: "500k"
      title: "NuGet ダウンロード"
      content: ".NET の GroupDocs.Watermark は NuGet で50万回以上ダウンロードされている人気のライブラリです。"

    # items loop
    - number: "15k"
      title: "Maven のダウンロード"
      content: "Mavenでのダウンロード数は15,000を超え、GroupDocs.Watermark は Java 人の開発者に人気があります。"

    # items loop
    - number: "140+"
      title: "幸せな顧客"
      content: "世界中の個人開発者やトップ企業が、革新的なソリューションを構築するために私たちのライブラリを好んでいます。"


############################# Customers ###############################
customers:
  enable: true
  title: "私たちの幸せな顧客"
  description: "GroupDocs の図書館は、世界中の世界的に有名で著名なブランドに採用されています。"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "始める準備はできましたか?"
  description: "お使いのプラットフォームで GroupDocs.Watermark の機能を無料でお試しください"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/watermark/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/watermark/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/watermark/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "よく寄せられる質問"
  description: "よくある質問をご覧ください"

  items:
    # items loop
    - question: "GroupDocs.Watermark は文書操作に外部ライブラリを必要としていますか？"
      answer: "GroupDocs.Watermark は独立して動作するため、Adobe Acrobat、Microsoft Office などのサードパーティ製ソフトウェアは必要ありません。"

    # items loop
    - question: "購入前に GroupDocs.Watermark 個の機能をテストできますか？"
      answer: "はい、GroupDocs.Watermark は無料トライアルを提供しています！インストールして試してみてください。ただし、試用版では文書に「トライアルバッジ」が追加され、最初の 3 ページのみが処理されることに注意してください。すべての体験をしてみたいですか？すべての機能を利用するには、30 日間無料の一時ライセンスを入手してください。詳細は [一時ライセンス](https://purchase.groupdocs.com/temporary-license/) をご覧ください。"

    # items loop
    - question: "どのような種類のライセンスが提供されていますか?"
      answer: "GroupDocs.Watermark ライセンスが必要ですか?選択肢があります！さまざまなオプションからライセンスを選択できます。チーム内の開発者の数。1 つのオフィスやリモートワークプレイスなどの導入場所。エンドカスタマーディストリビューションでは SDK/API をクライアントと共有する必要がありますか?また、月単位の使用ライセンスもあります。従量制プランでは、使用した分のみお支払いいただきます。さらに掘り下げて、最適な [価格](https://purchase.groupdocs.com/pricing/watermark/net/) を見つけてください。"

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Watermark ローコード API"
  description: "クラウドベースの REST API を使用して、アプリケーションでファイルにウォーターマークを追加します。"
  
  items:
    # items loop
    - title: "GroupDocs.Watermark Cloud for cURL"
      content: "cURL REST ful API を使用して、PDF、Word、Excel、PowerPoint、JPEG などの一般的なファイル形式にウォーターマークを付けます。"
      icon: "groupdocs_watermark-for-curl"
      link: "https://products.groupdocs.cloud/watermark/curl"

    # items loop
    - title: "GroupDocs.Watermark Cloud for .NET"
      content: ".NET 用のCloud SDKによるドキュメントウォーターマーク機能で .NET 個のアプリケーションを強化します。ビジネス文書はご自身で保護してください。"
      icon: "groupdocs_watermark-for-net"
      link: "https://products.groupdocs.cloud/watermark/net"

    # items loop
    - title: "GroupDocs.Watermark Cloud for Java"
      content: "Java 向けに設計された GroupDocs.Watermark SDKは、Java 個のアプリケーションとビジネスファイルに新しい可能性をもたらします。"
      icon: "groupdocs_watermark-for-java"
      link: "https://products.groupdocs.cloud/watermark/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Watermark ウェブアプリ"
  description: "GroupDocs は、ドキュメントにウォーターマークを追加するためのウェブアプリケーションへのアクセスを許可します。50 種類以上の一般的なファイル形式に、お好きなブラウザで無料で透かしを入れることができます。"

  items:
    # items loop
    - title: "GroupDocs.Watermark Total"
      content: "どのデバイスからでもドキュメントにウォーターマークを追加できるオンラインツール。"
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/watermark/total"

    # items loop
    - title: "GroupDocs.Watermark DOCX"
      content: "ウォーターマーク MS Word DOCX オンライン。"
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/watermark/docx"

    # items loop
    - title: "GroupDocs.Watermark PDF"
      content: "PDF 件の文書をオンラインで保護します。"
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/watermark/pdf"


      


---