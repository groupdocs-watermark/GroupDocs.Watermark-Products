---
############################# Static ############################
layout: "landing"
date: 2024-04-29T14:27:13
draft: false

lang: ko
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js 워터마킹 라이브러리 | 문서 워터마크"
head_description: "Node.js 솔루션은 텍스트 및 이미지 워터마크를 사용하여 비즈니스 문서를 보호합니다.PDF, Word, Excel, PowerPoint 와 같은 널리 사용되는 형식이 지원됩니다."

############################# Header ############################
title: "Java 솔루션을 통해 Node.js 워터마킹 기술을 이용할 수 있습니다."
description: "이 Node.js 솔루션으로 지적 재산을 보호하고 무단 복사를 방지하십시오.이를 통해 사용자는 PDF, Word, Excel, PowerPoint, 이미지 등 다양한 형식의 비즈니스 문서에 워터마크를 쉽게 추가할 수 있습니다."
words:
  for: "...에 대한"

actions:
  main: "NPM을 사용하여 무료로 다운로드하십시오"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.watermark"
  alt: "라이선싱"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Watermark 기능을 무료로 체험하거나 라이선스를 요청하세요"

release:
  title: "버전 {4.13} 출시"
  notes: "새 소식 보기"
  downloads: "다운로드"
  link: "https://releases.groupdocs.com/watermark/nodejs-java/"

code:
  title: "타입스크립트로 PDF 에 워터마크 추가"
  more: "더 많은 예시"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.watermarker"
  content: |
    ```javascript {style=abap}

    // PDF 경로를 통과하는 워터마커 인스턴스화
    let loadOptions = new PdfLoadOptions();
    let watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // 워터마크 옵션 사용자 지정
    let textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // PDF 문서에 워터마크 적용
    watermarker.add(textWatermark);

    // 결과 문서 저장
    watermarker.save("result.pdf");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark 한 눈에"
  description: "워터마킹을 위한 Node.js 타입스크립트 라이브러리"
  features:
    # feature loop
    - title: "Node.js 파일 워터마킹"
      content: "GroupDocs.Watermark for Node.js via Java 를 사용하여 비즈니스 문서를 보호하십시오.텍스트, 이미지, 다이어그램 또는 이메일 첨부 파일을 다양한 파일 형식에 워터마크로 추가합니다."

    # feature loop
    - title: "필요에 맞게 워터마크를 사용자 지정하세요"
      content: "GroupDocs.Watermark for Node.js via Java 는 워터마크에 대한 광범위한 사용자 지정 옵션을 제공합니다.텍스트 스타일 (굵게, 기울임꼴, 글꼴) 과 이미지 속성 (회전 등) 을 세밀하게 조정하여 문서 처리를 사용자 지정할 수 있습니다."

    # feature loop
    - title: "포괄적인 포맷 지원"
      content: "GroupDocs.Watermark for Node.js via Java 는 PDF, Word, Excel, PowerPoint, JPEG, PNG, GIF 다이어그램, Visio 등의 이미지, 이메일 등 다양한 파일 형식과 원활하게 통합됩니다. 문서 처리를 강화하여 비즈니스 목표를 달성할 수 있습니다."

    # feature loop
    - title: "강력한 워터마크 검색 및 업데이트"
      content: "워터마크가 있는 문서의 기존 워터마크를 가져오고 업데이트합니다.텍스트, 스타일, 이미지 내용을 수정하거나 완전히 제거합니다. GroupDocs.Watermark for Node.js via Java 는 광범위한 워터마크 처리 기능을 제공합니다."

############################# Platforms ############################
platforms:
  enable: true
  title: "플랫폼 독립성"
  description: "GroupDocs.Watermark for Node.js via Java 는 다양한 운영 체제 및 패키지 관리자와 쉽게 통합됩니다."
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
    GroupDocs.Watermark for Node.js via Java 를 사용하면 다양한 파일 형식을 처리할 수 있습니다.[전체 목록 보기](https://docs.groupdocs.com/watermark/net/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Node.js via Java: 기능 세트"
  description: "프로그래밍 방식의 워터마킹을 통해 강력한 문서 보안을 강화합니다.PDF, DOCX, XLSX, PPTX 및 이미지 형식 (PNG, JPG 등) 을 비롯한 다양한 파일 형식을 지원합니다."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "정밀한 워터마킹 제어"
      content: "다양한 파일 형식의 특정 섹션, 전체 문서 또는 개별 첨부 파일 및 모양에서 워터마크를 추가하거나 제거하여 워터마크를 정밀하게 조작할 수 있습니다."

    # feature loop
    - icon: "watermark_style"
      title: "워터마크 모양 사용자 지정"
      content: "문서 내에서 색상, 글꼴, 불투명도, 회전 및 위치와 같은 속성을 수정하여 워터마크의 미학을 세밀하게 제어할 수 있습니다."

    # feature loop
    - icon: "hidden_print"
      title: "PDF 워터마킹 인쇄"
      content: "일반 문서를 볼 때는 보이지 않지만 인쇄 프로세스 중에만 눈에 띄는 스텔스 워터마크를 배치하여 문서 보안을 신중하게 강화합니다."

    # feature loop
    - icon: "image_only"
      title: "특정 이미지 워터마킹"
      content: "솔루션을 사용하여 문서 내의 특정 이미지에 워터마크를 추가하세요.워터마크를 지정된 섹션 (예: 페이지, 슬라이드) 에 삽입하거나 전체 문서에 삽입할 수 있습니다."

    # feature loop
    - icon: "image_frame"
      title: "멀티프레임 이미지 워터마킹"
      content: "멀티프레임 이미지 형식 내의 특정 프레임에 워터마크를 선택적으로 적용하여 워터마크 배치를 세밀하게 제어할 수 있습니다."

    # feature loop
    - icon: "attachments"
      title: "포괄적인 콘텐츠 보호"
      content: "Excel 문서 내의 첨부 파일 및 프레젠테이션 내 이미지 셰이프와 같은 다양한 문서 요소로 보호를 확장하여 추가 보안 계층을 제공합니다."

    # feature loop
    - icon: "pdf_objects"
      title: "PDF 의 고급 워터마킹"
      content: "블리드 박스, 아트 박스, 크롭 박스, 트림 박스 등 PDF 의 다양한 영역에 워터마크를 표시합니다."

    # feature loop
    - icon: "doc_background"
      title: "배경 이미지 워터마킹"
      content: "스프레드시트 및 프레젠테이션의 배경 이미지 내에서 워터마크를 관리하여 시각적 보안 조치를 위한 추가 사용자 지정 옵션을 제공합니다."

    # feature loop
    - icon: "unreadable_characters"
      title: "읽을 수 없는 문자가 있는 텍스트 워터마크"
      content: "프레젠테이션에 포함된 텍스트 워터마크에 읽을 수 없는 문자를 사용하여 무단 워터마크 추출을 훨씬 더 어렵게 만들어 보안을 강화합니다."

    # feature loop
    - icon: "watermark_text_search"
      title: "고급 워터마크 검색"
      content: "포괄적인 검색 기능을 활용하여 특정 매개 변수를 기반으로 하거나 다양한 기준을 결합하여 문서 내에서 워터마크를 찾을 수 있으므로 효율적인 검색 및 관리가 가능합니다."

    # feature loop
    - icon: "watermark_image_search"
      title: "유사 이미지 워터마크 감지"
      content: "소스 이미지와 시각적으로 유사한 유사한 워터마크 이미지를 문서 내에서 찾을 수 있습니다."

    # feature loop
    - icon: "document_info"
      title: "프로그래밍 방식의 문서 정보 추출"
      content: "지원되는 파일 형식에 대한 페이지 설정 세부 정보 및 기타 문서 정보를 포함하여 중요한 메타데이터를 프로그래밍 방식으로 추출합니다."

############################# Code samples ############################
code_samples:
  enable: true
  title: "코드 샘플"
  description: "일반적인 GroupDocs.Watermark for Node.js via Java 기능을 보여주는 코드 예제를 자세히 살펴보세요."
  items:
    # code sample loop
    - title: "문서에 이미지 워터마크 추가"
      content: |
        GroupDocs.Watermark for Node.js via Java 를 활용하여 이미지 워터마크를 추가하여 문서 보안을 강화하십시오.자세히 알아보기: [이미지 워터마크](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="이미지 워터마크로 파일을 보호하는 방법">}}
        ```javascript {style=abap}
        // 워터마커에 소스 문서 불러오기
        let watermarker = new Watermarker("document.pdf");
        
        // 워터마크 이미지의 경로 지정
        let watermark = new ImageWatermark("watermark.jpg");

        // 파일을 보호하고 저장합니다.
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "기존 워터마크 검색 및 수정"
      content: |
        GroupDocs.Watermark for Node.js via Java 를 사용하면 문서 워터마크를 관리할 수 있습니다.워터마크를 선택하고 속성을 수정하세요.방법 알아보기: [워터마크 수정](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="워터마크 검색 및 수정.">}}
        ```javascript {style=abap}   
        // 소스 문서 불러오기
        let watermarker = new Watermarker("document.pdf");

        // 업데이트할 워터마크 검색
        let searchCriteria = new TextSearchCriteria("test", false);                               
        let watermarks = watermarker.search(searchCriteria); 

        // 원하는 속성 업데이트
        watermarks.forEach((watermark)
        {  
            watermark.setText("New Text");
        }

        // 수정한 문서를 지정된 경로에 저장
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
