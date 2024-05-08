
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:18
draft: false
lang: ko
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "애드저스트 Excel 워터마크 툴 - GroupDocs.Watermark"
head_description: "GroupDocs.Watermark 를 사용하여 워터마크를 손쉽게 조정, 업데이트 및 관리할 수 있습니다.문서를 쉽게 사용자 지정할 수 있습니다."

############################# Header ############################
title: "스프레드시트 워터마크 조정 도구: 매우 간단함" 
description: "직관적인 워터마크 편집 도구를 사용하여 문서를 개선하세요.워크플로를 손쉽게 간소화하세요."
subtitle: "GroupDocs.Watermark for Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 Maven 다운로드"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java API"
    link: "/watermark/java/"
    link_title: "자세히 알아보기"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **워터마크 조정 도구**: 워터마크 도구는 문서를 개선하고 보호할 수 있는 사용자 친화적인 솔루션을 제공합니다.직관적인 편집 기능을 사용하면 워터마크를 쉽게 관리할 수 있어 문서 보안과 신뢰성이 보장됩니다.

############################# Steps ############################
steps:
    enable: true
    title: "Java을(를) 사용하여 Excel 문서의 워터마크를 조정합니다."
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** 를 사용하면 Java 개발자가 몇 가지 간단한 단계를 구현하여 애플리케이션에서 텍스트 워터마크를 쉽게 조정할 수 있습니다.
      
      1. Excel 파일을 **Watermarker** 라는 API의 기본 객체에 로드하세요. 추가 처리를 위해 파일을 스트림이나 로컬 디스크의 경로로 제공할 수 있습니다.
      2. 다음 단계는 조정해야 할 워터마크를 찾는 것입니다. **SearchCriteria** 는 이전에 문서에 추가된 올바른 속성을 가진 워터마크를 식별하는 데 도움이 됩니다.
      3. **Search** 절차의 결과로 적합한 워터마크 목록을 가져옵니다. 크기, 페이지 정렬, 텍스트, 색상, 이미지 내용 등과 같은 발견된 워터마크 속성을 조정합니다. 데이터를 사용자 정의하는 방법은 많습니다.
      4. 워터마크 조정 프로세스가 완료되면 업데이트된 문서를 저장해야 합니다. 결과를 저장하려면 로컬 파일 경로, 파일 또는 바이트 스트림을 사용하십시오.
   
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

        // EXCEL 텍스트 워터마크 조정

        // 입력 EXCEL 문서로 Watermarker 를 인스턴스화합니다.
        Watermarker watermarker = new Watermarker("input.xslx");

        // TextSearchCriteria 를 초기화하고 텍스트 워터마크를 찾습니다.
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        
        // 텍스트 워터마크 속성 조정
        for (PossibleWatermark watermark : watermarks)
        {
            watermark.getFormattedTextFragments().clear();
            watermark.getFormattedTextFragments().
                add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
        }

        // 업데이트된 문서 저장
        watermarker.save("output.xslx");
        
        ```            
        
############################# More features ############################
more_features:
  enable: true
  title: "EXCEL 워터마크 조정 심층 분석"
  description: "우리의 API는 Java 애플리케이션이 널리 사용되는 문서 형식에서 워터마크를 추가, 편집, 제거 및 검색할 수 있도록 합니다."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "워터마크 조정"
  features:
    # feature loop
    - title: "문서에 손쉽게 워터마크 추가"
      content: "GroupDocs.Watermark 는 Java 명의 개발자를 위한 워터마킹을 간소화합니다.다양한 비즈니스 문서 및 파일에 다양한 워터마크를 추가합니다.워터마크를 적용할 수 있을 뿐만 아니라 기존 워터마크를 업데이트하거나 제거할 수도 있습니다."

    # feature loop
    - title: "필요에 맞게 워터마크를 사용자 지정하세요"
      content: "API는 광범위한 사용자 지정 옵션을 제공합니다.크기, 회전, 색상, 글꼴, 스타일 등을 쉽게 조정하여 완벽한 워터마크를 얻을 수 있습니다."

    # feature loop
    - title: "EXCEL 개의 기본 문서 기능 사용"
      content: "특정 문서 형식에 따라 기본 기능을 활용할 수 있습니다.여기에는 문서 페이지 배경, 주석, 헤더 또는 워터마크 컨테이너로 사용되는 기타 개체가 포함될 수 있습니다."
      
  code_samples:
    # code sample loop
    - title: "PDF 텍스트 워터마크 조정"
      content: |
        이 예제에서는 특정 아티팩트의 텍스트를 조정하는 방법을 보여줍니다.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  PDF 문서 불러오기
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  문서 콘텐츠 가져오기
        PdfContent pdfContent = watermarker.getContent(PdfContent.class);

        //  특정 워터마크 텍스트 조정
        for (PdfArtifact artifact : pdfContent.getPages().get_Item(0).getArtifacts())
        {
            if (artifact.getText().contains("Test"))
            {
                artifact.setText("Passed");
            }
        }

        //  문서 저장
        watermarker.save("result.pdf");
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
    title: "다른 포맷의 경우 GroupDocs.Watermark for Java 를 통해 워터마크를 조정합니다."
    exclude: "EXCEL"
    description: "다양한 문서 형식에서 워터마크를 쉽게 사용자 지정할 수 있습니다.문서 보안 및 신뢰성을 손쉽게 강화하세요."
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