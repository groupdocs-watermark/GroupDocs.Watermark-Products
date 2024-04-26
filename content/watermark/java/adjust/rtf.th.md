
---
############################# Static ############################
layout: "format"
date:  2024-04-26T21:39:01
draft: false
lang: th
format: Rtf
product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "ปรับลายน้ำใน RTF - GroupDocs.Watermark"
head_description: "ขัดเอกสารของคุณด้วยความแม่นยำโดยใช้ GroupDocs.Watermarkปรับและอัปเดตลายน้ำได้อย่างง่ายดาย"

############################# Header ############################
title: "ขัดเอกสาร RTF ของคุณ: การแก้ไขลายน้ำ" 
description: "ปรับแต่งเอกสารของคุณด้วยความสามารถในการแก้ไขลายน้ำที่ครอบคลุมของเราขัดเนื้อหาของคุณด้วยความแม่นยำ"
subtitle: "GroupDocs.Watermark for Java เอพีอี" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดที่ Maven ฟรี"
      link: "https://releases.groupdocs.com/watermark/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Java เอพีอี"
    link: "/watermark/java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **ขัดเอกสารของคุณ**: ความสามารถในการแก้ไขลายน้ำที่ครอบคลุมของเราช่วยให้คุณปรับแต่งเอกสารของคุณได้อย่างแม่นยำตั้งแต่การปรับเปลี่ยนเล็กน้อยไปจนถึงการเปลี่ยนแปลงที่สมบูรณ์ ให้ผลลัพธ์ที่ขัดแย้งได้อย่างง่ายดาย

############################# Steps ############################
steps:
    enable: true
    title: "ปรับลายน้ำเอกสาร Rtf โดยใช้ Java"
    content: |
      **[GroupDocs.Watermark for Java](https://products.groupdocs.com/watermark/java/)** ช่วยให้นักพัฒนา Java สามารถปรับลายน้ำในเอกสารจำนวนมากโดยใช้แอปพลิเคชันของตนได้อย่างง่ายดายนี่คือคำแนะนำฉบับย่อ:
      
      1. **Watermarker**ให้ไบต์หรือสตรีมไฟล์หรือเส้นทางดิสก์ท้องถิ่น
      2. **SearchCriteria** เพื่อระบุลายน้ำที่มีคุณสมบัติเฉพาะที่เพิ่มไว้ในเอกสารก่อนหน้านี้
      3. หลังจากการค้นหา คุณจะได้รับรายการลายน้ำที่เกี่ยวข้องจากนั้นคุณสามารถปรับคุณสมบัติ ได้แก่ ขนาด การจัดตำแหน่งหน้า ข้อความ สี เนื้อหาภาพ และอื่นๆสิ่งนี้ให้การปรับแต่งในระดับสูงสำหรับข้อมูลของคุณ
      4. เมื่อคุณปรับลายน้ำเสร็จแล้วให้บันทึกเอกสารที่อัปเดตคุณสามารถใช้เส้นทางไฟล์ท้องถิ่นหรือสตรีมเพื่อจัดเก็บผลลัพธ์
   
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
        // ปรับลายน้ำรูปภาพ RTF

        // สร้างเครื่องหมายน้ำทันทีด้วย RTF
        Watermarker watermarker = new Watermarker("input.rtf");
        
        // เริ่มต้นการค้นหาCriteria เพื่อให้ตรงกับภาพที่เฉพาะเจาะจง
        SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
        PossibleWatermarkCollection watermarks = watermarker.search(searchCriteria);

        for (PossibleWatermark watermark : watermarks)
        {
            // แทนที่ภาพที่พบ
            watermark.setImageData(imageData);
        }

        // บันทึกไฟล์ที่แก้ไข
        watermarker.save("output.rtf");
        
        ```
        
############################# More features ############################
more_features:
  enable: true
  title: "การจัดการลายน้ำ RTF ขั้นสูงสำหรับการใช้งาน Java"
  description: "API GroupDocs.Watermark ช่วยให้นักพัฒนาสามารถรวมฟังก์ชันการทำลายน้ำเข้ากับแอปพลิเคชัน Java ได้อย่างราบรื่นรองรับการเพิ่ม แก้ไข ลบ และการค้นหาลายน้ำในรูปแบบเอกสารที่หลากหลาย"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "การปรับลายน้ำ"
  features:
    # feature loop
    - title: "การรวมลายน้ำได้อย่างง่ายดาย"
      content: "GroupDocs.Watermark ช่วยลดความยุ่งยากในการเพิ่มลายน้ำที่หลากหลายให้กับเอกสารและไฟล์ธุรกิจต่าง ๆ ภายในแอปพลิเคชัน Javaนักพัฒนาไม่เพียง แต่สามารถใช้ลายน้ำ แต่ยังอัปเดตหรือลบลายที่มีอยู่ด้วยโปรแกรม"

    # feature loop
    - title: "การปรับแต่งลายน้ำแบบเม็ด"
      content: "API มีตัวเลือกการปรับแต่งที่กว้างขวางสำหรับลายน้ำนักพัฒนาสามารถปรับขนาดการหมุนสีแบบอักษรสไตล์และคุณสมบัติอื่น ๆ ได้อย่างง่ายดายเพื่อให้ได้เอฟเฟกต์ภาพที่ต้องการ"

    # feature loop
    - title: "ใช้ประโยชน์จากคุณลักษณะเอกสารดั้งเดิม RTF"
      content: "นักพัฒนาสามารถใช้ฟังก์ชันดั้งเดิมสำหรับการจัดวางลายน้ำขึ้นอยู่กับรูปแบบเอกสารเป้าหมายฟังก์ชันเหล่านี้อาจรวมถึงพื้นหลังหน้าเอกสาร คำอธิบายประกอบ ส่วนหัว หรือวัตถุอื่น ๆ เป็นคอนเทนเนอร์ลายน้ำ"
      
  code_samples:
    # code sample loop
    - title: "ปรับลายน้ำภาพในสเปรดชีต"
      content: |
        ตัวอย่างนี้แสดงวิธีการปรับรูปภาพของรูปร่างเฉพาะในแผ่นงาน Excel
        {{< landing/code title="Java">}}
        ```java {style=abap}
        
        //  โหลดเอกสารเป็นสเปรดชีต
        SpreadsheetLoadOptions loadOptions = new SpreadsheetLoadOptions();
        Watermarker watermarker = new Watermarker("source.xlsx", loadOptions);

        //  รับไบต์ลายน้ำใหม่
        File file = new File("new_watermark.png");
        byte[] imageBytes = new byte[(int) file.length()];
        FileInputStream inputStream = new FileInputStream(file);
        inputStream.read(imageBytes);
        inputStream.close();

        //  ปรับเนื้อหาของลายน้ำเฉพาะ
        for (SpreadsheetShape shape : content.getWorksheets().get_Item(0).getShapes())
        {
            if (shape.getImage() != null)
            {
                shape.setImage(new SpreadsheetWatermarkableImage(imageBytes));
            }
        }

        //  บันทึกเอกสารผลลัพธ์
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
    title: "ลายน้ำเอกสารโปแลนด์ในรูปแบบอื่นด้วย GroupDocs.Watermark for Java"
    exclude: "RTF"
    description: "ปรับแต่งเอกสารของคุณด้วยความแม่นยำโดยใช้ความสามารถในการแก้ไขลายน้ำที่ครอบคลุมของเราเพิ่มความถูกต้องของเอกสารได้อย่างง่ายดาย"
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