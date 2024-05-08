---
############################# Static ############################
layout: "family"
date:  2024-05-08T17:25:28
draft: false

product: "Watermark"
product_tag: "watermark"

lang: vi

############################# Head ############################
head_title: "Hình mờ tài liệu C # Java Node.js | thêm hình mờ"
head_description: "Thêm hình mờ vào PDF, hình ảnh và tài liệu. Giải pháp đánh dấu hình mờ cho Microsoft Office, PDF, OpenDocument, Hình ảnh, v.v."

############################# Header ############################
title: "Giải pháp hình mờ tài liệu"
description:  |
  Thêm hình mờ văn bản và hình ảnh cho tài liệu và hình ảnh của bạn.

  Tìm kiếm và sửa đổi hình mờ tài liệu một cách thuận tiện.

  Nhận thông tin về hình mờ được trình bày trong tài liệu của bạn.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Chọn nền tảng của bạn"
  title: "Độc lập nền tảng"
  description: "Thư viện GroupDocs.Watermark hỗ trợ các hệ điều hành và framework sau:"
  details_link_title: "Tìm hiểu thêm"

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
                    .NET Framework 4.6.2 or higher <br> .NET Core 2.0 or higher <br> .NET 6.0 or higher
      
          # features loop
          - rows: "1"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider
      
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
                    Atom <br> Visual Studio Code <br> Bất kỳ trình soạn thảo văn bản nào khác
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

############################# Features ###############################
features:
  enable: true
  title: "Đánh giá tính năng GroupDocs.Watermark"
  description: "Thư viện được thiết kế để thêm, tìm kiếm và cập nhật các loại hình mờ khác nhau cho các định dạng tài liệu phổ biến."

  items:
    # items loop
    - icon: "protect"
      title: "Bảo vệ tệp bằng hình mờ"
      content: "Thêm hình mờ văn bản và hình ảnh vào tài liệu kinh doanh của bạn."

    # items loop
    - icon: "search"
      title: "Tìm kiếm hình mờ hiện có"
      content: "Nhận thông tin chi tiết về hình mờ được đặt trong tài liệu trước đó."

    # items loop
    - icon: "manipulate"
      title: "Thao tác hình mờ tài liệu"
      content: "Kiểm soát văn bản, kiểu dáng, hình ảnh và các tính năng hình mờ khác."

    # items loop
    - icon: "additional"
      title: "Các tính năng bổ sung khác nhau"
      content: "Nhận thông tin tài liệu, cập nhật siêu liên kết hoặc nền trang, v.v."

############################# Code Samples ###############################
code_samples:
  enable: true
  title: "Bảo vệ tài liệu bằng hình mờ"
  description: "GroupDocs.Watermark ví dụ mã hoạt động điển hình."

  items:
    # items loop
    - title: "Tạo hình mờ."
      content: "Để thêm hình mờ vào tài liệu, hãy cung cấp đường dẫn đến tệp đích. Bạn có nhiều tùy chọn để chọn để có được hình mờ tùy chỉnh trên một trang cụ thể."
      samples:
          # samples loop
          - language: "C#"
            color: "blue"
            content: |
                    <code class="language-csharp" data-lang="csharp">
                        // Chỉ định tài liệu sẽ được đánh dấu hình mờ

                        using (Watermarker watermarker = new Watermarker("source.docx"))
                        {
                          // Tạo đối tượng hình mờ
                          TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                          // Đặt tùy chọn hình mờ
                          watermark.ForegroundColor = Color.Red;
                          watermark.HorizontalAlignment = HorizontalAlignment.Center;
                          watermark.VerticalAlignment = VerticalAlignment.Center;

                          // Thêm hình mờ và lưu tệp đã xử lý
                          watermarker.Add(watermark);
                          watermarker.Save("result.docx");
                        }                    
                    </code>

          # samples loop
          - language: "Java"
            color: "red"
            content: |
                    <code class="language-java" data-lang="java">
                        // Chỉ định tài liệu sẽ được đánh dấu hình mờ

                        Watermarker watermarker = new Watermarker("source.docx");

                        // Tạo đối tượng hình mờ
                        TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // Đặt tùy chọn hình mờ
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // Thêm hình mờ và lưu tệp đã xử lý
                        watermarker.add(watermark);
                        watermarker.save("result.docx");
                        watermarker.close();

                    </code>

          # samples loop
          - language: "TypeScript"
            color: "green"
            content: |
                    <code class="language-java" data-lang="javascript">
                        // Chỉ định tài liệu sẽ được đánh dấu hình mờ

                        const watermarker = new Watermarker("source.docx");
    
                        // Tạo đối tượng hình mờ
                        const watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // Đặt tùy chọn hình mờ
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // Thêm hình mờ và lưu tệp đã xử lý
                        watermarker.add(watermark);
                        watermarker.save("result.docx");                        

                    </code>

############################# Supported Formats ###############################
formats:
  enable: true
  title: "50+ định dạng tệp được hỗ trợ"
  description: "GroupDocs.Watermark cung cấp hình mờ cho các định dạng tài liệu và tệp phổ biến."

############################# Metrics ###############################
metrics:
  enable: true
  title: "Dữ liệu thống kê thư viện của chúng tôi"
  description: "Đi sâu vào các chỉ số chính, tiết lộ thông tin chi tiết về thành tích, tác động và tăng trưởng của chúng tôi."

  items:
    # items loop
    - number: "50+"
      title: "Các định dạng được hỗ trợ"
      content: "Thư viện có thể xử lý hơn 50 định dạng tệp phổ biến nhất."

    # items loop
    - number: "800k"
      title: "NuGet lượt tải"
      content: "GroupDocs.Watermark for .NET là một thư viện phổ biến với hơn 800.000 lượt tải xuống trên NuGet."

    # items loop
    - number: "15k"
      title: "Tải xuống Maven"
      content: "Với hơn 15K lượt tải xuống trên Maven, GroupDocs.Watermark là một lựa chọn phổ biến cho Java nhà phát triển."

    # items loop
    - number: "140+"
      title: "Khách hàng hài lòng"
      content: "Các nhà phát triển cá nhân và các công ty hàng đầu trên toàn thế giới thích thư viện của chúng tôi để xây dựng các giải pháp sáng tạo."


############################# Customers ###############################
customers:
  enable: true
  title: "Khách hàng hài lòng của chúng tôi"
  description: "GroupDocs thư viện được sử dụng bởi các thương hiệu nổi tiếng và nổi tiếng trên toàn thế giới."

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
  title: "Sẵn sàng để bắt đầu?"
  description: "Dùng thử GroupDocs.Watermark tính năng miễn phí trên nền tảng của bạn"

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
  title: "Câu hỏi thường gặp"
  description: "Kiểm tra các câu hỏi thường gặp của chúng tôi"

  items:
    # items loop
    - question: "Thư viện bên ngoài có yêu cầu bởi GroupDocs.Watermark để thao tác tài liệu không?"
      answer: "GroupDocs.Watermark hoạt động độc lập, không cần phần mềm của bên thứ ba như Adobe Acrobat, Microsoft Office, v.v."

    # items loop
    - question: "Tôi có thể kiểm tra GroupDocs.Watermark tính năng trước khi mua không?"
      answer: "Có, GroupDocs.Watermark cung cấp bản dùng thử miễn phí! Cài đặt nó và dùng thử, nhưng hãy nhớ: Phiên bản dùng thử thêm 'huy hiệu dùng thử' vào tài liệu của bạn, chỉ 3 trang đầu tiên được xử lý. Bạn muốn trải nghiệm đầy đủ? Nhận giấy phép tạm thời 30 ngày miễn phí cho đầy đủ chức năng. Xem chi tiết trong [giấy phép tạm thời](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Những loại giấy phép nào được cung cấp?"
      answer: "Cần giấy phép GroupDocs.Watermark? Chúng tôi có những lựa chọn! Chọn từ các giấy phép dựa trên nhiều tùy chọn. Số lượng nhà phát triển trong nhóm của bạn Các vị trí triển khai như văn phòng đơn lẻ hoặc nơi làm việc từ xa. Phân phối khách hàng cuối có cần chia sẻ SDK/API với khách hàng không? Ngoài ra, có giấy phép sử dụng hàng tháng: Chỉ thanh toán cho những gì bạn sử dụng với các gói tính phí. Lặn sâu hơn và tìm ra [giá hoàn hảo](https://purchase.groupdocs.com/pricing/watermark/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Watermark API mã thấp"
  description: "Thêm hình mờ vào tệp bằng ứng dụng của bạn bằng cách sử dụng API REST dựa trên đám mây của chúng tôi."
  
  items:
    # items loop
    - title: "GroupDocs.Watermark Cloud for cURL"
      content: "Sử dụng API cURL REST ful để tạo hình mờ PDF, Word, Excel, PowerPoint, JPEG và các định dạng tệp phổ biến khác."
      icon: "groupdocs_watermark-for-curl"
      link: "https://products.groupdocs.cloud/watermark/curl"

    # items loop
    - title: "GroupDocs.Watermark Cloud for .NET"
      content: "Hỗ trợ .NET ứng dụng của bạn với các tính năng tạo hình mờ tài liệu bằng Cloud SDK cho .NET. Tự bảo vệ tài liệu kinh doanh của bạn."
      icon: "groupdocs_watermark-for-net"
      link: "https://products.groupdocs.cloud/watermark/net"

    # items loop
    - title: "GroupDocs.Watermark Cloud for Java"
      content: "GroupDocs.Watermark SDK được thiết kế cho Java cung cấp khả năng mới cho Java ứng dụng và tệp doanh nghiệp của bạn."
      icon: "groupdocs_watermark-for-java"
      link: "https://products.groupdocs.cloud/watermark/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Watermark Ứng dụng web"
  description: "GroupDocs cấp quyền truy cập vào ứng dụng web để thêm hình mờ vào tài liệu của bạn. Hơn 50 định dạng tệp phổ biến có thể được đánh dấu trong trình duyệt yêu thích của bạn MIỄN PHÍ."

  items:
    # items loop
    - title: "GroupDocs.Watermark Total"
      content: "Công cụ trực tuyến để thêm hình mờ vào tài liệu từ bất kỳ thiết bị nào."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/watermark/total"

    # items loop
    - title: "GroupDocs.Watermark DOCX"
      content: "Hình mờ MS Word DOCX trực tuyến."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/watermark/docx"

    # items loop
    - title: "GroupDocs.Watermark PDF"
      content: "Bảo vệ PDF tài liệu trực tuyến."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/watermark/pdf"


      


---