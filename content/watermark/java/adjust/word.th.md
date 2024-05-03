
---
############################# Static ############################
layout: "format"
date:  2024-05-03T13:37:05
draft: false
lang: th
format: Word
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "ปรับลายน้ำ Word ได้อย่างง่ายดาย - GroupDocs.Watermark"
head_description: "ปรับลายน้ำได้อย่างราบรื่นในรูปแบบเอกสารหลายรูปแบบโดยใช้ GroupDocs.Watermarkเพิ่มความปลอดภัยของเอกสารของคุณ"

############################# Header ############################
title: "ปรับลายน้ำ Word: ปลอดภัยได้อย่างง่ายดาย" 
description: "รักษาความปลอดภัยเอกสารของคุณได้อย่างง่ายดายด้วยความสามารถในการปรับเปลี่ยนลายน้ำอันทรงพลังของเราปกป้องเนื้อหาของคุณด้วยความมั่นใจ"
subtitle: "GroupDocs.Watermark for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดที่ Maven ฟรี"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java"
    link: "/watermark/java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **แก้ไขลายน้ำ**: GroupDocs.Watermark ช่วยให้ผู้ใช้สามารถแก้ไขลายน้ำในรูปแบบเอกสารต่างๆได้อย่างราบรื่นด้วยการควบคุมที่แม่นยำและตัวเลือกที่หลากหลาย ปรับแต่งเอกสารของคุณด้วยความมั่นใจ

############################# Steps ############################
steps:
    enable: true
    title: "ปรับลายน้ำในเอกสาร Word ด้วย Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** ทำให้นักพัฒนา Java ปรับลายน้ำข้อความในแอปพลิเคชันได้อย่างง่ายดายโดยทำตามขั้นตอนง่ายๆ ไม่กี่ขั้นตอน:
      
      1. โหลดไฟล์ Word ของคุณไปยังออบเจ็กต์หลักของ API ของเราชื่อ **Watermarker** คุณสามารถจัดเตรียมไฟล์สำหรับการประมวลผลเพิ่มเติมในรูปแบบสตรีมหรือเส้นทางบนดิสก์ภายในเครื่องได้
      2. ขั้นตอนต่อไปคือการค้นหาลายน้ำซึ่งจะต้องปรับเปลี่ยน **SearchCriteria** ช่วยในการระบุลายน้ำที่มีคุณสมบัติที่ถูกต้องซึ่งถูกเพิ่มลงในเอกสารก่อนหน้านี้
      3. รับรายการลายน้ำที่เหมาะสมตามขั้นตอน **Search** ปรับคุณสมบัติลายน้ำที่พบ เช่น ขนาด การจัดแนวหน้า ข้อความ สี เนื้อหารูปภาพ ฯลฯ มีหลายวิธีในการปรับแต่งข้อมูลของคุณ
      4. หลังจากเสร็จสิ้นกระบวนการปรับลายน้ำแล้ว คุณจะต้องบันทึกเอกสารที่อัปเดต ใช้เส้นทางไฟล์ในเครื่อง ไฟล์หรือสตรีมไบต์เพื่อจัดเก็บผลลัพธ์
   
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

        // ปรับลายน้ำข้อความ WORD

        // สร้างอินสแตนซ์ Watermarker ด้วยเอกสารอินพุต WORD
        Watermarker watermarker = new Watermarker("input.ด็อกซ์");

        // เริ่มต้น TextSearchCriteria และค้นหาลายน้ำข้อความ
        TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);
        
        // ปรับคุณสมบัติลายน้ำข้อความ
        for (PossibleWatermark watermark : watermarks)
        {
            watermark.getFormattedTextFragments().clear();
            watermark.getFormattedTextFragments().
                add("passed", new Font("Calibri", 19, FontStyle.Bold), Color.getRed(), Color.getAqua());
        }

        // บันทึกเอกสารที่อัพเดต
        watermarker.save("output.ด็อกซ์");
        
        ```            
        
############################# More features ############################
more_features:
  enable: true
  title: "ดำดิ่งลึกเข้าสู่การปรับลายน้ำ WORD"
  description: "API ของเราช่วยให้แอปพลิเคชัน Java สามารถเพิ่ม แก้ไข ลบ และค้นหาลายน้ำในรูปแบบเอกสารยอดนิยม"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "ปรับลายน้ำ"
  features:
    # feature loop
    - title: "ลายน้ำเอกสารของคุณได้อย่างง่ายดาย"
      content: "GroupDocs.Watermark ช่วยลดความซับซ้อนให้กับนักพัฒนา Javaเพิ่มลายน้ำที่หลากหลายลงในเอกสารและไฟล์ธุรกิจต่างๆไม่เพียง แต่คุณสามารถใช้ลายน้ำเท่านั้น แต่คุณยังสามารถอัปเดตหรือลบลายที่มีอยู่ได้อีกด้วย"

    # feature loop
    - title: "ปรับแต่งลายน้ำตามความต้องการของคุณ"
      content: "API ของเรามีตัวเลือกการปรับแต่งที่กว้างขวางปรับขนาด การหมุน สี แบบอักษร สไตล์ และอื่นๆ ได้อย่างง่ายดายเพื่อให้ได้ลายน้ำที่สมบูรณ์แบบ"

    # feature loop
    - title: "ใช้คุณสมบัติเอกสารดั้งเดิม WORD"
      content: "คุณสามารถใช้ฟังก์ชันดั้งเดิมได้ขึ้นอยู่กับรูปแบบเอกสารเฉพาะสิ่งเหล่านี้อาจรวมถึงพื้นหลังหน้าเอกสาร คำอธิบายประกอบ ส่วนหัว หรือวัตถุอื่น ๆ เป็นคอนเทนเนอร์ลายน้ำ"
      
  code_samples:
    # code sample loop
    - title: "PDF ปรับลายน้ำข้อความ"
      content: |
        ตัวอย่างนี้แสดงวิธีการปรับข้อความของสิ่งประดิษฐ์เฉพาะ
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  โหลดเอกสาร PDF
        PdfLoadOptions loadOptions = new PdfLoadOptions();
        Watermarker watermarker = new Watermarker("source.pdf", loadOptions);

        //  รับเนื้อหาเอกสาร
        PdfContent pdfContent = watermarker.getContent(PdfContent.class);

        //  ปรับข้อความลายน้ำเฉพาะ
        for (PdfArtifact artifact : pdfContent.getPages().get_Item(0).getArtifacts())
        {
            if (artifact.getText().contains("Test"))
            {
                artifact.setText("Passed");
            }
        }

        //  บันทึกเอกสาร
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
    title: "ปรับลายน้ำโดยใช้ GroupDocs.Watermark for Java สำหรับรูปแบบยอดนิยม"
    exclude: "WORD"
    description: "GroupDocs.Watermark รองรับการดัดแปลงลายน้ำอย่างราบรื่นในรูปแบบต่างๆปรับแต่งกลยุทธ์การทำลายน้ำของคุณให้ตรงกับความต้องการเฉพาะของคุณ"
    items: 
        # format loop 1
        - name: "ลายน้ำ PDF"
          format: "PDF"
          link: "/watermark/java/adjust//pdf/"
          description: "รูปแบบเอกสาร Adobe Portable"

        # format loop 2
        - name: "ลายน้ำ Word"
          format: "WORD"
          link: "/watermark/java/adjust//word/"
          description: "MS Word และเอกสาร Open Office"
          
        # format loop 3
        - name: "ลายน้ำ Excel"
          format: "EXCEL"
          link: "/watermark/java/adjust//excel/"
          description: "MS Excel และสเปรดชีตโอเพ่นออฟฟิศ"

        # format loop 4
        - name: "ลายน้ำ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/java/adjust//powerpoint/"
          description: "MS PowerPoint และงานนำเสนอแบบโอเพ่นออฟฟิศ"

        # format loop 5
        - name: "ลายน้ำ DOCX"
          format: "DOCX"
          link: "/watermark/java/adjust//docx/"
          description: "ไมโครซอฟท์ Word เปิดเอกสาร XML"
          
        # format loop 6
        - name: "ลายน้ำ PPTX"
          format: "PPTX"
          link: "/watermark/java/adjust//pptx/"
          description: "PowerPoint เปิดการนำเสนอ XML"
          
        # format loop 7
        - name: "ลายน้ำ XLSX"
          format: "XLSX"
          link: "/watermark/java/adjust//xlsx/"
          description: "ไมโครซอฟท์ Excel เปิดสเปรดชีต XML"

        # format loop 8
        - name: "ลายน้ำ DOC"
          format: "DOC"
          link: "/watermark/java/adjust//doc/"
          description: "ไมโครซอฟท์ Word 97 - เอกสาร 2007"

        # format loop 9
        - name: "ลายน้ำ XLS"
          format: "XLS"
          link: "/watermark/java/adjust//xls/"
          description: "ไมโครซอฟท์ Excel สมุดงาน 97-2003"

        # format loop 10
        - name: "ลายน้ำ PPT"
          format: "PPT"
          link: "/watermark/java/adjust//ppt/"
          description: "PowerPoint การนำเสนอ 97-2003"

        # format loop 11
        - name: "ลายน้ำ RTF"
          format: "RTF"
          link: "/watermark/java/adjust//rtf/"
          description: "รูปแบบข้อความที่หลากหลาย"

---