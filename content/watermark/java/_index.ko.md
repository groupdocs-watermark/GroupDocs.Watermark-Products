---
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

head_title: "PDF Word Excel 이미지에 워터마크 제거 검색을 추가하는 Java API"
head_description: "Java 문서 워터마킹 API – 문서에서 워터마크 생성, 검색 및 제거: PDF, Word, Excel, 프레젠테이션, Visio, 이메일 및 이미지 파일 형식."

title: "워터마크를 조작하는 Java API"
description: "스마트 검색 및 강력한 보안으로 이미지 및 텍스트 워터마킹 작업을 수행하는 Java 애플리케이션 개발."
button:
    enable: true

submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Watermark for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-watermark-java.png"
        product: "GroupDocs.Watermark"
        platform: "Java"

    middle:
        button:
            - link: "#overview"
              text: "개요"

            - link: "#features"
              text: "특징"

            - link: "#support"
              text: "지원하다"

            - link: "https://products.groupdocs.app/watermark"
              text: "라이브 데모"

            - link: "https://purchase.groupdocs.com/pricing/watermark/java"
              text: "가격"

    right:
        link_download: "https://downloads.groupdocs.com/watermark"
        link_learn: "https://docs.groupdocs.com/watermark/java/"
        link_buy: "https://purchase.groupdocs.com"

overview:
    enable: true
    content: |
      Java용 GroupDocs.Watermark를 사용하면 최종 사용자가 지원되는 형식의 파일에서 새 워터마크를 적용하고 기존 워터마크를 검색 및 삭제할 수 있도록 하는 비즈니스 응용 프로그램을 만들 수 있습니다. 프로그래밍 방식으로 디지털 워터마크를 많은 파일 형식에 할당하고 강력한 스마트 검색 기능을 활용할 수 있습니다. GroupDocs.Watermark for Java는 민감한 정보나 지적 재산 콘텐츠가 포함된 디지털 문서의 오용을 방지하기 위해 사용할 수 있는 다양한 기본 제공 보안 조치를 제공합니다.
    tabs:
      enable: true     
      
      tab_one:
        description: |
          다음은 Java용 GroupDocs.Watermark의 개요입니다.

        rright:
          enable: true
          icon: "fab fa-html5"
          title: "개요"
          content: |
            * 워터마크 추가 및 제거
            * 워터마크 검색 및 바꾸기
            * 서식으로 검색
            * 이미지 비교로 검색
            * 머리글 및 바닥글 작업
            * 배경 이미지 작업
            * 첨부 파일 작업
            * 페이지 래스터화
            * 편집 제한 적용
      
      tab_two:
        description: |
          각 형식에 대해 지원되는 [문서 형식 및 워터마크 유형](https://docs.groupdocs.com/watermark/java/supported-document-formats/)은 다음과 같습니다.

        left:
          enable: true
          table:
            - title: "마이크로 소프트 오피스"
              content: |
                * **단어:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT‎
                * **엑셀:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **파워포인트:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
                * **Visio:** VSD, VDX, VSS, VSSX, VSX, VST, VSTX, VTX, VSDX, VDW, VSTM, VSSM, VSDM

            - title: "워터마크 추가"
              content: |
                * **PDF**: XObject, 아티팩트, 주석
                * **단어**: 모양
                * **Excel**: 도형, 머리글 및 바닥글
                * **파워포인트**: 모양
                * **Visio**: 모양
                * **래스터 이미지**: 텍스트, 이미지
                * **여러 페이지 Tiff**: 텍스트, 이미지
                * **애니메이션 GIF**: 텍스트, 이미지

        right:
          enable: true
          table:
            - title: "PDF 및 이미지 문서"
              content: |
                * **Portable Document Format**: PDF
                * **문서 열기**: ODT
                * **이메일**: EML, MSG, EMLX, OFT
                * **이미지**: PNG, BMP, GIF, JPG, JPEG, JP2, TIF, TIFF, WebP

            - title: "워터마크 제거"
              content: |
                * **PDF**: XObject, 아티팩트, 주석, 일반 텍스트
                * **단어**: 모양, 일반 텍스트
                * **Excel**: 도형, 머리글 및 바닥글, 배경 이미지, 셀의 텍스트 및 수식
                * **파워포인트**: 모양
                * **Visio**: 모양, 다이어그램 설명
                * **이메일**: 첨부 및 포함된 이미지, 제목 및 본문 텍스트 조각

      tab_three:
        description: |
          Java용 GroupDocs.Watermark는 다음 운영 체제, 프레임워크 및 패키지 ‎관리자:‎를 지원합니다.
        
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "운영체제"
              content: |
                * 마이크로소프트 윈도우 데스크탑
                * 마이크로소프트 윈도우 서버
                * 리눅스
                * 맥 OS

            - icon: "fas fa-code"
              title: "지원되는 프레임워크"
              content: |
                * 자바 7(1.7) 이상

        right:
          enable: true
          table:
            - icon: "fas fa-cogs"
              title: "개발 환경"
              content: |
                * 넷빈
                * IntelliJ 아이디어
                * 이클립스
            - icon: "fas fa-tools"
              title: "빌드 자동화 도구"
              content: |
                * 메이븐

features:
    enable: true
    title: "Java 기능을 위한 GroupDocs.Watermark"

    feature:
      - icon: "fas fa-copy"
        content: "폴더에서 다양한 형식의 모든 문서를 가져오고 워터마크를 적용하거나 제거합니다."

      - icon: "fas fa-eye"
        content: "특정 섹션 또는 전체 문서에서 워터마크 사용 또는 삭제"

      - icon: "fas fa-bolt"
        content: "특정 섹션, 페이지, 슬라이드 또는 문서의 모든 이미지에 워터마크 적용‎"
      
      - icon: "fas fa-file-powerpoint"
        content: "다중 프레임 이미지의 선택된 프레임에 워터마크 첨부"

      - icon: "fas fa-code"
        content: "문서 인쇄 시 표시되도록 PDF에 숨겨진 워터마크 적용"

      - icon: "fas fa-cloud"
        content: "Excel 문서의 첨부 파일 및 슬라이드의 모든 이미지 모양에 워터마크 사용"

      - icon: "fas fa-remove-format"
        content: "슬라이드 또는 Excel 시트의 배경 이미지에서 워터마크 삽입 또는 삭제"

      - icon: "fas fa-comment-slash"
        content: "이메일 또는 PDF 파일의 첨부 파일에서 지원되는 파일로 워터마크 설정"

      - icon: "fas fa-location-arrow"
        content: "PDF 파일에서 XObject, 아티팩트 및 주석으로 워터마크 추가 또는 삭제"

      - icon: "fas fa-border-all"
        content: "특정 서식이 있는 텍스트와 일치하는 워터마크 삭제"

      - icon: "fas fa-wrench"
        content: "특정 이미지와 유사한 이미지 워터마크 찾기"

      - icon: "fas fa-columns"
        content: "글자 사이에 읽을 수 없는 문자가 있어도 텍스트 워터마크 식별"

      - icon: "fas fa-file-word"
        content: "특정 매개변수를 기반으로 하거나 여러 기준을 할당하여 워터마크 찾기"

      - icon: "fas fa-envelope"
        content: "일치하는 텍스트 워터마크를 찾기 위해 글꼴 서식 지정"

      - icon: "fas fa-print"
        content: "워터마크의 절대 크기 및 위치 지정을 위한 페이지, 슬라이드, 셀 치수 가져오기"

      - icon: "fas fa-file-archive"
        content: "지원되는 문서 형식의 머리글 및 바닥글 내부 이미지에 워터마크 적용"

      - icon: "fas fa-lock"
        content: "Word 문서의 이미지 모양에 워터마크 추가 및 워터마크 편집 제한"

      - icon: "fas fa-file-code"
        content: "읽을 수 없는 문자를 사용하여 프레젠테이션의 보안 텍스트 워터마크"
      
      - icon: "fas fa-fill-drip"
        content: "단일 페이지 또는 전체 문서를 래스터화하여 PDF 문서 워터마크 보호"

      - icon: "fas fa-file-excel"
        content: "현재 텍스트 워터마크를 바꿀 때 텍스트 서식 수정"

      - icon: "fas fa-heading"
        content: "PDF 파일의 도련 상자, 아트 상자, 자르기 상자 또는 자르기 상자에 워터마크 정렬"

    more_feature:
      - title: "워터마크 사용"
        content: |
          Java용 GroupDocs.Watermark를 사용하면 다양한 종류의 워터마크로 작업할 수 있습니다. 모든 유형의 워터마크를 추가하는 것은 몇 줄의 코드만으로 충분합니다. 다음 예제에서는 Java를 사용하여 Word 문서에 이미지 워터마크를 추가하는 방법을 공유합니다.
          
          ```java
          Document doc = Document.load(Common.mapSourceFilePath("D://test.docx"));
          Font font = new Font("Times New Roman", 12);
          TextWatermark watermark = new TextWatermark("Test watermark", font);

          // 사이징 유형 설정
          watermark.setSizingType(SizingType.ScaleToParentDimensions);

          // 워터마크 스케일 설정
          watermark.setScaleFactor(0.5);

          doc.addWatermark(watermark);
          doc.save(Common.mapOutputFilePath("D://test.docx"));
          doc.close();
          ```
      - title: "Go에서 다양한 형식의 파일에 워터마크 추가"
        content: "GroupDocs.Watermark for Java API를 사용하면 배치 모드에서 특정 폴더에 있는 모든 문서의 워터마크를 추가하거나 제거할 수 있습니다. 문서 형식이 다른 경우 중요하지 않습니다. Java용 GroupDocs.Watermark는 모든 파일에 워터마크를 정확하게 적용합니다.."

      - title: "워터마크에 완벽한 보안 할당"
        content: "최소한의 코드로 워터마크에 완벽한 보안을 할당하고 제3자 도구가 PDF 파일에서 할당된 워터마크를 수정하거나 제거하는 것을 극도로 어렵게 만들 수 있습니다. Java용 GroupDocs.Watermark를 사용하면 PDF 파일의 모든 페이지를 래스터화된 이미지로 변환할 수 있기 때문입니다. 이 접근 방식을 사용하면 원본에 가까운 품질을 유지하면서 디지털 워터마크를 안전하게 보호할 수 있습니다.‎"

support:
    enable: true

solutions:
    enable: true
    title: "GroupDocs.Watermark는 다른 인기 있는 개발 환경을 위한 문서 보기 API를 제공합니다."

    solution:
        - img_alt: "GroupDocs.Watermark for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-watermark-net.png"
          product: "GroupDocs.Watermark"
          platform: ".NET"
          link: "/watermark/net/"

back_to_top:
  enable: true
---
