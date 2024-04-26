
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:58
draft: false
lang: ko
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Excel 형식의 워터마크 편집"
head_description: "GroupDocs.Watermark for .NET 를 사용하여 문서를 손쉽게 사용자 지정하고 보호할 수 있습니다.문서 무결성을 높이고 Excel 워터마크를 쉽게 편집할 수 있습니다."

############################# Header ############################
title: "Excel 스프레드시트 편집 워터마크: .NET 효율성" 
description: ".NET 효율성을 위해 설계된 맞춤형 워터마킹 도구를 사용하여 문서 보안을 강화하십시오.Excel 개의 워터마크를 손쉽게 편집할 수 있습니다."
subtitle: "GroupDocs.Watermark for .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 Nuget 다운로드"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET 라이브러리"
    link: "/watermark/net/"
    link_title: "자세히 알아보기"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **저희 툴로 Excel 개의 워터마크 편집:** 저희 GroupDocs.Watermark for .NET 툴은 문서를 개선하고 보호하기 위한 효율적인 전략을 제공합니다..NET 명의 개발자를 위한 다양한 기능을 통해 워터마크를 쉽게 관리할 수 있어 문서 보안과 신뢰성을 보장할 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: ".NET 을 사용하여 Excel 문서의 워터마크 편집"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)**는 .NET 개발자가 다양한 Excel 문서 내에서 워터마크를 손쉽게 편집할 수 있도록 합니다.다음은 애플리케이션에서 API를 사용하는 방법에 대한 간단한 가이드입니다.
      
      1. **Watermarker** 클래스 생성자에 파라미터로 전달합니다.파일을 바이트 스트림, 파일 스트림 또는 로컬 디스크 경로로 제공할 수 있습니다.
      2. **SearchCriteria**를 활용하여 이전에 문서에 추가한 해당 속성을 가진 워터마크를 식별하십시오.
      3. 검색 후 관련 워터마크 목록을 얻을 수 있습니다.그런 다음 크기, 페이지 정렬, 텍스트, 색상, 이미지 콘텐츠 등과 같은 속성을 사용자 지정할 수 있습니다.이를 통해 데이터를 광범위하게 제어할 수 있습니다.
      4. 워터마크 편집을 완료한 후 업데이트된 문서를 저장합니다.로컬 파일 경로 또는 스트림을 활용하여 최종 결과를 저장할 수 있습니다.
   
    code:
      platform: "net"
      copy_title: "복사"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "클릭하여 복사"
        copy_done: "복사"
      links:
        #  loop
        - title: "더 많은 예시"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "문서화"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // EXCEL 텍스트 워터마크 편집

        // EXCEL 파일을 제공하는 워터마커 만들기
        using (Watermarker watermarker = new Watermarker("input.xslx"))
        {
            // 텍스트 검색 기준 구성 및 텍스트 워터마크 가져오기
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                 // 텍스트 워터마크 편집
                 watermark.FormattedTextFragments.Clear();
                 watermark.FormattedTextFragments.Add("passed", 
                    new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
            }

            // 문서 저장
            watermarker.Save("output.xslx");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "워터마크 수정에 대해 더 알아보기"
  description: "라이브러리를 통해 .NET 애플리케이션의 성능을 높이고 다양한 파일 형식 내에서 워터마크를 추가, 편집, 제거 또는 검색하십시오."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "워터마크 편집"
  features:
    # feature loop
    - title: "비즈니스용 워터마크 파일"
      content: "GroupDocs.Watermark for .NET 를 사용하여 파일 및 문서에 워터마크를 지정합니다.애플리케이션에 API를 구현하여 별도의 노력 없이 워터마크를 추가하고 관리할 수 있습니다.이전에 추가한 워터마크를 검색, 편집 및 제거할 수 있습니다."

    # feature loop
    - title: "요구 사항에 맞게 워터마크 미세 조정"
      content: "API는 포괄적인 사용자 지정 옵션 세트를 제공합니다.크기, 방향, 색 구성표, 글꼴 모음 등과 같은 요소를 손쉽게 수정하여 이상적인 워터마크를 만들 수 있습니다."

    # feature loop
    - title: "문서별 기능 활용"
      content: "사용 중인 파일 형식에 따라 내장 기능을 통합할 수 있습니다.여기에는 문서 배경, 주석, 헤더 또는 워터마크 컨테이너로 사용할 기타 요소가 포함될 수 있습니다."
      
  code_samples:
    # code sample loop
    - title: "Excel 워터마크 텍스트 편집"
      content: |
        이 예에서는 Excel 워크시트의 특정 워터마크에 대한 텍스트를 편집하는 방법을 보여 줍니다.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  XLSX 스프레드시트 불러오기
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  스프레드시트 콘텐츠 로드
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();

                //  워터마크 내부 텍스트 편집
                foreach (SpreadsheetShape shape in content.Worksheets[0].Shapes)
                {
                    if (shape.Text == "GroupDocs 2016")
                    {
                        shape.Text = "GroupDocs 2017";
                    }
                }

                //  출력 결과 저장
                watermarker.save("result.xlsx");
            }

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Watermark 기능을 무료로 체험하거나 라이선스를 요청하세요"
  items:
    #  loop
    - title: "Nuget 다운로드"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "라이선싱"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "워터마크를 다른 형식으로 사용자 지정하세요"
    exclude: "EXCEL"
    description: "GroupDocs.Watermark for .NET 를 사용하여 다양한 문서 형식을 필요에 맞게 워터마킹할 수 있습니다."
    items: 
        # format loop 1
        - name: "워터마크 PDF"
          format: "PDF"
          link: "/watermark/net/edit//pdf/"
          description: "어도비 Portable 문서 형식"

        # format loop 2
        - name: "워터마크 Word"
          format: "WORD"
          link: "/watermark/net/edit//word/"
          description: "MS Word 및 오픈 오피스 문서"
          
        # format loop 3
        - name: "워터마크 Excel"
          format: "EXCEL"
          link: "/watermark/net/edit//excel/"
          description: "MS Excel 및 오픈 오피스 스프레드시트"

        # format loop 4
        - name: "워터마크 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/edit//powerpoint/"
          description: "MS PowerPoint 및 오픈 오피스 프레젠테이션"

        # format loop 5
        - name: "워터마크 DOCX"
          format: "DOCX"
          link: "/watermark/net/edit//docx/"
          description: "마이크로소프트 Word 오픈 XML 문서"
          
        # format loop 6
        - name: "워터마크 PPTX"
          format: "PPTX"
          link: "/watermark/net/edit//pptx/"
          description: "PowerPoint 오픈 XML 프레젠테이션"
          
        # format loop 7
        - name: "워터마크 XLSX"
          format: "XLSX"
          link: "/watermark/net/edit//xlsx/"
          description: "마이크로소프트 Excel 오픈 XML 스프레드시트"

        # format loop 8
        - name: "워터마크 DOC"
          format: "DOC"
          link: "/watermark/net/edit//doc/"
          description: "마이크로소프트 Word 97 - 2007 문서"

        # format loop 9
        - name: "워터마크 XLS"
          format: "XLS"
          link: "/watermark/net/edit//xls/"
          description: "마이크로소프트 Excel 워크북 97-2003"

        # format loop 10
        - name: "워터마크 PPT"
          format: "PPT"
          link: "/watermark/net/edit//ppt/"
          description: "PowerPoint 프레젠테이션 97-2003"

        # format loop 11
        - name: "워터마크 RTF"
          format: "RTF"
          link: "/watermark/net/edit//rtf/"
          description: "리치 텍스트 포맷"

---