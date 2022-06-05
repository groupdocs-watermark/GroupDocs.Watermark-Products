---
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

head_title: ".NET API를 사용하여 Word Excel PDF 이미지에 워터마크 제거 검색 추가"
head_description: "문서에서 이미지 및 텍스트 기반 워터마크를 추가, 검색 및 제거하는 C# .NET API: PDF, Word, Excel, 프레젠테이션, Visio, 이메일 및 이미지 파일 형식."

title: ".워터마크 조작을 위한 NET API"
description: "스마트 검색 및 강력한 보안 기능으로 텍스트 및 이미지 기반 워터마크를 작동하는 .NET 애플리케이션 구축."
button:
    enable: true

submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Watermark for .NET"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-watermark-net.png"
        product: "GroupDocs.Watermark"
        platform: ".NET"

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

            - link: "https://purchase.groupdocs.com/pricing/watermark/net"
              text: "가격"

    right:
        link_download: "https://downloads.groupdocs.com/watermark"
        link_learn: "https://docs.groupdocs.com/watermark/net/"
        link_buy: "https://purchase.groupdocs.com"

overview:
    enable: true
    content: |
      .NET용 GroupDocs.Watermark를 사용하면 C#, ASP.NET 및 기타 .NET 관련 기술로 즉시 출시되는 비즈니스 응용 프로그램을 구축할 수 있습니다. 이를 통해 최종 사용자는 지원되는 파일 형식에서 새 워터마크를 추가하고 기존 워터마크를 검색 및 제거할 수 있습니다. . .NET용 GroupDocs.Watermark를 사용하면 디지털 워터마크를 다양한 파일 형식에 프로그래밍 방식으로 적용하고 지적 재산의 무단 사용을 방지하고 이 API에서 제공하는 다양한 기본 제공 보안 수단을 사용하여 민감한 성격의 문서에 안전하게 레이블을 지정할 수 있습니다.
    tabs:
      enable: true
      
      tab_one:
        description: |
          다음은 .NET용 GroupDocs.Watermark의 개요입니다.
      
        right:
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
          각 형식에 대해 지원되는 [문서 형식 및 워터마크 유형](https://docs.groupdocs.com/watermark/net/supported-document-formats/)은 다음과 같습니다.

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
          .NET용 GroupDocs.Watermark는 다음 운영 체제, 프레임워크 및 패키지 관리자를 지원합니다.‎
        
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "운영체제"
              content: |
                * 윈도우 데스크탑
                * 윈도우 서버
                * 윈도우 애저
                * 리눅스

            - icon: "fas fa-code"
              title: "지원되는 프레임워크"
              content: |
                * .NET 프레임워크 2.0 이상
                * 모노 프레임워크 1.2 이상
                * .NET 표준 2.0
                * .NET 코어 2.0
                * .NET 코어 2.1

        right:
          enable: true
          table:
            - icon: "fas fa-box"
              title: "패키지 관리자"
              content: |
                * 누겟

            - icon: "fas fa-tools"
              title: "개발 환경"
              content: |
                * 마이크로소프트 비주얼 스튜디오
                * 자마린.안드로이드
                * 자마린.IOS
                * 자마린.맥
                * 모노디벨롭

features:
    enable: true
    title: ".NET 기능을 위한 GroupDocs.Watermark"

    feature:
      - icon: "fas fa-copy"
        content: "다양한 파일 형식의 특정 섹션 또는 전체 문서에서 워터마크 추가 또는 제거"

      - icon: "fas fa-eye"
        content: "특정 섹션, 페이지, 슬라이드 또는 문서의 모든 이미지에 워터마크 첨부"

      - icon: "fas fa-bolt"
        content: "다중 프레임 이미지의 특정 프레임에만 워터마크 할당"
      
      - icon: "fas fa-file-powerpoint"
        content: "문서를 인쇄할 때만 나타나는 숨겨진 워터마크를 PDF에 할당"

      - icon: "fas fa-code"
        content: "Excel 문서의 모든 첨부 파일 및 슬라이드의 모든 이미지 모양에 워터마크 설정"

      - icon: "fas fa-cloud"
        content: "스프레드시트 또는 슬라이드의 배경 이미지에서 워터마크 삽입 또는 제거"

      - icon: "fas fa-remove-format"
        content: "이메일 또는 PDF 문서의 모든 첨부 파일에서 지원되는 파일에 워터마크 사용"

      - icon: "fas fa-comment-slash"
        content: "PDF 문서에서 XObject, 인공물 및 주석으로 워터마크 적용 또는 제거‎"

      - icon: "fas fa-location-arrow"
        content: "특정 형식의 텍스트가 포함된 워터마크 제거"

      - icon: "fas fa-border-all"
        content: "특정 이미지를 닮은 이미지 워터마크 찾기"

      - icon: "fas fa-wrench"
        content: "글자 사이에 읽을 수 없는 문자가 있어도 텍스트 워터마크 식별"

      - icon: "fas fa-columns"
        content: "특정 매개변수 또는 여러 기준을 결합하여 워터마크 검색"

      - icon: "fas fa-file-word"
        content: "일치하는 텍스트 워터마크를 찾기 위해 글꼴 서식 지정"

      - icon: "fas fa-envelope"
        content: "프로그래밍 방식으로 지원되는 형식에 대한 페이지 설정 및 기타 정보 추출"

      - icon: "fas fa-print"
        content: "지원되는 문서 형식의 머리글 및 바닥글 내부 이미지에 워터마크 추가"

      - icon: "fas fa-file-archive"
        content: "Word 문서의 이미지 모양에 워터마크 추가 및 편집을 제한하기 위해 워터마크 잠그기"

      - icon: "fas fa-lock"
        content: "프레젠테이션에서 읽을 수 없는 문자를 사용하여 텍스트 워터마크 보호"

      - icon: "fas fa-file-code"
        content: "추가된 워터마크를 보호하기 위해 특정 페이지 또는 전체 PDF 문서를 래스터화"
      
      - icon: "fas fa-fill-drip"
        content: "기존 텍스트 워터마크를 바꾸는 동안 텍스트 서식 변경"

      - icon: "fas fa-file-excel"
        content: "PDF 문서의 도련 상자, 아트 상자, 자르기 상자 또는 자르기 상자에 워터마크 정렬"

      - icon: "fas fa-heading"
        content: "Microsoft Visio 문서에서 모양 속성 편집"

    more_feature:
      - title: "워터마크 추가"
        content: |
          .NET용 GroupDocs.Watermark는 여러 유형의 워터마크를 지원합니다. 모든 유형의 워터마크를 추가하는 것은 몇 줄의 코드에 불과합니다. 다음 예제에서는 C#을 사용하여 Word 문서에 이미지 워터마크를 적용하는 방법을 보여줍니다.

          ```cs
          // 문서 로드
          using (FileStream stream = File.Open("document.docx", FileMode.Open, FileAccess.ReadWrite))
          {
            using (Watermarker watermarker = new(Watermarker(stream))
            {
                    // 이미지 경로를 생성자의 매개변수로 사용
                    using (ImageWatermark watermark = new ImageWatermark("logo.png"))
                      {
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermarker.Add(watermark);
                }
                // 결과 문서 저장
                watermarker.Save("document_watermarked.docx");
                }
          }
          ```
      - title: "Go에서 다양한 형식의 파일에 워터마크 적용"
        content: "GroupDocs.Watermark API를 사용하면 워터마크를 적용하거나 특정 폴더에 있는 모든 파일의 워터마크를 한 번에 삭제할 수 있습니다. 파일 형식이 다를 수 있지만 워터마크는 모든 파일에 정확하게 적용됩니다.‎"

      - title: "워터마크를 위한 완벽한 보안"
        content: "단 한 줄의 코드로 모든 도구가 PDF 파일에서 워터마크를 제거하는 것을 매우 어렵게 만들 수 있습니다. 이것은 원본 품질을 그대로 유지하면서 PDF 문서의 모든 페이지를 래스터 이미지로 변환함으로써 달성됩니다.."

support:
    enable: true

solutions:
    enable: true
    title: "GroupDocs.Watermark는 다른 인기 있는 개발 환경을 위한 문서 보기 API를 제공합니다."

    solution:
        - img_alt: "GroupDocs.Watermark for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-watermark-java.png"
          product: "GroupDocs.Watermark"
          platform: "Java"
          link: "/watermark/java/"

back_to_top:
  enable: true
---
