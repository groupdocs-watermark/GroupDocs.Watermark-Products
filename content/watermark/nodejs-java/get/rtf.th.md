
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:46
draft: false
lang: th
format: Rtf
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "เอกสารการสกัดลายน้ำ RTF ที่มีประสิทธิภาพ"
head_description: "แยกลายน้ำจากเอกสารอย่างมีประสิทธิภาพโดยใช้ GroupDocs.Watermark for Node.js via Java"

############################# Header ############################
title: "การดึงลายน้ำเอกสาร RTF ที่คล่องตัว" 
description: "ดึงลายน้ำได้อย่างง่ายดายโดยใช้แนวทางที่คล่องตัว GroupDocs.Watermark for Node.js via Java"
subtitle: "GroupDocs.Watermark for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดที่ NPM ฟรี"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "เรียนรู้เพิ่มเติมเกี่ยวกับ GroupDocs.Watermark for Node.js via Java"
    link: "/watermark/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Node.js via Java นำเสนอความสามารถในการสกัดลายน้ำที่มีประสิทธิภาพสำหรับการจัดการลายน้ำใน Node.js via Java ปรับปรุงกระบวนการดึงลายน้ำในรูปแบบไฟล์ต่างๆ

############################# Steps ############################
steps:
    enable: true
    title: "รับลายน้ำจากไฟล์ Rtf โดยใช้ GroupDocs.Watermark"
    content: |
      **[GroupDocs.Watermark for Node.js via Java](https://products.groupdocs.com/watermark/nodejs-java/)** นำเสนอโซลูชั่นที่ครอบคลุมสำหรับการใส่ลายน้ำในรูปแบบเอกสารทางธุรกิจยอดนิยม ด้วยการรวมไลบรารีของเราเข้ากับแอปพลิเคชัน Node.js via Java ของคุณ คุณสามารถจัดเตรียมความสามารถในการค้นหาลายน้ำอันทรงพลังให้กับพวกเขาได้
      
      1. หากต้องการเข้าถึงฟังก์ชันการทำงานที่ GroupDocs.Watermark ให้ไว้ ให้สร้างอินสแตนซ์คลาส **Watermarker** และระบุเส้นทางไฟล์ Rtf นอกจากนี้คุณยังสามารถใช้ไฟล์ที่บันทึกเป็นสตรีมไบต์ได้ การดำเนินการนี้จะโหลดเอกสารเป้าหมายเพื่อการวิเคราะห์ลายน้ำที่ครอบคลุม
      2. เพื่อให้บรรลุการระบุลายน้ำเป้าหมาย ให้สร้างออบเจ็กต์ **SearchCriteria** คุณสามารถระบุรูปภาพเพื่อค้นหาลายน้ำรูปภาพที่คล้ายกันได้ สำหรับลายน้ำข้อความ ให้กำหนดเนื้อหาข้อความ คุณสมบัติแบบอักษร คุณลักษณะสี และพารามิเตอร์อื่นๆ ที่เกี่ยวข้อง เพื่อปรับแต่งเกณฑ์การค้นหาและให้ผลลัพธ์ที่แม่นยำยิ่งขึ้น
      3. เรียกใช้เมธอด **Search** (หรือรูปแบบการตั้งชื่อที่คล้ายกัน) ของออบเจ็กต์ **Watermarker** เพื่อเริ่มกระบวนการรับลายน้ำภายในเอกสารที่โหลด ฟังก์ชันนี้จะส่งคืนคอลเลกชันของออบเจ็กต์ที่แสดงลายน้ำที่อาจเกิดขึ้น ซึ่งช่วยอำนวยความสะดวกในการประมวลผลเพิ่มเติมตามความต้องการเฉพาะของคุณ
      4. การรวบรวมลายน้ำผลลัพธ์ช่วยให้คุณสามารถควบคุมลายน้ำที่ระบุในเอกสารได้ คุณสามารถลบลายน้ำที่ไม่ต้องการออกหรือปรับเปลี่ยนคุณสมบัติแบบไดนามิกได้ เช่น การปรับขนาด ตำแหน่ง หรือเนื้อหาข้อความ เพื่อให้เหมาะกับความต้องการของคุณ
   
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

        // รับลายน้ำรูปภาพวางไว้ใน RTF

        // สร้างออบเจ็กต์ Watermarker ด้วยเส้นทางต้นทาง
        const watermarker = new groupdocs.watermark.Watermarker("input.rtf");
        
        // รับลายน้ำด้วยแฮชรูปภาพที่คล้ายกัน
        const imageSearchCriteria = 
            new groupdocs.watermark.ImageDctHashSearchCriteria("watermark.jpg");
        imageSearchCriteria.setMaxDifference(0.9);
        const possibleWatermarks = watermarker.search(imageSearchCriteria);

        // ประมวลผลลายน้ำตามที่คุณต้องการ
        console.log(`Found ${possibleWatermarks.getCount()} possible watermark(s).`);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ใช้ประโยชน์จาก Node.js สำหรับการค้นหาลายน้ำด้วย GroupDocs.Watermark"
  description: "ใช้ฟังก์ชันการค้นหาลายน้ำแบบไดนามิกและมีประสิทธิภาพในแอปพลิเคชัน Node.js ของคุณโดยใช้ GroupDocs.Watermark ภายในแพลตฟอร์ม Node.js via Java"
  image: "/img/watermark/features_search.webp" # 500x500 px
  image_description: "ค้นหาลายน้ำ Node.js"
  features:
    # feature loop
    - title: "Node.js API สำหรับการค้นหาลายน้ำที่ยืดหยุ่น"
      content: "ใช้ประโยชน์จากความยืดหยุ่นของ Node.js ด้วย GroupDocs.Watermark เพื่อค้นหาลายน้ำในรูปแบบเอกสารหลายรูปแบบกำหนดค่าการค้นหาให้ตรงกับข้อกำหนดเฉพาะ เช่น ขนาด ประเภท หรือเนื้อหาได้อย่างง่ายดาย"

    # feature loop
    - title: "การระบุลายน้ำที่ได้รับการปรับปรุงด้วย Node.js"
      content: "ปรับปรุงการประมวลผลเอกสารของคุณโดยการระบุลายน้ำอย่างถูกต้องโดยใช้ Node.jsใช้ API ของ GroupDocs.Watermark เพื่อตรวจจับลายน้ำแม้ภายในโครงสร้างเอกสารที่ซับซ้อน"

    # feature loop
    - title: "โซลูชันการค้นหาลายน้ำที่ปรับขนาดได้"
      content: "ปรับขนาดโซลูชันความปลอดภัยเอกสารของคุณด้วย Node.js GroupDocs.Watermark ช่วยให้สามารถประมวลผลชุดเอกสารขนาดใหญ่ได้อย่างมีประสิทธิภาพ ทำให้เหมาะสำหรับการใช้งานระดับองค์กร"
      
  code_samples:
    # code sample loop
    - title: "Node.js ตัวอย่าง: ค้นหาและดึงลายน้ำ"
      content: |
        ตัวอย่าง Node.js นี้แสดงวิธีการใช้ GroupDocs.Watermark สำหรับการค้นหาและดึงลายน้ำ แสดงให้เห็นถึงการดำเนินการค้นหาที่มีประสิทธิภาพและปรับขนาดได้
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            const files = ["source.docx", "source.xlsx", "source.pptx", "source.vsdx"];
            for (const file of files) {
                //  ตั้งค่าสภาพแวดล้อม Node.js และโหลดเอกสารที่จำเป็น
                const settings = new groupdocsWatermark.WatermarkerSettings();
                settings.setSearchableObjects(new groupdocsWatermark.SearchableObjects());
                settings.getSearchableObjects().setWordProcessingSearchableObjects(
                    groupdocsWatermark.WordProcessingSearchableObjects.Hyperlinks | 
                    groupdocsWatermark.WordProcessingSearchableObjects.Text
                );
                settings.getSearchableObjects().setSpreadsheetSearchableObjects(
                    groupdocsWatermark.SpreadsheetSearchableObjects.HeadersFooters
                );
                settings.getSearchableObjects().setPresentationSearchableObjects(
                    groupdocsWatermark.PresentationSearchableObjects.SlidesBackgrounds |
                    groupdocsWatermark.PresentationSearchableObjects.Shapes
                );
                settings.getSearchableObjects().setDiagramSearchableObjects(groupdocsWatermark.DiagramSearchableObjects.None);
                settings.getSearchableObjects().setPdfSearchableObjects(groupdocsWatermark.PdfSearchableObjects.All);

                //  กำหนดค่าการค้นหาของคุณเพื่อระบุลายน้ำตามเกณฑ์ที่หลากหลาย
                const watermarker = new groupdocsWatermark.Watermarker(file, settings);

                //  ดำเนินการค้นหาลายน้ำและรวบรวมข้อมูลเกี่ยวกับลายน้ำที่ระบุ
                const watermarks = watermarker.search();

                //  ประมวลผลลัพธ์เพื่อแก้ไขหรือลบลายน้ำตามความต้องการทางธุรกิจ
                console.log(`In ${documentPath} found ${watermarks.getCount()} possible watermark(s).`);
                watermarker.close();
            }

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
    title: "สกัดลายน้ำอย่างมีประสิทธิภาพ"
    exclude: "RTF"
    description: "แยกลายน้ำจากรูปแบบไฟล์ที่แตกต่างกันได้อย่างมีประสิทธิภาพด้วย GroupDocs.Watermark for Node.js via Java"
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