---
############################# Static ############################
layout: "landing"
date: 2024-04-29T14:27:13
draft: false

lang: ko
product: "Watermark"
product_tag: "watermark"
platform: "Net"
platform_tag: "net"

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

############################# Head ############################
head_title: "C# .NET 문서 워터마크 소프트웨어 | 워터마크 추가"
head_description: "문서에서 워터마크를 추가, 검색 및 제거하기 위한 C# .NET 라이브러리: PDF, Word, Excel, 프레젠테이션, Visio 다이어그램, 이메일 및 이미지 파일 형식"

############################# Header ############################
title: "C# .NET 애플리케이션에서 문서에 손쉽게 워터마크 추가"
description: "모든 인기 있는 문서 형식에 사용자 지정 가능한 워터마크를 추가할 수 있는 유연한 문서 워터마킹 API로 C# 솔루션을 강화하세요."
words:
  for: "...에 대한"

actions:
  main: "무료 NuGet 다운로드"
  main_link: "https://www.nuget.org/packages/GroupDocs.Watermark"
  alt: "라이선싱"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/net/"
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Watermark 기능을 무료로 체험하거나 라이선스를 요청하세요"

release:
  title: "버전 {4.13} 출시"
  notes: "새 소식 보기"
  downloads: "다운로드"

code:
  title: "C #의 PDF 개 파일에 워터마크 추가"
  more: "더 많은 예시"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
  install: "dotnet add package GroupDocs.Watermark"
  content: |
    ```csharp {style=abap}   
    // PDF 경로를 통과하는 워터마커 인스턴스화
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    using (Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions))
    {
        // 워터마크 옵션 사용자 지정
        TextWatermark textWatermark = 
            new TextWatermark("Approved", new Font("Arial", 8));
        
        // PDF 문서에 워터마크 적용
        watermarker.Add(textWatermark);

        // 결과 문서 저장
        watermarker.Save("result.pdf");
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark 한 눈에"
  description: ".NET 을 통해 문서에 워터마크를 넣는 API"
  features:
    # feature loop
    - title: "C# 파일 워터마크"
      content: "GroupDocs.Watermark 를 사용하여 비즈니스 파일에 워터마크를 추가합니다.텍스트, 이미지, 다이어그램 또는 이메일 첨부 파일을 사용하세요."

    # feature loop
    - title: "워터마크를 목표에 맞게 사용자 지정하세요"
      content: "GroupDocs.Watermark for .NET 소프트웨어를 사용하면 다양한 방식으로 워터마크를 사용자 지정할 수 있습니다.굵게, 기울임꼴, 글꼴 유형과 같은 텍스트 스타일과 회전과 같은 이미지 속성 등은 워터마킹 프로세스를 더욱 풍부하게 합니다."

    # feature loop
    - title: "널리 사용되는 모든 파일 형식이 지원됩니다."
      content: "GroupDocs.Watermark 솔루션은 많은 파일 및 문서 형식을 지원합니다. PDF, Microsoft Office Word, Excel, PowerPoint, JPEG, PNG, BMP, Visio 다이어그램, 이메일 등과 같은 이미지는 워터마크로 보호될 수 있습니다."

    # feature loop
    - title: "워터마크 검색 및 업데이트"
      content: "문서에 이미 표시된 워터마크를 찾아 다시 처리할 수 있습니다.별도의 노력 없이 텍스트, 스타일, 이미지를 수정하거나 드러난 워터마크를 제거할 수 있습니다."

############################# Platforms ############################
platforms:
  enable: true
  title: "플랫폼 독립성"
  description: "GroupDocs.Watermark for .NET 는 아래 나열된 운영 체제, 프레임워크 및 패키지 관리자를 지원합니다."
  items:
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
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "지원되는 파일 형식"
  description: |
    GroupDocs.Watermark for .NET 는 다음 [파일 형식](https://docs.groupdocs.com/watermark/net/supported-document-formats/) 의 처리를 제공합니다.
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
  title: "GroupDocs.Watermark 개의 특징"
  description: "PDF, 오피스, 이미지 및 기타 형식을 워터마크로 보호합니다."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "문서 워터마킹"
      content: "다양한 파일 형식의 특정 섹션 또는 전체 문서에서 워터마크를 추가하거나 제거합니다."

    # feature loop
    - icon: "watermark_style"
      title: "워터마크 스타일 지정"
      content: "색상, 글꼴, 회전 등과 같은 다양한 워터마크 속성을 사용자 지정합니다."

    # feature loop
    - icon: "hidden_print"
      title: "PDF 숨겨진 인쇄 워터마크"
      content: "문서를 인쇄할 때만 나타나는 숨겨진 워터마크를 PDF 에 할당합니다."

    # feature loop
    - icon: "image_only"
      title: "문서 내 이미지만 워터마킹하기"
      content: "특정 섹션, 페이지, 슬라이드 또는 문서의 모든 이미지를 워터마킹합니다."

    # feature loop
    - icon: "image_frame"
      title: "선택한 이미지 프레임 처리"
      content: "멀티프레임 이미지의 특정 프레임에만 워터마크를 할당합니다."

    # feature loop
    - icon: "attachments"
      title: "어태치먼트 및 모양"
      content: "Excel 문서의 모든 첨부 파일과 슬라이드의 모든 이미지 모양에 워터마크를 설정합니다."

    # feature loop
    - icon: "pdf_objects"
      title: "PDF 오브젝트"
      content: "PDF 문서의 블리드 박스, 아트 박스, 크롭 박스 또는 트림 박스에 워터마크를 정렬합니다."

    # feature loop
    - icon: "doc_background"
      title: "문서 배경"
      content: "스프레드시트 또는 슬라이드의 배경 이미지에서 워터마크를 삽입하거나 제거합니다."

    # feature loop
    - icon: "unreadable_characters"
      title: "읽을 수 없는 문자 보호"
      content: "프레젠테이션에서 읽을 수 없는 문자를 사용하여 텍스트 워터마크를 보호합니다."

    # feature loop
    - icon: "watermark_text_search"
      title: "문서에서 워터마크 검색"
      content: "특정 파라미터를 기반으로 하거나 여러 기준을 결합하여 워터마크를 검색합니다."

    # feature loop
    - icon: "watermark_image_search"
      title: "비슷한 이미지 워터마크 검색"
      content: "특정 이미지와 비슷한 이미지 워터마크를 찾아보세요."

    # feature loop
    - icon: "document_info"
      title: "문서 정보 가져오기"
      content: "지원되는 형식에 대한 페이지 설정 및 기타 정보를 프로그래밍 방식으로 추출합니다."

############################# Code samples ############################
code_samples:
  enable: true
  title: "코드 샘플"
  description: "일반적인 GroupDocs.Watermark for .NET 작업의 일부 사용 사례"
  items:
    # code sample loop
    - title: "문서에 이미지를 추가하여 워터마킹합니다."
      content: |
        모든 문서를 보호하려면 [이미지 워터마크](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/) 를 사용할 수 있습니다.
        {{< landing/code title="이미지 워터마크로 파일을 보호하는 방법">}}
        ```csharp {style=abap}
        // 워터마커에 소스 문서 불러오기
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // 워터마크 이미지의 경로 지정
            using (ImageWatermark watermark = new ImageWatermark("watermark.jpg"))
            {
                // 파일을 보호하고 저장합니다.
                watermarker.Add(watermark);

                watermarker.Save("result.pdf");
            }
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "기존 워터마크를 검색하고 수정합니다."
      content: |
        GroupDocs.Watermark 는 문서에 이미 표시된 [워터마크 수정](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/) 을 할 수 있습니다.원하는 항목을 검색하고 속성을 업데이트합니다.
        {{< landing/code title="워터마크 검색 및 수정.">}}
        ```csharp {style=abap}   
        // 소스 문서 불러오기
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // 업데이트할 워터마크 검색
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                // 원하는 속성 업데이트
                watermark.Text = "New Text";
            }

            // 수정한 문서를 지정된 경로에 저장
            watermarker.Save("document.pdf");
        }
        ```
        {{< /landing/code >}}

---
