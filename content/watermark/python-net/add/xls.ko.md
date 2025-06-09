
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:28
draft: false
lang: ko
format: Xls
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Python로 XLS에 워터마크 추가하기"
head_description: "Python를 사용하여 XLS 파일에 워터마크를 추가하고 관리하여 보안성을 향상하세요."

############################# Header ############################
title: "Python의 XLS 파일을 위한 워터마크 생성하기" 
description: "Python에서 XLS 스프레드시트에 워터마크를 추가하세요. 재무 및 개인 데이터를 보호하기에 적합합니다."
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "PyPi에서 무료로 받기"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "자세히 알아보기"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET는 Python에서 XLS 파일에 워터마크를 추가할 수 있는 도구입니다. 가시적 또는 숨겨진 마크를 사용하고 필요에 맞춰 모양을 사용자 정의하세요. 재무 또는 클라이언트 데이터를 안전하게 유지할 수 있는 GroupDocs.Watermark은 모든 Python 환경에서 작동합니다.

############################# Steps ############################
steps:
    enable: true
    title: "Xls 파일에 워터마크 빠르게 추가하기"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/):** 문서에 워터마크를 추가할 수 있는 강력한 Python 라이브러리입니다.
      
      1. **주 클래스: Watermarker.** 먼저 **Watermarker** 객체를 생성합니다. 시작하려면 Xls 파일을 파일 경로나 스트림으로 전달하세요.
      2. **워터마크 만들기.** 원하는 유형의 워터마크 객체를 만드세요. 문서의 모든 페이지나 이미지, 헤더와 같은 요소에 배치할 수 있습니다.
      3. **모양 조정하기.** 워터마크의 크기, 위치, 글꼴 및 색상을 조정하여 필요에 맞춥니다.
      4. **추가하고 저장하기.** **Watermarker** 메서드를 사용하여 워터마크를 삽입합니다. 원하는 만큼 추가한 후, 원하는 장소에 파일을 저장하세요.
   
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
        # XLS 파일에 이미지 워터마크 추가하기
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # Watermarker 생성자에게 파일 경로 전달하기
        with gw.Watermarker("input.xls") as watermarker:

            # 이미지 파일을 사용하여 이미지 워터마크 만들기
            watermark = gww.ImageWatermark("watermark.png")

            watermarker.add(watermark)

            # 워터마크가 포함된 XLS 파일 저장하기
            watermarker.save("output.xls")
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "더 많은 워터마킹 도구 발견하기"
  description: "GroupDocs.Watermark for Python via .NET는 다양한 파일 형식에서 워터마크를 추가하고 사용자 정의할 수 있는 고급 옵션을 제공합니다. 유연하고 사용하기 쉬운 기능으로 문서와 이미지를 보호하세요."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "올인원 워터마킹"
  features:
    # feature loop
    - title: "전체 페이지 타일링"
      content: "타일된 워터마크로 전체 문서를 덮으세요. 이렇게 하면 워터마크를 제거하기가 어려워지고 레이아웃을 손상시키지 않으면서 파일을 안전하게 유지할 수 있습니다."

    # feature loop
    - title: "사용자 정의 색상"
      content: "브랜드나 문서 스타일에 맞는 색상을 선택하세요. 워터마크가 두드러지게 하거나 필요에 따라 조화롭게 만들 수 있습니다."

    # feature loop
    - title: "추가 보안 옵션"
      content: "다층 워터마크로 문서 보안을 강화하세요. 가시적 및 숨겨진 마크를 결합하여 복사를 방지하고 올바른 사람만 파일에 접근할 수 있도록 합니다."
      
  code_samples:
    # code sample loop
    - title: "PowerPoint에 워터마크 추가하기"
      content: |
        이 샘플은 PPTX 슬라이드 배경에 워터마크를 추가하는 방법을 보여줍니다.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.presentation as gwop

        # PPTX 파일 열기
        load_options = gwop.PresentationLoadOptions()
        with gw.Watermarker("source.pptx", load_options) as watermarker:

            # 워터마크 세부정보 설정하기
            with TextWatermark("Protected image", gww.Font("Arial", 8.0)) as watermark:

                watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
                watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
                watermark.rotate_angle = 45
                watermark.scale_factor = 1

                # 슬라이드 배경에 워터마크 적용하기
                watermarker.add(watermark)

                # 업데이트된 프레젠테이션 저장하기
                watermarker.save("result.pptx")
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
    title: "Python로 XLS에 워터마크 추가하기"
    exclude: "XLS"
    description: "Python를 사용하여 XLS 파일에 사용자 정의 워터마크를 추가하여 Excel 데이터를 안전하게 보호하세요."
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