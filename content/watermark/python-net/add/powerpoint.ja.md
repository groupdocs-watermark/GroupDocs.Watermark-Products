
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
head_title: "プレゼンテーションに透かしを追加"
head_description: "PowerPointスライドに透かしを簡単に追加して、追加のセキュリティを確保します。"

############################# Header ############################
title: "Pythonでのプレゼンテーション用の高度な透かし" 
description: "私たちのPython APIを使用して、PowerPointスライドにテキストと画像の透かしを追加します。プレゼンテーションを安全かつプロフェッショナルに保つのに最適。"
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料でPyPiをダウンロード"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "さらに詳しく"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NETは、PythonでPowerPointプレゼンテーションに高度な透かしを追加することができます。機密情報を保護したり、スライドに会社のロゴを追加したりできます。単独のスライドまたは全体のプレゼンテーションに透かしを追加でき、見た目や表示位置を調整できます。

############################# Steps ############################
steps:
    enable: true
    title: "Pythonを使った透かしの追加: Powerpoint向けの手順"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)**は、さまざまなビジネスファイルタイプに透かしを追加するためのライブラリです。Pythonで文書に透かしを迅速に追加するための手順は次のとおりです。
      
      1. **透かしの開始:** **Watermarker**クラスのインスタンスを作成します。透かしを追加するために、Powerpointファイルのパスまたはストリームをコンストラクタに渡して開きます。
      2. **透かしを作成:** 希望のテキストと設定を持つ**Watermark**オブジェクトを作成します。任意のページや文書要素（ヘッダーや付属文書など）に透かしを追加できます。
      3. **透かしをカスタマイズ:** 必要に応じて透かしのサイズ、位置、フォント、色、整列を調整します。これにより、文書内で透かしがちょうどよく見えるようになります。
      4. **適用して保存:** **Watermarker**メソッドを使用して、文書に透かしを追加します。結果を保存する際は、安全のため新しいファイルに保存することをお勧めします。
   
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
        # POWERPOINTファイルにテキスト透かしを追加
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # 透かしを追加したいファイルを選択
        with gw.Watermarker("input.pptx") as watermarker:

            # テキスト透かしオブジェクトを作成
            font = gww.Font("Arial", 36.0)
            watermark = gww.TextWatermark("top secret", font)
            watermark.foreground_color = gww.Color.red
            watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
            watermark.opacity = 0.4

            watermarker.add(watermark)

            # 更新したPOWERPOINTファイルを保存
            watermarker.save("output.pptx")
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "透かし機能をさらに探る"
  description: "Python APIを使用して、文書、スライド、図面などの透かしを追加、表示、変換、管理します。GroupDocs.Watermark for Python via .NETは、ファイルを保護し、著作権情報を簡単に追加します。"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "透かしの追加"
  features:
    # feature loop
    - title: "簡単に透かしを追加"
      content: "GroupDocs.Watermarkは、Python開発者がビジネス文書にテキスト、画像、または動的透かしを迅速に追加できるようにします。最小限の労力でファイルを安全に保ち、ブランドを維持できます。"

    # feature loop
    - title: "完全にカスタマイズ可能な透かし"
      content: "GroupDocs.Watermarkを使用して、透かしのサイズ、回転、透明度、色、フォントを変更できます。文書に完璧に合うように透かしを調整し、重要なコンテンツを鮮明に保ちます。"

    # feature loop
    - title: "文書機能を利用した透かし"
      content: "PDF注釈、Wordの背景、Excelのヘッダーなど、組み込みの文書機能を活用して透かしを追加してください。GroupDocs.Watermarkは文書の構造と連携し、効果的で非侵害的な透かしを提供します。"
      
  code_samples:
    # code sample loop
    - title: "DOCXに画像透かしを追加"
      content: |
        この例では、シェイプ透かしに画像効果を適用する方法を示します。
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.wordprocessing as gwow

        # Word文書を開く
        load_options = gwow.WordProcessingLoadOptions()
        with gw.Watermarker("source.docx", load_options) as watermarker:

            # 透かしオプションを設定
            with gww.ImageWatermark("logo.png") as watermark:

                effects = gwow.WordProcessingImageEffects()
                effects.brightness = 0.7
                effects.contrast = 0.6
                effects.chroma_key = gww.Color.red

                options = gwow.WordProcessingWatermarkSectionOptions()
                options.Effects = effects;

                # 透かしを作成
                watermarker.add(watermark, options)

                # 透かし付きの文書を保存
                watermarker.save("result.docx")
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
    title: "Pythonを使用してプレゼンテーションに透かし"
    exclude: "POWERPOINT"
    description: "私たちのPythonツールキットを使用して、PowerPointファイルに素早く透かしを追加します。スライドを安全に保ち、シャープな外観を維持します。"
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