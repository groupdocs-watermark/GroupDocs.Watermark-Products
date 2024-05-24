---
############################# Static ############################
layout: "family"
date:  2024-05-08T17:25:28
draft: false

product: "Watermark"
product_tag: "watermark"

lang: th

############################# Head ############################
head_title: "ลายน้ำ เอกสาร C# Java Node.js | เพิ่มลายน้ำ"
head_description: "เพิ่มลายน้ำลงใน PDF รูปภาพและเอกสารโซลูชันการทำลายน้ำสำหรับ Microsoft Office, PDF, OpenDocument, รูปภาพและอื่น ๆ"

############################# Header ############################
title: "โซลูชันลายลายน้ำ เอกสาร"
description:  |
  เพิ่มลายน้ำข้อความและรูปภาพสำหรับเอกสารและรูปภาพของคุณ

  ค้นหาและแก้ไขลายน้ำเอกสารด้วยวิธีที่สะดวก

  รับข้อมูลเกี่ยวกับลายน้ำที่แสดงในเอกสารของคุณ

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "เลือกแพลตฟอร์มของคุณ"
  title: "อิสระของแพลตฟอร์"
  description: "ไลบรารี GroupDocs.Watermark รองรับระบบปฏิบัติการและเฟรมเวิร์กต่อไปนี้:"
  details_link_title: "เรียนรู้เพิ่มเติม"

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
                    Atom <br> Visual Studio Code <br> โปรแกรมแก้ไขข้อความอื่น ๆ
      
          # features loop
          - rows: "1"
            content: |
                    50+ file formats

############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Watermark รีวิวคุณสมบัติ"
  description: "ไลบรารีที่ออกแบบมาเพื่อเพิ่มค้นหาและอัปเดตลายน้ำประเภทต่างๆสำหรับรูปแบบเอกสารยอดนิยม"

  items:
    # items loop
    - icon: "protect"
      title: "ปกป้องไฟล์ด้วยลายน้ำ"
      content: "เพิ่มลายน้ำข้อความและรูปภาพลงในเอกสารทางธุรกิจของคุณ"

    # items loop
    - icon: "search"
      title: "ค้นหาลายน้ำที่มีอยู่"
      content: "รับข้อมูลโดยละเอียดเกี่ยวกับลายน้ำที่วางไว้ในเอกสารก่อนหน้านี้"

    # items loop
    - icon: "manipulate"
      title: "จัดการลายน้ำเอกสาร"
      content: "ควบคุมข้อความ สไตล์ รูปภาพ และคุณสมบัติลายน้ำอื่น ๆ"

    # items loop
    - icon: "additional"
      title: "คุณสมบัติเพิ่มเติมต่างๆ"
      content: "รับข้อมูลเอกสารอัปเดตไฮเปอร์ลิงก์หรือพื้นหลังของหน้า ฯลฯ"

############################# Code Samples ###############################
code_samples:
  enable: true
  title: "ปกป้องเอกสารด้วยลายน้ำ"
  description: "GroupDocs.Watermark ตัวอย่างรหัสการดำเนินงานทั่วไป"

  items:
    # items loop
    - title: "การสร้างลายน้ำ"
      content: "หากต้องการผนวกลายน้ำลงในเอกสาร ให้ระบุเส้นทางไปยังไฟล์เป้าหมายคุณมีตัวเลือกมากมายให้เลือกเพื่อให้ได้ลายน้ำที่กำหนดเองในหน้าเฉพาะ"
      samples:
          # samples loop
          - language: "C#"
            color: "blue"
            content: |
                    <code class="language-csharp" data-lang="csharp">
                        // ระบุเอกสารที่จะเป็นลายน้ำ

                        using (Watermarker watermarker = new Watermarker("source.docx"))
                        {
                          // สร้างวัตถุลายน้ำ
                          TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                          // ตั้งค่าตัวเลือกลายน้ำ
                          watermark.ForegroundColor = Color.Red;
                          watermark.HorizontalAlignment = HorizontalAlignment.Center;
                          watermark.VerticalAlignment = VerticalAlignment.Center;

                          // เพิ่มลายน้ำและบันทึกไฟล์ที่ประมวลผล
                          watermarker.Add(watermark);
                          watermarker.Save("result.docx");
                        }                    
                    </code>

          # samples loop
          - language: "Java"
            color: "red"
            content: |
                    <code class="language-java" data-lang="java">
                        // ระบุเอกสารที่จะเป็นลายน้ำ

                        Watermarker watermarker = new Watermarker("source.docx");

                        // สร้างวัตถุลายน้ำ
                        TextWatermark watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // ตั้งค่าตัวเลือกลายน้ำ
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // เพิ่มลายน้ำและบันทึกไฟล์ที่ประมวลผล
                        watermarker.add(watermark);
                        watermarker.save("result.docx");
                        watermarker.close();

                    </code>

          # samples loop
          - language: "TypeScript"
            color: "green"
            content: |
                    <code class="language-java" data-lang="javascript">
                        // ระบุเอกสารที่จะเป็นลายน้ำ

                        const watermarker = new Watermarker("source.docx");
    
                        // สร้างวัตถุลายน้ำ
                        const watermark = new TextWatermark("top secret", new Font("Arial", 36));

                        // ตั้งค่าตัวเลือกลายน้ำ
                        watermark.setForegroundColor(Color.getRed());
                        watermark.setHorizontalAlignment(HorizontalAlignment.Center);
                        watermark.setVerticalAlignment(VerticalAlignment.Center);

                        // เพิ่มลายน้ำและบันทึกไฟล์ที่ประมวลผล
                        watermarker.add(watermark);
                        watermarker.save("result.docx");                        

                    </code>

############################# Supported Formats ###############################
formats:
  enable: true
  title: "รองรับรูปแบบไฟล์ 50+"
  description: "GroupDocs.Watermark มีเครื่องหมายน้ำสำหรับเอกสารและรูปแบบไฟล์ยอดนิยม"

############################# Metrics ###############################
metrics:
  enable: true
  title: "ข้อมูลสถิติห้องสมุดของเรา"
  description: "เจาะลึกในตัวชี้วัดที่สำคัญ โดยเปิดเผยข้อมูลเชิงลึกเกี่ยวกับความสำเร็จ ผลกระทบ และการเติบโตของเรา"

  items:
    # items loop
    - number: "50+"
      title: "รูปแบบที่รองรับ"
      content: "ห้องสมุดสามารถประมวลผลรูปแบบไฟล์ที่ได้รับความนิยมมากกว่า 50 รูปแบบ"

    # items loop
    - number: "500k"
      title: "NuGet ดาวน์โหลด"
      content: "GroupDocs.Watermark สำหรับ .NET เป็นไลบรารียอดนิยมที่มีการดาวน์โหลดมากกว่า 500,000 รายการบน NuGet"

    # items loop
    - number: "15k"
      title: "ดาวน์โหลด Maven"
      content: "ด้วยการดาวน์โหลดมากกว่า 15K รายการบน Maven แล้ว GroupDocs.Watermark เป็นตัวเลือกยอดนิยมสำหรับนักพัฒนา Java"

    # items loop
    - number: "140+"
      title: "ลูกค้าที่มีความสุข"
      content: "นักพัฒนาแต่ละรายและ บริษัท ชั้นนำทั่วโลกชอบไลบรารีของเราในการสร้างโซลูชันที่เป็นนวัตกรรม"


############################# Customers ###############################
customers:
  enable: true
  title: "ลูกค้าที่มีความสุขของเรา"
  description: "ไลบรารี GroupDocs ใช้โดยแบรนด์ที่มีชื่อเสียงระดับโลกและโดดเด่นทั่วโลก"

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
  title: "พร้อมที่จะเริ่มแล้วหรือยัง?"
  description: "ลองใช้ฟีเจอร์ GroupDocs.Watermark ฟรีบนแพลตฟอร์มของคุณ"

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
  title: "คำถามที่พบบ่อย"
  description: "ตรวจสอบคำถามที่พบบ่อยของเรา"

  items:
    # items loop
    - question: "GroupDocs.Watermark จำเป็นต้องใช้ไลบรารีภายนอกสำหรับการจัดการเอกสารหรือไม่"
      answer: "GroupDocs.Watermark ทำงานได้อย่างอิสระไม่จำเป็นต้องใช้ซอฟต์แวร์ของบุคคลที่สามเช่น Adobe Acrobat, Microsoft Office เป็นต้น"

    # items loop
    - question: "ฉันสามารถทดสอบคุณสมบัติ GroupDocs.Watermark ก่อนซื้อได้หรือไม่"
      answer: "ใช่ GroupDocs.Watermark มีการทดลองใช้ฟรี!ติดตั้งและลองใช้ แต่โปรดทราบ: รุ่นทดลองเพิ่ม 'ป้ายทดลองใช้' ลงในเอกสารของคุณเพียง 3 หน้าแรกเท่านั้นที่ได้รับการประมวลผลต้องการประสบการณ์เต็มรูปแบบหรือไม่?รับใบอนุญาตชั่วคราว 30 วันฟรีสำหรับการทำงานเต็มรูปแบบดูรายละเอียดภายใต้ [ใบอนุญาตชั่วคราว](https://purchase.groupdocs.com/temporary-license/)"

    # items loop
    - question: "มีใบอนุญาตประเภทใดบ้าง"
      answer: "ต้องการใบอนุญาต GroupDocs.Watermark หรือไม่เรามีตัวเลือก!เลือกจากใบอนุญาตตามตัวเลือกมากมายจำนวนนักพัฒนาในทีมของคุณตำแหน่งการปรับใช้เช่นสำนักงานเดียวหรือสถานที่ทำงานระยะไกลการกระจายลูกค้าปลายทางจำเป็นต้องแบ่งปัน SDK/API กับลูกค้าหรือไม่หรือมีใบอนุญาตสำหรับการใช้งานรายเดือน: จ่ายเฉพาะสำหรับสิ่งที่คุณใช้กับแผนที่มีการวัดปริมาณเท่านั้นดำดิ่งลึกและค้นหา [ราคา](https://purchase.groupdocs.com/pricing/watermark/net/) ที่สมบูรณ์แบบ"

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Watermark API โค้ดต่ำ"
  description: "เพิ่มลายน้ำลงในไฟล์โดยแอปพลิเคชันของคุณโดยใช้ API REST บนคลาวด์ของเรา"
  
  items:
    # items loop
    - title: "GroupDocs.Watermark Cloud for cURL"
      content: "ใช้ cURL REST ful API เพื่อทำลายน้ำ PDF, Word, Excel, PowerPoint, JPEG และรูปแบบไฟล์ยอดนิยมอื่น ๆ"
      icon: "groupdocs_watermark-for-curl"
      link: "https://products.groupdocs.cloud/watermark/curl"

    # items loop
    - title: "GroupDocs.Watermark Cloud for .NET"
      content: "เพิ่มพลังให้กับแอปพลิเคชัน .NET ของคุณด้วยคุณสมบัติการทำลายน้ำเอกสารด้วย Cloud SDK สำหรับ .NETปกป้องเอกสารทางธุรกิจด้วยตัวคุณเอง"
      icon: "groupdocs_watermark-for-net"
      link: "https://products.groupdocs.cloud/watermark/net"

    # items loop
    - title: "GroupDocs.Watermark Cloud for Java"
      content: "GroupDocs.Watermark SDK ที่ออกแบบมาสำหรับ Java มอบความเป็นไปได้ใหม่สำหรับแอปพลิเคชัน Java และไฟล์ธุรกิจของคุณ"
      icon: "groupdocs_watermark-for-java"
      link: "https://products.groupdocs.cloud/watermark/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Watermark เว็บแอป"
  description: "GroupDocs ให้สิทธิ์เข้าถึงเว็บแอปพลิเคชันเพื่อเพิ่มลายน้ำลงในเอกสารของคุณรูปแบบไฟล์ยอดนิยมมากกว่า 50 รูปแบบสามารถทำลายน้ำในเบราว์เซอร์ที่คุณชื่นชอบได้ฟรี"

  items:
    # items loop
    - title: "GroupDocs.Watermark Total"
      content: "เครื่องมือออนไลน์เพื่อเพิ่มลายน้ำลงในเอกสารจากอุปกรณ์ใด ๆ"
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/watermark/total"

    # items loop
    - title: "GroupDocs.Watermark DOCX"
      content: "ลายน้ำ MS Word DOCX ออนไลน์"
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/watermark/docx"

    # items loop
    - title: "GroupDocs.Watermark PDF"
      content: "ปกป้องเอกสาร PDF ออนไลน์"
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/watermark/pdf"


      


---