---
############################# Static ############################
layout: "family"
date:  2024-06-26T07:20:48
draft: false

product: "Watermark"
product_tag: "watermark"

lang: ko

############################# Head ############################
head_title: "문서 워터마크 C# Java Node.js Python | 워터 마크를 추가"
head_description: "PDF, 이미지 및 문서에 워터마크를 추가합니다.Microsoft Office, PDF, OpenDocument, 이미지 등에 대한 워터마킹 솔루션"

############################# Header ############################
title: "문서 워터마크 솔루션"
description:  |
  문서 및 이미지에 텍스트 및 이미지 워터마크를 추가합니다.

  편리한 방법으로 문서 워터마크를 검색하고 수정할 수 있습니다.

  문서에 표시된 워터마크에 대한 정보를 얻을 수 있습니다.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "플랫폼 선택"
  title: "플랫폼 독립성"
  description: "GroupDocs.Watermark 라이브러리는 다음 운영 체제 및 프레임워크를 지원합니다."
  details_link_title: "자세히 알아보기"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Watermark .NET 
      color: "blue"
      tag: "net"
      link: "/watermark/net/"
      features_link: "https://docs.groupdocs.com/watermark/net/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    .NET Framework 4.5 or higher <br> .NET Core 3.0 or higher <br> .NET 5.0 or higher
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Watermark Java
      color: "red"
      tag: "java"
      link: "/watermark/java/"
      features_link: "https://docs.groupdocs.com/watermark/java/system-requirements/"
      features:
          # features loop
          - rows: "4"
            content: |
                    Java 8 or higher <br> Kotlin
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Watermark Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/watermark/nodejs-java/"
      features_link: "https://docs.groupdocs.com/watermark/"
      features:
          # features loop
          - rows: "4"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> 기타 모든 텍스트 편집기
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

    # items loop
    - title: "Python"
      description: GroupDocs.Watermark Python
      color: "yellow"
      tag: "python-net"
      link: "/watermark/python-net/"
      features_link: "https://docs.groupdocs.com/watermark/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Python 3.9+ and .Net 6+
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "4"
            content: |
                    IDLE <br> PyCharm <br> Visual Studio Code
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Watermark 기능 리뷰"
  description: "널리 사용되는 문서 형식에 대해 다양한 워터마크 유형을 추가, 검색 및 업데이트하도록 설계된 라이브러리입니다."

  items:
    # items loop
    - icon: "protect"
      title: "워터마크로 파일 보호"
      content: "비즈니스 문서에 텍스트 및 이미지 워터마크를 추가합니다."

    # items loop
    - icon: "search"
      title: "기존 워터마크 검색"
      content: "이전에 문서에 삽입한 워터마크에 대한 자세한 정보를 얻을 수 있습니다."

    # items loop
    - icon: "manipulate"
      title: "문서 워터마크 조작"
      content: "텍스트, 스타일, 이미지 및 기타 워터마크 기능을 제어합니다."

    # items loop
    - icon: "additional"
      title: "다양한 추가 기능"
      content: "문서 정보 가져오기, 하이퍼링크 또는 페이지 배경 업데이트 등"

############################# Code Samples ###############################
code_samples:
  enable: true
  title: "워터마크로 문서 보호"
  description: "GroupDocs.Watermark 일반적인 작업 코드 예제"

  items:
    # items loop
    - title: "워터마크 만들기."
      content: "문서에 워터마크를 추가하려면 대상 파일의 경로를 입력합니다.특정 페이지에 사용자 지정 워터마크를 표시하려면 다양한 옵션을 선택할 수 있습니다."
      samples:
          # samples loop
          - language: "C#"
            color: "blue"
            content: |
                    <code class="language-csharp" data-lang="csharp">
                        // 워터마킹할 문서를 지정합니다.

                        using (Watermarker watermarker = new Watermarker("source.docx"))
                        {
                          // 워터마크 오브젝트 만들기
                          TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                          // 워터마크 옵션 설정
                          watermark.ForegroundColor = Color.Red;
                          watermark.HorizontalAlignment = HorizontalAlignment.Center;
                          watermark.VerticalAlignment = VerticalAlignment.Center;

                          // 워터마크 추가 및 처리된 파일 저장
                          watermarker.Add(watermark);
                          watermarker.Save("result.docx");
                        }                    
                    </code>

          # samples loop
          - language: "Java"
            color: "red"
            content: |
                    <code class="language-java" data-lang="java">
                        // 워터마킹할 문서를 지정합니다.

                        Watermarker watermarker = new Watermarker("source.docx");

                        // 워터마크 오브젝트 만들기
                        TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // 워터마크 옵션 설정
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // 워터마크 추가 및 처리된 파일 저장
                        watermarker.add(watermark);
                        watermarker.save("result.docx");
                        watermarker.close();

                    </code>

          # samples loop
          - language: "TypeScript"
            color: "green"
            content: |
                    <code class="language-java" data-lang="javascript">
                        // 워터마킹할 문서를 지정합니다.

                        const watermarker = new Watermarker("source.docx");
    
                        // 워터마크 오브젝트 만들기
                        const watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // 워터마크 옵션 설정
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // 워터마크 추가 및 처리된 파일 저장
                        watermarker.add(watermark);
                        watermarker.save("result.docx");                        

                    </code>

          # samples loop
          - language: "Python"
            color: "yellow"
            content: |
                    <code class="python-net" data-lang="python">
                        def run():

                            # 워터마킹할 문서를 지정합니다.
                            with groupdocs.watermark.Watermarker("source.docx") as watermarker:
                                font = groupdocs.watermark.watermarks.Font("Arial", 36.0)

                                # 워터마크 오브젝트 만들기
                                watermark = groupdocs.watermark.watermarks.TextWatermark("top secret", font)

                                # 워터마크 옵션 설정
                                watermark.foreground_color = groupdocs.watermark.watermarks.Color.red;
                                watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
                                watermark.vertical_alignment = groupdocs.watermark.common.VerticalAlignment.CENTER

                                # 워터마크 추가 및 처리된 파일 저장
                                watermarker.add(watermark)
                                watermarker.save("result.docx")

                    </code>

############################# Supported Formats ###############################
formats:
  enable: true
  title: "50개 이상의 파일 형식 지원"
  description: "GroupDocs.Watermark 는 널리 사용되는 문서 및 파일 형식에 워터마킹을 제공합니다."

############################# Metrics ###############################
metrics:
  enable: true
  title: "우리 도서관 통계 데이터"
  description: "주요 지표를 자세히 살펴보고 우리의 성과, 영향력, 성장에 대한 통찰력을 얻으세요."

  items:
    # items loop
    - number: "50+"
      title: "지원되는 형식"
      content: "라이브러리는 가장 널리 사용되는 50가지 이상의 파일 형식을 처리할 수 있습니다."

    # items loop
    - number: "500k"
      title: "NuGet 개 다운로드"
      content: ".NET 용 GroupDocs.Watermark 은 NuGet 에서 50만 회 이상 다운로드된 인기 라이브러리입니다."

    # items loop
    - number: "15k"
      title: "메이븐 다운로드"
      content: "Maven에서 15,000회 이상의 다운로드를 기록한 GroupDocs.Watermark 은 Java 명의 개발자들에게 인기 있는 앱입니다."

    # items loop
    - number: "140+"
      title: "행복한 고객"
      content: "전 세계 개인 개발자와 상위 기업은 혁신적인 솔루션을 구축하기 위해 당사의 라이브러리를 선호합니다."


############################# Customers ###############################
customers:
  enable: true
  title: "우리의 행복한 고객들"
  description: "GroupDocs 개의 도서관은 전 세계적으로 유명하고 유명한 브랜드에 고용되어 있습니다."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "시작할 준비가 되셨나요?"
  description: "플랫폼에서 GroupDocs.Watermark 개의 기능을 무료로 사용해 보세요"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/watermark/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/watermark/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/watermark/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "자주 묻는 질문"
  description: "자주 묻는 질문을 확인하세요"

  items:
    # items loop
    - question: "GroupDocs.Watermark 에서 문서 조작을 위해 외부 라이브러리가 필요합니까?"
      answer: "GroupDocs.Watermark 는 독립적으로 작동하므로 Adobe Acrobat, Microsoft Office 등과 같은 타사 소프트웨어가 필요하지 않습니다."

    # items loop
    - question: "구매하기 전에 GroupDocs.Watermark 개의 기능을 테스트할 수 있나요?"
      answer: "네, GroupDocs.Watermark 은 (는) 무료 평가판을 제공합니다!설치해서 사용해 보십시오. 단, 평가판 버전은 문서에 '평가판 배지'를 추가하므로 처음 3페이지만 처리됩니다.전체 경험을 원하시나요?30일 임시 라이선스를 무료로 받아 전체 기능을 이용할 수 있습니다.자세한 내용은 [임시 라이선스](https://purchase.groupdocs.com/temporary-license/) 를 참조하십시오."

    # items loop
    - question: "어떤 라이선스 유형이 제공되나요?"
      answer: "GroupDocs.Watermark 라이선스가 필요하세요?옵션이 있습니다!다양한 옵션을 기반으로 라이선스 중에서 선택하세요.팀의 개발자 수.배포 위치 (예: 단일 사무실 또는 원격 작업장).최종 고객 배포 부서에서 SDK/API를 클라이언트와 공유해야 하나요?또는 월별 사용 라이선스도 있습니다. 즉, 요금제 요금제로 사용한 만큼만 요금을 지불하면 됩니다.자세히 알아보고 완벽한 [가격](https://purchase.groupdocs.com/pricing/watermark/net/) 을 찾아보세요."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Watermark 로우 코드 API"
  description: "클라우드 기반 REST API를 사용하여 애플리케이션에서 파일에 워터마크를 추가합니다."
  
  items:
    # items loop
    - title: "GroupDocs.Watermark Cloud for cURL"
      content: "cURL REST ful API를 사용하여 PDF, Word, Excel, PowerPoint, JPEG 및 기타 널리 사용되는 파일 형식을 워터마킹할 수 있습니다."
      icon: "groupdocs_watermark-for-curl"
      link: "https://products.groupdocs.cloud/watermark/curl"

    # items loop
    - title: "GroupDocs.Watermark Cloud for .NET"
      content: ".NET 용 Cloud SDK의 문서 워터마킹 기능으로 .NET 애플리케이션을 강화하세요.비즈니스 문서를 직접 보호하세요."
      icon: "groupdocs_watermark-for-net"
      link: "https://products.groupdocs.cloud/watermark/net"

    # items loop
    - title: "GroupDocs.Watermark Cloud for Java"
      content: "GroupDocs.Watermark Java 용으로 설계된 SDK는 Java 개의 애플리케이션 및 비즈니스 파일에 새로운 가능성을 제공합니다."
      icon: "groupdocs_watermark-for-java"
      link: "https://products.groupdocs.cloud/watermark/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Watermark 웹 앱"
  description: "GroupDocs 은 문서에 워터마크를 추가할 수 있는 웹 애플리케이션에 대한 액세스 권한을 부여합니다.50가지 이상의 인기 있는 파일 형식을 즐겨 사용하는 브라우저에서 무료로 워터마킹할 수 있습니다."

  items:
    # items loop
    - title: "GroupDocs.Watermark Total"
      content: "모든 장치에서 문서에 워터마크를 추가할 수 있는 온라인 도구입니다."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/watermark/total"

    # items loop
    - title: "GroupDocs.Watermark DOCX"
      content: "워터마크 MS Word DOCX 온라인."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/watermark/docx"

    # items loop
    - title: "GroupDocs.Watermark PDF"
      content: "PDF 개의 문서를 온라인으로 보호하십시오."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/watermark/pdf"


      


---