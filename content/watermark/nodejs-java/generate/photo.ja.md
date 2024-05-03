
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:07
draft: false
lang: ja
format: Photo
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Node.js の高度なウォーターマーク機能で写真を保護しましょう"
head_description: "Node.js で写真の透かし処理をスピードアップしましょう。迅速で使いやすいコーディングソリューションを実装できます。"

############################# Header ############################
title: "Node.js via Java の高度なウォーターマークで写真を保護する" 
description: "Node.js を使用して、写真処理ワークフローに高度なウォーターマーク戦略を導入しましょう。当社のツールキットは JPG、PNG、および WEBP 画像ファイルの広範なカスタマイズをサポートしています。"
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
       GroupDocs.Watermark for Node.js via Java では、高度なウォーターマークを使用して写真を保護するのが簡単かつ柔軟に行えます。この API では、テキストベースまたは画像ベースのウォーターマークをすばやく適用できます。ウォーターマークは、基になる写真の美観に合わせてカスタマイズできます。さまざまな画像形式をサポートし、ウォーターマークの配置と外観を正確に制御できるため、写真の完全性を保ちながら不正使用を防ぐことができます。

############################# Steps ############################
steps:
    enable: true
    title: "安全なビジネス ドキュメント: Photo 形式のウォーターマークを生成"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/):** でドキュメントのセキュリティを強化します。API をアプリケーションに挿入し、サポートされている多くのファイル形式のウォーターマークを生成します。
      
      1. **ウォーターマークの開始:** 主な機能を提供する **Watermarker** クラスでドキュメント処理を開始します。生成されたウォーターマークによって保護されるはずの Photo ファイルをコンストラクターに渡してインスタンス化します。
      2. **メインのウォーターマーク オブジェクトを作成します:** 特注の **Watermark** オブジェクトを彫刻してドキュメントを強化します。単なるページを超えて、添付ファイルやヘッダーなどのネイティブ要素にシームレスに統合され、セキュリティとプロフェッショナリズムの層が追加されます。
      3. **透かし属性の調整:** 寸法、配置、配色を調整して、透かしを正確に微調整します。細部に至るまで文書の整合性が強化され、ファイルが紛れもなく自分のものになります。
      4. **正確に実装:** **Watermarker** メソッドを利用して、カスタマイズした透かしを完璧に適用します。単一か複数かに関係なく、各透かしにより保護層が追加されます。セキュリティを強化するには、処理されたドキュメントを別の安全な場所に保存することを検討してください。
   
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

        // PHOTO のテキスト透かしを生成します

        // ソース ファイルを Watermarker インスタンスに渡します
        const watermarker = new groupdocs.watermark.Watermarker("input.png");
        
        // テキスト透かしを生成し、そのオプションを設定する
        const  watermark = new groupdocs.watermark.TextWatermark
            ("My Watermark", groupdocs.watermark.new Font("Arial", 36));

        // PHOTO の結果を取得する
        watermarker.add(watermark);
        watermarker.save("output.png");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "高度なウォーターマークテクニック"
  description: ".NET 環境にシームレスに統合できるように設計された堅牢なAPIを使用して、最先端のウォーターマーク技術をご覧ください。プレゼンテーション、法律文書、技術図など、さまざまな種類の文書に高度で安全なウォーターマークを追加するのに最適です。"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "洗練されたウォーターマーク"
  features:
    # feature loop
    - title: "ダイナミックウォーターマーク配置"
      content: "当社のAPIには、ドキュメントの内容に基づいてウォーターマークの位置を調整する動的配置オプションが用意されています。この機能は、プレゼンテーションや技術図の複雑なレイアウトに最適で、基礎となる情報の読みやすさを損なうことなく、ウォーターマークを常に最適に配置できます。"

    # feature loop
    - title: "見えないウォーターマークによるセキュリティの強化"
      content: "目に見えない透かしを入れることで、書類の見た目を変えずにしっかり保護できます。これらのウォーターマークは特定のソフトウェアツールでのみ検出できるように設計されているため、法律文書や財務書類の機密情報を保護するのに最適です。"

    # feature loop
    - title: "自動ウォーターマークワークフロー"
      content: "ウォーターマークのワークフローを自動化して、文書のセキュリティプロセスを合理化します。文書の種類、コンテンツの機密性、ユーザーのアクセスレベルに基づいてルールを設定し、ウォーターマークを自動的に適用することで、すべての文書で一貫したセキュリティプロトコルが維持されるようにします。"
      
  code_samples:
    # code sample loop
    - title: "PDF 個の添付ファイルのウォーターマークを生成"
      content: |
        この例は、すべての PDF 個の添付ファイルにウォーターマークを生成する方法を示しています
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  PDF ドキュメントをロード
            const loadOptions = new groupdocsWatermark.PdfLoadOptions();
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf", loadOptions);
            const pdfContent = watermarker.getContent(groupdocsWatermark.PdfContent.class);

            //  テキストウォーターマークを生成
            const watermark = new groupdocsWatermark.TextWatermark('WaterMark', new groupdocsWatermark.Font('Arial', 19));
  
            //  適切な添付ファイルにウォーターマークを追加
            for (const attachment of pdfContent.getAttachments().getInnerList().toArray()) {
                const info = attachment.getDocumentInfo();
                if (info.getFileType() !== groupdocsWatermark.FileType.Unknown && !info.isEncrypted()) {
                    const attachedWatermarker = attachment.createWatermarker();
                    attachedWatermarker.add(watermark);
                    attachment.updateContent(attachedWatermarker);
                    attachedWatermarker.close();
                }
            }

            //  PDF の保存が処理されました
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
    title: "写真用の JavaScript の保護用ウォーターマーク"
    exclude: "PHOTO"
    description: "Node.js のカスタマイズ可能で高度なウォーターマーク技術で写真のセキュリティを強化しましょう。JPG、PNG、WEBP など、さまざまな形式の写真を品質を損なうことなく保護できます。"
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