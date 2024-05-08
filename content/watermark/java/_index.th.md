---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:29
draft: false

lang: th
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Java ห้องสมุดลายน้ำ | เพิ่มลายน้ำลงในเอกสาร"
head_description: "ซอฟต์แวร์ Java ดั้งเดิมเพื่อเพิ่มและจัดการลายน้ำข้อความและรูปภาพใน PDF, Word, Excel, งานนำเสนอ, ไดอะแกรม Visio, อีเมลและไฟล์รูปภาพ"

############################# Header ############################
title: "ใช้เอกสารลายน้ำในโครงการ Java ได้อย่างง่ายดาย"
description: "ปรับปรุงแอปพลิเคชัน Java ของคุณด้วยความสามารถในการทำลายน้ำไฟล์โดยใช้ไลบรารี GroupDocs.WatermarkAPI ของเรามีลายน้ำที่ปรับแต่งได้สำหรับรูปแบบไฟล์ยอดนิยมที่หลากหลาย"
words:
  for: "สำหรับ"

actions:
  main: "ดาวน์โหลดฟรีจาก Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-watermark/"
  alt: "การออกใบอนุญาต"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/java/"
  title: "พร้อมที่จะเริ่มแล้วหรือยัง?"
  description: "ลองใช้คุณสมบัติ GroupDocs.Watermark ฟรีหรือขอใบอนุญาต"

release:
  title: "เวอร์ชัน {0} เผยแพร่"
  notes: "ดูว่ามีอะไรใหม่"
  downloads: "ดาวน์โหลด"

code:
  title: "ลายน้ำ PDF s ผ่าน Java"
  more: "ตัวอย่างเพิ่มเติม"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-watermark</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // ใช้เครื่องหมายน้ำแบบทันทีที่ผ่านเส้นทาง PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // ปรับแต่งตัวเลือกลายน้ำ
    TextWatermark textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // ใช้ลายน้ำกับเอกสาร PDF
    watermarker.add(textWatermark);

    // บันทึกเอกสารผลลัพธ์
    watermarker.save("result.pdf");
    watermarker.close();
      
    ```

############################# Overview ############################
overview:
  enable: true
  title: "สรุปภาพ GroupDocs.Watermark"
  description: "ไลบรารีที่ออกแบบมาเพื่อเพิ่มลายน้ำโดยใช้เทคโนโลยี Java"
  features:
    # feature loop
    - title: "ไฟล์ลายน้ำผ่าน Java"
      content: "ปกป้องเอกสารทางธุรกิจของคุณโดยใช้ GroupDocs.Watermark for Javaเพิ่มข้อความ รูปภาพ ไดอะแกรม หรือไฟล์แนบอีเมลเป็นลายน้ำในรูปแบบไฟล์ต่างๆ"

    # feature loop
    - title: "ปรับแต่งลายน้ำสำหรับความต้องการเฉพาะ"
      content: "GroupDocs.Watermark for Java มีตัวเลือกการปรับแต่งที่กว้างขวางสำหรับลายน้ำปรับรูปแบบข้อความ (ตัวหนา ตัวเอียง ตัวอักษร) และคุณสมบัติของภาพ (หมุน ฯลฯ) เพื่อปรับกระบวนการทำลายน้ำให้เหมาะกับเป้าหมายเฉพาะของคุณ"

    # feature loop
    - title: "รองรับรูปแบบกว้าง"
      content: "GroupDocs.Watermark for Java รวมเข้ากับรูปแบบไฟล์ที่หลากหลายอย่างราบรื่น ได้แก่: PDF, Microsoft Office (Word, Excel, PowerPoint) รูปภาพ (JPEG, PNG, GIF, BMP), Visio ไดอะแกรม และอีเมลเพิ่มความปลอดภัยของเอกสารในประเภทไฟล์ที่หลากหลาย"

    # feature loop
    - title: "การค้นหาและจัดการลายน้ำได้อย่างง่ายดาย"
      content: "จัดการลายน้ำที่มีอยู่ภายในเอกสารอย่างมีประสิทธิภาพค้นหาลายน้ำที่เฉพาะเจาะจง แก้ไขข้อความ สไตล์ หรือรูปภาพ หรือลบออกไปทั้งหมด GroupDocs.Watermark for Java ช่วยลดขั้นตอนการทำงานของเครื่องหมายน้ำ"

############################# Platforms ############################
platforms:
  enable: true
  title: "อิสระของแพลตฟอร์"
  description: "GroupDocs.Watermark for Java รองรับระบบปฏิบัติการและผู้จัดการแพ็คเกจต่างๆ"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "รูปแบบไฟล์ที่รองรับ"
  description: |
    GroupDocs.Watermark for Java ช่วยให้สามารถประมวลผลรูปแบบไฟล์ได้หลากหลาย[ดูรายการทั้งหมด](https://docs.groupdocs.com/watermark/net/supported-document-formats/)
  groups:
    # group loop
    - color: "green"
      content: |
        ### รูปแบบ Microsoft Office และ OpenDocument
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### รูปภาพและกราฟิก
        * **รูปแบบภาพยอดนิยม:** BMP, JPG, JPEG, PNG
        * **ภาพหลายหน้า:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### อื่น ๆ
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Watermark for Java: คุณสมบัติ"
  description: "ปกป้องไฟล์ของคุณโดยการเพิ่มลายน้ำรองรับรูปแบบต่างๆ รวมถึง PDF เอกสาร Office และรูปภาพ"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "ไฟล์ลายน้ำ"
      content: "เพิ่มหรือลบลายน้ำจากส่วนเฉพาะหรือเอกสารทั้งหมดสำหรับรูปแบบไฟล์ที่รองรับต่างๆ"

    # feature loop
    - icon: "watermark_style"
      title: "การปรับแต่งลายน้ำ"
      content: "ปรับแต่งรูปลักษณ์ของลายน้ำของคุณด้วยตัวเลือกเช่นสี แบบอักษร การหมุน และอื่น ๆ"

    # feature loop
    - icon: "hidden_print"
      title: "ลายน้ำการพิมพ์ที่ซ่อนอยู่สำหรับ PDF"
      content: "เพิ่มลายน้ำที่ปรากฏขึ้นเมื่อพิมพ์เอกสาร PDF เท่านั้น"

    # feature loop
    - icon: "image_only"
      title: "เครื่องหมายน้ำภาพที่เลือกไว้"
      content: "ลายน้ำรูปภาพทั้งหมดภายในส่วน หน้า สไลด์ หรือเอกสารทั้งหมด"

    # feature loop
    - icon: "image_frame"
      title: "กรอบรูปภาพเฉพาะลายน้ำ"
      content: "ใช้ลายน้ำกับเฟรมเฉพาะภายในภาพหลายกรอบ"

    # feature loop
    - icon: "attachments"
      title: "สิ่งที่แนบและรูปร่างลายน้ำ"
      content: "เพิ่มลายน้ำให้กับไฟล์แนบทั้งหมดในเอกสาร Excel หรือรูปร่างภาพทั้งหมดในงานนำเสนอ"

    # feature loop
    - icon: "pdf_objects"
      title: "การจัดตำแหน่งลายน้ำใน PDF"
      content: "จัดตำแหน่งลายน้ำไปยังพื้นที่ต่างๆของเอกสาร PDF รวมถึง Bleed Box, Art Box, Crop Box และ Trim Box"

    # feature loop
    - icon: "doc_background"
      title: "ลายน้ำตามภาพพื้นหลัง"
      content: "เพิ่มหรือลบลายน้ำภาพพื้นหลังลงในสเปรดชีตหรืองานนำเสนอ"

    # feature loop
    - icon: "unreadable_characters"
      title: "การป้องกันด้วยตัวอักษรที่ไม่สามารถอ่านได้"
      content: "ปกป้องงานนำเสนอโดยใช้ลายน้ำข้อความด้วยอักขระที่ไม่สามารถอ่านได้"

    # feature loop
    - icon: "watermark_text_search"
      title: "ค้นหาลายน้ำ"
      content: "รับรายการลายน้ำที่นำเสนอในไฟล์โดยใช้พารามิเตอร์ต่างๆรวมถึงนิพจน์ปกติ"

    # feature loop
    - icon: "watermark_image_search"
      title: "ค้นหาลายน้ำภาพที่คล้ายกัน"
      content: "ค้นหาลายน้ำของภาพที่ดูเหมือนภาพเฉพาะ"

    # feature loop
    - icon: "document_info"
      title: "แยกข้อมูลเอกสาร"
      content: "รับข้อมูลเอกสารต่างๆ เช่น การตั้งค่าหน้าสำหรับรูปแบบไฟล์ที่รองรับ"

############################# Code samples ############################
code_samples:
  enable: true
  title: "ตัวอย่างรหัส"
  description: "สำรวจตัวอย่างโค้ดแสดงฟังก์ชันทั่วไป GroupDocs.Watermark for Java"
  items:
    # code sample loop
    - title: "ลายน้ำในเอกสารโดยใช้รูปภาพ"
      content: |
        ใช้ GroupDocs.Watermark for Java เพื่อเพิ่มความปลอดภัยของเอกสารโดยการเพิ่มลายน้ำรูปภาพเรียนรู้เพิ่มเติม: [ลายน้ำรูปภาพ](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/)
        {{< landing/code title="วิธีป้องกันไฟล์ด้วยลายน้ำรูปภาพ">}}
        ```csharp {style=abap}
        // โหลดเอกสารต้นฉบับไปยัง Watermarker
        Watermarker watermarker = new Watermarker("document.pdf");
        
        // ระบุเส้นทางไปยังภาพลายน้ำ
        ImageWatermark watermark = new ImageWatermark("watermark.jpg");

        // ปกป้องไฟล์และบันทึก
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "แก้ไขลายน้ำ"
      content: |
        GroupDocs.Watermark for Java ช่วยให้คุณจัดการลายน้ำที่มีอยู่ภายในเอกสารค้นหาลายน้ำเฉพาะและ [แก้ไขคุณสมบัติ](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/)
        {{< landing/code title="การค้นหาและแก้ไขลายน้ำ">}}
        ```csharp {style=abap}   
        // โหลดเอกสารต้นทาง
        Watermarker watermarker = new Watermarker("document.pdf");

        // ค้นหาลายน้ำที่จะอัปเดต
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);                               
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);                             

        // อัปเดตคุณสมบัติที่ต้องการ
        for (PossibleWatermark watermark : watermarks)                                                           
        {  
            watermark.setText("New Text");
        }

        // บันทึกเอกสารที่แก้ไขไปยังเส้นทางที่ระบุ
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
