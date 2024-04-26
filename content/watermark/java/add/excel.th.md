
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:38:57
draft: false
lang: th
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "สร้างลายน้ำใน Excel สเปรดชีตสำหรับ Java"
head_description: "ใช้การสร้างลายน้ำข้อความและรูปภาพใน Excel ได้อย่างง่ายดายด้วย Java เพื่อปกป้องสเปรดชีตข้อมูล Excel ของคุณ"

############################# Header ############################
title: "ทำลายน้ำ Excel โดยอัตโนมัติด้วยรหัส Java" 
description: "ใช้ลายน้ำข้อความหรือรูปภาพที่กำหนดเองในสเปรดชีต Excel โดยใช้ Javaคู่มือนี้มีคำแนะนำทีละขั้นตอนเพื่อเพิ่มความปลอดภัยของเอกสารและการสร้างแบรนด์ ซึ่งปรับให้เหมาะกับความต้องการระดับมืออาชีพที่หลากหลาย"
subtitle: "GroupDocs.Watermark for Java เอพีอี" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดฟรี Maven"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java ห้องสมุด"
    link: "/watermark/java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Java นำเสนอการจัดการลายน้ำที่ครอบคลุมในสเปรดชีต Excel ช่วยให้นักพัฒนาสามารถสร้าง ปรับแต่ง และล้างลายน้ำได้อย่างง่ายดายรองรับรูปแบบไฟล์ Excel ยอดนิยมทั้งหมด ช่วยให้สามารถฝังลายน้ำทั้งข้อความและรูปภาพที่สามารถปรับแต่งได้ในแบบอักษร สี ขนาด และตำแหน่ง GroupDocs.Watermark ยังรวมถึงคุณสมบัติสำหรับการค้นหาลายน้ำ เพื่อให้แน่ใจว่าลายน้ำของคุณยังคงสภาพและป้องกันการงัดแงะเหมาะสำหรับแอปพลิเคชันที่ต้องการการปรับปรุงความปลอดภัยของเอกสารภายใน Java สภาพแวดล้อม

############################# Steps ############################
steps:
    enable: true
    title: "เพิ่มลายน้ำลงในเอกสาร Excel ผ่าน Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** ทำให้นักพัฒนา Java สามารถเพิ่มลายน้ำประเภทต่างๆลงในรูปแบบไฟล์ธุรกิจยอดนิยมได้ง่ายเพิ่มไลบรารีของเราลงในเอกสารแอปพลิเคชันและลายน้ำของคุณในขั้นตอนง่ายๆสองสามขั้นตอนดังที่ระบุไว้ด้านล่าง
      
      1. **Watermarker**คุณต้องสร้างอินสแตนซ์ก่อนการประมวลผลเอกสารอย่าลืมส่งไฟล์ Excel ไปยังตัวสร้างเป็นเส้นทางหรือวัตถุสตรีม
      2. **ลายน้ำ** ประเภทที่ต้องการสามารถวางได้ไม่เพียง แต่ในหน้าเอกสารเฉพาะ แต่ยังอยู่ในส่วนเอกสารดั้งเดิมเช่นไฟล์แนบหรือส่วนหัว
      3. ตั้งค่าคุณสมบัติลายน้ำ เช่น ความสูงและความกว้าง การจัดตำแหน่งหน้า (ด้านบน ซ้าย กลาง ฯลฯ) ตระกูลและสีแบบอักษรและอื่น ๆ อีกมากมาย
      4. **Watermarker** เพื่อเพิ่มลายน้ำใหม่คุณสามารถเพิ่มลายน้ำได้มากเท่าที่คุณต้องการขอแนะนำให้บันทึกเอกสารที่ประมวลผลไปยังตำแหน่งอื่น
   
    code:
      platform: "net"
      copy_title: "คัดลอก"
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
        copy_tip: "คลิกเพื่อคัดลอก"
        copy_done: "คัดลอก"
      links:
        #  loop
        - title: "ตัวอย่างเพิ่มเติม"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
        #  loop
        - title: "เอกสาร"
          link: "https://docs.groupdocs.com/watermark/java/"
          
      content: |
        ```java {style=abap}

        // เพิ่มลายน้ำข้อความลงใน EXCEL

        // ส่งไฟล์เพื่อเป็นลายน้ำไปยังเครื่องหมายน้ำ
        Watermarker watermarker = new Watermarker("input.xslx");
        
        // สร้างลายน้ำข้อความและตั้งค่าคุณสมบัติ
        TextWatermark watermark = new TextWatermark("My Watermark", new Font("Arial", 36));
        watermark.setForegroundColor(Color.getRed());

        // บันทึกไฟล์ลายน้ำ
        watermarker.add(watermark);
        watermarker.save("output.xslx");
        
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "เพิ่มลายน้ำของคุณได้อย่างง่ายดาย"
  description: "ใช้พลังของ GroupDocs.Watermark เพื่อสร้าง เขียน และเพิ่มลายน้ำในรูปแบบเอกสารหลายรูปแบบAPI นี้ไม่เพียง แต่ช่วยเพิ่มความปลอดภัยของเอกสาร แต่ยังปกป้องทรัพย์สินทางปัญญาของคุณด้วยการฝังลายน้ำที่ปรับแต่งได้ซึ่งมีความหลากหลายและทนทาน"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "เพิ่มลายน้ำ"
  features:
    # feature loop
    - title: "ตัวเลือกลายน้ำอเนกประสงค์"
      content: "สำรวจตัวเลือกลายน้ำที่หลากหลายด้วย GroupDocs.Watermarkตั้งแต่การปรับความทึบและการหมุนไปจนถึงขนาดการปรับขนาดตามสัดส่วน API ของเราช่วยให้คุณปรับแต่งลายน้ำได้อย่างแม่นยำตามความต้องการของคุณ เพื่อให้แน่ใจว่าสิ่งเหล่านี้ผสมผสานเข้ากับเอกสารของคุณได้อย่างราบรื่นในขณะที่ยังคงความสมบูรณ์ของเนื้อหา"

    # feature loop
    - title: "การจัดแต่งทรงลายน้ำขั้นสูง"
      content: "GroupDocs.Watermark ช่วยให้คุณสามารถจัดแต่งลายน้ำของคุณด้วยแบบอักษร สี และเงาต่างๆ ทำให้โดดเด่นและลบได้ยากขึ้นเพิ่มความสวยงามของเอกสารและภาพที่มีการป้องกันของคุณด้วยลายน้ำที่มีสไตล์ที่สะท้อนเอกลักษณ์และความเป็นมืออาชีพของแบรนด์ของคุณ"

    # feature loop
    - title: "การปูกระเบื้องและการวางตำแหน่งลายน้ำ"
      content: "ด้วย GroupDocs.Watermark ใช้เอฟเฟกต์การปูกระเบื้องเพื่อครอบคลุมเอกสารทั้งหมดของคุณเพื่อให้มั่นใจได้ว่ามีการปกป้องอย่างสมบูรณ์วางลายน้ำในตำแหน่งที่คุณต้องการ ไม่ว่าจะเป็นศูนย์กลาง มุม หรือตำแหน่งที่กำหนดเองตัวเลือกการวางตำแหน่งที่ยืดหยุ่นของเราช่วยปกป้องเอกสารของคุณจากการใช้งานและการทำซ้ำโดยไม่ได้รับอนุญาต"
      
  code_samples:
    # code sample loop
    - title: "PDF ลายน้ำคำอธิบายประกอบ"
      content: |
        ตัวอย่างนี้แสดงวิธีเพิ่มคำอธิบายประกอบลายน้ำลงในเอกสาร PDF
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  โหลดเอกสารเป็น PDF
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  สร้างลายน้ำตามคำอธิบายประกอบ PDF
        PdfAnnotationWatermarkOptions options = new PdfAnnotationWatermarkOptions();
        TextWatermark textWatermark = new TextWatermark("Annotation watermark", new Font("Arial", 8));

        //  ตั้งค่าตัวเลือกลายน้ำ
        textWatermark.setHorizontalAlignment(HorizontalAlignment.Left);
        textWatermark.setVerticalAlignment(VerticalAlignment.Top);

        //  เพิ่มลายน้ำข้อความลงในเอกสารผลลัพธ์
        watermarker.add(textWatermark, options);
        watermarker.save("result.pdf");

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "พร้อมที่จะเริ่มแล้วหรือยัง?"
  description: "ลองใช้คุณสมบัติ GroupDocs.Watermark ฟรีหรือขอใบอนุญาต"
  items:
    #  loop
    - title: "Maven ดาวน์โหลด"
      link: "https://releases.groupdocs.com/watermark/java/"
      color: "red"
        #  loop
    - title: "การออกใบอนุญาต"
      link: "https://purchase.groupdocs.com/pricing/watermark/java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "Java เทคนิคสำหรับเครื่องหมายน้ำ Excel"
    exclude: "EXCEL"
    description: "ใช้ GroupDocs.Watermark for Java ใช้ลายน้ำตามข้อความหรือรูปภาพกับสเปรดชีต Excel ได้อย่างง่ายดาย ช่วยเพิ่มความปลอดภัยของเอกสารและการสร้างแบรนด์เป็นส่วนหนึ่งของเวิร์กโฟลว์ธุรกิจของคุณ"
    items: 
        # format loop 1
        - name: "ลายน้ำ PDF"
          format: "PDF"
          link: "/watermark/java/add//pdf/"
          description: "รูปแบบเอกสาร Adobe Portable"

        # format loop 2
        - name: "ลายน้ำ Word"
          format: "WORD"
          link: "/watermark/java/add//word/"
          description: "MS Word และเอกสาร Open Office"
          
        # format loop 3
        - name: "ลายน้ำ Excel"
          format: "EXCEL"
          link: "/watermark/java/add//excel/"
          description: "MS Excel และสเปรดชีตโอเพ่นออฟฟิศ"

        # format loop 4
        - name: "ภาพลายน้ำ"
          format: "IMAGE"
          link: "/watermark/java/add//image/"
          description: "รูปแบบภาพยอดนิยม"

        # format loop 5
        - name: "ภาพลายน้ำ"
          format: "PHOTO"
          link: "/watermark/java/add//photo/"
          description: "รูปแบบภาพถ่าย"

        # format loop 6
        - name: "ลายน้ำ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/add//powerpoint/"
          description: "MS PowerPoint และงานนำเสนอแบบโอเพ่นออฟฟิศ"

        # format loop 7
        - name: "ลายน้ำ DOCX"
          format: "DOCX"
          link: "/watermark/java/add//docx/"
          description: "ไมโครซอฟท์ Word เปิดเอกสาร XML"
          
        # format loop 8
        - name: "ลายน้ำ PPTX"
          format: "PPTX"
          link: "/watermark/java/add//pptx/"
          description: "PowerPoint เปิดการนำเสนอ XML"
          
        # format loop 9
        - name: "ลายน้ำ XLSX"
          format: "XLSX"
          link: "/watermark/java/add//xlsx/"
          description: "ไมโครซอฟท์ Excel เปิดสเปรดชีต XML"

        # format loop 10
        - name: "ลายน้ำ JPEG"
          format: "JPEG"
          link: "/watermark/java/add//jpeg/"
          description: "JPEG รูปภาพ"

        # format loop 11
        - name: "ลายน้ำ PNG"
          format: "PNG"
          link: "/watermark/java/add//png/"
          description: "Portable กราฟิกเครือข่าย"

        # format loop 12
        - name: "ลายน้ำ TIFF"
          format: "TIFF"
          link: "/watermark/java/add//tiff/"
          description: "รูปแบบไฟล์รูปภาพแท็ก"

        # format loop 13
        - name: "ลายน้ำ WEBP"
          format: "WEBP"
          link: "/watermark/java/add//webp/"
          description: "รูปภาพเว็บ"

        # format loop 14
        - name: "ลายน้ำ DOC"
          format: "DOC"
          link: "/watermark/java/add//doc/"
          description: "ไมโครซอฟท์ Word 97 - เอกสาร 2007"

        # format loop 15
        - name: "ลายน้ำ XLS"
          format: "XLS"
          link: "/watermark/java/add//xls/"
          description: "ไมโครซอฟท์ Excel สมุดงาน 97-2003"

        # format loop 16
        - name: "ลายน้ำ PPT"
          format: "PPT"
          link: "/watermark/java/add//ppt/"
          description: "PowerPoint การนำเสนอ 97-2003"

        # format loop 17
        - name: "ลายน้ำ RTF"
          format: "RTF"
          link: "/watermark/java/add//rtf/"
          description: "รูปแบบข้อความที่หลากหลาย"

---