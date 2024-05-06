
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:43
draft: false
lang: th
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "อัปเดตลายน้ำใน DOCX ได้อย่างราบรื่น"
head_description: "อัปเดตลายน้ำในเอกสาร DOCX ได้อย่างราบรื่นด้วย GroupDocs.Watermark for Node.js via Java ติดตั้งไลบรารีของเราลงในแอปพลิเคชันของคุณ"

############################# Header ############################
title: "ประมวลผลลายน้ำในเอกสาร DOCX" 
description: "ปรับลายน้ำได้อย่างง่ายดายด้วยความแม่นยำโดยใช้ GroupDocs.Watermark for Node.js via Java รักษาความลับของเอกสาร บริษัท ของคุณโดยใช้น้ำที่แตกต่างกันปรับแต่งคุณสมบัติลายน้ำ ได้แก่ ขนาด การจัดตำแหน่ง มุมการหมุน และตำแหน่งตามข้อกำหนดของคุณ"
subtitle: "GroupDocs.Watermark for Node.js via Java ห้องสมุด" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดฟรีที่ NPM"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "สืบสวน GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java ช่วยให้นักพัฒนาสามารถอัปเดตลายน้ำในเอกสาร DOCX ได้อย่างง่ายดายเครื่องมืออันทรงพลังนี้ช่วยให้สามารถปรับลายน้ำได้อย่างแม่นยำในรูปแบบไฟล์ต่างๆ รวมถึง PDF, Microsoft Word, Excel, PowerPoint, Visio, อีเมลและรูปแบบภาพ GroupDocs.Watermark for Node.js via Java สามารถใช้ได้บนแพลตฟอร์มยอดนิยมมากมาย

############################# Steps ############################
steps:
    enable: true
    title: "แก้ไขลายน้ำแบบไดนามิกสำหรับ DOCX ใน Node.js via Java"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** นำเสนอ API อันทรงพลังแก่นักพัฒนา Node.js via Java สำหรับการแก้ไขลายน้ำในเอกสาร DOCX ที่หลากหลาย คำแนะนำที่ครอบคลุมเพื่อปรับปรุงขั้นตอนการทำงานของคุณมีดังนี้
      
      1. **เริ่มกระบวนการ:** เริ่มต้นด้วยการให้ไฟล์ DOCX ของคุณเป็นอาร์กิวเมนต์ให้กับตัวสร้างคลาส **Watermarker** ไฟล์สามารถมีแหล่งที่มาเป็นสตรีมหรือจากตำแหน่งดิสก์ในเครื่องก็ได้ ทั้งนี้ขึ้นอยู่กับความต้องการของคุณ
      2. **ระบุลายน้ำ:** ใช้ออบเจ็กต์ **SearchCriteria** เพื่อระบุลายน้ำที่ต้องการแก้ไข เครื่องมืออเนกประสงค์นี้ช่วยให้สามารถเลือกลายน้ำเป้าหมายตามคุณสมบัติเฉพาะได้
      3. **ปรับแต่งอย่างแม่นยำ:** เมื่อดำเนินการค้นหาสำเร็จ คุณจะสามารถเข้าถึงชุดลายน้ำที่เกี่ยวข้องได้ เพลิดเพลินกับการควบคุมแต่ละองค์ประกอบอย่างละเอียด ด้วยความสามารถในการอัปเดตขนาด การวางตำแหน่งหน้า เนื้อหาข้อความ สี ข้อมูลรูปภาพ และอื่นๆ
      4. **ความต่อเนื่องที่ราบรื่น:** เมื่อการอัปเดตลายน้ำเสร็จสมบูรณ์ ให้จัดเก็บเอกสารที่แก้ไขอย่างปลอดภัย API มีตัวเลือกพื้นที่จัดเก็บข้อมูลที่ยืดหยุ่น ช่วยให้คุณสามารถบันทึกลงในเส้นทางไฟล์ในเครื่องหรือเป็นออบเจ็กต์สตรีมได้
   
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

        // อัปเดตลายน้ำรูปภาพ DOCX

        // เขียน Watermarker สำหรับไฟล์ DOCX
        const watermarker = new groupdocs.watermark.Watermarker("input.docx");

        // ใช้ SearchCriteria เพื่อค้นหารูปภาพที่ต้องการ
        const searchCriteria = 
            new groupdocs.watermark.ImageDctHashSearchCriteria("logo.png");
        const watermarks = watermarker.search(searchCriteria);
        
        // อัพเดตเนื้อหารูปภาพ
        for (const watermark of watermarks.getInnerList().toArray())
        {
            watermark.setImageData(imageData);
        }

        // บันทึกไฟล์ที่อัพเดต
        watermarker.save("output.docx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ดำดิ่งลึกในการเพิ่มลายน้ำ"
  description: "API เพื่อแสดงผล แสดงผล แปลงเอกสาร สไลด์ ไดอะแกรม และประเภทเอกสารอื่น ๆ อีกมากมายในแอปพลิเคชัน .NET"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "เพิ่มลายน้ำ"
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
    - title: "อัปเดตเนื้อหาลายน้ำการนำเสนอ"
      content: |
        ตัวอย่างนี้แสดงวิธีการอัปเดตเนื้อหาข้อความของลายน้ำการนำเสนอ
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  โหลดเอกสาร PDF เพื่อประมวลผล
            const watermarker = new groupdocsWatermark.Watermarker("source.pptx");

            //  ค้นหาลายน้ำเฉพาะที่ตรงตามเกณฑ์ของคุณ
            const searchCriteria = new groupdocsWatermark.TextSearchCriteria("denied", false);
            const watermarks = watermarker.search(searchCriteria);
  
            //  แก้ไขการตั้งค่าลายน้ำ เช่น ขนาด สี และตำแหน่ง
            for (const watermark of watermarks.getInnerList().toArray()) {
                watermark.setText("accepted");
            }

            //  บันทึกเอกสารที่อัปเดตลงในระบบท้องถิ่นหรือสตรีมโดยตรง
            watermarker.save("result.pptx");
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
    title: "อัปเดตลายน้ำสำหรับรูปแบบอื่น"
    exclude: "DOCX"
    description: "ปรับลายน้ำได้อย่างราบรื่นใน PDF, Word, Excel และอื่น ๆ ด้วย GroupDocs.Watermark for Node.js via Java รองรับรูปแบบอื่น ๆ อีกมากมาย"
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