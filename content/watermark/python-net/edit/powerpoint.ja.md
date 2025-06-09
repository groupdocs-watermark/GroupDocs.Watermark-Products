
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: ja
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Powerpointファイルの透かしを編集"
head_description: "GroupDocs.Watermark for Python via .NETを使用して、Powerpointプレゼンテーションの透かし内容を迅速に変更し、ドキュメントを安全に保ちます。"

############################# Header ############################
title: "Pythonでの正確なPowerpoint透かし編集" 
description: "GroupDocs.Watermark for Python via .NETを使用して、プレゼンテーション内の透かしレイアウトと可視性を完全に制御できます。"
subtitle: "GroupDocs.Watermark for Python via .NETライブラリ" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "PyPiから無料ダウンロード"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET API"
    link: "/watermark/python-net/"
    link_title: "さらに詳しく"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Powerpointファイル内の透かしレイアウトを制御：** GroupDocs.Watermark for Python via .NETを使用すると、透かしを正確に配置し、プレゼンテーションを簡単に保護できます。

############################# Steps ############################
steps:
    enable: true
    title: "PythonでPowerpointドキュメントの透かしを修正"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)**は、Python開発者がさまざまなPowerpointファイルの透かしを簡単に更新できるようにします。プロジェクトでの使用方法は次のとおりです：
      
      1. まず、**Watermarker**コンストラクタにPowerpointファイルを渡して開きます。ファイルパス、バイトストリーム、またはファイルストリームを使用できます。
      2. 次に、透かしテキストやプロパティを検索できる**SearchCriteria**を使用して、変更したい透かしを見つけます。
      3. 見つかったら、テキスト、フォント、サイズ、位置、色などの詳細を変更できます。これにより、透かしの外観が完全に制御できます。
      4. 変更を加えたら、ドキュメントを保存します。結果をストリームまたはファイルパスに書き込むことができます。
   
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
        # POWERPOINTファイルの透かしテキストを更新
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # POWERPOINTファイルを使用してWatermarkerを作成
        with gw.Watermarker("input.pptx") as watermarker:

            # 透かしテキストを見つけるためにTextSearchCriteriaを設定
            search_criteria = gwss.TextSearchCriteria("test", False)

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # 透かしテキストを修正
                        watermark.text = "passed"
                    except Exception as e:
                        pass
            
            watermarker.save("output.pptx")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "透かしを更新する他の方法を見つける"
  description: "当社のライブラリを使えば、Pythonアプリがさまざまなファイルタイプの透かしを追加、検索、編集、または削除できます。"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "透かし編集"
  features:
    # feature loop
    - title: "ファイルに透かしを追加"
      content: "GroupDocs.Watermark for Python via .NETを使用して、ドキュメント内の透かしを追加および管理します。簡単なAPIを使用して、透かしを検索、更新、または必要に応じて削除できます。"

    # feature loop
    - title: "ニーズに合わせて透かしをカスタマイズ"
      content: "柔軟なAPIを使用してフォント、サイズ、向き、色などの透かし設定を調整し、希望の結果を得られます。"

    # feature loop
    - title: "フォーマット固有の機能を使用"
      content: "ファイルフォーマットに応じて、透かし領域としてヘッダー、フッター、注釈、または背景などのネイティブ機能を使用できます。"
      
  code_samples:
    # code sample loop
    - title: "Excelでテキスト透かしを編集"
      content: |
        このコードでは、Excelスプレッドシート内の透かしテキストを変更する方法を示しています。
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # XLSXファイルを開く
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # スプレッドシートデータを読み込む
        with gw.Watermarker("source.xlsx") as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,3]

            # 透かしテキストを変更
            watermarks = watermarker.search(search_criteria)
            for watermark in watermarks:
                try:
                    watermark.formatted_text_fragments.clear()
                    watermark.formatted_text_fragments.add(
                       "passed", 
                        gww.Font("Calibri", 19.0, gww.FontStyle.bold), 
                        gww.Color.red, 
                        gww.Color.aqua
                    )
                except Exception as e:
                    pass
        
            # 結果を保存
            watermarker.save("output.xlsx")
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
    title: "他のファイルタイプの透かしを編集"
    exclude: "POWERPOINT"
    description: "GroupDocs.Watermark for Python via .NETを使用して、異なるドキュメントフォーマットの透かしに取り組みます。"
    items: 
        # format loop 1
        - name: "ウォーターマーク PDF"
          format: "PDF"
          link: "/watermark/python-net/edit//pdf/"
          description: "アドビ Portable ドキュメントフォーマット"

        # format loop 2
        - name: "ウォーターマーク Word"
          format: "WORD"
          link: "/watermark/python-net/edit//word/"
          description: "MS Word とオープンオフィス文書"
          
        # format loop 3
        - name: "ウォーターマーク Excel"
          format: "EXCEL"
          link: "/watermark/python-net/edit//excel/"
          description: "MS Excel とオープンオフィススプレッドシート"

        # format loop 4
        - name: "ウォーターマーク PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/edit//powerpoint/"
          description: "MS PowerPoint とオープンオフィスプレゼンテーション"

        # format loop 5
        - name: "ウォーターマーク DOCX"
          format: "DOCX"
          link: "/watermark/python-net/edit//docx/"
          description: "マイクロソフト Word XML ドキュメントを開く"
          
        # format loop 6
        - name: "ウォーターマーク PPTX"
          format: "PPTX"
          link: "/watermark/python-net/edit//pptx/"
          description: "PowerPoint XML プレゼンテーションを開く"
          
        # format loop 7
        - name: "ウォーターマーク XLSX"
          format: "XLSX"
          link: "/watermark/python-net/edit//xlsx/"
          description: "マイクロソフト Excel オープン XML スプレッドシート"

        # format loop 8
        - name: "ウォーターマーク DOC"
          format: "DOC"
          link: "/watermark/python-net/edit//doc/"
          description: "マイクロソフト Word 97-2007 ドキュメント"

        # format loop 9
        - name: "ウォーターマーク XLS"
          format: "XLS"
          link: "/watermark/python-net/edit//xls/"
          description: "マイクロソフト Excel ワークブック 97-2003"

        # format loop 10
        - name: "ウォーターマーク PPT"
          format: "PPT"
          link: "/watermark/python-net/edit//ppt/"
          description: "PowerPoint プレゼンテーション 97-2003"

        # format loop 11
        - name: "ウォーターマーク RTF"
          format: "RTF"
          link: "/watermark/python-net/edit//rtf/"
          description: "リッチテキスト形式"

---