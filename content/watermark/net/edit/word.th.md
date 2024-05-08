
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:19
draft: false
lang: th
format: Word
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "แก้ไขลายน้ำในเอกสาร Word"
head_description: "ปรับแต่งตำแหน่งลายน้ำและตรวจสอบความปลอดภัยของเอกสารด้วย GroupDocs.Watermark for .NET ปรับแต่งลายน้ำ Word ในโซลูชันของคุณได้อย่างง่ายดาย"

############################# Header ############################
title: "เพิ่มลายน้ำ Word: ความมั่นใจ .NET" 
description: "ตรวจสอบความถูกต้องของเอกสาร Word และความสมบูรณ์ของแบรนด์ด้วย GroupDocs.Watermark for .NET แก้ไขลายน้ำโดยใช้โซลูชันของเราอย่างมั่นใจ"
subtitle: "GroupDocs.Watermark for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดที่ Nuget ฟรี"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET"
    link: "/watermark/net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **เพิ่มความปลอดภัยของเอกสาร Word:** GroupDocs.Watermark for .NET ช่วยให้นักพัฒนาสามารถเพิ่มความปลอดภัยของเอกสารได้อย่างง่ายดายแก้ไขลายน้ำของคุณเพื่อตอบสนองความต้องการเฉพาะของคุณด้วยความมั่นใจ

############################# Steps ############################
steps:
    enable: true
    title: "แก้ไขลายน้ำในเอกสาร Word โดยใช้ .NET"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/)** ช่วยให้นักพัฒนา .NET แก้ไขลายน้ำภายในเอกสาร Word ต่างๆ ได้อย่างง่ายดาย คำแนะนำง่ายๆ ในการใช้ API ของเราในแอปพลิเคชันของคุณมีดังนี้:
      
      1. เริ่มต้นด้วยการส่งไฟล์ Word ของคุณเป็นพารามิเตอร์ไปยังตัวสร้างคลาส **Watermarker** คุณสามารถระบุไฟล์เป็นสตรีมไบต์ สตรีมไฟล์ หรือเส้นทางดิสก์ในเครื่องได้
      2. ถัดไป ค้นหาลายน้ำเฉพาะที่ต้องมีการแก้ไข ใช้ **SearchCriteria** เพื่อระบุลายน้ำที่มีคุณสมบัติที่เกี่ยวข้องซึ่งเพิ่มลงในเอกสารก่อนหน้านี้
      3. หลังจากการค้นหา คุณจะได้รับรายการลายน้ำที่เกี่ยวข้อง จากนั้นคุณสามารถปรับแต่งคุณสมบัติต่างๆ ได้ เช่น ขนาด การจัดแนวหน้า ข้อความ สี เนื้อหารูปภาพ และอื่นๆ สิ่งนี้ทำให้คุณสามารถควบคุมข้อมูลของคุณได้อย่างกว้างขวาง
      4. เมื่อคุณแก้ไขลายน้ำเสร็จแล้ว ให้บันทึกเอกสารที่อัปเดต คุณสามารถใช้เส้นทางไฟล์ในเครื่องหรือสตรีมเพื่อจัดเก็บผลลัพธ์สุดท้ายได้
   
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
        // แก้ไขลายน้ำข้อความ WORD

        // ทำให้ Watermarker มีไฟล์ WORD
        using (Watermarker watermarker = new Watermarker("input.ด็อกซ์"))
        {
            // สร้าง TextSearchCriteria และรับลายน้ำข้อความ
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);

            foreach (PossibleWatermark watermark in watermarks)
            {
                 // แก้ไขลายน้ำข้อความ
                 watermark.FormattedTextFragments.Clear();
                 watermark.FormattedTextFragments.Add("passed", 
                    new Font("Calibri", 19, FontStyle.Bold), Color.Red, Color.Aqua);
            }

            // บันทึกเอกสาร
            watermarker.Save("output.ด็อกซ์");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "เรียนรู้เพิ่มเติมเกี่ยวกับการปรับเปลี่ยนลายน้ำ"
  description: "เพิ่มพลังให้กับแอปพลิเคชัน .NET ของคุณด้วยไลบรารีของเรา และเพิ่ม แก้ไข ลบ หรือค้นหาลายน้ำในรูปแบบไฟล์ต่างๆ"
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "แก้ไขลายน้ำ"
  features:
    # feature loop
    - title: "ไฟล์ลายน้ำสำหรับธุรกิจของคุณ"
      content: "ใช้ GroupDocs.Watermark for .NET เพื่อทำลายน้ำไฟล์และเอกสารเพิ่มและจัดการลายน้ำโดยไม่ต้องใช้ความพยายามเป็นพิเศษในการใช้ API ของเราในแอปพลิเคชันของคุณค้นหา แก้ไข และลบลายน้ำที่เพิ่มไว้ก่อนหน้านี้"

    # feature loop
    - title: "ปรับลายน้ำให้ละเอียดตามความต้องการของคุณ"
      content: "API ของเรามีชุดตัวเลือกการปรับแต่งที่ครอบคลุมปรับเปลี่ยนแง่มุมต่างๆ เช่น ขนาด การวางแนวโทนสี ตระกูลแบบอักษร และอื่น ๆ ได้อย่างง่ายดายเพื่อสร้างลายน้ำในอุดมคติ"

    # feature loop
    - title: "ใช้ประโยชน์จากคุณสมบัติเฉพาะเอกสาร"
      content: "คุณสามารถรวมฟังก์ชันในตัวได้ทั้งนี้ขึ้นอยู่กับรูปแบบไฟล์ที่คุณใช้สิ่งเหล่านี้อาจรวมถึงพื้นหลังของเอกสาร คำอธิบายประกอบ ส่วนหัว หรือองค์ประกอบอื่น ๆ ที่จะทำหน้าที่เป็นคอนเทนเนอร์ลายน้ำ"
      
  code_samples:
    # code sample loop
    - title: "Excel แก้ไขข้อความลายน้ำ"
      content: |
        ตัวอย่างนี้แสดงวิธีแก้ไขข้อความสำหรับลายน้ำเฉพาะในแผ่นงาน Excel
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  โหลดสเปรดชีต XLSX
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  โหลดเนื้อหาสเปรดชีต
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();

                //  แก้ไขข้อความด้านในลายน้ำ
                foreach (SpreadsheetShape shape in content.Worksheets[0].Shapes)
                {
                    if (shape.Text == "GroupDocs 2016")
                    {
                        shape.Text = "GroupDocs 2017";
                    }
                }

                //  บันทึกผลลัพธ์ผลลัพธ์
                watermarker.save("result.xlsx");
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
    title: "เพิ่มความปลอดภัยในรูปแบบอื่น ๆ"
    exclude: "WORD"
    description: "GroupDocs.Watermark for .NET นำเสนอโซลูชันที่มีประสิทธิภาพเพื่อเพิ่มความปลอดภัยของเอกสารในรูปแบบต่างๆ"
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