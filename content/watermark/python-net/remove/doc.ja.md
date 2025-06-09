
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:30
draft: false
lang: ja
format: Doc
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Python で DOC ファイルから透かしを削除する"
head_description: "Python API を使用して DOC ファイルの透かしをクリアし、ドキュメントをクリーンに保ちます。"

############################# Header ############################
title: "DOC 透かし削除のための Python" 
description: "GroupDocs.Watermark for Python via .NET APIを使用すると、DOCファイルの透かしを容易に削除または編集で、ドキュメントを整理できます。"
subtitle: "GroupDocs.Watermark for Python via .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "PyPi から無料ダウンロード"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET ライブラリ"
    link: "/watermark/python-net/"
    link_title: "さらに詳しく"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET ライブラリは、DOC ファイルの透かしを管理するためのすべてのツールを提供します。透かしを削除または調整して、プロフェッショナルで整ったドキュメントを保ちます。

############################# Steps ############################
steps:
    enable: true
    title: "Python で Doc ファイルから透かしを削除する方法"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/python-net/)** は、Python 開発者が Doc ファイルから透かしを迅速に取り除くことを可能にします。方法は以下の通りです：
      
      1. **Watermarker** コンストラクタにあなたの Doc ファイルを渡して始めます。ファイルパス、バイトストリーム、またはファイルストリームを使用できます。
      2. **SearchCriteria** オブジェクトを使用して、削除したい透かしを検索します。画像、テキスト、または書式でフィルタリングし、正確な結果を得ます。
      3. 検索の後、透かしのリストが表示されます。必要ないものを選択して削除します。
      4. 完了したら、ドキュメントをファイルまたはストリームとして保存します。
   
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
        # DOC ファイルから画像の透かしを削除する
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # あなたの DOC ファイルで Watermarker インスタンスを作成する
        with gw.Watermarker("input.doc") as watermarker:

            # 検出された透かしを見つけて削除する
            search_criteria = gwss.ImageDctHashSearchCriteria("logo.png")

            possible_watermarks = watermarker.search(search_criteria)
            del possible_watermarks[i]

            # 更新したドキュメントを保存する
            watermarker.save("output.doc")
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "Python での強力な透かし削除 | GroupDocs.Watermark"
  description: "Python API を活用して PDF および Office ファイルから透かしを削除しましょう。どんな用途にも対応したクリーンでプロフェッショナルなドキュメントを手に入れましょう。"
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "透かしを消去"
  features:
    # feature loop
    - title: "Python での正確な透かし削除"
      content: "Python API は正確な透かしの削除のために作られているため、ファイルは元の外観や書式を保つことができます。ビジネス、法務、あるいは学術ドキュメントに最適です。"

    # feature loop
    - title: "Python を使用したバッチ透かし削除"
      content: "一度に多くのファイルから透かしを削除して、ワークフローを速度化します。大規模なドキュメントコレクションの効率的な処理に最適です。"

    # feature loop
    - title: "柔軟な透かしの編集と削除"
      content: "必要に応じて透かしを編集または削除できます。API では、ドキュメントを要求に合わせて適切に保つオプションが提供されます。"
      
  code_samples:
    # code sample loop
    - title: "プレゼンテーションから背景を削除する"
      content: |
        この例では、ハイパーリンクの透かしを削除する方法を示します。
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.presentation as gwop

        # プレゼンテーションを開く
        load_options = gwop.PresentationLoadOptions()
        with gw.Watermarker("source.pptx", load_options) as watermarker:

            # スライドの内容にアクセスする
            search_criteria = gwss.TextSearchCriteria("Lorem ipsum")

            # ハイパーリンクの透かしを削除する
            watermarks = watermarker.search(search_criteria)

            for i in range(len(watermarks) - 1, -1, -1):
                if isinstance(watermarks[i], gws.HyperlinkPossibleWatermark):
                    del watermarks[i]

            # プレゼンテーションを保存する
            watermarker.save("result.pptx");
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
    title: "Python での DOC ファイルからの透かし削除"
    exclude: "DOC"
    description: "GroupDocs.Watermark for Python via .NET API がどのように DOC ファイルの透かしをクリアして、より良いドキュメントクオリティを提供できるかを確認してください。"
    items: 
        # format loop 1
        - name: "ウォーターマーク PDF"
          format: "PDF"
          link: "/watermark/python-net/remove//pdf/"
          description: "アドビ Portable ドキュメントフォーマット"

        # format loop 2
        - name: "ウォーターマーク Word"
          format: "WORD"
          link: "/watermark/python-net/remove//word/"
          description: "MS Word とオープンオフィス文書"
          
        # format loop 3
        - name: "ウォーターマーク Excel"
          format: "EXCEL"
          link: "/watermark/python-net/remove//excel/"
          description: "MS Excel とオープンオフィススプレッドシート"

        # format loop 4
        - name: "ウォーターマーク PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/remove//powerpoint/"
          description: "MS PowerPoint とオープンオフィスプレゼンテーション"

        # format loop 5
        - name: "ウォーターマーク DOCX"
          format: "DOCX"
          link: "/watermark/python-net/remove//docx/"
          description: "マイクロソフト Word XML ドキュメントを開く"
          
        # format loop 6
        - name: "ウォーターマーク PPTX"
          format: "PPTX"
          link: "/watermark/python-net/remove//pptx/"
          description: "PowerPoint XML プレゼンテーションを開く"
          
        # format loop 7
        - name: "ウォーターマーク XLSX"
          format: "XLSX"
          link: "/watermark/python-net/remove//xlsx/"
          description: "マイクロソフト Excel オープン XML スプレッドシート"

        # format loop 8
        - name: "ウォーターマーク DOC"
          format: "DOC"
          link: "/watermark/python-net/remove//doc/"
          description: "マイクロソフト Word 97-2007 ドキュメント"

        # format loop 9
        - name: "ウォーターマーク XLS"
          format: "XLS"
          link: "/watermark/python-net/remove//xls/"
          description: "マイクロソフト Excel ワークブック 97-2003"

        # format loop 10
        - name: "ウォーターマーク PPT"
          format: "PPT"
          link: "/watermark/python-net/remove//ppt/"
          description: "PowerPoint プレゼンテーション 97-2003"

        # format loop 11
        - name: "ウォーターマーク RTF"
          format: "RTF"
          link: "/watermark/python-net/remove//rtf/"
          description: "リッチテキスト形式"

---