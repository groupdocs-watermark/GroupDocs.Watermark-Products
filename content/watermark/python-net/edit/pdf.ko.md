
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:29
draft: false
lang: ko
format: Pdf
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "GroupDocs.Watermark를 사용한 Pdf의 정확한 워터마크 편집"
head_description: "GroupDocs.Watermark for Python via .NET을 사용하여 Pdf 문서에서 워터마크 내용을 효율적으로 수정하세요."

############################# Header ############################
title: "Python 도구로 Pdf 워터마크 부드럽게 편집" 
description: "GroupDocs.Watermark for Python via .NET 개발 툴킷을 사용하여 PDF를 포함한 워터마크를 커스터마이즈하세요."
subtitle: "GroupDocs.Watermark for Python via .NET 도구" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "PyPi에서 무료로 시도하기"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET 도구"
    link: "/watermark/python-net/"
    link_title: "자세히 알아보기"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **PDF 문서에서 워터마크 업데이트:** GroupDocs.Watermark for Python via .NET 프레임워크를 활용하여 전문적인 포맷을 유지하면서 워터마크를 조정하세요.

############################# Steps ############################
steps:
    enable: true
    title: "Python API를 사용하여 Pdf 문서에서 워터마크 수정"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)**를 사용하여 Python 개발자가 다양한 Pdf 문서에서 워터마크 내용을 수정할 수 있습니다. 빠른 안내는 다음과 같습니다:
      
      1. **Watermarker** 클래스를 사용하여 Pdf 문서를 로드하며, 파일 경로, 메모리 스트림 또는 바이트 배열을 입력으로 받습니다.
      2. 문서에서 기존 워터마크 요소를 찾기 위해 **SearchCriteria** 객체를 작성합니다. 여기에는 텍스트 또는 그래픽 요소가 포함됩니다.
      3. 식별되면, 도구는 업데이트할 수 있는 일치하는 워터마크 인스턴스의 컬렉션을 제공합니다. 색상, 정렬, 글꼴 또는 임베디드 이미지 데이터와 같은 매개변수를 조정하세요.
      4. 변경된 문서를 디스크 또는 지원되는 출력 스트림에 저장하여 프로세스를 완료합니다.
   
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
        # PDF 파일의 이미지 워터마크 업데이트
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # Watermarker 인스턴스를 입력 파일과 함께 생성
        with gw.Watermarker("input.pdf") as watermarker:

            # 이미지 기반 워터마크를 찾기 위해 SearchCriteria 사용
            search_criteria = gwss.ImageDctHashSearchCriteria("logo.png")

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # 이미지 워터마크에 변경 사항 적용
                        watermark.ImageData = imageData
                    except Exception as e:
                        pass

            # 업데이트된 PDF 파일 내보내기
            watermarker.save("output.pdf")
        ```     

############################# More features ############################
more_features:
  enable: true
  title: "고급 워터마킹 도구로 생산성 향상"
  description: "Python에서 문서 브랜딩과 보호를 가속화하는 동적 워터마킹 API입니다. 최소한의 노력으로 워터마크 레이어를 삽입, 감지, 수정 또는 삭제할 수 있습니다."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "고급 워터마크 편집 작업 흐름"
  features:
    # feature loop
    - title: "통합된 워터마크 제어"
      content: "GroupDocs.Watermark for Python via .NET를 사용하여 Python 애플리케이션에서 전체 워터마크 생애 주기 제어를 제공합니다. 워터마크 설정, 업데이트 및 제거를 자동화하여 반복 작업을 피하세요."

    # feature loop
    - title: "워터마크 속성의 정밀 조정"
      content: "워터마크의 미적 요소를 완벽하게 제어하세요—크기 조정, 색상 변경, 회전 또는 재배치하여 모든 시각적 요구 사항을 충족할 수 있습니다."

    # feature loop
    - title: "네이티브 형식 기능 활용"
      content: "헤더, 푸터, 주석 또는 배경에 워터마크를 포함시켜 모든 파일 형식에 적응하세요. 우리의 API는 최적의 통합을 위해 네이티브 구조를 존중합니다."
      
  code_samples:
    # code sample loop
    - title: "PDF 파일에서 워터마크 수정"
      content: |
        PDF 문서에서 워터마크 속성을 변경하는 방법을 보여줍니다.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # PDF 파일 열기
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.pdf as gwop

        # 워터마크 내용 읽기
        load_options = gwop.PdfLoadOptions()
        with gw.Watermarker("source.pdf", load_options) as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,5,8]

            # 워터마크 업데이트 적용
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
        
            # 편집된 결과 저장
            watermarker.save("output.pdf")
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
    title: "여러 형식에서의 워터마크 조정"
    exclude: "PDF"
    description: "GroupDocs.Watermark for Python via .NET의 신뢰할 수 있는 API를 통해 워터마킹을 위한 폭넓은 형식 지원을 누리세요."
    items: 
        # format loop 1
        - name: "워터마크 PDF"
          format: "PDF"
          link: "/watermark/python-net/edit//pdf/"
          description: "어도비 Portable 문서 형식"

        # format loop 2
        - name: "워터마크 Word"
          format: "WORD"
          link: "/watermark/python-net/edit//word/"
          description: "MS Word 및 오픈 오피스 문서"
          
        # format loop 3
        - name: "워터마크 Excel"
          format: "EXCEL"
          link: "/watermark/python-net/edit//excel/"
          description: "MS Excel 및 오픈 오피스 스프레드시트"

        # format loop 4
        - name: "워터마크 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/edit//powerpoint/"
          description: "MS PowerPoint 및 오픈 오피스 프레젠테이션"

        # format loop 5
        - name: "워터마크 DOCX"
          format: "DOCX"
          link: "/watermark/python-net/edit//docx/"
          description: "마이크로소프트 Word 오픈 XML 문서"
          
        # format loop 6
        - name: "워터마크 PPTX"
          format: "PPTX"
          link: "/watermark/python-net/edit//pptx/"
          description: "PowerPoint 오픈 XML 프레젠테이션"
          
        # format loop 7
        - name: "워터마크 XLSX"
          format: "XLSX"
          link: "/watermark/python-net/edit//xlsx/"
          description: "마이크로소프트 Excel 오픈 XML 스프레드시트"

        # format loop 8
        - name: "워터마크 DOC"
          format: "DOC"
          link: "/watermark/python-net/edit//doc/"
          description: "마이크로소프트 Word 97 - 2007 문서"

        # format loop 9
        - name: "워터마크 XLS"
          format: "XLS"
          link: "/watermark/python-net/edit//xls/"
          description: "마이크로소프트 Excel 워크북 97-2003"

        # format loop 10
        - name: "워터마크 PPT"
          format: "PPT"
          link: "/watermark/python-net/edit//ppt/"
          description: "PowerPoint 프레젠테이션 97-2003"

        # format loop 11
        - name: "워터마크 RTF"
          format: "RTF"
          link: "/watermark/python-net/edit//rtf/"
          description: "리치 텍스트 포맷"

---