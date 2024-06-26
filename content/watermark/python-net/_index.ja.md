---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:49
draft: false

lang: ja
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"
    # supported_platforms loop
    - title: "Python"
      tag: "python-net"

############################# Head ############################
head_title: "Python 透かしライブラリ |文書の透かし"
head_description: "Python は、テキストと画像の透かしを使用してビジネス ドキュメントを保護します。 PDF、Word、Excel、PowerPoint などのファイル形式がサポートされています。"

############################# Header ############################
title: "Python via .NET 透かしテクノロジーにアクセスする"
description: "この Python ソリューションを使用してデータを保護し、不正コピーを防止します。 PDF、Word、Excel、PowerPoint、画像など、さまざまな形式のビジネス文書に透かしを簡単に追加できます。"
words:
  for: "にとって"

actions:
  main: "PyPi を無料でダウンロード"
  main_link: "https://pypi.org/project/groupdocs-watermark-net/"
  alt: "ライセンス"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
  title: "始める準備はできましたか?"
  description: "GroupDocs.Watermark の機能を無料で試すか、ライセンスをリクエストしてください"

release:
  title: "バージョン {0} がリリースされました"
  notes: "新機能を見る"
  downloads: "ダウンロード"
  link: "https://releases.groupdocs.com/watermark/python-net/"

code:
  title: "Python を使用して PDF にウォーターマークを追加する"
  more: "その他の例"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
  install: "pip install groupdocs-watermark-net"
  content: |
    ```python {style=abap}

    import groupdocs.watermark as gw
    import groupdocs.watermark.watermarks as gww
    import groupdocs.watermark.options.pdf as gwop
    import groupdocs.watermark.common as gwc

    # PDF パスを渡すウォーターマーカーをインスタンス化
    pdf_lo = gwop.PdfLoadOptions()
    with gw.Watermarker("source.pdf", pdf_lo) as watermarker:
        options = gwop.PdfArtifactWatermarkOptions()

        # ウォーターマークオプションのカスタマイズ
        text_watermark = 
            gww.TextWatermark("Approved", gww.Font("Arial", 8.0))
        text_watermark.horizontal_alignment = 
            gwc.HorizontalAlignment.RIGHT

        # PDF ドキュメントにウォーターマークを適用
        watermarker.add(text_watermark, options)

        # 結果文書を保存
        watermarker.save("result.pdf")

    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark 一目でわかる"
  description: "Python ウォーターマーク用ライブラリ"
  features:
    # feature loop
    - title: "Python ドキュメントの透かし"
      content: "GroupDocs.Watermark for Python via .NET を使用して機密データを保護します。さまざまなファイル形式にテキストまたは画像を透かしとして配置します。"

    # feature loop
    - title: "透かしをカスタマイズする"
      content: "GroupDocs.Watermark for Python via .NET では、多くのカスタマイズ オプションを利用できます。テキスト スタイル (太字、斜体、フォント) またはサイズや回転などの画像プロパティを設定して、ドキュメントの透かしを調整します。"

    # feature loop
    - title: "一般的なファイル形式のサポート"
      content: "GroupDocs.Watermark for Python via .NET は、PDF、Word、Excel、PowerPoint などの MS Office ドキュメント、JPEG、PNG、GIF、BMP、Visio 図、電子メールなどの画像を含む幅広いファイル形式をサポートしています。ビジネスに合わせてドキュメント処理を強化します。目標。"

    # feature loop
    - title: "ウォーターマークの検索と更新"
      content: "ドキュメントに配置された透かしを取得および更新します。テキストスタイルや画像コンテンツを変更するか、それらを完全に削除します。 GroupDocs.Watermark for Python via .NET は、幅広い透かし処理機能を提供します。"

############################# Platforms ############################
platforms:
  enable: true
  title: "プラットフォーム独立性"
  description: "GroupDocs.Watermark for Python via .NET は、さまざまなオペレーティング システムやパッケージ マネージャーとシームレスに統合します。"
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "対応ファイル形式"
  description: |
    GroupDocs.Watermark for Python via .NET を使用すると、さまざまなファイル形式を処理できます。 [完全なリストを確認](https://docs.groupdocs.com/watermark/net/supported-document-formats/)。
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office および OpenDocument フォーマット
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### イメージとグラフィックス
        * **人気の画像フォーマット:** BMP, JPG, JPEG, PNG
        * **複数ページの画像:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### その他
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark for Python via .NET の機能"
  description: "プログラムによる透かしを使用してドキュメントのセキュリティを強化します。 PDF、DOCX、XLSX、PPTX、画像形式 (PNG、JPG など) を含むさまざまなファイル形式を処理します。"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "正確な透かし制御"
      content: "さまざまなファイル形式内の特定のセクション、ドキュメント全体、または個々の添付ファイルや図形に対してウォーターマークを追加または削除することで、ウォーターマークを正確に管理します。"

    # feature loop
    - icon: "watermark_style"
      title: "透かしの外観をカスタマイズする"
      content: "ドキュメント内の色、フォント、不透明度、回転、位置などの属性を変更することで、透かしの美しさをきめ細かく制御できます。"

    # feature loop
    - icon: "hidden_print"
      title: "PDF の透かしを印刷する"
      content: "通常の文書に隠し透かしを追加し、印刷プロセス中にのみ表示されるようにして、文書のセキュリティを目立たなく強化します。"

    # feature loop
    - icon: "image_only"
      title: "特定の画像の透かし"
      content: "当社のソリューションを使用して、ドキュメント内の特定の画像に透かしを入れます。指定されたセクション (ページ、スライドなど) または文書全体に透かしを埋め込みます。"

    # feature loop
    - icon: "image_frame"
      title: "多層画像の透かし"
      content: "マルチフレーム画像形式内の特定のフレームに正確に透かしを追加し、透かしの配置をきめ細かく制御できます。"

    # feature loop
    - icon: "attachments"
      title: "包括的なコンテンツ保護"
      content: "Excel ドキュメント内の添付ファイルやプレゼンテーション内の画像図形など、さまざまなドキュメント要素に保護を拡張し、追加のセキュリティ層を提供します。"

    # feature loop
    - icon: "pdf_objects"
      title: "高度な PDF 透かし"
      content: "ブリード ボックス、アート ボックス、クロップ ボックス、トリム ボックスなど、PDF のさまざまな領域に透かしを入れます。"

    # feature loop
    - icon: "doc_background"
      title: "背景画像の透かし"
      content: "スプレッドシートやプレゼンテーションの背景画像内の透かしを管理し、視覚的なセキュリティ対策のための追加のカスタマイズ オプションを提供します。"

    # feature loop
    - icon: "unreadable_characters"
      title: "判読できない文字を含むテキスト透かし"
      content: "プレゼンテーションに埋め込まれたテキスト透かし内に判読できない文字を使用し、不正な透かし抽出を大幅に困難にすることでセキュリティを強化します。"

    # feature loop
    - icon: "watermark_text_search"
      title: "高度なウォーターマーク検索"
      content: "包括的な検索機能を使用して、特定のパラメーターに基づいて、またはさまざまな基準を組み合わせて、ドキュメント内のウォーターマークを見つけます。"

    # feature loop
    - icon: "watermark_image_search"
      title: "類似画像の透かし検出"
      content: "ドキュメント内でソース画像に視覚的に似ている類似の透かし画像を見つけます。"

    # feature loop
    - icon: "document_info"
      title: "文書情報の分析"
      content: "ページ設定などの重要な文書データを抽出して、さらに分析します。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "コードサンプル"
  description: "一般的な GroupDocs.Watermark for Python via .NET 機能を紹介するコード例をご覧ください。"
  items:
    # code sample loop
    - title: "文書に画像の透かしを入れる"
      content: |
        GroupDocs.Watermark for Python via .NET を使用して、画像の透かしを追加してドキュメントを保護します。 [詳細](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/)。
        {{< landing/code title="画像ウォーターマークでファイルを保護する方法">}}
        ```python {style=abap}

        # ソースドキュメントをウォーターマーカーに読み込み
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # ウォーターマーク画像へのパスを指定
            watermark = groupdocs.watermark.watermarks.ImageWatermark("watermark.jpg")
            watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwgroupdocs.watermark.common.VerticalAlignment.CENTER

            # ファイルを保護して保存する
            watermarker.add(watermark)
            watermarker.save("result.pdf")
       
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "既存のウォーターマークの検索と変更"
      content: |
        GroupDocs.Watermark for Python via .NET を使用すると、ドキュメントの透かしを管理できます。ウォーターマークを選択し、そのプロパティを変更します。 [方法を確認](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/)。
        {{< landing/code title="ウォーターマークの検索と変更。">}}
        ```python {style=abap}

        # ソースドキュメントをロード
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # 更新するウォーターマークを検索する
            search_criteria = groupdocs.watermark.search.searchcriteria.TextSearchCriteria("annotation", False)
            watermarks = watermarker.search(search_criteria)
            
            # 必要なプロパティを更新
            for watermark in watermarks:
                watermark.text = "passed"

            # 変更したドキュメントを指定したパスに保存
            watermarker.save("result.pdf")


        ```
        {{< /landing/code >}}

---
