
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:39:00
draft: false
lang: ko
format: Png
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "PNG 개의 파일을 위한 Java 개의 워터마크 솔루션"
head_description: "Java 을 사용하여 PNG 이미지에 동적 워터마크를 적용하여 디지털 자산을 보호하고 인증합니다."

############################# Header ############################
title: "Java 을 통한 PNG 보안 및 사용자 지정" 
description: "Java 을 활용하여 PNG 파일에 안전하고 조정 가능한 워터마크를 삽입하세요. 창작물을 보호하려는 사진작가와 디자이너에게 적합합니다."
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
       GroupDocs.Watermark for Java 는 Java 명의 개발자에게 PNG 개의 이미지에 워터마크를 적용할 수 있는 정교한 프레임워크를 제공합니다.이 API는 모든 Java 기반 애플리케이션에 원활하게 통합되도록 설계되었으므로 기본 이미지와 완벽하게 조화를 이루는 투명하거나 불투명한 워터마크를 삽입할 수 있습니다.텍스트, 로고 또는 저작권 기호로 워터마크를 사용자 지정하여 이미지 품질 저하 없이 보안을 강화하세요.완벽한 픽셀 포지셔닝 및 불투명도 제어와 같은 기능을 통해 GroupDocs.Watermark 은 이미지가 시각적으로 매력적이고 법적으로 보호되도록 합니다.전자 상거래 사이트, 온라인 포트폴리오 등에서 사용하기에 적합하며 Java 8 이상과 완벽하게 호환됩니다.

############################# Steps ############################
steps:
    enable: true
    title: "고급 기법: Java 을 통해 Png 문서에 워터마크 추가"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)**가 포함된 Png 문서에 대한 고급 워터마킹 기법 살펴보기
      
      1. **Watermarker** 클래스를 초기화하여 워터마킹 프로세스를 시작하십시오.이 기본 단계는 Png 문서에 워터마크를 추가하기 위한 단계를 설정합니다.Png 파일을 경로 또는 스트림 객체로 생성자에 제공하십시오.
      2. **워터마크** 오브젝트를 제작하여 다음 단계로 나아가세요.이러한 다용도 엔티티를 사용하면 지정된 문서 페이지뿐만 아니라 첨부 파일이나 머리글과 같은 기본 요소에도 정확하게 배치할 수 있습니다.
      3. 치수, 정렬, 글꼴 스타일 및 색상과 같은 속성을 미세 조정하여 워터마킹 프로세스를 개선합니다.이 수준의 사용자 지정을 통해 문서의 미학을 완벽하게 보완하는 워터마크를 만들 수 있습니다.
      4. **워터마커** 방법을 사용하여 새로 만든 워터마크를 문서에 적용하십시오.요구 사항에 따라 여러 워터마크를 유연하게 추가할 수 있습니다.문서를 보존하려면 안전한 장소에 보관하는 것이 좋습니다.
   
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
        // PNG 에 이미지 워터마크 추가

        // 워터마킹할 파일을 워터마커로 전달
        Watermarker watermarker = new Watermarker("input.png");
        
        // 워터마크가 포함된 이미지 경로 제공
        ImageWatermark watermark = new ImageWatermark("watermark.png");

        // 결과 저장
        watermarker.add(watermark);
        watermarker.save("output.png");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "문서 워터마크 마스터링"
  description: ".NET 명의 개발자를 위해 맞춤화된 정교한 워터마킹 API로 문서 관리를 향상시키세요.이 도구는 다양한 문서 형식에 워터마크를 적용, 사용자 지정 및 관리할 수 있는 포괄적인 솔루션을 제공하여 미적 매력과 향상된 보안을 모두 보장합니다."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "고급 문서 워터마킹"
  features:
    # feature loop
    - title: "유연한 워터마크 회전"
      content: "유연한 회전 설정으로 모든 문서 방향에 맞게 워터마크를 조정할 수 있습니다.세로 문서든 가로 문서든 관계없이 워터마크 각도를 쉽게 조정하여 문서 레이아웃을 보완하는 일관된 모양을 유지할 수 있습니다."

    # feature loop
    - title: "완벽한 투명성 제어"
      content: "워터마크의 투명도를 정밀하게 제어하여 문서 내용에 부담을 주지 않으면서도 섬세하면서도 안전한 마킹을 할 수 있습니다.이 기능은 보안을 강화하는 동시에 문서의 원래 미관을 유지하는 데 이상적입니다."

    # feature loop
    - title: "강조를 위한 그림자 효과"
      content: "워터마크의 가시성을 높이거나 사용자 지정 가능한 그림자 효과를 사용하여 문서에 섬세하게 통합할 수 있습니다.이 기능을 사용하면 다양한 흐림, 퍼짐 및 색상의 그림자를 만들 수 있으므로 필요에 따라 워터마크를 더욱 뚜렷하거나 눈에 잘 띄지 않게 만들 수 있습니다."
      
  code_samples:
    # code sample loop
    - title: "MS Word 개의 잠긴 워터마크"
      content: |
        이 예에서는 DOCX 개의 모든 페이지에서 워터마크를 잠그는 방법을 보여줍니다.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  문서를 MS Word 문서로 불러오기
        WordProcessingLoadOptions loadOptions = new WordProcessingLoadOptions();
        Watermarker watermarker = new Watermarker("source.docx", loadOptions);

        //  워터마크 만들기
        TextWatermark watermark = new TextWatermark("Watermark text", new Font("Arial", 19));
        watermark.setForegroundColor(Color.getRed());

        //  네이티브 Word 개의 옵션 조정
        WordProcessingWatermarkPagesOptions options = new WordProcessingWatermarkPagesOptions();
        options.setLocked(true);
        options.setLockType(WordProcessingLockType.AllowOnlyFormFields);

        //  결과 문서 페이지에 워터마크 추가
        watermarker.add(textWatermark, options);
        watermarker.save("result.docx");
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
    title: "Java 을 통한 PNG 이미지 보안 강화"
    exclude: "PNG"
    description: "Java 을 사용하여 PNG 파일에 강력한 워터마크를 삽입합니다.이 기능은 이미지 선명도를 유지하면서 시각적 콘텐츠를 무단으로 사용하지 못하도록 보호하는 데 매우 중요합니다."
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