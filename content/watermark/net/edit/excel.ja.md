
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:19
draft: false
lang: ja
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Excel フォーマットのウォーターマークを編集"
head_description: "GroupDocs.Watermark for .NET を使用すると、ドキュメントを簡単にカスタマイズして保護できます。文書の整合性を高め、Excel のウォーターマークを簡単に編集できます。"

############################# Header ############################
title: "Excel スプレッドシートのウォーターマークの編集:.NET 効率" 
description: ".NET の効率性を実現するように設計されたカスタマイズ可能なウォーターマークツールを使用して、文書のセキュリティを強化してください。Excel 個のウォーターマークを簡単に編集できます。"
subtitle: "GroupDocs.Watermark for .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料 Nuget ダウンロード"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET ライブラリ"
    link: "/watermark/net/"
    link_title: "さらに詳しく"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **当社のツールで Excel 個のウォーターマークを編集:** GroupDocs.Watermark for .NET ツールは、文書を強化し保護するための効率的な方法を提供します。.NET 開発者向けのさまざまな機能により、ウォーターマークの管理が簡単になり、文書のセキュリティと信頼性が確保されます。

############################# Steps ############################
steps:
    enable: true
    title: ".NET を使用して Excel ドキュメントのウォーターマークを編集します"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** を使用すると、.NET の開発者はさまざまな Excel ドキュメント内のウォーターマークを簡単に編集できます。アプリケーションで API を使用する方法の簡単なガイドは次のとおりです。
      
      1. まず、Excel ファイルをパラメータとして **Watermarker** クラス コンストラクターに渡します。ファイルは、バイト ストリーム、ファイル ストリーム、またはローカル ディスク パスのいずれかとして指定できます。
      2. 次に、編集が必要な特定のウォーターマークを見つけます。 **SearchCriteria** を利用して、ドキュメントに以前に追加された対応するプロパティを持つ透かしを識別します。
      3. 検索後、関連するウォーターマークのリストが取得されます。その後、サイズ、ページ配置、テキスト、色、画像コンテンツなどのプロパティをカスタマイズできます。これにより、データを広範囲に制御できるようになります。
      4. ウォーターマークの編集が完了したら、更新したドキュメントを保存します。ローカル ファイル パスまたはストリームを利用して、最終結果を保存できます。
   
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
        // EXCEL テキストの透かしを編集する

        // EXCEL ファイルを提供する Watermarker を作成します
        using (Watermarker watermarker = new Watermarker("input.xslx"))
        {
            // TextSearchCriteria を構築し、テキストの透かしを取得します
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                 // テキストの透かしを編集する
                 watermark.FormattedTextFragments.Clear();
                 watermark.FormattedTextFragments.Add("passed", 
                    new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
            }

            // 文書を保存する
            watermarker.Save("output.xslx");
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
    title: "ウォーターマークを他のフォーマットでカスタマイズ"
    exclude: "EXCEL"
    description: "GroupDocs.Watermark for .NET を使用して、必要に応じてさまざまなドキュメント形式にウォーターマークを付けます。"
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