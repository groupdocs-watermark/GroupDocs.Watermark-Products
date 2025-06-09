
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:29
draft: false
lang: ja
format: Pdf
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "GroupDocs.Watermarkを使用したPdfでの正確なウォーターマーク編集"
head_description: "GroupDocs.Watermark for Python via .NETを使用して、Pdfドキュメント内のウォーターマークコンテンツを効率的に変更します。"

############################# Header ############################
title: "PythonツールでPdfウォーターマークをスムーズに編集" 
description: "GroupDocs.Watermark for Python via .NET開発ツールキットを使用して、PDFやその他の形式でウォーターマークをカスタマイズします。"
subtitle: "GroupDocs.Watermark for Python via .NETツール" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "PyPiから無料でお試しください"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NETツール"
    link: "/watermark/python-net/"
    link_title: "さらに詳しく"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **PDFドキュメントのウォーターマークを更新：** GroupDocs.Watermark for Python via .NETフレームワークを活用して、プロフェッショナルなフォーマットを維持しながらウォーターマークを調整します。

############################# Steps ############################
steps:
    enable: true
    title: "Pdfドキュメント内のウォーターマークを変更するためのPython APIの使用"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)**を使用すると、Python開発者はさまざまなPdfドキュメント内のウォーターマークコンテンツを変更できます。簡単な手順は次のとおりです：
      
      1. **Watermarker**クラスを使用してPdfドキュメントを読み込み、ファイルパス、メモリストリーム、またはバイト配列を入力として受け入れます。
      2. ドキュメント内の既存のウォーターマーク要素（テキストまたはグラフィカル）を検索するために**SearchCriteria**オブジェクトを構築します。
      3. 特定されたら、ツールは更新できるウォーターマークのインスタンスコレクションを提供し、色、配置、フォント、または組み込みイメージデータなどのパラメータを調整できます。
      4. 組み込みの保存メソッドを使用して、改訂されたドキュメントをディスクまたはサポートされている出力ストリームに保存して、プロセスを完了します。
   
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
        # PDFファイルの画像ウォーターマークを更新
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # 入力ファイルを使用してWatermarkerインスタンスを作成
        with gw.Watermarker("input.pdf") as watermarker:

            # SearchCriteriaを使用して画像ベースのウォーターマークを特定
            search_criteria = gwss.ImageDctHashSearchCriteria("logo.png")

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # 画像ウォーターマークに変更を適用
                        watermark.ImageData = imageData
                    except Exception as e:
                        pass

            # 更新されたPDFファイルをエクスポート
            watermarker.save("output.pdf")
        ```     

############################# More features ############################
more_features:
  enable: true
  title: "高度なウォーターマーキングツールで生産性を向上"
  description: "Pythonでドキュメントのブランディングと保護を加速する動的なウォーターマーキングAPIを使用します。ウォーターマークのレイヤーを挿入、検出、変更、または削除してください。"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "高度なウォーターマーク編集ワークフロー"
  features:
    # feature loop
    - title: "統合されたウォーターマーク制御"
      content: "GroupDocs.Watermark for Python via .NETを使用して、Pythonアプリケーションにウォーターマークライフサイクルの完全な制御を導入します。ウォーターマークのセットアップ、更新、削除を自動化して繰り返しの作業を回避します。"

    # feature loop
    - title: "ウォーターマーク属性の精密調整"
      content: "ウォーターマークの美観を完全に制御し、サイズ変更、再着色、回転、または再配置して、あらゆる視覚的要件を満たすことができる柔軟なAPIを提供します。"

    # feature loop
    - title: "ネイティブフォーマット機能の活用"
      content: "ウォーターマークをヘッダー、フッター、注釈、または背景に埋め込むことで、任意のファイル形式に適応します。私たちのAPIは、最適な統合のためにネイティブ構造を尊重します。"
      
  code_samples:
    # code sample loop
    - title: "PDFファイルのウォーターマークを変更"
      content: |
        PDFドキュメント内のウォーターマークプロパティを変更する方法を示します。
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # PDFファイルを開く
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.pdf as gwop

        # ウォーターマークコンテンツを読み込む
        load_options = gwop.PdfLoadOptions()
        with gw.Watermarker("source.pdf", load_options) as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,5,8]

            # ウォーターマークの更新を適用
            watermarks = watermarker.search(search_criteria)
            for watermark in watermarks:
                try:
                    watermark.formatted_text_fragments.clear()
                    watermark.formatted_text_fragments.add(
                        "New text", 
                        gww.Font("Calibri", 5.0, gww.FontStyle.bold), 
                        gww.Color.white, 
                        gww.Color.aqua
                    )
                except Exception as e:
                    pass
        
            # 編集された結果を保存
            watermarker.save("output.pdf")
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
    title: "さまざまなフォーマットでのウォーターマーク調整"
    exclude: "PDF"
    description: "GroupDocs.Watermark for Python via .NETの信頼性の高いAPIを使用して、ウォーターマーキングに広範なフォーマットサポートを楽しみます。"
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