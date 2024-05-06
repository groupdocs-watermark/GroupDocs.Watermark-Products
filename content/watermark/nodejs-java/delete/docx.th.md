
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:44
draft: false
lang: th
format: Docx
product: "Watermark"
product_tag: "watermark"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Node.js via Java API สำหรับการกำจัดลายน้ำ DOCX"
head_description: "ลบลายน้ำออกจากเอกสาร DOCX ได้อย่างมีประสิทธิภาพโดยใช้ API Node.js via Java ของเราเพื่อให้แน่ใจว่าไฟล์ที่สะอาดและดูเป็นมืออาชีพ"

############################# Header ############################
title: "Node.js via Java สำหรับการจัดการลายน้ำ DOCX" 
description: "ใช้ GroupDocs.Watermark for Node.js via Java API เพื่อลบหรือแก้ไขลายน้ำในไฟล์ DOCX ได้อย่างมีประสิทธิภาพ เหมาะอย่างยิ่งสำหรับการรักษาการจัดรูปแบบเอกสารที่แท้จริง"
subtitle: "GroupDocs.Watermark for Node.js via Java เอพีอี" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดแพ็คเกจ NPM ฟรี"
      link: "https://releases.groupdocs.com/watermark/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Node.js via Java ห้องสมุด"
    link: "/watermark/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       ไลบรารี GroupDocs.Watermark for Node.js via Java นำเสนอเครื่องมือที่แข็งแกร่งสำหรับการจัดการลายน้ำในเอกสาร DOCX ตั้งแต่การลบง่ายไปจนถึงการแก้ไขที่ซับซ้อน API นี้ช่วยให้นักพัฒนาสามารถรักษาความสวยงามและความซื่อสัตย์ของเอกสาร ตอบสนองความต้องการทางธุรกิจ กฎหมาย และวิชาการ

############################# Steps ############################
steps:
    enable: true
    title: "ลบลายน้ำจาก Docx ได้อย่างง่ายดายโดย Node.js via Java"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/nodejs-java/)** ปรับปรุงกระบวนการลบลายน้ำออกจากเอกสารทางธุรกิจ ยกระดับแอปพลิเคชัน Node.js via Java ของคุณด้วยการผสานรวมไลบรารีของเราอย่างราบรื่น และทำตามขั้นตอนที่ตรงไปตรงมาเหล่านี้:
      
      1. เริ่มต้นกระบวนการโดยสร้างอินสแตนซ์คลาสหลัก **Watermarker** ด้วยเอกสาร Docx API อเนกประสงค์ของเราประมวลผลเอกสารได้อย่างราบรื่น ไม่ว่าจะจัดทำเป็นสตรีมหรือเส้นทางในเครื่อง
      2. ใช้ประโยชน์จาก **SearchCriteria** เพื่อระบุลายน้ำที่จะแก้ไขได้อย่างแม่นยำ ใช้พารามิเตอร์ต่างๆ เช่น รูปภาพ ข้อความ หรือคุณลักษณะการจัดรูปแบบ เพื่อปรับแต่งการค้นหาของคุณ ยิ่งเกณฑ์ของคุณมีรายละเอียดมากเท่าใด ผลลัพธ์ก็จะยิ่งแม่นยำมากขึ้นเท่านั้น
      3. ดำเนินการขั้นตอนการลบในรายการลายน้ำเอกสารที่ดึงมาจากการค้นหาของคุณ ลบออกจากเอกสารได้อย่างง่ายดาย
      4. เมื่อลบลายน้ำสำเร็จ ให้บันทึกเอกสารผลลัพธ์อย่างปลอดภัยเป็นไฟล์ในเครื่องหรือสตรีมไบต์ โดยรักษาความสมบูรณ์ของเอกสาร
   
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

        // ลบลายน้ำรูปภาพในเอกสาร DOCX

        // รับ Watermarker ผ่านเส้นทาง DOCX เป็นอาร์กิวเมนต์
        const watermarker = new groupdocs.watermark.Watermarker("input.docx");
        
        // ล้างลายน้ำรูปภาพตามเกณฑ์การค้นหา
        const searchCriteria = 
            new groupdocs.watermark.ImageDctHashSearchCriteria("logo.png");
        const watermarks = watermarker.search(searchCriteria);
        watermarks.clear();

        // บันทึกไฟล์ที่ประมวลผล
        watermarker.save("output.docx");
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Node.js via Java API สำหรับการกำจัดลายน้ำ | GroupDocs.Watermark"
  description: "ผสานรวม API Node.js via Java ของเราเพื่อลบลายน้ำออกจากเอกสารได้อย่างง่ายดาย เพิ่มความชัดเจนและความสวยงามของเอกสารAPI นี้เหมาะสำหรับสภาพแวดล้อม Node.js via Java เหมาะสำหรับแอปพลิเคชันที่ต้องการประมวลผลและนำเสนอเอกสารที่สะอาดปราศจากลายน้ำ"
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "ลบลายน้ำ"
  features:
    # feature loop
    - title: "การกำจัดลายน้ำที่คล่องตัวสำหรับ Node.js via Java"
      content: "API ของเรานำเสนอเครื่องมือกำจัดลายน้ำที่คล่องตัวที่ออกแบบมาโดยเฉพาะสำหรับแอปพลิเคชัน Node.js via Java ช่วยให้นักพัฒนาสามารถเพิ่มความสามารถในการอ่านเอกสารและรูปลักษณ์ระดับมืออาชีพโดยไม่ต้องเข้ารหัสที่ซับซ้อน"

    # feature loop
    - title: "Node.js via Java การล้างลายน้ำแบบแบทช์"
      content: "ใช้ประโยชน์จากความสามารถในการล้างลายน้ำจากเอกสารหลายฉบับในคราวเดียวด้วยคุณสมบัติการประมวลผลแบบแบทช์ของเราสิ่งนี้มีประโยชน์อย่างยิ่งสำหรับแอปพลิเคชันที่ต้องการจัดการกระแสเอกสารขนาดใหญ่ได้อย่างรวดเร็วและมีประสิทธิภาพ"

    # feature loop
    - title: "การแก้ไขลายน้ำแบบยืดหยุ่นผ่าน Node.js via Java"
      content: "ปรับแก้ไข หรือลบลายน้ำอย่างสมบูรณ์โดยใช้เครื่องมือแก้ไขที่ยืดหยุ่นของเราคุณลักษณะนี้ช่วยให้นักพัฒนา Node.js via Java สามารถปรับแต่งการประมวลผลเอกสารให้เหมาะกับความต้องการทางธุรกิจหรือคำขอของลูกค้า เพื่อให้แน่ใจว่าผลลัพธ์ที่ดีที่สุด"
      
  code_samples:
    # code sample loop
    - title: "ลบลายน้ำส่วนหัวของสเปรดชีต"
      content: |
        ตัวอย่างนี้แสดงวิธีการลบลายน้ำที่ใส่ไว้ในส่วนหัว XLSX
        {{< landing/code title="TypeScript">}}
        ```javascript {style=abap}
        
            const groupdocsWatermark = require('@groupdocs/groupdocs.watermark')

            //  โหลดสมุดงานสเปรดชีต
            const loadOptions = new groupdocsWatermark.SpreadsheetLoadOptions();
            const watermarker = new groupdocsWatermark.Watermarker("source.xlsx", loadOptions);

            //  รับรายการส่วนหัวข้อ
            const content = watermarker.getContent(groupdocsWatermark.SpreadsheetContent.class);
            const sections = content.getWorksheets().get_Item(0).getHeadersFooters()
                .getByOfficeHeaderFooterType(groupdocsWatermark.OfficeHeaderFooterType.HeaderPrimary).getSections();
  
            //  ลบลายน้ำจากส่วนหัว
            for (const section of sections.getInnerList().toArray()) {
                section.setScript(null);
                section.setImage(null);
            }

            //  บันทึกสมุดงานที่ล้างแล้ว
            watermarker.save("result.xlsx");
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
    title: "มาสเตอร์การลบลายน้ำไฟล์ DOCX ด้วย Node.js via Java"
    exclude: "DOCX"
    description: "ค้นพบความสามารถของ GroupDocs.Watermark for Node.js via Java API ในการจัดการและลบลายน้ำออกจากไฟล์ DOCX เพิ่มความปลอดภัยของเอกสารและการนำเสนอโดยไม่กระทบต่อคุณภาพ"
    items: 
        # format loop 1
        - name: "ลายน้ำ PDF"
          format: "PDF"
          link: "/watermark/nodejs-java/delete//pdf/"
          description: "รูปแบบเอกสาร Adobe Portable"

        # format loop 2
        - name: "ลายน้ำ Word"
          format: "WORD"
          link: "/watermark/nodejs-java/delete//word/"
          description: "MS Word และเอกสาร Open Office"
          
        # format loop 3
        - name: "ลายน้ำ Excel"
          format: "EXCEL"
          link: "/watermark/nodejs-java/delete//excel/"
          description: "MS Excel และสเปรดชีตโอเพ่นออฟฟิศ"

        # format loop 4
        - name: "ลายน้ำ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/nodejs-java/delete//powerpoint/"
          description: "MS PowerPoint และงานนำเสนอแบบโอเพ่นออฟฟิศ"

        # format loop 5
        - name: "ลายน้ำ DOCX"
          format: "DOCX"
          link: "/watermark/nodejs-java/delete//docx/"
          description: "ไมโครซอฟท์ Word เปิดเอกสาร XML"
          
        # format loop 6
        - name: "ลายน้ำ PPTX"
          format: "PPTX"
          link: "/watermark/nodejs-java/delete//pptx/"
          description: "PowerPoint เปิดการนำเสนอ XML"
          
        # format loop 7
        - name: "ลายน้ำ XLSX"
          format: "XLSX"
          link: "/watermark/nodejs-java/delete//xlsx/"
          description: "ไมโครซอฟท์ Excel เปิดสเปรดชีต XML"

        # format loop 8
        - name: "ลายน้ำ DOC"
          format: "DOC"
          link: "/watermark/nodejs-java/delete//doc/"
          description: "ไมโครซอฟท์ Word 97 - เอกสาร 2007"

        # format loop 9
        - name: "ลายน้ำ XLS"
          format: "XLS"
          link: "/watermark/nodejs-java/delete//xls/"
          description: "ไมโครซอฟท์ Excel สมุดงาน 97-2003"

        # format loop 10
        - name: "ลายน้ำ PPT"
          format: "PPT"
          link: "/watermark/nodejs-java/delete//ppt/"
          description: "PowerPoint การนำเสนอ 97-2003"

        # format loop 11
        - name: "ลายน้ำ RTF"
          format: "RTF"
          link: "/watermark/nodejs-java/delete//rtf/"
          description: "รูปแบบข้อความที่หลากหลาย"

---