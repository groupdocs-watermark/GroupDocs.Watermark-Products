
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:22
draft: false
lang: ko
format: Pdf
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "PDF - GroupDocs.Watermark 에서 워터마크를 조정하세요"
head_description: "GroupDocs.Watermark 를 사용하여 다양한 문서 유형에서 워터마크를 손쉽게 조정하고 다듬을 수 있습니다.문서의 신뢰성을 보장하세요."

############################# Header ############################
title: "PDF 개의 워터마크 조정: 다양한 보호" 
description: "다양한 워터마크 조정 기능을 사용하여 다양한 형식의 콘텐츠를 보호하세요.필요에 맞게 원활하게 조정하세요."
subtitle: "GroupDocs.Watermark for Java 솔루션" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 Maven 패키지"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java 솔루션"
    link: "/watermark/java/"
    link_title: "자세히 알아보기"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **워터마크 조정**: 다양한 워터마크 조정 기능을 사용하여 다양한 문서 형식에서 콘텐츠를 보호합니다.특정 요구 사항을 쉽게 충족하도록 워터마킹 전략을 조정하세요.

############################# Steps ############################
steps:
    enable: true
    title: "Java 을(를) 사용하여 Pdf 문서 워터마크 조정"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** 를 사용하면 Java 개발자가 애플리케이션을 사용하여 많은 문서에서 워터마크를 쉽게 조정할 수 있습니다. 빠른 가이드는 다음과 같습니다.
      
      1. 먼저, **Watermarker** 클래스 생성자의 매개변수로 Pdf 파일을 전달해야 합니다. 바이트나 파일 스트림 또는 로컬 디스크 경로를 제공합니다.
      2. 둘째, 조정해야 할 워터마크를 찾습니다. 이전에 문서에 추가된 특정 속성이 있는 워터마크를 식별하려면 **SearchCriteria** 를 사용하세요.
      3. 검색하면 관련 워터마크 목록이 표시됩니다. 그런 다음 크기, 페이지 정렬, 텍스트, 색상, 이미지 콘텐츠 등을 포함한 속성을 조정할 수 있습니다. 이는 데이터에 대한 높은 수준의 사용자 정의를 제공합니다.
      4. 워터마크 조정을 마쳤으면 업데이트된 문서를 저장하세요. 로컬 파일 경로나 스트림을 사용하여 결과를 저장할 수 있습니다.
   
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
        // PDF 이미지 워터마크 조정

        // PDF 을 사용하여 Watermarker 를 인스턴스화합니다.
        Watermarker watermarker = new Watermarker("input.pdf");
        
        // 특정 이미지와 일치하도록 SearchCriteria 를 초기화합니다.
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);

        for (PossibleWatermark watermark : watermarks)
        {
            // 발견된 이미지 교체
            watermark.setImageData(imageData);
        }

        // 조정된 파일 저장
        watermarker.save("output.pdf");
        
        ```
        
############################# More features ############################
more_features:
  enable: true
  title: "Java 애플리케이션을 위한 고급 PDF 워터마크 관리"
  description: "GroupDocs.Watermark API는 개발자가 워터마킹 기능을 Java 애플리케이션에 원활하게 통합할 수 있도록 합니다.광범위한 문서 형식에서 워터마크를 추가, 편집, 제거 및 검색할 수 있습니다."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "워터마크 조정"
  features:
    # feature loop
    - title: "간편한 워터마크 통합"
      content: "GroupDocs.Watermark 는 Java 애플리케이션 내의 다양한 비즈니스 문서 및 파일에 다양한 워터마크를 추가하는 프로세스를 간소화합니다.개발자는 워터마크를 적용할 수 있을 뿐만 아니라 프로그래밍 방식으로 기존 워터마크를 업데이트하거나 제거할 수도 있습니다."

    # feature loop
    - title: "세분화된 워터마크 커스터마이징"
      content: "API는 워터마크에 대한 광범위한 사용자 지정 옵션을 제공합니다.개발자는 크기, 회전, 색상, 글꼴, 스타일 및 기타 속성을 쉽게 조정하여 원하는 시각적 효과를 얻을 수 있습니다."

    # feature loop
    - title: "PDF 개의 기본 문서 기능 활용"
      content: "개발자는 대상 문서 형식에 따라 워터마크 배치를 위한 기본 기능을 활용할 수 있습니다.이러한 기능에는 문서 페이지 배경, 주석, 헤더 또는 워터마크 컨테이너인 기타 개체가 포함될 수 있습니다."
      
  code_samples:
    # code sample loop
    - title: "스프레드시트에서 이미지 워터마크 조정"
      content: |
        이 예제에서는 Excel 워크시트에서 특정 도형의 이미지를 조정하는 방법을 보여줍니다.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  문서를 스프레드시트로 불러오기
        SpreadsheetLoadOptions loadOptions = new SpreadsheetLoadOptions();
        Watermarker watermarker = new Watermarker("source.xlsx", loadOptions);

        //  새 워터마크 바이트 가져오기
        File file = new File("new_watermark.png");
        byte[] imageBytes = new byte[(int) file.length()];
        FileInputStream inputStream = new FileInputStream(file);
        inputStream.read(imageBytes);
        inputStream.close();

        //  특정 워터마크의 내용 조정
        for (SpreadsheetShape shape : content.getWorksheets().get_Item(0).getShapes())
        {
            if (shape.getImage() != null)
            {
                shape.setImage(new SpreadsheetWatermarkableImage(imageBytes));
            }
        }

        //  결과 문서 저장
        watermarker.save("result.xlsx");
        watermarker.close();
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
    title: "GroupDocs.Watermark for Java 를 사용하여 인기 있는 형식의 워터마크 관리"
    exclude: "PDF"
    description: "다양한 워터마크 조정 기능을 사용하여 다양한 형식의 콘텐츠를 보호하세요.필요에 맞게 원활하게 조정하세요."
    items: 
        # format loop 1
        - name: "워터마크 PDF"
          format: "PDF"
          link: "/watermark/java/adjust//pdf/"
          description: "어도비 Portable 문서 형식"

        # format loop 2
        - name: "워터마크 Word"
          format: "WORD"
          link: "/watermark/java/adjust//word/"
          description: "MS Word 및 오픈 오피스 문서"
          
        # format loop 3
        - name: "워터마크 Excel"
          format: "EXCEL"
          link: "/watermark/java/adjust//excel/"
          description: "MS Excel 및 오픈 오피스 스프레드시트"

        # format loop 4
        - name: "워터마크 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/adjust//powerpoint/"
          description: "MS PowerPoint 및 오픈 오피스 프레젠테이션"

        # format loop 5
        - name: "워터마크 DOCX"
          format: "DOCX"
          link: "/watermark/java/adjust//docx/"
          description: "마이크로소프트 Word 오픈 XML 문서"
          
        # format loop 6
        - name: "워터마크 PPTX"
          format: "PPTX"
          link: "/watermark/java/adjust//pptx/"
          description: "PowerPoint 오픈 XML 프레젠테이션"
          
        # format loop 7
        - name: "워터마크 XLSX"
          format: "XLSX"
          link: "/watermark/java/adjust//xlsx/"
          description: "마이크로소프트 Excel 오픈 XML 스프레드시트"

        # format loop 8
        - name: "워터마크 DOC"
          format: "DOC"
          link: "/watermark/java/adjust//doc/"
          description: "마이크로소프트 Word 97 - 2007 문서"

        # format loop 9
        - name: "워터마크 XLS"
          format: "XLS"
          link: "/watermark/java/adjust//xls/"
          description: "마이크로소프트 Excel 워크북 97-2003"

        # format loop 10
        - name: "워터마크 PPT"
          format: "PPT"
          link: "/watermark/java/adjust//ppt/"
          description: "PowerPoint 프레젠테이션 97-2003"

        # format loop 11
        - name: "워터마크 RTF"
          format: "RTF"
          link: "/watermark/java/adjust//rtf/"
          description: "리치 텍스트 포맷"

---