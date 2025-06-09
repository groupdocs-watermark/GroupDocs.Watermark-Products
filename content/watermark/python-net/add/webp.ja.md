
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:28
draft: false
lang: ja
format: Webp
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "PythonによるWEBPへの透かし"
head_description: "Pythonを使用してWEBP画像に透かしを追加し、強力な保護を提供します。"

############################# Header ############################
title: "PythonによるWEBPの透かし作成" 
description: "PythonでWEBPファイルにカスタム透かしを追加します。アーティストやコンテンツクリエイターに最適です。"
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "PyPiで無料で入手"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "さらに詳しく"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NETを使用して、PythonでWEBP画像に透かしを追加します。テキスト、ロゴ、またはデジタル署名を使用し、ニーズに合った外観を調整します。オンラインで画像を共有する方には最適で、GroupDocs.Watermarkは作品を安全に保ち、素晴らしい見た目を保ちます。

############################# Steps ############################
steps:
    enable: true
    title: "Webpファイルに透かしを素早く追加する"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/):** あなたの文書に透かしを追加する強力なPythonライブラリです。
      
      1. **メインクラス: Watermarker.** 最初に、**Watermarker**オブジェクトを作成します。Webpファイルをファイルパスまたはストリームとして渡して開始します。
      2. **透かしを作成する.** 次に、必要なタイプのWatermarkオブジェクトを作成します。任意のページや画像、ヘッダーなどの文書要素に配置できます。
      3. **外観を調整する.** 透かしのサイズ、位置、フォント、色を設定してニーズに合わせます。
      4. **追加して保存する.** **Watermarker**メソッドを使用して透かしを挿入します。必要なだけ追加し、好きな場所にファイルを保存します。
   
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
        # WEBPファイルに画像の透かしを追加する
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # Watermarkerのコンストラクタにファイルパスを渡す
        with gw.Watermarker("input.webp") as watermarker:

            # 画像ファイルを使用して画像の透かしを作成する
            watermark = gww.ImageWatermark("watermark.png")

            watermarker.add(watermark)

            # 透かし付きのWEBPファイルを保存する
            watermarker.save("output.webp")
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "さらなる透かし機能を発見する"
  description: "GroupDocs.Watermark for Python via .NETは、さまざまなファイルタイプで透かしを追加しカスタマイズするための高度なオプションを提供します。柔軟で使いやすい機能で文書や画像を保護します。"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "オールインワン透かし機能"
  features:
    # feature loop
    - title: "全ページタイル"
      content: "タイル状の透かしで文書全体を覆います。これにより、透かしを削除しにくくし、レイアウトを損なうことなくファイルを保護します。"

    # feature loop
    - title: "カスタムカラー"
      content: "ブランドや文書スタイルに合わせて任意の色を選択できます。透かしを目立たせたり、必要に応じてなじませたりできます。"

    # feature loop
    - title: "追加のセキュリティオプション"
      content: "レイヤー透かしで文書のセキュリティを強化します。目に見えるマークと隠されたマークを組み合わせてコピーを防止し、適切な人だけがファイルにアクセスできるようにします。"
      
  code_samples:
    # code sample loop
    - title: "PowerPointに透かしを追加する"
      content: |
        このサンプルはPPTXスライドの背景に透かしを追加する方法を示しています。
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.presentation as gwop

        # PPTXファイルを開く
        load_options = gwop.PresentationLoadOptions()
        with gw.Watermarker("source.pptx", load_options) as watermarker:

            # 透かしの詳細を設定
            with TextWatermark("Protected image", gww.Font("Arial", 8.0)) as watermark:

                watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
                watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
                watermark.rotate_angle = 45
                watermark.scale_factor = 1

                # スライドの背景に透かしを適用
                watermarker.add(watermark)

                # 更新したプレゼンテーションを保存
                watermarker.save("result.pptx")
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
    title: "PythonによるWEBP画像の保護"
    exclude: "WEBP"
    description: "Pythonを使ってWEBP画像に高度でカスタムな透かしを追加し、創造的な作品を保護します。"
    items: 
        # format loop 1
        - name: "ウォーターマーク PDF"
          format: "PDF"
          link: "/watermark/python-net/add//pdf/"
          description: "アドビ Portable ドキュメントフォーマット"

        # format loop 2
        - name: "ウォーターマーク Word"
          format: "WORD"
          link: "/watermark/python-net/add//word/"
          description: "MS Word とオープンオフィス文書"
          
        # format loop 3
        - name: "ウォーターマーク Excel"
          format: "EXCEL"
          link: "/watermark/python-net/add//excel/"
          description: "MS Excel とオープンオフィススプレッドシート"

        # format loop 4
        - name: "ウォーターマーク画像"
          format: "IMAGE"
          link: "/watermark/python-net/add//image/"
          description: "人気の画像フォーマット"

        # format loop 5
        - name: "ウォーターマーク写真"
          format: "PHOTO"
          link: "/watermark/python-net/add//photo/"
          description: "写真フォーマット"

        # format loop 6
        - name: "ウォーターマーク PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/add//powerpoint/"
          description: "MS PowerPoint とオープンオフィスプレゼンテーション"

        # format loop 7
        - name: "ウォーターマーク DOCX"
          format: "DOCX"
          link: "/watermark/python-net/add//docx/"
          description: "マイクロソフト Word XML ドキュメントを開く"
          
        # format loop 8
        - name: "ウォーターマーク PPTX"
          format: "PPTX"
          link: "/watermark/python-net/add//pptx/"
          description: "PowerPoint XML プレゼンテーションを開く"
          
        # format loop 9
        - name: "ウォーターマーク XLSX"
          format: "XLSX"
          link: "/watermark/python-net/add//xlsx/"
          description: "マイクロソフト Excel オープン XML スプレッドシート"

        # format loop 10
        - name: "ウォーターマーク JPEG"
          format: "JPEG"
          link: "/watermark/python-net/add//jpeg/"
          description: "JPEG イメージ"

        # format loop 11
        - name: "ウォーターマーク PNG"
          format: "PNG"
          link: "/watermark/python-net/add//png/"
          description: "Portable ネットワークグラフィック"

        # format loop 12
        - name: "ウォーターマーク TIFF"
          format: "TIFF"
          link: "/watermark/python-net/add//tiff/"
          description: "タグ画像ファイル形式"

        # format loop 13
        - name: "ウォーターマーク WEBP"
          format: "WEBP"
          link: "/watermark/python-net/add//webp/"
          description: "ウェブ画像"

        # format loop 14
        - name: "ウォーターマーク DOC"
          format: "DOC"
          link: "/watermark/python-net/add//doc/"
          description: "マイクロソフト Word 97-2007 ドキュメント"

        # format loop 15
        - name: "ウォーターマーク XLS"
          format: "XLS"
          link: "/watermark/python-net/add//xls/"
          description: "マイクロソフト Excel ワークブック 97-2003"

        # format loop 16
        - name: "ウォーターマーク PPT"
          format: "PPT"
          link: "/watermark/python-net/add//ppt/"
          description: "PowerPoint プレゼンテーション 97-2003"

        # format loop 17
        - name: "ウォーターマーク RTF"
          format: "RTF"
          link: "/watermark/python-net/add//rtf/"
          description: "リッチテキスト形式"

---