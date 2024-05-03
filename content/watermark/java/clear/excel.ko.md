
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:05
draft: false
lang: ko
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java API를 사용하여 Excel 에서 워터마크를 제거합니다."
head_description: "GroupDocs.Watermark for Java API를 사용하여 Excel 파일에서 워터마크를 쉽게 지우고, 삭제하거나, 편집할 수 있습니다.문서 무결성과 프레젠테이션을 개선하세요."

############################# Header ############################
title: "Java Excel 워터마크 관리" 
description: "GroupDocs.Watermark for Java 를 활용하여 Excel 스프레드시트의 워터마크를 효율적이고 정확하게 제거하거나 편집할 수 있습니다."
subtitle: "GroupDocs.Watermark for Java API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Maven 에서 무료 다운로드"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java 라이브러리"
    link: "/watermark/java/"
    link_title: "자세히 알아보기"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       개발자는 GroupDocs.Watermark for Java 라이브러리를 사용하여 Excel 파일의 워터마크를 원활하게 관리할 수 있습니다.이 도구는 텍스트와 이미지 워터마크의 제거, 조정 및 검색과 같은 작업을 지원합니다.문서의 보안이나 레이아웃을 손상시키지 않으면서 데이터를 깔끔하게 시각적으로 표현해야 하는 애플리케이션에 적합합니다.

############################# Steps ############################
steps:
    enable: true
    title: "Java을(를) 사용하여 워터마크의 Excel 문서를 지웁니다."
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/java/)**를 사용하면 이전에 추가된 워터마크가 포함된 비즈니스 문서를 쉽게 지울 수 있습니다. 라이브러리를 설치하고 몇 가지 간단한 단계를 통해 귀하의 Java 애플리케이션을 강화하세요.
      
      1. 먼저 Excel 문서를 사용하여 **Watermarker**라는 기본 클래스를 인스턴스화합니다. 우리 API는 스트림 또는 로컬 경로로 처리할 문서 전달을 지원합니다.
      2. 처리할 워터마크 세트를 제한하려면 **SearchCriteria**를 사용하세요. 텍스트나 형식 지정 기능뿐만 아니라 이미지를 검색 매개변수로 사용할 수도 있습니다. 그러면 더 구체적인 검색 매개변수를 제공하고 더 정확한 결과를 얻을 수 있습니다.
      3. 검색결과로 얻은 문서 워터마크 목록을 처리합니다. 문서를 지웁니다.
      4. 문서를 지운 후 결과를 로컬 파일 또는 바이트 스트림으로 저장합니다.
   
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

        // Excel 문서의 텍스트 워터마크 지우기

        // Excel 문서로 Watermarker를 인스턴스화합니다.
        Watermarker watermarker = new Watermarker("input.xslx");
        
        // 특정 워터마크 지우기
        PossibleWatermarkCollection possibleWatermarks = watermarker.search();
        possibleWatermarks.removeAt(0);

        // 처리된 파일 저장
        watermarker.save("output.xslx");
        
        ```    
        
############################# More features ############################
more_features:
  enable: true
  title: "Java API를 통한 효율적인 워터마크 제거"
  description: "PDF 및 Office 파일을 비롯한 다양한 문서 유형에서 워터마크를 제거하거나 지우는 Java API의 강력한 기능을 살펴보세요.깔끔한 시각적 효과를 유지하고 문서 무결성을 보호하려는 개발자에게 적합합니다."
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "워터마크 지우기"
  features:
    # feature loop
    - title: "워터마크를 정밀하게 제거하세요"
      content: "Java API를 활용하여 원본 문서 레이아웃을 그대로 유지하면서 워터마크를 정확하게 타겟팅하고 삭제할 수 있습니다.명확성과 정확성이 가장 중요한 민감한 문서 또는 공식 문서에 적합합니다."

    # feature loop
    - title: "워터마크 일괄 삭제"
      content: "여러 파일에서 동시에 워터마크를 제거하여 문서 처리 효율성을 향상시키세요.API는 일괄 작업을 지원하므로 대규모 작업에 필요한 시간과 리소스를 절약할 수 있습니다."

    # feature loop
    - title: "워터마크 요소 편집"
      content: "당사의 고급 편집 도구를 사용하면 워터마크 구성 요소를 선택적으로 편집할 수 있으므로 콘텐츠 보안을 보장하는 동시에 문서 프레젠테이션을 유연하게 관리할 수 있습니다."
      
  code_samples:
    # code sample loop
    - title: "PDF 투명 텍스트 워터마크"
      content: |
        이 예제에서는 PDF 문서에서 특정 형식의 텍스트가 포함된 모든 주석을 찾아 제거하는 방법을 보여 줍니다.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  PDF 문서 불러오기
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  문서 콘텐츠 가져오기
        PdfContent pdfContent = watermarker.getContent(PdfContent.class);

        //  특정 글꼴의 투명 텍스트 워터마크
        for (PdfPage page : pdfContent.getPages()){
            for (int i = page.getAnnotations().getCount() - 1; i >= 0; i--){
                for (FormattedTextFragment fragment : page.getAnnotations().get_Item(i).getFormattedTextFragments()){
                    if (fragment.getFont().getFamilyName() == "Verdana"){
                        page.getAnnotations().removeAt(i);
                        break;
                    }
                }
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
    title: "Java 에서 Excel 개의 워터마크 관리"
    exclude: "EXCEL"
    description: "Excel API가 Excel 문서에서 워터마크 제거를 단순화하여 파일 무결성과 명확성을 유지하는 방법을 알아보십시오."
    items: 
        # format loop 1
        - name: "워터마크 PDF"
          format: "PDF"
          link: "/watermark/java/clear//pdf/"
          description: "어도비 Portable 문서 형식"

        # format loop 2
        - name: "워터마크 Word"
          format: "WORD"
          link: "/watermark/java/clear//word/"
          description: "MS Word 및 오픈 오피스 문서"
          
        # format loop 3
        - name: "워터마크 Excel"
          format: "EXCEL"
          link: "/watermark/java/clear//excel/"
          description: "MS Excel 및 오픈 오피스 스프레드시트"

        # format loop 4
        - name: "워터마크 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/clear//powerpoint/"
          description: "MS PowerPoint 및 오픈 오피스 프레젠테이션"

        # format loop 5
        - name: "워터마크 DOCX"
          format: "DOCX"
          link: "/watermark/java/clear//docx/"
          description: "마이크로소프트 Word 오픈 XML 문서"
          
        # format loop 6
        - name: "워터마크 PPTX"
          format: "PPTX"
          link: "/watermark/java/clear//pptx/"
          description: "PowerPoint 오픈 XML 프레젠테이션"
          
        # format loop 7
        - name: "워터마크 XLSX"
          format: "XLSX"
          link: "/watermark/java/clear//xlsx/"
          description: "마이크로소프트 Excel 오픈 XML 스프레드시트"

        # format loop 8
        - name: "워터마크 DOC"
          format: "DOC"
          link: "/watermark/java/clear//doc/"
          description: "마이크로소프트 Word 97 - 2007 문서"

        # format loop 9
        - name: "워터마크 XLS"
          format: "XLS"
          link: "/watermark/java/clear//xls/"
          description: "마이크로소프트 Excel 워크북 97-2003"

        # format loop 10
        - name: "워터마크 PPT"
          format: "PPT"
          link: "/watermark/java/clear//ppt/"
          description: "PowerPoint 프레젠테이션 97-2003"

        # format loop 11
        - name: "워터마크 RTF"
          format: "RTF"
          link: "/watermark/java/clear//rtf/"
          description: "리치 텍스트 포맷"

---