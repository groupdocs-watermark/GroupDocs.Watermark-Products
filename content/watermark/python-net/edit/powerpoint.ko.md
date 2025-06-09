
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: ko
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Powerpoint 파일에서 워터마크 편집"
head_description: "GroupDocs.Watermark for Python via .NET을 사용하여 Powerpoint 프레젠테이션에서 워터마크 콘텐츠를 신속하게 변경하고 문서를 안전하게 유지하십시오."

############################# Header ############################
title: "Python에서 Powerpoint 워터마크 정밀 편집" 
description: "GroupDocs.Watermark for Python via .NET을 사용하여 프레젠테이션에서 워터마크의 레이아웃과 가시성을 완전히 제어하십시오."
subtitle: "GroupDocs.Watermark for Python via .NET 라이브러리" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "PyPi에서 무료 다운로드"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET API"
    link: "/watermark/python-net/"
    link_title: "자세히 알아보기"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **Powerpoint 파일에서 워터마크 레이아웃 제어:** GroupDocs.Watermark for Python via .NET을 사용하여 필요한 위치에 워터마크를 정확하게 배치하고 손쉽게 프레젠테이션을 보호할 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "Python을 사용하여 Powerpoint 문서의 워터마크 수정"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)**은 Python 개발자가 다양한 Powerpoint 파일에서 워터마크를 업데이트할 수 있도록 도와줍니다. 사용 방법은 다음과 같습니다:
      
      1. 먼저, **Watermarker** 생성자에 Powerpoint 파일을 전달하여 열어야 합니다. 파일 경로, 바이트 스트림 또는 파일 스트림을 사용할 수 있습니다.
      2. 그런 다음, 워터마크 텍스트나 속성을 검색할 수 있게 해주는 **SearchCriteria**를 사용하여 변경하고자 하는 워터마크를 찾습니다.
      3. 찾은 후에는 텍스트, 글꼴, 크기, 위치, 색상 등과 같은 세부 정보를 변경할 수 있습니다. 이를 통해 워터마크의 모양을 완전히 제어할 수 있습니다.
      4. 변경한 후에는 문서를 저장해야 합니다. 결과를 스트림이나 파일 경로에 쓸 수 있습니다.
   
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
        # POWERPOINT에서 워터마크 텍스트 업데이트
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # POWERPOINT 파일을 사용하여 Watermarker 생성
        with gw.Watermarker("input.pptx") as watermarker:

            # 워터마크 텍스트를 찾기 위해 TextSearchCriteria 설정
            search_criteria = gwss.TextSearchCriteria("test", False)

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # 워터마크 텍스트 수정
                        watermark.text = "passed"
                    except Exception as e:
                        pass
            
            watermarker.save("output.pptx")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "워터마크 업데이트 방법 더 알아보기"
  description: "우리 라이브러리를 사용하면 Python 앱에서 다양한 파일 형식에 대해 워터마크를 추가, 검색, 편집 또는 삭제할 수 있습니다."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "워터마크 편집"
  features:
    # feature loop
    - title: "간편하게 파일에 워터마크 추가"
      content: "GroupDocs.Watermark for Python via .NET을 사용하여 문서에서 워터마크를 추가하고 관리하십시오. 간단한 API를 사용하여 필요에 따라 워터마크를 검색, 업데이트 또는 제거할 수 있습니다."

    # feature loop
    - title: "필요에 맞게 워터마크 사용자화"
      content: "유연한 API를 사용하여 글꼴, 크기, 방향, 색상과 같은 워터마크 설정을 조정하여 원하는 결과를 얻을 수 있습니다."

    # feature loop
    - title: "형식별 기능 활용"
      content: "파일 형식에 따라 머리글, 바닥글, 주석 또는 배경과 같은 워터마크 영역으로 사용할 수 있는 기본 기능을 사용할 수 있습니다."
      
  code_samples:
    # code sample loop
    - title: "Excel에서 텍스트 워터마크 편집"
      content: |
        이 코드는 Excel 스프레드시트에서 워터마크 텍스트를 변경하는 방법을 보여줍니다.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # XLSX 파일 열기
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # 스프레드시트 데이터 읽기
        with gw.Watermarker("source.xlsx") as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,3]

            # 워터마크 텍스트 변경
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
        
            # 결과 저장
            watermarker.save("output.xlsx")
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
    title: "다른 문서 형식의 워터마크 편집"
    exclude: "POWERPOINT"
    description: "GroupDocs.Watermark for Python via .NET을 사용하여 다양한 문서 형식의 워터마크로 작업할 수 있습니다."
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