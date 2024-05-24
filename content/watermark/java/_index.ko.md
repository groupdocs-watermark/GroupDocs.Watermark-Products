---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:29
draft: false

lang: ko
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

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
head_title: "Java 워터마크 라이브러리 | 문서에 워터마크 추가"
head_description: "PDF, Word, Excel, 프레젠테이션, Visio 다이어그램, 이메일 및 이미지 파일에 텍스트 및 이미지 워터마크를 추가하고 조작하는 네이티브 Java 소프트웨어입니다."

############################# Header ############################
title: "Java 프로젝트에서 문서 워터마킹을 쉽게 구현하세요."
description: "GroupDocs.Watermark 라이브러리를 사용하여 파일을 워터마킹하는 기능으로 Java 애플리케이션을 개선하십시오.당사의 API는 널리 사용되는 다양한 파일 형식에 대해 사용자 지정 가능한 워터마크를 제공합니다."
words:
  for: "...에 대한"

actions:
  main: "Maven에서 무료 다운로드"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "라이선싱"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java/"
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Watermark 기능을 무료로 체험하거나 라이선스를 요청하세요"

release:
  title: "버전 {0} 출시"
  notes: "새 소식 보기"
  downloads: "다운로드"

code:
  title: "Java 을 통해 PDF 을 (를) 워터마킹합니다."
  more: "더 많은 예시"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-watermark</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // PDF 경로를 통과하는 워터마커 인스턴스화
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // 워터마크 옵션 사용자 지정
    TextWatermark textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // PDF 문서에 워터마크 적용
    watermarker.add(textWatermark);

    // 결과 문서 저장
    watermarker.save("result.pdf");
    watermarker.close();
      
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Watermark 한 눈에"
  description: "Java 기술을 사용하여 워터마크를 추가하도록 설계된 라이브러리"
  features:
    # feature loop
    - title: "Java 을 통한 워터마크 파일"
      content: "GroupDocs.Watermark for Java 를 사용하여 비즈니스 문서를 보호하십시오.텍스트, 이미지, 다이어그램 또는 이메일 첨부 파일을 다양한 파일 형식에 워터마크로 추가합니다."

    # feature loop
    - title: "특정 요구 사항에 맞게 워터마크 사용자 지정"
      content: "GroupDocs.Watermark for Java 는 워터마크에 대한 광범위한 사용자 지정 옵션을 제공합니다.텍스트 스타일 (굵게, 기울임꼴, 글꼴) 과 이미지 속성 (회전 등) 을 조정하여 특정 목표에 맞게 워터마킹 프로세스를 조정할 수 있습니다."

    # feature loop
    - title: "광범위한 포맷 지원"
      content: "GroupDocs.Watermark for Java 는 PDF, Microsoft Office (Word, Excel, PowerPoint), 이미지 (JPEG, PNG, GIF, BMP), Visio 다이어그램 및 이메일을 비롯한 다양한 파일 형식과 원활하게 통합됩니다.다양한 파일 유형에서 문서 보안을 강화합니다."

    # feature loop
    - title: "간편한 워터마크 검색 및 관리"
      content: "문서 내 기존 워터마크를 효율적으로 관리합니다.특정 워터마크를 찾거나 텍스트, 스타일 또는 이미지를 수정하거나 완전히 제거합니다. GroupDocs.Watermark for Java 는 워터마킹 워크플로를 간소화합니다."

############################# Platforms ############################
platforms:
  enable: true
  title: "플랫폼 독립성"
  description: "GroupDocs.Watermark for Java 는 다양한 운영 체제와 패키지 관리자를 지원합니다."
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "지원되는 파일 형식"
  description: |
    GroupDocs.Watermark for Java 를 사용하면 다양한 파일 형식을 처리할 수 있습니다.[전체 목록 보기](https://docs.groupdocs.com/watermark/java/supported-document-formats/).
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
  title: "GroupDocs.Watermark for Java: 특징"
  description: "워터마크를 추가하여 파일을 보호하세요.PDF, Office 문서 및 이미지를 비롯한 다양한 형식을 지원합니다."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "파일 워터마킹"
      content: "지원되는 다양한 파일 형식에 대해 특정 섹션 또는 전체 문서에서 워터마크를 추가하거나 제거합니다."

    # feature loop
    - icon: "watermark_style"
      title: "워터마크 커스터마이징"
      content: "색상, 글꼴, 회전 등과 같은 옵션을 사용하여 워터마크의 모양을 사용자 지정할 수 있습니다."

    # feature loop
    - icon: "hidden_print"
      title: "PDF 에 대한 숨겨진 인쇄 워터 마크"
      content: "PDF 문서를 인쇄할 때만 나타나는 워터마크를 추가합니다."

    # feature loop
    - icon: "image_only"
      title: "선택적 이미지 워터마킹"
      content: "특정 섹션, 페이지, 슬라이드 또는 전체 문서 내의 모든 이미지에 워터마크를 추가합니다."

    # feature loop
    - icon: "image_frame"
      title: "특정 이미지 프레임에 워터마킹"
      content: "다중 프레임 이미지 내의 특정 프레임에 워터마크를 적용합니다."

    # feature loop
    - icon: "attachments"
      title: "어태치먼트 및 도형에 워터마킹"
      content: "Excel 문서의 모든 첨부 파일 또는 프레젠테이션의 모든 이미지 셰이프에 워터마크를 추가합니다."

    # feature loop
    - icon: "pdf_objects"
      title: "PDF 에서의 워터마크 정렬"
      content: "블리드 박스, 아트 박스, 크롭 박스, 트림 박스 등 PDF 문서의 다양한 영역에 워터마크를 정렬합니다."

    # feature loop
    - icon: "doc_background"
      title: "배경 이미지별 워터마크"
      content: "스프레드시트 또는 프레젠테이션에 배경 이미지 워터마크를 추가하거나 제거합니다."

    # feature loop
    - icon: "unreadable_characters"
      title: "읽을 수 없는 문자로 보호"
      content: "읽을 수 없는 문자가 포함된 텍스트 워터마크를 사용하여 프레젠테이션을 보호합니다."

    # feature loop
    - icon: "watermark_text_search"
      title: "워터마크 검색"
      content: "정규 표현식을 비롯한 다양한 파라미터를 사용하여 파일에 표시된 워터마크 목록을 가져옵니다."

    # feature loop
    - icon: "watermark_image_search"
      title: "비슷한 이미지 워터마크 찾기"
      content: "특정 이미지처럼 보이는 이미지 워터마크를 찾습니다."

    # feature loop
    - icon: "document_info"
      title: "문서 정보 추출"
      content: "지원되는 파일 형식의 페이지 설정과 같은 다양한 문서 데이터를 가져옵니다."

############################# Code samples ############################
code_samples:
  enable: true
  title: "코드 샘플"
  description: "일반적인 GroupDocs.Watermark for Java 기능을 보여주는 코드 예제 살펴보기"
  items:
    # code sample loop
    - title: "이미지를 사용하여 문서에 워터마크 추가"
      content: |
        GroupDocs.Watermark for Java 를 활용하여 이미지 워터마크를 추가하여 문서 보안을 강화하십시오.자세히 알아보기: [이미지 워터마크](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/).
        {{< landing/code title="이미지 워터마크로 파일을 보호하는 방법">}}
        ```java {style=abap}
        // 워터마커에 소스 문서 불러오기
        Watermarker watermarker = new Watermarker("document.pdf");
        
        // 워터마크 이미지의 경로 지정
        ImageWatermark watermark = new ImageWatermark("watermark.jpg");

        // 파일을 보호하고 저장합니다.
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "워터마크 수정"
      content: |
        GroupDocs.Watermark for Java 를 사용하면 문서 내의 기존 워터마크를 관리할 수 있습니다.특정 워터마크를 찾아 [속성 수정](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/).
        {{< landing/code title="워터마크 검색 및 수정.">}}
        ```java {style=abap}   
        // 소스 문서 불러오기
        Watermarker watermarker = new Watermarker("document.pdf");

        // 업데이트할 워터마크 검색
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);                               
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);                             

        // 원하는 속성 업데이트
        for (PossibleWatermark watermark : watermarks)                                                           
        {  
            watermark.setText("New Text");
        }

        // 수정한 문서를 지정된 경로에 저장
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
