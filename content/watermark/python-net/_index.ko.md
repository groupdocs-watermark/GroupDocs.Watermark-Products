---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:49
draft: false

lang: ko
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
head_title: "Python 워터마킹 라이브러리 | 문서 워터마크"
head_description: "Python는 텍스트 및 이미지 워터마크로 비즈니스 문서를 보호합니다. PDF, Word, Excel, PowerPoint와 같은 파일 형식이 지원됩니다."

############################# Header ############################
title: "Python via .NET 워터마킹 기술에 액세스하세요"
description: "이 Python 솔루션으로 데이터를 보호하고 무단 복사를 방지하세요. PDF, Word, Excel, PowerPoint, 이미지 등 다양한 형식의 비즈니스 문서에 워터마크를 쉽게 추가할 수 있습니다."
words:
  for: "...에 대한"

actions:
  main: "PyPi 무료 다운로드"
  main_link: "https://pypi.org/project/groupdocs-watermark-net/"
  alt: "라이선싱"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Watermark 기능을 무료로 체험하거나 라이선스를 요청하세요"

release:
  title: "버전 {0} 출시"
  notes: "새 소식 보기"
  downloads: "다운로드"
  link: "https://releases.groupdocs.com/watermark/python-net/"

code:
  title: "Python을 사용하여 PDF에 워터마크 추가"
  more: "더 많은 예시"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
  install: "pip install groupdocs-watermark-net"
  content: |
    ```python {style=abap}

    import groupdocs.watermark as gw
    import groupdocs.watermark.watermarks as gww
    import groupdocs.watermark.options.pdf as gwop
    import groupdocs.watermark.common as gwc

    # PDF 경로를 통과하는 워터마커 인스턴스화
    pdf_lo = gwop.PdfLoadOptions()
    with gw.Watermarker("source.pdf", pdf_lo) as watermarker:
        options = gwop.PdfArtifactWatermarkOptions()

        # 워터마크 옵션 사용자 지정
        text_watermark = 
            gww.TextWatermark("Approved", gww.Font("Arial", 8.0))
        text_watermark.horizontal_alignment = 
            gwc.HorizontalAlignment.RIGHT

        # PDF 문서에 워터마크 적용
        watermarker.add(text_watermark, options)

        # 결과 문서 저장
        watermarker.save("result.pdf")

    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark 한 눈에"
  description: "워터마킹용 Python 라이브러리"
  features:
    # feature loop
    - title: "Python 문서 워터마킹"
      content: "GroupDocs.Watermark for Python via .NET으로 민감한 데이터를 보호하세요. 다양한 파일 형식의 텍스트나 이미지를 워터마크로 삽입하세요."

    # feature loop
    - title: "워터마크 사용자 정의"
      content: "GroupDocs.Watermark for Python via .NET에서는 다양한 맞춤설정 옵션을 사용할 수 있습니다. 텍스트 스타일(굵게, 기울임꼴, 글꼴)이나 크기나 회전과 같은 이미지 속성을 설정하여 문서 워터마킹을 조정하세요."

    # feature loop
    - title: "인기 있는 파일 형식 지원"
      content: "GroupDocs.Watermark for Python via .NET은(는) PDF, Word, Excel, PowerPoint 등의 MS Office 문서와 JPEG, PNG, GIF, BMP, Visio 다이어그램, 이메일 등의 이미지를 포함한 광범위한 파일 형식을 지원합니다. 비즈니스에 맞게 문서 처리를 향상하세요. 목표."

    # feature loop
    - title: "워터마크 검색 및 업데이트"
      content: "문서에 배치된 워터마크를 검색하고 업데이트합니다. 텍스트 스타일, 이미지 콘텐츠를 수정하거나 완전히 제거하세요. GroupDocs.Watermark for Python via .NET은 광범위한 워터마크 처리 기능을 제공합니다."

############################# Platforms ############################
platforms:
  enable: true
  title: "플랫폼 독립성"
  description: "GroupDocs.Watermark for Python via .NET은 다양한 운영 체제 및 패키지 관리자와 원활하게 통합됩니다."
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
  title: "지원되는 파일 형식"
  description: |
    GroupDocs.Watermark for Python via .NET을(를) 사용하면 다양한 범위의 파일 형식을 처리할 수 있습니다. [전체 목록 살펴보기](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office 및 OpenDocument 형식
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### 이미지 및 그래픽
        * **인기 이미지 형식:** BMP, JPG, JPEG, PNG
        * **여러 페이지 이미지:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### 기타
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark for Python via .NET 기능"
  description: "프로그래밍 방식의 워터마킹을 통해 문서 보안을 강화합니다. PDF, DOCX, XLSX, PPTX 및 이미지 형식(PNG, JPG 등)을 포함한 다양한 파일 형식을 처리합니다."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "정확한 워터마킹 제어"
      content: "다양한 파일 형식 내의 특정 섹션, 전체 문서, 개별 첨부 파일 및 도형에서 워터마크를 추가하거나 제거하여 정밀하게 관리하세요."

    # feature loop
    - icon: "watermark_style"
      title: "워터마크 모양 사용자 정의"
      content: "문서 내에서 색상, 글꼴, 불투명도, 회전, 위치 지정과 같은 속성을 수정하여 워터마크 미학을 세밀하게 제어할 수 있습니다."

    # feature loop
    - icon: "hidden_print"
      title: "PDF 워터마킹 인쇄"
      content: "인쇄 프로세스 중에만 표시되는 숨겨진 워터마크를 일반 문서에 추가하여 문서 보안을 눈에 띄게 강화합니다."

    # feature loop
    - icon: "image_only"
      title: "특정 이미지 워터마킹"
      content: "당사 솔루션을 사용하여 문서 내의 특정 이미지에 워터마크를 표시하세요. 지정된 섹션(예: 페이지, 슬라이드) 또는 전체 문서에 워터마크를 삽입합니다."

    # feature loop
    - icon: "image_frame"
      title: "다중 레이어 이미지 워터마크"
      content: "다중 프레임 이미지 형식 내의 특정 프레임에 워터마크를 정확하게 추가하여 워터마크 배치를 세부적으로 제어할 수 있습니다."

    # feature loop
    - icon: "attachments"
      title: "포괄적인 콘텐츠 보호"
      content: "Excel 문서 내의 첨부 파일, 프레젠테이션 내의 이미지 모양 등 다양한 문서 요소로 보호를 확장하여 추가 보안 계층을 제공합니다."

    # feature loop
    - icon: "pdf_objects"
      title: "고급 PDF 워터마킹"
      content: "재단 물림 상자, 아트 상자, 자르기 상자, 자르기 상자 등을 포함하여 PDF의 다양한 영역에 워터마크를 표시합니다."

    # feature loop
    - icon: "doc_background"
      title: "배경 이미지 워터마킹"
      content: "스프레드시트 및 프리젠테이션의 배경 이미지 내에서 워터마크를 관리하고 시각적 보안 조치를 위한 추가 사용자 정의 옵션을 제공합니다."

    # feature loop
    - icon: "unreadable_characters"
      title: "읽을 수 없는 문자가 포함된 텍스트 워터마크"
      content: "프레젠테이션에 포함된 텍스트 워터마크 내에 읽을 수 없는 문자를 사용하여 무단 워터마크 추출을 훨씬 더 어렵게 만들어 보안을 강화합니다."

    # feature loop
    - icon: "watermark_text_search"
      title: "고급 워터마크 검색"
      content: "포괄적인 검색 기능을 사용하여 특정 매개변수를 기반으로 하거나 다양한 기준을 결합하여 문서에서 워터마크를 찾습니다."

    # feature loop
    - icon: "watermark_image_search"
      title: "유사 이미지 워터마크 감지"
      content: "원본 이미지와 시각적으로 유사한 문서 내에서 유사한 워터마크 이미지를 찾습니다."

    # feature loop
    - icon: "document_info"
      title: "문서 정보 분석"
      content: "추가 분석을 위해 페이지 설정과 같은 필수 문서 데이터를 추출합니다."

############################# Code samples ############################
code_samples:
  enable: true
  title: "코드 샘플"
  description: "일반적인 GroupDocs.Watermark for Python via .NET 기능을 보여주는 코드 예제를 살펴보세요."
  items:
    # code sample loop
    - title: "이미지로 문서 워터마킹"
      content: |
        이미지 워터마크를 추가하여 문서를 보호하려면 GroupDocs.Watermark for Python via .NET을(를) 사용하세요. [자세히 알아보기](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="이미지 워터마크로 파일을 보호하는 방법">}}
        ```python {style=abap}

        # 워터마커에 소스 문서 불러오기
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # 워터마크 이미지의 경로 지정
            watermark = groupdocs.watermark.watermarks.ImageWatermark("watermark.jpg")
            watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwgroupdocs.watermark.common.VerticalAlignment.CENTER

            # 파일을 보호하고 저장합니다.
            watermarker.add(watermark)
            watermarker.save("result.pdf")
       
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "기존 워터마크 검색 및 수정"
      content: |
        GroupDocs.Watermark for Python via .NET을 사용하면 문서 워터마크를 관리할 수 있습니다. 워터마크를 선택하고 해당 속성을 수정합니다. [방법을 알아보세요](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/).
        {{< landing/code title="워터마크 검색 및 수정.">}}
        ```python {style=abap}

        # 소스 문서 불러오기
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # 업데이트할 워터마크 검색
            search_criteria = groupdocs.watermark.search.searchcriteria.TextSearchCriteria("annotation", False)
            watermarks = watermarker.search(search_criteria)
            
            # 원하는 속성 업데이트
            for watermark in watermarks:
                watermark.text = "passed"

            # 수정한 문서를 지정된 경로에 저장
            watermarker.save("result.pdf")


        ```
        {{< /landing/code >}}

---
