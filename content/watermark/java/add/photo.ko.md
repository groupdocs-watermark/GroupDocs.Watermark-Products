
---
############################# Static ############################
layout: "format"
date:  2024-04-29T14:26:57
draft: false
lang: ko
format: Photo
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java 에서 사진 워터마킹이 쉬워졌습니다"
head_description: "워터마킹으로 사진 보호를 간소화하세요.빠르고 안정적입니다."

############################# Header ############################
title: "사진 워터마킹을 위한 효율적인 Java 도구" 
description: "Java API를 사용하여 사진에 워터마크를 빠르고 효율적으로 추가하세요.최소한의 노력으로 디지털 이미지를 보호하고 브랜드 가시성을 높이는 데 적합합니다."
subtitle: "GroupDocs.Watermark for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Maven 에서 무료로 다운로드"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java"
    link: "/watermark/java/"
    link_title: "자세히 알아보기"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java 는 사진 파일의 빠르고 효과적인 워터마킹에 최적화되어 있습니다.이 도구를 사용하면 텍스트와 이미지 워터마크를 JPEG, PNG, BMP 등 다양한 사진 형식에 빠르게 통합할 수 있습니다.스타일, 투명도 및 배치에 대한 광범위한 옵션을 사용하여 워터마크를 사용자 정의하여 사진 품질을 떨어뜨리지 않고 매끄럽게 조화를 이루도록 하세요.대용량 작업에 적합하며 한 번에 여러 사진에 워터마크를 적용할 수 있는 일괄 처리를 지원하므로 시각적 자산을 효율적으로 보호하고 브랜딩해야 하는 기업 및 디지털 콘텐츠 제작자에게 적합합니다.

############################# Steps ############################
steps:
    enable: true
    title: "Java 을 통해 Photo 문서에 워터마크 추가"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** 를 사용하면 Java 개발자가 널리 사용되는 비즈니스 파일 형식에 다양한 유형의 워터마크를 쉽게 추가할 수 있습니다.아래 나열된 몇 가지 간단한 단계를 통해 애플리케이션 및 워터마크 문서에 라이브러리를 추가할 수 있습니다.
      
      1. **워터마커** 입니다.문서 처리 전에 인스턴스화해야 합니다.Photo 파일을 생성자에 경로 또는 스트림 객체로 전달하는 것을 잊지 마세요.
      2. **Watermark** 객체를 생성하는 것입니다.특정 문서 페이지뿐만 아니라 첨부 파일이나 머리글과 같은 기본 문서 부분에도 배치할 수 있습니다.
      3. 높이 및 너비, 페이지 정렬 (상단, 왼쪽, 중앙 등), 글꼴군 및 색상 등과 같은 워터마크 속성을 설정합니다.
      4. **워터마커** 메서드를 호출하여 새 워터마크를 추가합니다.워터마크는 필요한 만큼 추가할 수 있습니다.처리된 문서를 다른 위치에 저장하는 것이 좋습니다.
   
    code:
      platform: "net"
      copy_title: "복사"
      install:
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-watermark</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "클릭하여 복사"
        copy_done: "복사"
      links:
        #  loop
        - title: "더 많은 예시"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
        #  loop
        - title: "문서화"
          link: "https://docs.groupdocs.com/watermark/java/"
          
      content: |
        ```java {style=abap}

        // PHOTO 에 텍스트 워터마크 추가

        // 워터마킹할 파일을 워터마커로 전달
        Watermarker watermarker = new Watermarker("input.png");
        
        // 텍스트 워터마크 생성 및 속성 설정
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        watermark.setForegroundColor(Color.getRed());

        // 워터마크 파일 저장
        watermarker.add(watermark);
        watermarker.save("output.png");
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "워터마크를 쉽게 보정하세요"
  description: "GroupDocs.Watermark 의 기능을 활용하여 여러 문서 형식에서 워터마크를 생성, 작성 및 추가할 수 있습니다.이 API는 문서 보안을 강화할 뿐만 아니라 다재다능하고 강력한 사용자 지정 가능한 워터마크를 내장하여 지적 재산을 보호합니다."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "워터마크 추가"
  features:
    # feature loop
    - title: "다양한 워터마크 옵션."
      content: "GroupDocs.Watermark 의 다양한 워터마킹 옵션을 살펴보세요.API를 사용하면 불투명도 및 회전을 조정하는 것부터 비례적인 크기 조절에 이르기까지 워터마크를 필요에 맞게 정확하게 사용자 지정할 수 있으므로 콘텐츠 무결성을 유지하면서 문서와 원활하게 조화를 이룰 수 있습니다."

    # feature loop
    - title: "고급 워터마크 스타일링."
      content: "GroupDocs.Watermark 을 사용하면 다양한 글꼴, 색상 및 그림자로 워터마크의 스타일을 지정하여 독특하고 제거하기 어렵게 만들 수 있습니다.브랜드의 정체성과 전문성을 반영하는 세련된 워터마크를 사용하여 보호된 문서와 이미지의 미적 매력을 높이세요."

    # feature loop
    - title: "워터마크 타일링 및 포지셔닝"
      content: "GroupDocs.Watermark 을 사용하면 전체 문서를 포괄하는 타일링 효과를 구현하여 완벽한 보호를 보장할 수 있습니다.워터마크를 필요한 위치 (중앙, 모서리 또는 사용자 지정 위치) 에 정확히 배치하세요.당사의 유연한 위치 지정 옵션은 무단 사용 및 복제로부터 문서를 보호하는 데 도움이 됩니다."
      
  code_samples:
    # code sample loop
    - title: "PDF 주석 워터마크"
      content: |
        이 예에서는 PDF 문서에 워터마크 주석을 추가하는 방법을 보여 줍니다.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  문서를 PDF 로 불러오기
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  PDF 주석을 기반으로 워터마크 생성
        PdfAnnotationWatermarkOptions options = new PdfAnnotationWatermarkOptions();
        TextWatermark textWatermark = new TextWatermark("Annotation watermark", new Font("Arial", 8));

        //  워터마크 옵션 설정
        textWatermark.setHorizontalAlignment(HorizontalAlignment.Left);
        textWatermark.setVerticalAlignment(VerticalAlignment.Top);

        //  결과 문서에 텍스트 워터마크 추가
        watermarker.add(textWatermark, options);
        watermarker.save("result.pdf");

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Watermark 기능을 무료로 체험하거나 라이선스를 요청하세요"
  items:
    #  loop
    - title: "Maven 다운로드"
      link: "https://releases.groupdocs.com/watermark/java/"
      color: "red"
        #  loop
    - title: "라이선싱"
      link: "https://purchase.groupdocs.com/pricing/watermark/java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Java 를 통한 사진에 대한 신속한 워터마크 통합"
    exclude: "PHOTO"
    description: "Java API를 활용하여 사진에 워터마크를 빠르게 적용하여 보안과 브랜드 정체성을 강화하세요.자동화된 프로세스를 통해 대량 적용이 가능하므로 일관되고 전문적인 결과를 얻을 수 있습니다."
    items: 
        # format loop 1
        - name: "워터마크 PDF"
          format: "PDF"
          link: "/watermark/java/add//pdf/"
          description: "어도비 Portable 문서 형식"

        # format loop 2
        - name: "워터마크 Word"
          format: "WORD"
          link: "/watermark/java/add//word/"
          description: "MS Word 및 오픈 오피스 문서"
          
        # format loop 3
        - name: "워터마크 Excel"
          format: "EXCEL"
          link: "/watermark/java/add//excel/"
          description: "MS Excel 및 오픈 오피스 스프레드시트"

        # format loop 4
        - name: "워터마크 이미지"
          format: "IMAGE"
          link: "/watermark/java/add//image/"
          description: "인기 이미지 형식"

        # format loop 5
        - name: "워터마크 사진"
          format: "PHOTO"
          link: "/watermark/java/add//photo/"
          description: "사진 형식"

        # format loop 6
        - name: "워터마크 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/add//powerpoint/"
          description: "MS PowerPoint 및 오픈 오피스 프레젠테이션"

        # format loop 7
        - name: "워터마크 DOCX"
          format: "DOCX"
          link: "/watermark/java/add//docx/"
          description: "마이크로소프트 Word 오픈 XML 문서"
          
        # format loop 8
        - name: "워터마크 PPTX"
          format: "PPTX"
          link: "/watermark/java/add//pptx/"
          description: "PowerPoint 오픈 XML 프레젠테이션"
          
        # format loop 9
        - name: "워터마크 XLSX"
          format: "XLSX"
          link: "/watermark/java/add//xlsx/"
          description: "마이크로소프트 Excel 오픈 XML 스프레드시트"

        # format loop 10
        - name: "워터마크 JPEG"
          format: "JPEG"
          link: "/watermark/java/add//jpeg/"
          description: "JPEG 이미지"

        # format loop 11
        - name: "워터마크 PNG"
          format: "PNG"
          link: "/watermark/java/add//png/"
          description: "Portable 네트워크 그래픽"

        # format loop 12
        - name: "워터마크 TIFF"
          format: "TIFF"
          link: "/watermark/java/add//tiff/"
          description: "태그 이미지 파일 형식"

        # format loop 13
        - name: "워터마크 WEBP"
          format: "WEBP"
          link: "/watermark/java/add//webp/"
          description: "웹 사진"

        # format loop 14
        - name: "워터마크 DOC"
          format: "DOC"
          link: "/watermark/java/add//doc/"
          description: "마이크로소프트 Word 97 - 2007 문서"

        # format loop 15
        - name: "워터마크 XLS"
          format: "XLS"
          link: "/watermark/java/add//xls/"
          description: "마이크로소프트 Excel 워크북 97-2003"

        # format loop 16
        - name: "워터마크 PPT"
          format: "PPT"
          link: "/watermark/java/add//ppt/"
          description: "PowerPoint 프레젠테이션 97-2003"

        # format loop 17
        - name: "워터마크 RTF"
          format: "RTF"
          link: "/watermark/java/add//rtf/"
          description: "리치 텍스트 포맷"

---