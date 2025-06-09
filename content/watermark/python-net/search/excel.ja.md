
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:16
draft: false
lang: ja
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Excelスプレッドシート内の隠れた透かしを検出する"
head_description: "GroupDocs.Watermarkを使用して、スプレッドシートファイル内の隠れたマークを迅速かつ正確に明らかにします。"

############################# Header ############################
title: "Excelスプレッドシート内の透かしをすぐに特定する" 
description: "GroupDocs.Watermark for Python via .NETを使用して透かしをシームレスに特定し、管理します。"
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "今すぐPyPiをダウンロード - 無料です"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NETの概要"
    link: "/watermark/python-net/"
    link_title: "さらに詳しく"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NETは、Python開発者向けのフル機能の透かしツールキットを提供します。Excel、Word、PDFなどの文書から透かしコンテンツを生成、変更、検出、削除するのに最小限の労力で実現します。

############################# Steps ############################
steps:
    enable: true
    title: "Pythonを使用してExcelファイル内の透かしを検出する方法"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/python-net/)**を使用することで、ビジネス文書内の埋め込まれた透かしを簡単に特定できます。その機能をPythonのワークフローに統合して、シームレスに検出しましょう。
      
      1. **Watermarker**クラスのインスタンスにExcel文書を読み込むことから始めます。入力としてパス、ストリーム、またはバイト配列を受け付けます。
      2. **SearchCriteria**オブジェクトを使用して検索を絞り込みます。画像ベースの透かしを見つけるには、サンプル画像を使用します。テキストの場合は、コンテンツ、スタイル、または色などの特性を指定します。
      3. **Watermarker**オブジェクトから**Search**メソッドを呼び出して、透かしデータを抽出します。調査のために透かしインスタンスのコレクションが返されます。
      4. 取得後、結果を管理できます：不要なマークを削除したり、サイズやメッセージ内容などの詳細を更新できます。
   
    code:
      platform: "python-net"
      copy_title: "[コピー]"
      install:
        command: |
        command: "pip install groupdocs-watermark-net"
        copy_tip: "クリックしてコピー"
        copy_done: "コピーされました"
      links:
        #  loop
        - title: "その他の例"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
        #  loop
        - title: "ドキュメンテーション"
          link: "https://docs.groupdocs.com/watermark/python-net/"
          
      content: |
        ```python {style=abap}
        # EXCEL形式のテキスト透かしを検出する
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # EXCELファイルでWatermarkerを初期化する
        with gw.Watermarker("input.xlsx") as watermarker:

            # 透かし検索を実行する
            search_criteria = gwss.TextSearchCriteria("test", False)
            possible_watermarks = watermarker.search(search_criteria)

            # 検出された透かしのリストを処理する
            print("\nFound {0} possible watermark(s).".format(len(possible_watermarks)))
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "GroupDocs.Watermarkによる強力な透かし検出"
  description: "PythonプロジェクトにGroupDocs.Watermarkを使用して、さまざまな文書タイプ内の透かし要素を効率的にスキャンして特定します。"
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "透かしを検出する"
  features:
    # feature loop
    - title: "スマートフィルターによる高度な検出"
      content: "幅広い文書形式で透かしを特定できます。GroupDocs.Watermarkは、形状、透明度などの視覚的およびテキスト的特性によるフィルタリングをサポートしています。"

    # feature loop
    - title: "検索のための柔軟な基準"
      content: "GroupDocs.Watermarkを使用してカスタマイズされた透かし検索パラメータを定義します。この精密さにより、隠されたりカスタマイズされた透かしデータのターゲット取得が可能になります。"

    # feature loop
    - title: "検出された透かしのアクセスと整理"
      content: "すべての埋め込まれた透かしを取得することで文書監査を簡素化します。当社のツールは、発見したアイテムの効率的な抽出、表示、および管理を可能にします。"
      
  code_samples:
    # code sample loop
    - title: "コード例：透かしを検出する"
      content: |
        GroupDocs.Watermarkを使用して柔軟な検出ルールで埋め込まれた透かしコンテンツを文書内で検索する方法を見てみましょう。
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # ディスクまたはストリームからターゲット文書を開く
        load_options = gwos.SpreadsheetLoadOptions()
        with gw.Watermarker("source.xlsx", load_options) as watermarker:

            # 検索に使用する具体的な透かしの属性を定義する
            criteria = gwss.TextFormattingSearchCriteria()
            criteria.foreground_color_range = gwss.ColorRange()
            criteria.foreground_color_range.min_hue = -5.0
            criteria.foreground_color_range.max_hue = 10.0
            criteria.foreground_color_range.min_brightness = 0.01
            criteria.foreground_color_range.max_brightness = 0.99
            criteria.background_color_range = gwss.ColorRange()
            criteria.background_color_range.is_empty = True
            criteria.font_name = "Arial"
            criteria.min_font_size = 19.0
            criteria.max_font_size = 42.0
            criteria.font_bold = True

            # 検索を実行し、一致を収集する
            possible_watermarks = watermarker.search(criteria)

            # 見つかった結果を操作してあらゆるアクションを行う
            print("Found {0} possible watermark(s).".format(len(possible_watermarks)))
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか?"
  description: "GroupDocs.Watermark の機能を無料で試すか、ライセンスをリクエストしてください"
  items:
    #  loop
    - title: "PyPi ダウンロード"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      color: "red"
        #  loop
    - title: "ライセンス"
      link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "マルチフォーマット透かし検索"
    exclude: "EXCEL"
    description: "GroupDocs.Watermarkがサポートするすべてのファイルタイプにわたる透かしコンテンツを特定します。"
    items: 
        # format loop 1
        - name: "ウォーターマーク PDF"
          format: "PDF"
          link: "/watermark/python-net/search//pdf/"
          description: "アドビ Portable ドキュメントフォーマット"

        # format loop 2
        - name: "ウォーターマーク Word"
          format: "WORD"
          link: "/watermark/python-net/search//word/"
          description: "MS Word とオープンオフィス文書"
          
        # format loop 3
        - name: "ウォーターマーク Excel"
          format: "EXCEL"
          link: "/watermark/python-net/search//excel/"
          description: "MS Excel とオープンオフィススプレッドシート"

        # format loop 4
        - name: "ウォーターマーク PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/search//powerpoint/"
          description: "MS PowerPoint とオープンオフィスプレゼンテーション"

        # format loop 5
        - name: "ウォーターマーク DOCX"
          format: "DOCX"
          link: "/watermark/python-net/search//docx/"
          description: "マイクロソフト Word XML ドキュメントを開く"
          
        # format loop 6
        - name: "ウォーターマーク PPTX"
          format: "PPTX"
          link: "/watermark/python-net/search//pptx/"
          description: "PowerPoint XML プレゼンテーションを開く"
          
        # format loop 7
        - name: "ウォーターマーク XLSX"
          format: "XLSX"
          link: "/watermark/python-net/search//xlsx/"
          description: "マイクロソフト Excel オープン XML スプレッドシート"

        # format loop 8
        - name: "ウォーターマーク DOC"
          format: "DOC"
          link: "/watermark/python-net/search//doc/"
          description: "マイクロソフト Word 97-2007 ドキュメント"

        # format loop 9
        - name: "ウォーターマーク XLS"
          format: "XLS"
          link: "/watermark/python-net/search//xls/"
          description: "マイクロソフト Excel ワークブック 97-2003"

        # format loop 10
        - name: "ウォーターマーク PPT"
          format: "PPT"
          link: "/watermark/python-net/search//ppt/"
          description: "PowerPoint プレゼンテーション 97-2003"

        # format loop 11
        - name: "ウォーターマーク RTF"
          format: "RTF"
          link: "/watermark/python-net/search//rtf/"
          description: "リッチテキスト形式"

---