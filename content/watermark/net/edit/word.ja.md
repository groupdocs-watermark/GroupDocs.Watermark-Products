
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:58
draft: false
lang: ja
format: Word
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Word 文書のウォーターマークを編集"
head_description: "GroupDocs.Watermark for .NET でウォーターマークの配置を調整し、文書のセキュリティを確保してください。ソリューションの Word ウォーターマークを簡単に調整できます。"

############################# Header ############################
title: "Word ウォーターマークの強化:.NET コンフィデンス" 
description: "Word 件の文書の信頼性とブランドインテグリティを GroupDocs.Watermark for .NET で保証してください。当社のソリューションを使用してウォーターマークを自信を持って編集できます。"
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
       **{ 425} ドキュメントセキュリティの強化:** GroupDocs.Watermark for .NET により、開発者はドキュメントセキュリティを簡単に強化できます。特定の要件に合わせてウォーターマークを自信を持って編集できます。

############################# Steps ############################
steps:
    enable: true
    title: ".NET を使用して Word ドキュメントのウォーターマークを編集"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** を使用すると、.NET 開発者はさまざまな Word ドキュメント内のウォーターマークを簡単に編集できます。アプリケーションで API を使用する方法を簡略化したガイドは次のとおりです。
      
      1. **Watermarker**クラスコンストラクターに渡します。ファイルは、バイトストリーム、ファイルストリーム、またはローカルディスクパスのいずれかとして提供できます。
      2. **SearchCriteria** を使用して、以前に文書に追加された対応するプロパティを持つウォーターマークを特定します。
      3. 検索すると、関連するウォーターマークのリストが表示されます。その後、サイズ、ページ配置、テキスト、色、画像コンテンツなどのプロパティをカスタマイズできます。これにより、データを広範囲に制御できます。
      4. ウォーターマークの編集が完了したら、更新した文書を保存します。ローカルファイルパスまたはストリームを使用して最終結果を保存できます。
   
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
        // WORD テキストウォーターマークを編集

        // WORD ファイルを提供するウォーターマーカーを作成
        using (Watermarker watermarker = new Watermarker("input.docx"))
        {
            // テキスト検索条件を作成してテキストウォーターマークを取得する
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                 // テキストウォーターマークの編集
                 watermark.FormattedTextFragments.Clear();
                 watermark.FormattedTextFragments.Add("passed", 
                    new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
            }

            // 文書を保存する
            watermarker.Save("output.docx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ウォーターマークの修正について詳しく見る"
  description: ".NET 個のアプリケーションを当社のライブラリで強化し、さまざまなファイル形式のウォーターマークを追加、編集、削除、または検索できます。"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "ウォーターマークを編集"
  features:
    # feature loop
    - title: "ビジネス用のウォーターマークファイル"
      content: "GroupDocs.Watermark for .NET を使用してファイルやドキュメントにウォーターマークを付けます。アプリケーションに当社の API を実装する手間をかけずに、ウォーターマークを追加および管理できます。以前に追加したウォーターマークを検索、編集、削除できます。"

    # feature loop
    - title: "要件に合わせてウォーターマークを微調整"
      content: "当社の API には、包括的なカスタマイズオプションが用意されています。サイズ、向き、配色、フォントファミリーなどの要素を簡単に変更して、理想的なウォーターマークを作成できます。"

    # feature loop
    - title: "文書固有の機能を活用"
      content: "使用しているファイル形式によっては、組み込み機能を組み込むことができます。これらには、文書の背景、注釈、ヘッダー、またはウォーターマークコンテナとして機能するその他の要素が含まれる場合があります。"
      
  code_samples:
    # code sample loop
    - title: "Excel ウォーターマークテキスト編集"
      content: |
        この例は、Excel ワークシートの特定のウォーターマークのテキストを編集する方法を示します
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  XLSX スプレッドシートをロード
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  スプレッドシートのコンテンツを読み込む
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();

                //  ウォーターマークの内部テキストを編集
                foreach (SpreadsheetShape shape in content.Worksheets[0].Shapes)
                {
                    if (shape.Text == "GroupDocs 2016")
                    {
                        shape.Text = "GroupDocs 2017";
                    }
                }

                //  出力結果を保存
                watermarker.save("result.xlsx");
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
    title: "他の形式のセキュリティを強化"
    exclude: "WORD"
    description: "GroupDocs.Watermark for .NET は、さまざまな形式のドキュメントセキュリティを強化する効率的なソリューションを提供します。"
    items: 
        # format loop 1
        - name: "ウォーターマーク PDF"
          format: "PDF"
          link: "/watermark/net/edit//pdf/"
          description: "アドビ Portable ドキュメントフォーマット"

        # format loop 2
        - name: "ウォーターマーク Word"
          format: "WORD"
          link: "/watermark/net/edit//word/"
          description: "MS Word とオープンオフィス文書"
          
        # format loop 3
        - name: "ウォーターマーク Excel"
          format: "EXCEL"
          link: "/watermark/net/edit//excel/"
          description: "MS Excel とオープンオフィススプレッドシート"

        # format loop 4
        - name: "ウォーターマーク PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/edit//powerpoint/"
          description: "MS PowerPoint とオープンオフィスプレゼンテーション"

        # format loop 5
        - name: "ウォーターマーク DOCX"
          format: "DOCX"
          link: "/watermark/net/edit//docx/"
          description: "マイクロソフト Word XML ドキュメントを開く"
          
        # format loop 6
        - name: "ウォーターマーク PPTX"
          format: "PPTX"
          link: "/watermark/net/edit//pptx/"
          description: "PowerPoint XML プレゼンテーションを開く"
          
        # format loop 7
        - name: "ウォーターマーク XLSX"
          format: "XLSX"
          link: "/watermark/net/edit//xlsx/"
          description: "マイクロソフト Excel オープン XML スプレッドシート"

        # format loop 8
        - name: "ウォーターマーク DOC"
          format: "DOC"
          link: "/watermark/net/edit//doc/"
          description: "マイクロソフト Word 97-2007 ドキュメント"

        # format loop 9
        - name: "ウォーターマーク XLS"
          format: "XLS"
          link: "/watermark/net/edit//xls/"
          description: "マイクロソフト Excel ワークブック 97-2003"

        # format loop 10
        - name: "ウォーターマーク PPT"
          format: "PPT"
          link: "/watermark/net/edit//ppt/"
          description: "PowerPoint プレゼンテーション 97-2003"

        # format loop 11
        - name: "ウォーターマーク RTF"
          format: "RTF"
          link: "/watermark/net/edit//rtf/"
          description: "リッチテキスト形式"

---