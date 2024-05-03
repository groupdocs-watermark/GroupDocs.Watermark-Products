
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:08
draft: false
lang: th
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "อัปเดตลายน้ำสำหรับ Excel สเปรดชีต"
head_description: "อัปเดตลายน้ำในสเปรดชีตในรูปแบบต่างๆโดยใช้ GroupDocs.Watermark for Node.js via Javaเสริมสร้างแอปพลิเคชัน Node.js via Java ของคุณ"

############################# Header ############################
title: "ปฏิวัติสเปรดชีตลายน้ำโดยใช้ Node.js via Java" 
description: "สัมผัสพลังของ GroupDocs.Watermark for Node.js via Javaรักษาความปลอดภัยเอกสารทางธุรกิจของคุณด้วยลายน้ำต่างๆอัปเดตขนาดลายน้ำ การจัดตำแหน่งมุมหมุน ตำแหน่ง ฯลฯ"
subtitle: "GroupDocs.Watermark for Node.js via Java เอพีอี" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดฟรี NPM"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java ห้องสมุด"
    link: "/watermark/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java เป็นโซลูชันที่ครอบคลุมสำหรับการจัดการลายน้ำโดยใช้สภาพแวดล้อม Node.js via Javaด้วยเครื่องมือนี้ นักพัฒนาสามารถดำเนินการได้อย่างง่ายดาย เช่น การเพิ่ม แก้ไข ค้นหา และลบลายน้ำออกจากเอกสารในรูปแบบไฟล์ต่างๆ รวมถึง PDF, Microsoft Word, Excel, PowerPoint, Visio อีเมลและรูปแบบภาพ GroupDocs.Watermark รองรับระบบปฏิบัติการหลักทั้งหมดและเวอร์ชัน Node.js

############################# Steps ############################
steps:
    enable: true
    title: "อัปเดตลายน้ำใน EXCEL ผ่าน Node.js via Java"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** ช่วยให้นักพัฒนา Node.js via Java มี API ที่มีประสิทธิภาพสำหรับการอัปเดตลายน้ำทางโปรแกรมภายในเอกสาร EXCEL ต่างๆ คู่มือนี้จะสรุปกระบวนการ:
      
      1. เริ่มต้นกระบวนการโดยระบุไฟล์ EXCEL ของคุณเป็นอาร์กิวเมนต์ให้กับตัวสร้างคลาส **Watermarker** ทั้งนี้ขึ้นอยู่กับความต้องการของคุณ ไฟล์สามารถจัดเตรียมเป็นสตรีมหรือการอ้างอิงไปยังตำแหน่งของดิสก์ในเครื่องได้
      2. จากนั้น ใช้ประโยชน์จากออบเจ็กต์ **SearchCriteria** เพื่อระบุลายน้ำเฉพาะที่ต้องมีการแก้ไข วัตถุนี้ช่วยให้สามารถระบุลายน้ำตามคุณสมบัติที่ต้องการได้
      3. เมื่อดำเนินการค้นหาสำเร็จ คุณจะได้รับชุดลายน้ำที่เกี่ยวข้อง ลายน้ำเหล่านี้ให้การควบคุมแบบละเอียด ช่วยให้คุณสามารถอัปเดตคุณสมบัติต่างๆ เช่น ขนาด การวางตำแหน่งหน้า เนื้อหาข้อความ รูปแบบสี ข้อมูลรูปภาพ และอื่นๆ
      4. หลังจากการอัปเดตลายน้ำเสร็จสิ้น ให้คงเอกสารที่แก้ไขไว้ API อำนวยความสะดวกในการจัดเก็บข้อมูลโดยใช้เส้นทางไฟล์ในเครื่องหรือออบเจ็กต์สตรีม
   
    code:
      platform: "net"
      copy_title: "คัดลอก"
      install:
        command: "npm i @groupdocs/groupdocs.watermark"
        copy_tip: "คลิกเพื่อคัดลอก"
        copy_done: "คัดลอก"
      links:
        #  loop
        - title: "ตัวอย่างเพิ่มเติม"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java/"
        #  loop
        - title: "เอกสาร"
          link: "https://docs.groupdocs.com/watermark/nodejs-java/"
          
      content: |
        ```javascript {style=abap}

        // อัปเดตลายน้ำข้อความ EXCEL

        // ระบุอินสแตนซ์ Watermarker สำหรับไฟล์ EXCEL
        const watermarker = new groupdocs.watermark.Watermarker("input.xslx");

        // ใช้ TextSearchCriteria เพื่อค้นหาลายน้ำข้อความ
        const searchCriteria = 
            new groupdocs.watermark.TextSearchCriteria("test", false);
        const watermarks = watermarker.search(searchCriteria);
        
        // อัปเดตลายน้ำข้อความ
        for (const watermark of watermarks.getInnerList().toArray())
        {
            watermark.setText("passed");
        }

        // เพลิดเพลินไปกับผลลัพธ์
        watermarker.save("output.xslx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "เรียนรู้การแก้ไขลายน้ำใน PDF วินาทีด้วย GroupDocs.Watermark"
  description: "สำรวจคุณสมบัติ API ที่ครอบคลุมสำหรับการปรับและจัดการลายน้ำใน PDF s ภายในแอปพลิเคชัน Node.js via Java"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "แก้ไขลายน้ำ"
  features:
    # feature loop
    - title: "แก้ไขลายน้ำได้อย่างง่ายดายใน PDF s"
      content: "GroupDocs.Watermark นำเสนอเครื่องมือที่แข็งแกร่งใน Node.js via Java เพื่อแก้ไขลายน้ำที่มีอยู่ในเอกสาร PDF ได้อย่างราบรื่นปรับตำแหน่ง ความโปร่งใส และอื่น ๆ ได้อย่างง่ายดาย"

    # feature loop
    - title: "ปรับแต่งรายละเอียดลายน้ำเพื่อความแม่นยำ"
      content: "ควบคุมรายละเอียดAPI ของเราช่วยให้คุณสามารถปรับลักษณะของลายน้ำได้อย่างละเอียด ทำให้สามารถปรับเปลี่ยนขนาด ความทึบแสง และสีได้อย่างแม่นยำใน PDF s ของคุณ"

    # feature loop
    - title: "การจัดการลายน้ำที่คล่องตัว"
      content: "API ของเราช่วยลดความยุ่งยากในการจัดการลายน้ำไม่ว่าจะอัปเดตหรือลบ คุณสามารถจัดการลายน้ำได้อย่างมีประสิทธิภาพ รักษาความสมบูรณ์ของเอกสารในขณะที่ตอบสนองความต้องการด้านการสร้างแบรนด์ของคุณ"
      
  code_samples:
    # code sample loop
    - title: "Java ตัวอย่าง: แก้ไข PDF ลายน้ำ"
      content: |
        ตัวอย่าง Java นี้แสดงให้เห็นถึงวิธีการแก้ไขลายน้ำที่มีอยู่ในเอกสาร PDF โดยแสดงวิธีการปรับคุณสมบัติเป็นโปรแกรม
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  โหลดเอกสาร PDF เพื่อประมวลผล
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  ค้นหาลายน้ำเฉพาะที่ตรงตามเกณฑ์ของคุณ
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria("test", false);
            const watermarks = watermarker.search(searchCriteria);
  
            //  แก้ไขการตั้งค่าลายน้ำ เช่น ขนาด สี และตำแหน่ง
            for (const watermark of watermarks.getInnerList().toArray()) {
                watermark.getFormattedTextFragments().clear();
                watermark.getFormattedTextFragments().add("passed", 
                    new groupdocsWatermark.Font("Calibri", 19, groupdocsWatermark.FontStyle.Bold), 
                    groupdocsWatermark.Color.getRed(), groupdocsWatermark.Color.getAqua());
            }

            //  บันทึกเอกสารที่อัปเดตลงในระบบท้องถิ่นหรือสตรีมโดยตรง
            watermarker.save("result.pdf");
            watermarker.close();

        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "พร้อมที่จะเริ่มแล้วหรือยัง?"
  description: "ลองใช้คุณสมบัติ GroupDocs.Watermark ฟรีหรือขอใบอนุญาต"
  items:
    #  loop
    - title: "NPM ดาวน์โหลด"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      color: "red"
        #  loop
    - title: "การออกใบอนุญาต"
      link: "https://purchase.groupdocs.com/pricing/watermark/nodejs-java/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "อัปเดตลายน้ำในรูปแบบไฟล์ที่รองรับ"
    exclude: "EXCEL"
    description: "อัปเดตลายน้ำอย่างมีประสิทธิภาพใน PDF, Word, Excel และอื่น ๆ ด้วย GroupDocs.Watermark for Node.js via Javaเอกสารลายน้ำอาจเสริมกระบวนการทางธุรกิจของคุณ"
    items: 
        # format loop 1
        - name: "ลายน้ำ PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/update//pdf/"
          description: "รูปแบบเอกสาร Adobe Portable"

        # format loop 2
        - name: "ลายน้ำ Word"
          format: "WORD"
          link: "/watermark/nodejs-java/update//word/"
          description: "MS Word และเอกสาร Open Office"
          
        # format loop 3
        - name: "ลายน้ำ Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/update//excel/"
          description: "MS Excel และสเปรดชีตโอเพ่นออฟฟิศ"

        # format loop 4
        - name: "ลายน้ำ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/update//powerpoint/"
          description: "MS PowerPoint และงานนำเสนอแบบโอเพ่นออฟฟิศ"

        # format loop 5
        - name: "ลายน้ำ DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/update//docx/"
          description: "ไมโครซอฟท์ Word เปิดเอกสาร XML"
          
        # format loop 6
        - name: "ลายน้ำ PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/update//pptx/"
          description: "PowerPoint เปิดการนำเสนอ XML"
          
        # format loop 7
        - name: "ลายน้ำ XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/update//xlsx/"
          description: "ไมโครซอฟท์ Excel เปิดสเปรดชีต XML"

        # format loop 8
        - name: "ลายน้ำ DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/update//doc/"
          description: "ไมโครซอฟท์ Word 97 - เอกสาร 2007"

        # format loop 9
        - name: "ลายน้ำ XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/update//xls/"
          description: "ไมโครซอฟท์ Excel สมุดงาน 97-2003"

        # format loop 10
        - name: "ลายน้ำ PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/update//ppt/"
          description: "PowerPoint การนำเสนอ 97-2003"

        # format loop 11
        - name: "ลายน้ำ RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/update//rtf/"
          description: "รูปแบบข้อความที่หลากหลาย"

---