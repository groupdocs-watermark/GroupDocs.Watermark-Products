---
############################# Static ############################
layout: "landing"
date: 2024-05-08T17:25:29
draft: false

lang: th
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js ห้องสมุดลายน้ำ | ลายน้ำเอกสาร"
head_description: "โซลูชัน Node.js ปกป้องเอกสารทางธุรกิจด้วยลายน้ำข้อความและรูปภาพรองรับรูปแบบยอดนิยม เช่น PDF, Word, Excel, PowerPoint"

############################# Header ############################
title: "การเข้าถึงเทคโนโลยีลายน้ำใน Node.js ผ่านโซลูชัน Java"
description: "ปกป้องทรัพย์สินทางปัญญาของคุณและป้องกันการคัดลอกโดยไม่ได้รับอนุญาตด้วยโซลูชัน Node.js นี้ช่วยให้ผู้ใช้สามารถเพิ่มลายน้ำลงในเอกสารทางธุรกิจในรูปแบบต่างๆ ได้ง่าย รวมถึง PDF, Word, Excel, PowerPoint รูปภาพ ฯลฯ"
words:
  for: "สำหรับ"

actions:
  main: "ใช้ NPM เพื่อดาวน์โหลดฟรี"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.watermark"
  alt: "การออกใบอนุญาต"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
  title: "พร้อมที่จะเริ่มแล้วหรือยัง?"
  description: "ลองใช้คุณสมบัติ GroupDocs.Watermark ฟรีหรือขอใบอนุญาต"

release:
  title: "เวอร์ชัน {0} เผยแพร่"
  notes: "ดูว่ามีอะไรใหม่"
  downloads: "ดาวน์โหลด"
  link: "https://releases.groupdocs.com/watermark/nodejs-java/"

code:
  title: "เพิ่มลายน้ำไปยัง PDF ด้วย TypeScript"
  more: "ตัวอย่างเพิ่มเติม"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.watermarker"
  content: |
    ```javascript {style=abap}

    // ใช้เครื่องหมายน้ำแบบทันทีที่ผ่านเส้นทาง PDF
    let loadOptions = new PdfLoadOptions();
    let watermarker = 
        new Watermarker("source.pdf", loadOptions);

    // ปรับแต่งตัวเลือกลายน้ำ
    let textWatermark = 
        new TextWatermark("Approved", new Font("Arial", 8));

    // ใช้ลายน้ำกับเอกสาร PDF
    watermarker.add(textWatermark);

    // บันทึกเอกสารผลลัพธ์
    watermarker.save("result.pdf");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "สรุปภาพ GroupDocs.Watermark"
  description: "Node.js ไลบรารี TypeScript สำหรับลายน้ำ"
  features:
    # feature loop
    - title: "Node.js ไฟล์ ลายน้ำ"
      content: "ปกป้องเอกสารทางธุรกิจของคุณด้วย GroupDocs.Watermark for Node.js via Javaเพิ่มข้อความ รูปภาพ ไดอะแกรม หรือไฟล์แนบอีเมลเป็นลายน้ำในรูปแบบไฟล์ต่างๆ"

    # feature loop
    - title: "ปรับแต่งลายน้ำตามความต้องการของคุณ"
      content: "GroupDocs.Watermark for Node.js via Java มีตัวเลือกการปรับแต่งที่กว้างขวางสำหรับลายน้ำปรับแต่งรูปแบบข้อความ (ตัวหนา ตัวเอียง ตัวอักษร) และคุณสมบัติของภาพ (หมุน ฯลฯ) ช่วยให้สามารถปรับแต่งการประมวลผลเอกสาร"

    # feature loop
    - title: "การสนับสนุนรูปแบบที่ครอบคลุม"
      content: "GroupDocs.Watermark for Node.js via Java รวมเข้ากับรูปแบบไฟล์ที่หลากหลายอย่างราบรื่น ได้แก่: PDF, MS Office เช่น Word, Excel, PowerPoint รูปภาพ เช่น JPEG, PNG, GIF, BMP, Visio ไดอะแกรม อีเมล ฯลฯ เพิ่มศักยภาพในการประมวลผลเอกสารเพื่อให้บรรลุเป้าหมายทางธุรกิจ"

    # feature loop
    - title: "การค้นหาและอัปเดตลายน้ำที่มีประสิทธิภาพ"
      content: "รับและอัปเดตลายน้ำที่มีอยู่ในเอกสารลายน้ำแก้ไขข้อความ สไตล์ เนื้อหาของรูปภาพ หรือลบออกทั้งหมด GroupDocs.Watermark for Node.js via Java ให้การประมวลผลลายน้ำได้หลากหลาย"

############################# Platforms ############################
platforms:
  enable: true
  title: "อิสระของแพลตฟอร์"
  description: "GroupDocs.Watermark for Node.js via Java ผสานเข้ากับระบบปฏิบัติการต่างๆและผู้จัดการแพ็คเกจได้อย่างง่ายดาย"
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "รูปแบบไฟล์ที่รองรับ"
  description: |
    GroupDocs.Watermark for Node.js via Java ช่วยให้คุณประมวลผลรูปแบบไฟล์ที่หลากหลาย[สำรวจรายการเต็ม](https://docs.groupdocs.com/watermark/net/supported-document-formats/)
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
  title: "GroupDocs.Watermark for Node.js via Java: ชุดคุณลักษณะ"
  description: "เพิ่มความปลอดภัยของเอกสารที่แข็งแกร่งผ่านลายน้ำแบบโปรแกรมรองรับรูปแบบไฟล์ที่หลากหลาย ได้แก่: PDF, DOCX, XLSX, PPTX และรูปแบบภาพ (PNG, JPG เป็นต้น)"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "การควบคุมลายน้ำที่แม่นยำ"
      content: "จัดการลายน้ำได้อย่างแม่นยำโดยการเพิ่มหรือลบออกจากส่วนเฉพาะ เอกสารทั้งหมด หรือไฟล์แนบและรูปร่างแต่ละรายการภายในรูปแบบไฟล์ที่แตกต่างกัน"

    # feature loop
    - icon: "watermark_style"
      title: "การปรับแต่งลักษณะลายน้ำ"
      content: "ควบคุมความสวยงามของลายน้ำอย่างละเอียดโดยการแก้ไขแอตทริบิวต์ เช่น สี แบบอักษร ความทึบแสง การหมุน และการวางตำแหน่งภายในเอกสาร"

    # feature loop
    - icon: "hidden_print"
      title: "พิมพ์ลายน้ำ PDF"
      content: "ใช้ลายน้ำที่ลอบซ่อนซึ่งยังคงมองไม่เห็นในระหว่างการดูเอกสารปกติ แต่จะเห็นได้ชัดในระหว่างกระบวนการพิมพ์เท่านั้น ซึ่งจะช่วยเพิ่มความปลอดภัยของเอกสารอย่างรอบคอบ"

    # feature loop
    - icon: "image_only"
      title: "ลายน้ำภาพเฉพาะ"
      content: "ภาพเฉพาะลายน้ำภายในเอกสารโดยใช้โซลูชันของเราเลือกที่จะฝังลายน้ำในส่วนที่กำหนด (เช่น หน้า สไลด์) หรือทั่วทั้งเอกสาร"

    # feature loop
    - icon: "image_frame"
      title: "ภาพหลายกรอบลายน้ำ"
      content: "ใช้ลายน้ำให้เลือกกับเฟรมเฉพาะภายในรูปแบบภาพหลายเฟรม เพื่อให้มั่นใจได้ว่าการควบคุมตำแหน่งลายน้ำแบบละเอียด"

    # feature loop
    - icon: "attachments"
      title: "การป้องกันเนื้อหาที่ครอบคลุม"
      content: "ขยายการป้องกันไปยังองค์ประกอบเอกสารต่างๆ เช่น ไฟล์แนบภายในเอกสาร Excel และรูปร่างภาพภายในงานนำเสนอ เพื่อเพิ่มระดับความปลอดภัยเพิ่มเติม"

    # feature loop
    - icon: "pdf_objects"
      title: "เครื่องหมายน้ำขั้นสูงใน PDF"
      content: "ลายน้ำบริเวณที่แตกต่างกันของ PDF s รวมถึง Bleed Box, Art Box, Crop Box, Trim Box ฯลฯ"

    # feature loop
    - icon: "doc_background"
      title: "ภาพพื้นหลัง ลายน้ำ"
      content: "จัดการลายน้ำภายในภาพพื้นหลังของสเปรดชีตและการนำเสนอ นำเสนอตัวเลือกการปรับแต่งเพิ่มเติมสำหรับมาตรการรักษาความปลอดภัยทางภาพ"

    # feature loop
    - icon: "unreadable_characters"
      title: "ลายน้ำข้อความที่มีอักขระที่ไม่สามารถอ่านได้"
      content: "ใช้อักขระที่ไม่สามารถอ่านได้ภายในลายน้ำข้อความที่ฝังอยู่ในงานนำเสนอ เสริมสร้างความปลอดภัยด้วยการทำให้การแยกลายน้ำโดยไม่ได้รับอนุญาตมีความท้าทายมากขึ้นอย่างมีนัยสำคัญ"

    # feature loop
    - icon: "watermark_text_search"
      title: "การค้นหาลายน้ำขั้นสูง"
      content: "ใช้ความสามารถในการค้นหาที่ครอบคลุมเพื่อค้นหาลายน้ำภายในเอกสารตามพารามิเตอร์ที่เฉพาะเจาะจงหรือโดยการรวมเกณฑ์ต่างๆ เพื่อให้การดึงและการจัดการได้อย่างมีประสิทธิภาพ"

    # feature loop
    - icon: "watermark_image_search"
      title: "การตรวจจับลายน้ำภาพที่คล้ายกัน"
      content: "ค้นหาภาพลายน้ำที่คล้ายกันภายในเอกสารที่คล้ายคลึงกับภาพต้นฉบับ"

    # feature loop
    - icon: "document_info"
      title: "การแยกข้อมูลเอกสารแบบโปรแกรม"
      content: "แยกข้อมูลเมตาที่มีค่าโดยโปรแกรม รวมถึงรายละเอียดการตั้งค่าหน้าและข้อมูลเอกสารอื่น ๆ สำหรับรูปแบบไฟล์ที่รองรับ"

############################# Code samples ############################
code_samples:
  enable: true
  title: "ตัวอย่างรหัส"
  description: "ดูตัวอย่างโค้ดที่แสดงฟังก์ชันทั่วไป GroupDocs.Watermark for Node.js via Java"
  items:
    # code sample loop
    - title: "ลายน้ำในเอกสารที่มีรูปภาพ"
      content: |
        ใช้ประโยชน์จาก GroupDocs.Watermark for Node.js via Java เพื่อเพิ่มความปลอดภัยของเอกสารโดยการเพิ่มลายน้ำรูปภาพเรียนรู้เพิ่มเติม: [ลายน้ำรูปภาพ](https://docs.groupdocs.com/watermark/java/adding-image-watermarks/#add-image-watermark-from-local-file/)
        {{< landing/code title="วิธีป้องกันไฟล์ด้วยลายน้ำรูปภาพ">}}
        ```javascript {style=abap}
        // โหลดเอกสารต้นฉบับไปยัง Watermarker
        let watermarker = new Watermarker("document.pdf");
        
        // ระบุเส้นทางไปยังภาพลายน้ำ
        let watermark = new ImageWatermark("watermark.jpg");

        // ปกป้องไฟล์และบันทึก
        watermarker.add(watermark); 
        watermarker.save("result.pdf");

        watermark.close();                                                                                               
        watermarker.close();

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "ค้นหาและแก้ไขลายน้ำที่มีอยู่"
      content: |
        GroupDocs.Watermark for Node.js via Java ช่วยให้คุณจัดการลายน้ำในเอกสารเลือกลายน้ำแก้ไขคุณสมบัติค้นพบวิธีการ: [แก้ไขลายน้ำ](https://docs.groupdocs.com/watermark/java/modifying-found-watermark-properties/#replacing-text/)
        {{< landing/code title="การค้นหาและแก้ไขลายน้ำ">}}
        ```javascript {style=abap}   
        // โหลดเอกสารต้นทาง
        let watermarker = new Watermarker("document.pdf");

        // ค้นหาลายน้ำที่จะอัปเดต
        let searchCriteria = new TextSearchCriteria("test", false);                               
        let watermarks = watermarker.search(searchCriteria); 

        // อัปเดตคุณสมบัติที่ต้องการ
        watermarks.forEach((watermark)
        {  
            watermark.setText("New Text");
        }

        // บันทึกเอกสารที่แก้ไขไปยังเส้นทางที่ระบุ
        watermarker.Save("document.pdf");
        watermarker.close();

        ```
        {{< /landing/code >}}

---
