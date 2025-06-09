
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: ko
format: Photo
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "사진에 워터마크 쉽게 추가하기"
head_description: "Python를 사용하여 사진에 워터마크를 추가하여 작업과 저작권을 보호하세요."

############################# Header ############################
title: "Python로 빠른 사진 워터마킹" 
description: "우리의 Python 라이브러리를 사용하여 사진에 워터마크를 빠르게 추가하세요. 저작권과 브랜드를 보호하면서 이미지 품질을 유지합니다."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료로 PyPi 다운로드"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "자세히 알아보기"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET는 자신의 작업을 보호하려는 사진작가에게 최적입니다. JPEG, PNG, RAW와 같은 형식의 사진에 텍스트 또는 이미지 워터마크를 추가할 수 있습니다. 워터마크의 투명도, 크기 및 위치를 조정하여 완벽하게 맞추고 사진의 외관도 유지하세요.

############################# Steps ############################
steps:
    enable: true
    title: "Python로 워터마크 추가하기"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)**는 다양한 비즈니스 파일 형식에 워터마크를 추가하는 경우를 간편하게 만들어주는 라이브러리입니다. Python에서 문서에 워터마크를 빠르게 추가하려면 다음 단계를 따르십시오:
      
      1. **워터마킹 시작하기:** **Watermarker** 클래스의 인스턴스를 생성하는 것으로 시작합니다. 생성자에 워터마크를 추가할 Photo 파일을 경로 또는 스트림으로 전달하여 엽니다.
      2. **워터마크 만들기:** 원하는 텍스트와 설정으로 **Watermark** 객체를 만드세요. 각 페이지나 문서의 헤더 및 첨부 파일과 같은 요소에 워터마크를 추가할 수 있습니다.
      3. **워터마크 사용자 정의:** 워터마크의 크기, 위치, 글꼴, 색상 및 정렬을 조정하여 필요에 맞게 조정하십시오. 이는 문서에 워터마크를 적절히 보이게 합니다.
      4. **적용 및 저장:** **Watermarker** 메서드를 사용하여 문서에 워터마크를 추가합니다. 결과를 저장하고, 안전을 위해 새 파일에 저장하는 것이 좋습니다.
   
    code:
      platform: "python-net"
      copy_title: "복사"
      install:
        command: |
        command: "pip install groupdocs-watermark-net"
        copy_tip: "클릭하여 복사"
        copy_done: "복사"
      links:
        #  loop
        - title: "더 많은 예시"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
        #  loop
        - title: "문서화"
          link: "https://docs.groupdocs.com/watermark/python-net/"
          
      content: |
        ```python {style=abap}
        # PHOTO 파일에 텍스트 워터마크 추가
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # 워터마크를 추가할 파일 선택
        with gw.Watermarker("input.png") as watermarker:

            # 텍스트 워터마크 객체 생성
            font = gww.Font("Arial", 36.0)
            watermark = gww.TextWatermark("top secret", font)
            watermark.foreground_color = gww.Color.red
            watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
            watermark.opacity = 0.4

            watermarker.add(watermark)

            # 업데이트된 PHOTO 파일 저장
            watermarker.save("output.png")
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "추가 워터마킹 기능 탐색"
  description: "우리의 Python API를 사용하여 문서, 슬라이드, 다이어그램 등에서 워터마크를 추가하고, 보기, 변환 및 관리하십시오. GroupDocs.Watermark for Python via .NET은 파일을 보호하고 저작권 정보를 쉽게 추가할 수 있도록 도와줍니다."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "워터마크 추가"
  features:
    # feature loop
    - title: "워터마크를 쉽게 추가하세요"
      content: "GroupDocs.Watermark는 Python 개발자가 비즈니스 문서에 텍스트, 이미지 또는 동적 워터마크를 빠르게 추가할 수 있게 해줍니다. 최소한의 노력으로 파일을 안전하고 브랜드화하세요."

    # feature loop
    - title: "완전한 사용자 정의가 가능한 워터마크"
      content: "GroupDocs.Watermark로 워터마크의 크기, 회전, 투명도, 색상 및 글꼴을 변경할 수 있습니다. 워터마크를 문서에 완벽하게 맞추고 중요한 콘텐츠는 가시성을 유지하세요."

    # feature loop
    - title: "워터마킹을 위한 문서 기능 사용하기"
      content: "PDF 주석, 워드 배경 또는 엑셀 헤더와 같은 내장 문서 기능을 활용하여 워터마크를 추가할 수 있습니다. GroupDocs.Watermark은 효과적이고 비침해적인 워터마킹을 위해 문서 구조와 함께 작동합니다."
      
  code_samples:
    # code sample loop
    - title: "DOCX에 이미지 워터마크 추가"
      content: |
        이 예제는 형태 워터마크에 이미지 효과를 적용하는 방법을 보여줍니다.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.wordprocessing as gwow

        # 워드 문서 열기
        load_options = gwow.WordProcessingLoadOptions()
        with gw.Watermarker("source.docx", load_options) as watermarker:

            # 워터마크 옵션 설정
            with gww.ImageWatermark("logo.png") as watermark:

                effects = gwow.WordProcessingImageEffects()
                effects.brightness = 0.7
                effects.contrast = 0.6
                effects.chroma_key = gww.Color.red

                options = gwow.WordProcessingWatermarkSectionOptions()
                options.Effects = effects;

                # 워터마크 생성
                watermarker.add(watermark, options)

                # 워터마크가 포함된 문서 저장
                watermarker.save("result.docx")
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Watermark 기능을 무료로 체험하거나 라이선스를 요청하세요"
  items:
    #  loop
    - title: "PyPi 다운로드"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      color: "red"
        #  loop
    - title: "라이선싱"
      link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Python으로 사진에 워터마크 추가"
    exclude: "PHOTO"
    description: "우리의 Python API를 사용하여 사진에 맞춤형 워터마크를 추가하세요. 이미지를 안전하고 전문적으로 유지하세요."
    items: 
        # format loop 1
        - name: "워터마크 PDF"
          format: "PDF"
          link: "/watermark/python-net/add//pdf/"
          description: "어도비 Portable 문서 형식"

        # format loop 2
        - name: "워터마크 Word"
          format: "WORD"
          link: "/watermark/python-net/add//word/"
          description: "MS Word 및 오픈 오피스 문서"
          
        # format loop 3
        - name: "워터마크 Excel"
          format: "EXCEL"
          link: "/watermark/python-net/add//excel/"
          description: "MS Excel 및 오픈 오피스 스프레드시트"

        # format loop 4
        - name: "워터마크 이미지"
          format: "IMAGE"
          link: "/watermark/python-net/add//image/"
          description: "인기 이미지 형식"

        # format loop 5
        - name: "워터마크 사진"
          format: "PHOTO"
          link: "/watermark/python-net/add//photo/"
          description: "사진 형식"

        # format loop 6
        - name: "워터마크 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/add//powerpoint/"
          description: "MS PowerPoint 및 오픈 오피스 프레젠테이션"

        # format loop 7
        - name: "워터마크 DOCX"
          format: "DOCX"
          link: "/watermark/python-net/add//docx/"
          description: "마이크로소프트 Word 오픈 XML 문서"
          
        # format loop 8
        - name: "워터마크 PPTX"
          format: "PPTX"
          link: "/watermark/python-net/add//pptx/"
          description: "PowerPoint 오픈 XML 프레젠테이션"
          
        # format loop 9
        - name: "워터마크 XLSX"
          format: "XLSX"
          link: "/watermark/python-net/add//xlsx/"
          description: "마이크로소프트 Excel 오픈 XML 스프레드시트"

        # format loop 10
        - name: "워터마크 JPEG"
          format: "JPEG"
          link: "/watermark/python-net/add//jpeg/"
          description: "JPEG 이미지"

        # format loop 11
        - name: "워터마크 PNG"
          format: "PNG"
          link: "/watermark/python-net/add//png/"
          description: "Portable 네트워크 그래픽"

        # format loop 12
        - name: "워터마크 TIFF"
          format: "TIFF"
          link: "/watermark/python-net/add//tiff/"
          description: "태그 이미지 파일 형식"

        # format loop 13
        - name: "워터마크 WEBP"
          format: "WEBP"
          link: "/watermark/python-net/add//webp/"
          description: "웹 사진"

        # format loop 14
        - name: "워터마크 DOC"
          format: "DOC"
          link: "/watermark/python-net/add//doc/"
          description: "마이크로소프트 Word 97 - 2007 문서"

        # format loop 15
        - name: "워터마크 XLS"
          format: "XLS"
          link: "/watermark/python-net/add//xls/"
          description: "마이크로소프트 Excel 워크북 97-2003"

        # format loop 16
        - name: "워터마크 PPT"
          format: "PPT"
          link: "/watermark/python-net/add//ppt/"
          description: "PowerPoint 프레젠테이션 97-2003"

        # format loop 17
        - name: "워터마크 RTF"
          format: "RTF"
          link: "/watermark/python-net/add//rtf/"
          description: "리치 텍스트 포맷"

---