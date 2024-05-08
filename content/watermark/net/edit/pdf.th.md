
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:25
draft: false
lang: th
format: Pdf
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "แก้ไขลายน้ำ Pdf ด้วย GroupDocs.Watermark"
head_description: "แก้ไขลายน้ำ Pdf ในไฟล์ Pdf โดยใช้ GroupDocs.Watermark for .NET เฟรมเวิร์กปรับให้เข้ากับความต้องการเอกสารของคุณได้อย่างง่ายดาย"

############################# Header ############################
title: "แก้ไขลายน้ำในความสามารถในการปรับตัว Pdf: .NET" 
description: "ปรับให้เข้ากับความต้องการของเอกสารของคุณได้อย่างราบรื่นด้วย GroupDocs.Watermark for .NET Frameworkแก้ไขลายน้ำในหลายรูปแบบได้อย่างง่ายดาย"
subtitle: "GroupDocs.Watermark for .NET โซลูชั่น" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "แพ็คเกจฟรี Nuget"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET โซลูชั่น"
    link: "/watermark/net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **แก้ไขลายน้ำใน PDF s:** ปกป้องเนื้อหาของคุณในหลายรูปแบบด้วย GroupDocs.Watermark for .NET Frameworkปรับให้เข้ากับความต้องการของเอกสารของคุณได้อย่างราบรื่นด้วยเครื่องมืออเนกประสงค์ของเรา

############################# Steps ############################
steps:
    enable: true
    title: "แก้ไขลายน้ำโดยทางโปรแกรมในเอกสาร Pdf ด้วย .NET API"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** มอบ API ที่มีประสิทธิภาพสำหรับนักพัฒนาซอฟต์แวร์ .NET เพื่อจัดการลายน้ำโดยทางโปรแกรมภายในเอกสาร Pdf ที่หลากหลาย คู่มือนี้จะสรุปกระบวนการ:
      
      1. เริ่มต้นเวิร์กโฟลว์โดยระบุไฟล์ Pdf ของคุณเป็นอาร์กิวเมนต์ให้กับตัวสร้างคลาส **Watermarker** ไฟล์สามารถระบุเป็นสตรีมไบต์ สตรีมไฟล์ หรือการอ้างอิงไปยังตำแหน่งของดิสก์ในเครื่อง
      2. จากนั้น ใช้ประโยชน์จากออบเจ็กต์ **SearchCriteria** เพื่อระบุลายน้ำเฉพาะที่ต้องมีการแก้ไข ออบเจ็กต์นี้ช่วยให้สามารถระบุลายน้ำที่ฝังไว้ก่อนหน้านี้ภายในเอกสารได้
      3. เมื่อดำเนินการค้นหาสำเร็จ คุณจะได้รับชุดลายน้ำที่เกี่ยวข้อง ลายน้ำเหล่านี้ให้การควบคุมแบบละเอียด ช่วยให้คุณสามารถปรับเปลี่ยนคุณสมบัติ เช่น ขนาด การวางตำแหน่งหน้า เนื้อหาข้อความ โทนสี ข้อมูลรูปภาพ และอื่นๆ
      4. หลังจากการแก้ไขลายน้ำเสร็จสิ้น ให้คงเอกสารที่แก้ไขไว้ API อำนวยความสะดวกในการจัดเก็บข้อมูลโดยใช้เส้นทางไฟล์ในเครื่องหรือออบเจ็กต์สตรีม
   
    code:
      platform: "net"
      copy_title: "คัดลอก"
      install:
        command: |
        command: "dotnet add package GroupDocs.Watermark"
        copy_tip: "คลิกเพื่อคัดลอก"
        copy_done: "คัดลอก"
      links:
        #  loop
        - title: "ตัวอย่างเพิ่มเติม"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
        #  loop
        - title: "เอกสาร"
          link: "https://docs.groupdocs.com/watermark/net/"
          
      content: |
        ```csharp {style=abap}
        // แก้ไขลายน้ำรูปภาพในเอกสาร PDF

        // เริ่มต้น Watermarker ด้วยไฟล์ต้นฉบับ
        using (Watermarker watermarker = new Watermarker("input.pdf"))
        {
            // สร้าง SearchCriteria สำหรับการค้นหาลายน้ำรูปภาพ
            SearchCriteria searchCriteria = new ImageDctHashSearchCriteria("logo.png");
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                // แก้ไขลายน้ำรูปภาพ
                watermark.ImageData = imageData;
            }

            // บันทึกผลลัพธ์ PDF
            watermarker.Save("output.pdf");
        }
        
        ```     

############################# More features ############################
more_features:
  enable: true
  title: "เติมเต็มเวิร์กโฟลว์ของคุณด้วยการจัดการลายน้ำ"
  description: "ลดความซับซ้อนในการทำลายน้ำในรูปแบบไฟล์ที่หลากหลายในแอปพลิเคชัน .NET ของคุณด้วยไลบรารีที่แข็งแกร่งของเราเพิ่ม แก้ไข ค้นหา หรือลบลายน้ำได้อย่างง่ายดายเพื่อเพิ่มความปลอดภัยของเอกสารและการสร้างแบรนด์"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "การแก้ไขลายน้ำได้อย่างราบรื่น"
  features:
    # feature loop
    - title: "เพิ่มความคล่องตัวในการทำลายน้ำในแอปพลิเคชันของคุณ"
      content: "ใช้ประโยชน์จากพลังของ GroupDocs.Watermark for .NET เพื่อรวมฟังก์ชันการทำลายน้ำเข้ากับแอปพลิเคชัน .NET ของคุณได้อย่างราบรื่นAPI ที่ใช้งานง่ายของเราช่วยลดความซับซ้อนในการสร้างลายน้ำ การจัดการ ค้นหา และการแก้ไข ไม่จำเป็นต้องใช้กระบวนการด้วยตนเองที่ซับซ้อน"

    # feature loop
    - title: "การปรับแต่งลายน้ำแบบเม็ด"
      content: "ปลดปล่อยศักยภาพเต็มรูปแบบของการปรับแต่งลายน้ำด้วย API ที่ครอบคลุมของเราปรับแต่งทุกรายละเอียด รวมถึงขนาด การวางแนว โทนสี และการเลือกแบบอักษร เพื่อสร้างลายน้ำที่สอดคล้องกับข้อกำหนดด้านการสร้างแบรนด์และความปลอดภัยของคุณได้อย่างสมบูรณ์แบบ"

    # feature loop
    - title: "ฟีเจอร์เฉพาะเอกสารของชุดสายรัดสำหรับการทำลายน้ำที่ยืดหยุ่น"
      content: "ปลดล็อกพลังของฟังก์ชันดั้งเดิมภายในรูปแบบเอกสารต่างๆใช้องค์ประกอบต่างๆ เช่น พื้นหลังเอกสาร คำอธิบายประกอบ ส่วนหัว หรือวัตถุอื่น ๆ เป็นคอนเทนเนอร์ลายน้ำที่ไม่ซ้ำกัน ตอบสนองประเภทเอกสารที่หลากหลายและความต้องการด้านความปลอดภัย"
      
  code_samples:
    # code sample loop
    - title: "PDF แก้ไขลายน้ำรูปภาพ"
      content: |
        ตัวอย่างนี้แสดงวิธีการแก้ไขเนื้อหาของลายน้ำรูปภาพ
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  โหลดเอกสารเป็น PDF
            var loadOptions = new PdfLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pdf", loadOptions))
            {
                //  โหลดเนื้อหา
                PdfContent pdfContent = watermarker.GetContent<PdfContent>();

                //  แก้ไขลายน้ำภาพ
                foreach (PdfArtifact artifact in pdfContent.Pages[0].Artifacts)
                {
                    if (artifact.Image != null)
                    {
                        artifact.Image = new PdfWatermarkableImage(File.ReadAllBytes("test.png"));
                    }
                }

                //  เพลิดเพลินกับผลลัพธ์
                watermarker.save("result.pdf");
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
    - title: "Nuget ดาวน์โหลด"
      link: "https://releases.groupdocs.com/watermark/net/"
      color: "red"
        #  loop
    - title: "การออกใบอนุญาต"
      link: "https://purchase.groupdocs.com/pricing/watermark/net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "ปรับลายน้ำในหลายรูปแบบ"
    exclude: "PDF"
    description: "ปกป้องเนื้อหาของคุณในรูปแบบเอกสารต่างๆ ด้วย GroupDocs.Watermark for .NET Framework"
    items: 
        # format loop 1
        - name: "ลายน้ำ PDF"
          format: "PDF"
          link: "/watermark/net/edit//pdf/"
          description: "รูปแบบเอกสาร Adobe Portable"

        # format loop 2
        - name: "ลายน้ำ Word"
          format: "WORD"
          link: "/watermark/net/edit//word/"
          description: "MS Word และเอกสาร Open Office"
          
        # format loop 3
        - name: "ลายน้ำ Excel"
          format: "EXCEL"
          link: "/watermark/net/edit//excel/"
          description: "MS Excel และสเปรดชีตโอเพ่นออฟฟิศ"

        # format loop 4
        - name: "ลายน้ำ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/edit//powerpoint/"
          description: "MS PowerPoint และงานนำเสนอแบบโอเพ่นออฟฟิศ"

        # format loop 5
        - name: "ลายน้ำ DOCX"
          format: "DOCX"
          link: "/watermark/net/edit//docx/"
          description: "ไมโครซอฟท์ Word เปิดเอกสาร XML"
          
        # format loop 6
        - name: "ลายน้ำ PPTX"
          format: "PPTX"
          link: "/watermark/net/edit//pptx/"
          description: "PowerPoint เปิดการนำเสนอ XML"
          
        # format loop 7
        - name: "ลายน้ำ XLSX"
          format: "XLSX"
          link: "/watermark/net/edit//xlsx/"
          description: "ไมโครซอฟท์ Excel เปิดสเปรดชีต XML"

        # format loop 8
        - name: "ลายน้ำ DOC"
          format: "DOC"
          link: "/watermark/net/edit//doc/"
          description: "ไมโครซอฟท์ Word 97 - เอกสาร 2007"

        # format loop 9
        - name: "ลายน้ำ XLS"
          format: "XLS"
          link: "/watermark/net/edit//xls/"
          description: "ไมโครซอฟท์ Excel สมุดงาน 97-2003"

        # format loop 10
        - name: "ลายน้ำ PPT"
          format: "PPT"
          link: "/watermark/net/edit//ppt/"
          description: "PowerPoint การนำเสนอ 97-2003"

        # format loop 11
        - name: "ลายน้ำ RTF"
          format: "RTF"
          link: "/watermark/net/edit//rtf/"
          description: "รูปแบบข้อความที่หลากหลาย"

---