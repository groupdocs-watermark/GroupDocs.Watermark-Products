
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:24
draft: false
lang: ko
format: Webp
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C #을 사용하여 WEBP 에 워터마크 추가"
head_description: ".NET C #을 활용하여 WEBP 개의 이미지에 워터마크를 동적으로 생성하고 임베드하여 포괄적인 보호를 보장합니다."

############################# Header ############################
title: "C #을 사용하여 WEBP 에 대한 워터마크 생성" 
description: ".NET C #을 사용하여 사용자 지정 워터마크를 만들고 WEBP 파일에 적용할 수 있습니다. 작업 보안을 유지해야 하는 디지털 아티스트와 콘텐츠 제작자에게 적합합니다."
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Nuget 에서 무료로 다운로드"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "자세히 알아보기"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for .NET 는 개발자에게 .NET C #을 통해 WEBP 이미지에 정교한 워터마크를 생성, 구성 및 추가할 수 있는 기능을 제공합니다.이 API를 사용하면 텍스트, 로고, 디지털 서명을 비롯한 워터마크를 정밀하게 사용자 지정할 수 있습니다.워터마크의 불투명도, 크기 및 위치를 조정하여 이미지의 미적 요소를 손상시키지 않으면서 완벽하게 통합할 수 있습니다.사진작가, 그래픽 디자이너 및 디지털 이미지 제작 및 배포에 관련된 모든 전문가에게 적합한 GroupDocs.Watermark 은 저작권이 WEBP 파일에 안전하게 포함되도록 합니다.모든 최신 .NET 프레임워크와 호환되므로 시각적 품질에 미치는 영향을 최소화하면서 이미지 보안을 강화합니다.

############################# Steps ############################
steps:
    enable: true
    title: "Webp 문서에 대한 워터마크를 손쉽게 생성"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/):** .NET 애플리케이션용 고급 워터마킹 라이브러리입니다. 적시에 워터마크를 사용하여 솔루션을 강화하고 문서를 보호하세요.
      
      1. **핵심 클래스: Watermarker.** 우리 API의 주요 클래스는 **Watermarker** 입니다. 문서를 처리하기 전에 인스턴스화해야 합니다. Webp 파일을 생성자에 경로 또는 스트림 객체로 전달하는 것을 잊지 마세요.
      2. **워터마크 만들기.** 다음 단계는 원하는 유형의 워터마크 개체를 만드는 것입니다. 특정 문서 페이지뿐만 아니라 이미지나 헤더와 같은 기본 문서 부분에도 배치할 수 있습니다.
      3. **모양 미세 조정.** 높이 및 너비, 위쪽, 왼쪽, 중앙 정렬, 글꼴 및 색상 등과 같은 워터마크 속성을 설정합니다.
      4. **적용 및 저장.** 새로운 워터마크를 추가하려면 **Watermarker** 메소드를 사용하세요. 필요한 만큼 워터마크를 자유롭게 추가하세요. 워터마크가 있는 문서를 원하는 위치에 저장할 수 있습니다.
   
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
        // WEBP 파일에 이미지 워터마크 생성

        // Watermarker 생성자에 소스 파일 경로를 제공하세요.
        using (Watermarker watermarker = new Watermarker("input.webp"))
        {
            // 이미지 파일로 이미지 워터마크 인스턴스 생성
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // 워터마크가 표시된 WEBP 결과 저장
            watermarker.Save("output.webp");
        }
        
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "워터마킹 게임의 품격을 높이세요"
  description: ".NET 용 GroupDocs.Watermark API를 사용하여 고급 워터마킹 기능을 활용하세요.이 강력한 도구를 사용하면 다양한 문서 유형에 워터마크를 정밀하게 사용자 지정하고 적용할 수 있으므로 시각적 방해를 최소화하면서 보안 및 저작권 준수를 극대화할 수 있습니다."
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "포괄적인 워터마킹 솔루션"
  features:
    # feature loop
    - title: "정교한 타일링 옵션"
      content: "타일링 옵션을 사용하여 문서 전체에 워터마크를 원활하게 확장할 수 있습니다.이 기능을 사용하면 워터마크가 문서 전체 영역을 덮을 수 있으므로 제거를 방지하고 디자인이나 가독성을 손상시키지 않으면서 문서를 완벽하게 보호할 수 있습니다."

    # feature loop
    - title: "생생한 컬러 커스터마이징"
      content: "워터마크에 색상을 더하세요!API를 사용하면 전체 스펙트럼 색상 사용자 정의가 가능하므로 기업 브랜딩 또는 문서 스타일에 완벽하게 맞는 워터마크를 적용할 수 있습니다.강력한 보안 기능을 유지하면서 시각적 매력을 향상시키세요."

    # feature loop
    - title: "향상된 보안 설정"
      content: "고급 워터마크 설정을 통해 문서 보안을 한 단계 끌어올리세요.보이는 요소와 보이지 않는 요소를 모두 포함하는 다중 레이어 워터마크를 구성하여 무단 복제를 방지하고 의도된 수신자만 중요한 정보에 액세스할 수 있도록 하십시오."
      
  code_samples:
    # code sample loop
    - title: "PowerPoint 개의 워터마크 생성"
      content: |
        이 예에서는 PPTX 개의 배경 이미지에 워터마크를 추가하는 방법을 보여줍니다.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  PPTX 프레젠테이션 불러오기
            var loadOptions = new PresentationLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pptx", loadOptions))
            {
                //  워터마크 속성 설정
                TextWatermark watermark = new TextWatermark("Protected image", new Font("Arial", 8));
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermark.RotateAngle = 45;
                watermark.SizingType = SizingType.ScaleToParentDimensions;
                watermark.ScaleFactor = 1;

                //  워터마크 슬라이드 배경
                PresentationContent content = watermarker.GetContent<PresentationContent>();
                foreach (PresentationSlide slide in content.Slides)
                {
                    if (slide.ImageFillFormat.BackgroundImage != null)
                    {
                        slide.ImageFillFormat.BackgroundImage.Add(watermark);
                    }
                }

                //  처리된 프레젠테이션 저장
                watermarker.save("result.pptx");
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
    title: ".NET C# 워터마크로 WEBP 개의 이미지 보호"
    exclude: "WEBP"
    description: ".NET C #을 사용하여 WEBP 개의 이미지에 사용자 지정 가능한 고급 워터마크를 삽입하여 창작물을 강력하게 보호하고 시각적으로 돋보이게 할 수 있습니다."
    items: 
        # format loop 1
        - name: "워터마크 PDF"
          format: "PDF"
          link: "/watermark/net/generate//pdf/"
          description: "어도비 Portable 문서 형식"

        # format loop 2
        - name: "워터마크 Word"
          format: "WORD"
          link: "/watermark/net/generate//word/"
          description: "MS Word 및 오픈 오피스 문서"
          
        # format loop 3
        - name: "워터마크 Excel"
          format: "EXCEL"
          link: "/watermark/net/generate//excel/"
          description: "MS Excel 및 오픈 오피스 스프레드시트"

        # format loop 4
        - name: "워터마크 이미지"
          format: "IMAGE"
          link: "/watermark/net/generate//image/"
          description: "인기 이미지 형식"

        # format loop 5
        - name: "워터마크 사진"
          format: "PHOTO"
          link: "/watermark/net/generate//photo/"
          description: "사진 형식"

        # format loop 6
        - name: "워터마크 PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/generate//powerpoint/"
          description: "MS PowerPoint 및 오픈 오피스 프레젠테이션"

        # format loop 7
        - name: "워터마크 DOCX"
          format: "DOCX"
          link: "/watermark/net/generate//docx/"
          description: "마이크로소프트 Word 오픈 XML 문서"
          
        # format loop 8
        - name: "워터마크 PPTX"
          format: "PPTX"
          link: "/watermark/net/generate//pptx/"
          description: "PowerPoint 오픈 XML 프레젠테이션"
          
        # format loop 9
        - name: "워터마크 XLSX"
          format: "XLSX"
          link: "/watermark/net/generate//xlsx/"
          description: "마이크로소프트 Excel 오픈 XML 스프레드시트"

        # format loop 10
        - name: "워터마크 JPEG"
          format: "JPEG"
          link: "/watermark/net/generate//jpeg/"
          description: "JPEG 이미지"

        # format loop 11
        - name: "워터마크 PNG"
          format: "PNG"
          link: "/watermark/net/generate//png/"
          description: "Portable 네트워크 그래픽"

        # format loop 12
        - name: "워터마크 TIFF"
          format: "TIFF"
          link: "/watermark/net/generate//tiff/"
          description: "태그 이미지 파일 형식"

        # format loop 13
        - name: "워터마크 WEBP"
          format: "WEBP"
          link: "/watermark/net/generate//webp/"
          description: "웹 사진"

        # format loop 14
        - name: "워터마크 DOC"
          format: "DOC"
          link: "/watermark/net/generate//doc/"
          description: "마이크로소프트 Word 97 - 2007 문서"

        # format loop 15
        - name: "워터마크 XLS"
          format: "XLS"
          link: "/watermark/net/generate//xls/"
          description: "마이크로소프트 Excel 워크북 97-2003"

        # format loop 16
        - name: "워터마크 PPT"
          format: "PPT"
          link: "/watermark/net/generate//ppt/"
          description: "PowerPoint 프레젠테이션 97-2003"

        # format loop 17
        - name: "워터마크 RTF"
          format: "RTF"
          link: "/watermark/net/generate//rtf/"
          description: "리치 텍스트 포맷"

---