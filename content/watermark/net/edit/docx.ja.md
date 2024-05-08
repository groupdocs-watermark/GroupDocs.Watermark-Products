
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:24
draft: false
lang: ja
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Docx ファイル全体のウォーターマークを編集"
head_description: "GroupDocs.Watermark for .NET アプリケーションで Docx ファイル全体のウォーターマークを編集します。文書の信頼性を簡単に強化できます。"

############################# Header ############################
title: "ファイル全体で Docx ウォーターマークを編集:.NET 汎用性" 
description: "GroupDocs.Watermark for .NET アプリケーションを使用して、自信を持って文書をカスタマイズできます。さまざまなファイル形式のウォーターマークを簡単に編集できます。"
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
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "さらに詳しく"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Docx ファイルにわたるウォーターマークの編集:** GroupDocs.Watermark for .NET アプリケーションを使用すると、さまざまなファイル形式のウォーターマークをシームレスに編集できます。自信を持って効率的に文書をカスタマイズできます。

############################# Steps ############################
steps:
    enable: true
    title: ".NET API を使用して、Docx ドキュメントのウォーターマークをプログラムで編集する"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** は、.NET の開発者に、さまざまな Docx ドキュメント内のウォーターマークをプログラムで操作するための堅牢な API を提供します。このガイドでは、プロセスの概要を説明します。
      
      1. Docx ファイルを引数として **Watermarker** クラス コンストラクターに指定して、ワークフローを開始します。ファイルは、バイト ストリーム、ファイル ストリーム、またはローカル ディスクの場所への参照として提供できます。
      2. 次に、**SearchCriteria** オブジェクトを利用して、変更が必要な特定のウォーターマークを特定します。このオブジェクトを使用すると、ドキュメント内に以前に埋め込まれた透かしを識別できます。
      3. 検索が正常に実行されると、関連するウォーターマークのコレクションを受け取ります。これらの透かしを使用すると、詳細な制御が可能になり、寸法、ページの位置、テキスト コンテンツ、配色、画像データなどのプロパティを変更できます。
      4. ウォーターマークの編集が完了したら、変更したドキュメントを永続化します。 API は、ローカル ファイル パスまたはストリーム オブジェクトを使用してストレージを容易にします。
   
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
        // DOCX ドキュメントで画像の透かしを編集する

        // ソースファイルで Watermarker を初期化する
        using (Watermarker watermarker = new Watermarker("input.docx"))
        {
            // 画像透かし検索用の SearchCriteria を作成します
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                // 画像の透かしを編集する
                watermark.ImageData = imageData;
            }

            // 結果を保存 DOCX
            watermarker.Save("output.docx");
        }
        
        ```     

############################# More features ############################
more_features:
  enable: true
  title: "ウォーターマーク管理でワークフローを強化"
  description: "当社の堅牢なライブラリを使用すると、.NET アプリケーション内のさまざまなファイル形式のウォーターマークを簡単に行うことができます。ウォーターマークの追加、編集、検索、削除が簡単に行え、文書のセキュリティとブランディングを強化できます。"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "シームレスなウォーターマーク編集"
  features:
    # feature loop
    - title: "アプリケーションのウォーターマーキングを効率化"
      content: "GroupDocs.Watermark for .NET の機能を活用して、ウォーターマーク機能を .NET アプリケーションにシームレスに統合してください。直感的な API により、ウォーターマークの作成、管理、検索、編集が簡単になり、複雑な手動処理が不要になります。"

    # feature loop
    - title: "きめ細かなウォーターマークのカスタマイズ"
      content: "包括的な API でウォーターマークカスタマイズの可能性を最大限に引き出しましょう。サイズ、向き、配色、フォントの選択など細部まで微調整して、ブランディングやセキュリティ要件に完全に合致するウォーターマークを作成できます。"

    # feature loop
    - title: "ハーネス文書固有の機能を活用してフレキシブルウォーターマーキングを実現"
      content: "さまざまなドキュメント形式のネイティブ機能を最大限に活用できます。文書の背景、注釈、ヘッダー、その他のオブジェクトなどの要素を独自のウォーターマークコンテナとして利用し、さまざまな文書タイプやセキュリティニーズに対応します。"
      
  code_samples:
    # code sample loop
    - title: "PDF 画像ウォーターマーク編集"
      content: |
        この例は、画像ウォーターマークの内容を編集する方法を示しています
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  PDF としてドキュメントをロード
            var loadOptions = new PdfLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pdf", loadOptions))
            {
                //  コンテンツを読み込む
                PdfContent pdfContent = watermarker.GetContent<PdfContent>();

                //  画像ウォーターマークを編集
                foreach (PdfArtifact artifact in pdfContent.Pages[0].Artifacts)
                {
                    if (artifact.Image != null)
                    {
                        artifact.Image = new PdfWatermarkableImage(File.ReadAllBytes("test.png"));
                    }
                }

                //  出力結果をお楽しみください
                watermarker.save("result.pdf");
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
    title: "複数のファイルにわたるウォーターマークの編集"
    exclude: "DOCX"
    description: "GroupDocs.Watermark for .NET を搭載したアプリケーションで、複数のファイル形式のウォーターマークをシームレスに編集できます。"
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