
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:39:00
draft: false
lang: th
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "ค้นพบ Powerpoint งานนำเสนอ ลายน้ำที่ซ่อนอยู่"
head_description: "เปิดเผยลายน้ำที่ซ่อนอยู่ภายในเอกสารโดยใช้ GroupDocs.Watermark"

############################# Header ############################
title: "เปิดตัวลายน้ำที่วางไว้ในงานนำเสนอ Powerpoint" 
description: "ค้นพบและเปิดเผยลายน้ำที่ซ่อนอยู่ในเอกสารของคุณด้วย GroupDocs.Watermark for Node.js via Java"
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดฟรี NPM"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "เรียนรู้เพิ่มเติมเกี่ยวกับ GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       สำรวจความสามารถของ GroupDocs.Watermark for Node.js via Java ในการจัดการลายน้ำได้อย่างราบรื่นใน Node.js via Javaจัดการการดำเนินการลายน้ำได้อย่างง่ายดาย เช่น สร้าง อัปเดต รับ และลบในรูปแบบไฟล์ต่างๆ

############################# Steps ############################
steps:
    enable: true
    title: "รับลายน้ำในไฟล์ Powerpoint ได้อย่างมีประสิทธิภาพโดย GroupDocs.Watermark"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** ช่วยเพิ่มประสิทธิภาพในการดึงลายน้ำที่ฝังอยู่ในรูปแบบเอกสารธุรกิจต่างๆรวม GroupDocs.Watermark เข้ากับแอปพลิเคชัน Node.js via Java ของคุณได้อย่างราบรื่นเพื่อเพิ่มประสิทธิภาพให้กับพวกเขาด้วยความสามารถในการตรวจจับลายน้ำที่แข็งแกร่ง
      
      1. **Watermarker** และให้เส้นทางไฟล์ Powerpoint สตรีมไฟล์ หรือไบต์สตรีมเป็นอินพุตการกระทำนี้โหลดเอกสารสำหรับการวิเคราะห์ลายน้ำ
      2. **SearchCriteria**ระบุภาพสำหรับการค้นหาลายน้ำภาพที่คล้ายกันหรือสำหรับลายน้ำที่เป็นข้อความ ให้กำหนดเนื้อหาข้อความ คุณสมบัติตัวอักษร แอตทริบิวต์สี และพารามิเตอร์ที่เกี่ยวข้องอื่น ๆ เพื่อปรับแต่งเกณฑ์การค้นหา
      3. **Get** ของวัตถุ **Watermarker** เพื่อเริ่มกระบวนการตรวจจับลายน้ำภายในเอกสารที่โหลดฟังก์ชันนี้จะส่งคืนคอลเลกชันของวัตถุที่เป็นตัวแทนของลายน้ำที่อาจเกิดขึ้นทำให้สามารถประมวลผลต่อไป
      4. คอลเลกชันของวัตถุลายน้ำที่ดึงมาช่วยให้คุณมีความเป็นไปได้มากมายคุณสามารถลบลายน้ำที่ไม่ต้องการหรือแก้ไขคุณสมบัติเปลี่ยนเนื้อหา ย้ายลายน้ำบนหน้าและอื่น ๆ อีกมากมาย
   
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

        // รับรายการลายน้ำข้อความสำหรับ POWERPOINT

        // คลาสเครื่องหมายน้ำ Instantiate
        const watermarker = new groupdocs.watermark.Watermarker("input.พีพีทีเอ็กซ์");
        
        // รับลายน้ำตามเกณฑ์ข้อความ
        const searchCriteria = new groupdocs.watermark.TextSearchCriteria("test", false);
        const watermarks = watermarker.search(searchCriteria);

        // ใช้ข้อมูลลายน้ำ
        console.log(`Found ${watermarks.getCount()} possible watermark(s).`);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ปรับปรุงการค้นหาลายน้ำของคุณด้วย GroupDocs.Watermark ใน Node.js"
  description: "เรียนรู้การใช้ฟังก์ชันการค้นหาลายน้ำขั้นสูงในแอปพลิเคชัน Node.js ของคุณด้วย GroupDocs.Watermark เพิ่มประสิทธิภาพการจัดการเอกสารภายใน Node.js via Java"
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "ค้นหาลายน้ำใน Node.js"
  features:
    # feature loop
    - title: "การตรวจจับลายน้ำขั้นสูงใน Node.js"
      content: "ใช้ GroupDocs.Watermark เพื่อเพิ่มความสามารถในการตรวจจับและระบุลายน้ำในรูปแบบเอกสารใด ๆค้นหาอย่างมีประสิทธิภาพโดยใช้ตัวเลือกการกรองที่ซับซ้อน"

    # feature loop
    - title: "Node.js API สำหรับการค้นหาลายน้ำที่กำหนดเอง"
      content: "ปรับแต่งการดำเนินการค้นหาของคุณด้วย Node.js API ของเราค้นหาลายน้ำโดยระบุพารามิเตอร์โดยละเอียด เช่น ตำแหน่ง ความทึบแสง และประเภทเนื้อหา เพื่อเพิ่มประสิทธิภาพเวิร์กโฟลว์เอกสารของคุณ"

    # feature loop
    - title: "การดึงข้อมูลและการวิเคราะห์ลายน้ำที่มีประสิทธิภาพ"
      content: "ด้วย GroupDocs.Watermark แยกและวิเคราะห์ลายน้ำจากเอกสารต่าง ๆ ได้อย่างรวดเร็วAPI ของเรารองรับการดึงข้อมูลอย่างรวดเร็ว ช่วยให้คุณรักษาความสอดคล้องและความสม่ำเสมอของแบรนด์"
      
  code_samples:
    # code sample loop
    - title: "ตัวอย่าง Node.js: การค้นหาลายน้ำที่มีประสิทธิภาพ"
      content: |
        สำรวจวิธีใช้ Node.js กับ GroupDocs.Watermark เพื่อค้นหาลายน้ำในเอกสารประเภทต่างๆ แสดงให้เห็นถึงการใช้เกณฑ์การค้นหาแบบไดนามิกสำหรับผลลัพธ์ที่แม่นยำ
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  เริ่มต้นสภาพแวดล้อม Node.js และโหลดเอกสารเป้าหมาย
            const watermarker = new groupdocsWatermark.Watermarker("source.pdf");

            //  ตั้งค่าแบบสอบถามการค้นหาโดยใช้เกณฑ์ที่ยืดหยุ่นเพื่อค้นหาลายน้ำเฉพาะ
            const criteria = new groupdocsWatermark.TextFormattingSearchCriteria();
            criteria.setForegroundColorRange(new groupdocsWatermark.ColorRange());
            criteria.getForegroundColorRange().setMinHue(-5);
            criteria.getForegroundColorRange().setMaxHue(10);
            criteria.setBackgroundColorRange(new groupdocsWatermark.ColorRange());
            criteria.getBackgroundColorRange().setEmpty(true);
            criteria.setFontName("Arial");
            criteria.setMinFontSize(19);
            criteria.setMaxFontSize(42);
            criteria.setFontBold(true);
  
            //  ดำเนินการค้นหาและรวบรวมลายน้ำที่ตรงตามเกณฑ์
            const watermarks = watermarker.search(criteria);

            //  ประมวลผลและวิเคราะห์ผลลัพธ์เพื่อกำหนดการกระทำที่จำเป็น
            console.log(`Found ${watermarks.getCount()} possible watermark(s).`);
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
    title: "ค้นพบลายน้ำในรูปแบบ"
    exclude: "POWERPOINT"
    description: "ค้นพบลายน้ำในรูปแบบไฟล์ที่แตกต่างกันได้อย่างง่ายดายด้วย GroupDocs.Watermark for Node.js via Java"
    items: 
        # format loop 1
        - name: "ลายน้ำ PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/get//pdf/"
          description: "รูปแบบเอกสาร Adobe Portable"

        # format loop 2
        - name: "ลายน้ำ Word"
          format: "WORD"
          link: "/watermark/nodejs-java/get//word/"
          description: "MS Word และเอกสาร Open Office"
          
        # format loop 3
        - name: "ลายน้ำ Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/get//excel/"
          description: "MS Excel และสเปรดชีตโอเพ่นออฟฟิศ"

        # format loop 4
        - name: "ลายน้ำ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/get//powerpoint/"
          description: "MS PowerPoint และงานนำเสนอแบบโอเพ่นออฟฟิศ"

        # format loop 5
        - name: "ลายน้ำ DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/get//docx/"
          description: "ไมโครซอฟท์ Word เปิดเอกสาร XML"
          
        # format loop 6
        - name: "ลายน้ำ PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/get//pptx/"
          description: "PowerPoint เปิดการนำเสนอ XML"
          
        # format loop 7
        - name: "ลายน้ำ XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/get//xlsx/"
          description: "ไมโครซอฟท์ Excel เปิดสเปรดชีต XML"

        # format loop 8
        - name: "ลายน้ำ DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/get//doc/"
          description: "ไมโครซอฟท์ Word 97 - เอกสาร 2007"

        # format loop 9
        - name: "ลายน้ำ XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/get//xls/"
          description: "ไมโครซอฟท์ Excel สมุดงาน 97-2003"

        # format loop 10
        - name: "ลายน้ำ PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/get//ppt/"
          description: "PowerPoint การนำเสนอ 97-2003"

        # format loop 11
        - name: "ลายน้ำ RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/get//rtf/"
          description: "รูปแบบข้อความที่หลากหลาย"

---