
---
############################# Static ############################
layout: "format"
date:  2024-05-06T23:13:38
draft: false
lang: th
format: Xlsx
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "ฝังลายน้ำใน XLSX ด้วย C#"
head_description: "ใช้ประโยชน์จาก .NET C# เพื่อสร้างและใช้ลายน้ำในไฟล์ XLSX เพื่อรักษาความปลอดภัยเอกสาร Excel ของคุณ"

############################# Header ############################
title: "รักษาความปลอดภัยแผ่นงาน XLSX ด้วย .NET C #" 
description: "ใช้ .NET C# เพื่อสร้างลายน้ำที่ปรับแต่งได้สำหรับไฟล์ XLSX เหมาะสำหรับการเพิ่มความสมบูรณ์ของเอกสารและปกป้องข้อมูลที่ละเอียดอ่อน"
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
       GroupDocs.Watermark for .NET เป็นโซลูชันที่มีประสิทธิภาพสำหรับนักพัฒนา C# .NET ในการสร้าง เพิ่ม และจัดการลายน้ำในไฟล์ XLSXAPI นี้มีความจำเป็นสำหรับการรักษาความลับและความถูกต้องของเอกสาร Excel โดยเฉพาะอย่างยิ่งในสภาพแวดล้อมขององค์กร การเงิน และกฎหมายปรับแต่งลายน้ำของคุณด้วยตัวเลือกที่หลากหลาย รวมถึงการซ้อนทับข้อความและรูปภาพ ซึ่งออกแบบมาให้ทั้งใช้งานได้และละเอียดอ่อนคุณสมบัติเพิ่มเติมช่วยให้สามารถทำลายน้ำอัตโนมัติตามคุณสมบัติเอกสารและเงื่อนไขที่ผู้ใช้กำหนด ทำให้มั่นใจได้ว่าลายน้ำของคุณจะถูกนำไปใช้อย่างสม่ำเสมอและเฉพาะในกรณีที่จำเป็นเท่านั้น GroupDocs.Watermark เข้ากันได้กับแพลตฟอร์ม .NET ร่วมสมัยและรองรับฟังก์ชันขั้นสูง Excel

############################# Steps ############################
steps:
    enable: true
    title: "สร้างลายน้ำได้อย่างง่ายดายสำหรับเอกสาร Xlsx"
    content: |
      **[GroupDocs.Watermark for .NET](https://products.groupdocs.com/watermark/net/):** ไลบรารีลายน้ำขั้นสูงสำหรับแอปพลิเคชัน .NET เสริมศักยภาพให้กับโซลูชันของคุณและรักษาความปลอดภัยเอกสารด้วยลายน้ำได้ทันเวลา
      
      1. **คลาสหลัก: Watermarker** คลาสหลักของ API ของเราคือ **Watermarker** คุณต้องสร้างอินสแตนซ์ก่อนการประมวลผลเอกสาร อย่าลืมส่งไฟล์ Xlsx ไปยังตัวสร้างเป็นเส้นทางหรือวัตถุสตรีม
      2. **การสร้างลายน้ำของคุณ** ขั้นตอนต่อไปคือการสร้างวัตถุลายน้ำตามประเภทที่ต้องการ สามารถวางได้ไม่เพียงแต่บนหน้าเอกสารใดหน้าหนึ่งเท่านั้น แต่ยังวางในส่วนเอกสารดั้งเดิม เช่น รูปภาพหรือส่วนหัวได้อีกด้วย
      3. **การปรับแต่งรูปลักษณ์แบบละเอียด** ตั้งค่าคุณสมบัติลายน้ำ เช่น ความสูงและความกว้าง ด้านบน ซ้าย การจัดตำแหน่งตรงกลาง แบบอักษรและสี เป็นต้น
      4. **การใช้และการบันทึก** ใช้วิธี **Watermarker** เพื่อเพิ่มลายน้ำใหม่ คุณสามารถเพิ่มลายน้ำได้มากเท่าที่คุณต้องการ คุณสามารถบันทึกเอกสารลายน้ำไว้ที่ใดก็ได้
   
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
        // สร้างลายน้ำรูปภาพในไฟล์ XLSX

        // ระบุเส้นทางไฟล์ต้นฉบับให้กับตัวสร้าง Watermarker
        using (Watermarker watermarker = new Watermarker("input.xlsx"))
        {
            // สร้างตัวอย่างลายน้ำรูปภาพด้วยไฟล์รูปภาพ
            using (ImageWatermark watermark = new ImageWatermark("watermark.png"))
            {
                watermarker.Add(watermark);
            }
            // บันทึกผลลัพธ์ที่มีลายน้ำ XLSX
            watermarker.Save("output.xlsx");
        }
        
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "ยกระดับเกมลายน้ำของคุณ"
  description: "ปลดล็อกความสามารถในการทำลายน้ำขั้นสูงด้วย API GroupDocs.Watermark ของเราสำหรับ .NETเครื่องมืออันทรงพลังนี้ช่วยให้สามารถปรับแต่งและใช้ลายน้ำได้อย่างแม่นยำในเอกสารประเภทต่างๆ เพื่อให้มั่นใจถึงความปลอดภัยสูงสุดและการปฏิบัติตามลิขสิทธิ์โดยการหยุดชะงักทางสายตาน้อยที่สุด"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "โซลูชันลายน้ำที่ครอบคลุม"
  features:
    # feature loop
    - title: "ตัวเลือกปูกระเบื้องที่ซับซ้อน"
      content: "ขยายลายน้ำของคุณให้ทั่วทั้งเอกสารได้อย่างราบรื่นด้วยตัวเลือกการปูกระเบื้องของเราคุณลักษณะนี้ช่วยให้ลายน้ำครอบคลุมพื้นที่เอกสารทั้งหมด ป้องกันการลบออกและรับประกันการป้องกันเอกสารที่สมบูรณ์โดยไม่กระทบต่อการออกแบบหรือการอ่านได้"

    # feature loop
    - title: "การปรับแต่งสีสดใส"
      content: "เพิ่มสีสันให้กับลายน้ำของคุณ!API ของเราช่วยให้สามารถปรับแต่งสีแบบเต็มสเปกตรัมช่วยให้คุณสามารถใช้ลายน้ำที่ตรงกับแบรนด์ขององค์กรหรือรูปแบบเอกสารของคุณได้อย่างสมบูรณ์แบบเพิ่มความน่าดึงดูดภาพในขณะที่รักษาคุณสมบัติการรักษาความปลอดภัยที่แข็งแกร่ง"

    # feature loop
    - title: "การตั้งค่าความปลอดภัยที่เพิ่มขึ้น"
      content: "ยกระดับความปลอดภัยของเอกสารไปอีกขั้นด้วยการตั้งค่าลายน้ำขั้นสูงกำหนดค่าลายน้ำหลายชั้น รวมทั้งองค์ประกอบที่มองเห็นได้และมองไม่เห็น เพื่อป้องกันการคัดลอกโดยไม่ได้รับอนุญาต และตรวจสอบให้แน่ใจว่าเฉพาะผู้รับที่ต้องการเท่านั้นที่สามารถเข้าถึงข้อมูลสำคัญได้"
      
  code_samples:
    # code sample loop
    - title: "สร้างลายน้ำ PowerPoint"
      content: |
        ตัวอย่างนี้แสดงวิธีเพิ่มลายน้ำให้กับภาพพื้นหลัง PPTX
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  โหลดการนำเสนอ PPTX
            var loadOptions = new PresentationLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.pptx", loadOptions))
            {
                //  ตั้งค่าคุณสมบัติลายน้ำ
                TextWatermark watermark = new TextWatermark("Protected image", new Font("Arial", 8));
                watermark.HorizontalAlignment = HorizontalAlignment.Center;
                watermark.VerticalAlignment = VerticalAlignment.Center;
                watermark.RotateAngle = 45;
                watermark.SizingType = SizingType.ScaleToParentDimensions;
                watermark.ScaleFactor = 1;

                //  พื้นหลังสไลด์ลายน้ำ
                PresentationContent content = watermarker.GetContent<PresentationContent>();
                foreach (PresentationSlide slide in content.Slides)
                {
                    if (slide.ImageFillFormat.BackgroundImage != null)
                    {
                        slide.ImageFillFormat.BackgroundImage.Add(watermark);
                    }
                }

                //  บันทึกงานนำเสนอที่ประมวลผล
                watermarker.save("result.pptx");
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
    title: "การใช้ลายน้ำใน XLSX ด้วย C#"
    exclude: "XLSX"
    description: "ปรับใช้ .NET C# เพื่อเพิ่มลายน้ำขั้นสูงที่ปลอดภัยให้กับไฟล์ XLSX ได้อย่างมีประสิทธิภาพ เพื่อปกป้องข้อมูล Excel ระดับมืออาชีพของคุณ"
    items: 
        # format loop 1
        - name: "ลายน้ำ PDF"
          format: "PDF"
          link: "/watermark/net/generate//pdf/"
          description: "รูปแบบเอกสาร Adobe Portable"

        # format loop 2
        - name: "ลายน้ำ Word"
          format: "WORD"
          link: "/watermark/net/generate//word/"
          description: "MS Word และเอกสาร Open Office"
          
        # format loop 3
        - name: "ลายน้ำ Excel"
          format: "EXCEL"
          link: "/watermark/net/generate//excel/"
          description: "MS Excel และสเปรดชีตโอเพ่นออฟฟิศ"

        # format loop 4
        - name: "ภาพลายน้ำ"
          format: "IMAGE"
          link: "/watermark/net/generate//image/"
          description: "รูปแบบภาพยอดนิยม"

        # format loop 5
        - name: "ภาพลายน้ำ"
          format: "PHOTO"
          link: "/watermark/net/generate//photo/"
          description: "รูปแบบภาพถ่าย"

        # format loop 6
        - name: "ลายน้ำ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/generate//powerpoint/"
          description: "MS PowerPoint และงานนำเสนอแบบโอเพ่นออฟฟิศ"

        # format loop 7
        - name: "ลายน้ำ DOCX"
          format: "DOCX"
          link: "/watermark/net/generate//docx/"
          description: "ไมโครซอฟท์ Word เปิดเอกสาร XML"
          
        # format loop 8
        - name: "ลายน้ำ PPTX"
          format: "PPTX"
          link: "/watermark/net/generate//pptx/"
          description: "PowerPoint เปิดการนำเสนอ XML"
          
        # format loop 9
        - name: "ลายน้ำ XLSX"
          format: "XLSX"
          link: "/watermark/net/generate//xlsx/"
          description: "ไมโครซอฟท์ Excel เปิดสเปรดชีต XML"

        # format loop 10
        - name: "ลายน้ำ JPEG"
          format: "JPEG"
          link: "/watermark/net/generate//jpeg/"
          description: "JPEG รูปภาพ"

        # format loop 11
        - name: "ลายน้ำ PNG"
          format: "PNG"
          link: "/watermark/net/generate//png/"
          description: "Portable กราฟิกเครือข่าย"

        # format loop 12
        - name: "ลายน้ำ TIFF"
          format: "TIFF"
          link: "/watermark/net/generate//tiff/"
          description: "รูปแบบไฟล์รูปภาพแท็ก"

        # format loop 13
        - name: "ลายน้ำ WEBP"
          format: "WEBP"
          link: "/watermark/net/generate//webp/"
          description: "รูปภาพเว็บ"

        # format loop 14
        - name: "ลายน้ำ DOC"
          format: "DOC"
          link: "/watermark/net/generate//doc/"
          description: "ไมโครซอฟท์ Word 97 - เอกสาร 2007"

        # format loop 15
        - name: "ลายน้ำ XLS"
          format: "XLS"
          link: "/watermark/net/generate//xls/"
          description: "ไมโครซอฟท์ Excel สมุดงาน 97-2003"

        # format loop 16
        - name: "ลายน้ำ PPT"
          format: "PPT"
          link: "/watermark/net/generate//ppt/"
          description: "PowerPoint การนำเสนอ 97-2003"

        # format loop 17
        - name: "ลายน้ำ RTF"
          format: "RTF"
          link: "/watermark/net/generate//rtf/"
          description: "รูปแบบข้อความที่หลากหลาย"

---