---
############################# Static ############################
layout: "landing"
date: 2024-04-29T14:27:13
draft: false

lang: th
product: "Watermark"
product_tag: "watermark"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "C# .NET ซอฟต์แวร์ลายน้ำเอกสาร | เพิ่มลายน้ำ"
head_description: "C# .NET ไลบรารี เพื่อเพิ่ม ค้นหา และลบลายน้ำในเอกสาร: PDF, Word, Excel, งานนำเสนอ, ไดอะแกรม Visio, รูปแบบไฟล์อีเมลและรูปภาพ"

############################# Header ############################
title: "เอกสารลายน้ำได้อย่างง่ายดายในแอปพลิเคชัน C# .NET"
description: "เพิ่มพลังให้กับโซลูชัน C# ของคุณด้วย API ลายน้ำเอกสารที่ยืดหยุ่นซึ่งให้การเพิ่มลายน้ำที่ปรับแต่งได้ให้กับรูปแบบเอกสารยอดนิยมทั้งหมด"
words:
  for: "สำหรับ"

actions:
  main: "ดาวน์โหลดฟรี NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Watermark"
  alt: "การออกใบอนุญาต"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/net/"
  title: "พร้อมที่จะเริ่มแล้วหรือยัง?"
  description: "ลองใช้คุณสมบัติ GroupDocs.Watermark ฟรีหรือขอใบอนุญาต"

release:
  title: "เวอร์ชัน {0} เผยแพร่"
  notes: "ดูว่ามีอะไรใหม่"
  downloads: "ดาวน์โหลด"

code:
  title: "ลายน้ำ PDF ไฟล์ C#"
  more: "ตัวอย่างเพิ่มเติม"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/"
  install: "dotnet add package GroupDocs.Watermark"
  content: |
    ```csharp {style=abap}   
    // ใช้เครื่องหมายน้ำแบบทันทีที่ผ่านเส้นทาง PDF
    PdfLoadOptions loadOptions = new PdfLoadOptions();
    using (Watermarker watermarker = 
        new Watermarker("source.pdf", loadOptions))
    {
        // ปรับแต่งตัวเลือกลายน้ำ
        TextWatermark textWatermark = 
            new TextWatermark("Approved", new Font("Arial", 8));
        
        // ใช้ลายน้ำกับเอกสาร PDF
        watermarker.Add(textWatermark);

        // บันทึกเอกสารผลลัพธ์
        watermarker.Save("result.pdf");
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "สรุปภาพ GroupDocs.Watermark"
  description: "API เพื่อใส่ลายน้ำบนเอกสารผ่าน .NET"
  features:
    # feature loop
    - title: "ลายน้ำ ไฟล์ C #"
      content: "เพิ่มลายน้ำลงในไฟล์ธุรกิจของคุณโดยใช้ GroupDocs.Watermarkใช้ข้อความ รูปภาพ ไดอะแกรม หรือไฟล์แนบอีเมล"

    # feature loop
    - title: "ปรับแต่งลายน้ำให้เหมาะกับเป้าหมายของคุณ"
      content: "ซอฟต์แวร์ GroupDocs.Watermark for .NET ช่วยให้สามารถปรับแต่งลายน้ำได้หลายวิธีรูปแบบข้อความ เช่น ตัวหนา ตัวเอียง ประเภทตัวอักษรพร้อมกับคุณสมบัติของรูปภาพ เช่น การหมุน ฯลฯ ช่วยเสริมกระบวนการทำลายน้ำ"

    # feature loop
    - title: "รองรับรูปแบบไฟล์ยอดนิยมทั้งหมด"
      content: "รูปแบบไฟล์และเอกสารจำนวนมากได้รับการสนับสนุนโดยโซลูชัน GroupDocs.Watermark PDF, Microsoft Office Word, Excel, PowerPoint รูปภาพเช่น JPEG, PNG, GIF, BMP, Visio ไดอะแกรม อีเมล ฯลฯ สามารถป้องกันด้วยลายน้ำของเรา"

    # feature loop
    - title: "ค้นหาและอัปเดตลายน้ำ"
      content: "ลายน้ำที่แสดงไว้ในเอกสารอาจพบและประมวลผลอีกครั้งแก้ไขข้อความ สไตล์ รูปภาพ หรือลบลายน้ำที่เปิดเผยโดยไม่ต้องใช้ความพยายามเป็นพิเศษ"

############################# Platforms ############################
platforms:
  enable: true
  title: "อิสระของแพลตฟอร์"
  description: "GroupDocs.Watermark for .NET รองรับระบบปฏิบัติการ เฟรมเวิร์ก และผู้จัดการแพ็คเกจที่ระบุไว้ด้านล่าง"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "รูปแบบไฟล์ที่รองรับ"
  description: |
    GroupDocs.Watermark for .NET ให้การประมวลผล [รูปแบบไฟล์] ต่อไปนี้ (https://docs.groupdocs.com/watermark/net/supported-document-formats/)
  groups:
    # group loop
    - color: "green"
      content: |
        ### รูปแบบ Microsoft Office และ OpenDocument
        * **Portable:** PDF 
        * **Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF
        * **Excel:** XLSX, XLS, XLT, XLTM, XLSB, XLSM
        * **PowerPoint:** PPTX, PPT, PPTM, POTX, POTM, PPSM, PPSX
        * **OpenDocument:** ODT, ODP, ODS
    # group loop
    - color: "blue"
      content: |
        ### รูปภาพและกราฟิก
        * **รูปแบบภาพยอดนิยม:** BMP, JPG, JPEG, PNG
        * **ภาพหลายหน้า:** GIF, WEBP, TIFF
      # group loop
    - color: "red"
      content: |
        ### อื่น ๆ
        * **Outlook:** EML, EMLX, MSG, OFT
        * **Microsoft Visio:** VSDX, VSTX, VSSX, VSDM, VSSM, VSTM, VSD, VDX, VSX, VTX, VSS, VST, VDW

############################# Features ############################
features:
  enable: true
  title: "คุณสมบัติ GroupDocs.Watermark"
  description: "ปกป้อง PDF, สำนักงาน, รูปภาพ และรูปแบบอื่น ๆ ด้วยลายน้ำ"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "เอกสารลายน้ำ"
      content: "เพิ่มหรือลบลายน้ำออกจากส่วนใดส่วนหนึ่งหรือเอกสารทั้งหมดของรูปแบบไฟล์ต่างๆ"

    # feature loop
    - icon: "watermark_style"
      title: "จัดแต่งลายน้ำของคุณ"
      content: "ปรับแต่งคุณสมบัติลายน้ำต่างๆเช่นสีแบบอักษรการหมุน ฯลฯ"

    # feature loop
    - icon: "hidden_print"
      title: "PDF ลายน้ำการพิมพ์ที่ซ่อนอยู่"
      content: "จัดสรรลายน้ำที่ซ่อนอยู่เป็น PDF ที่ปรากฏขึ้นเมื่อพิมพ์เอกสารเท่านั้น"

    # feature loop
    - icon: "image_only"
      title: "ลายน้ำเท่านั้นรูปภาพในเอกสาร"
      content: "ลายน้ำรูปภาพทั้งหมดในส่วนหน้า สไลด์ หรือเอกสารเฉพาะ"

    # feature loop
    - icon: "image_frame"
      title: "ประมวลผลกรอบภาพที่เลือก"
      content: "กำหนดลายน้ำให้เฉพาะเฟรมเฉพาะของภาพหลายกรอบ"

    # feature loop
    - icon: "attachments"
      title: "สิ่งที่แนบมาและรูปร่าง"
      content: "ตั้งค่าลายน้ำเป็นไฟล์แนบทั้งหมดในเอกสาร Excel และรูปร่างภาพทั้งหมดในสไลด์"

    # feature loop
    - icon: "pdf_objects"
      title: "PDF วัตถุ"
      content: "จัดตำแหน่งลายน้ำให้เป็นกล่องเลือดออก กล่องงานศิลปะ กล่องครอบตัด หรือกล่องตัดแต่งในเอกสาร PDF"

    # feature loop
    - icon: "doc_background"
      title: "พื้นหลังของเอกสาร"
      content: "วางลายน้ำหรือลบออกจากภาพพื้นหลังของสเปรดชีตหรือสไลด์"

    # feature loop
    - icon: "unreadable_characters"
      title: "การป้องกันตัวอักษรที่ไม่สามารถอ่านได้"
      content: "ปกป้องลายน้ำข้อความโดยใช้อักขระที่ไม่สามารถอ่านได้ในงานนำเสนอ"

    # feature loop
    - icon: "watermark_text_search"
      title: "ค้นหาลายน้ำในเอกสาร"
      content: "ค้นหาลายน้ำตามพารามิเตอร์ที่เฉพาะเจาะจงหรือโดยการรวมเกณฑ์หลายเกณฑ์"

    # feature loop
    - icon: "watermark_image_search"
      title: "ค้นหาลายน้ำภาพที่คล้ายกัน"
      content: "มองหาลายน้ำรูปภาพที่คล้ายกับภาพเฉพาะ"

    # feature loop
    - icon: "document_info"
      title: "รับข้อมูลเอกสาร"
      content: "แยกการตั้งค่าหน้าเว็บแบบโปรแกรมและข้อมูลอื่น ๆ สำหรับรูปแบบที่รองรับ"

############################# Code samples ############################
code_samples:
  enable: true
  title: "ตัวอย่างรหัส"
  description: "บางกรณีการใช้งานของการดำเนินการ GroupDocs.Watermark for .NET ทั่วไป"
  items:
    # code sample loop
    - title: "ลายน้ำโดยการเพิ่มรูปภาพลงในเอกสาร"
      content: |
        เพื่อปกป้องเอกสารใด ๆ คุณสามารถใช้ [ลายน้ำภาพ](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/):
        {{< landing/code title="วิธีป้องกันไฟล์ด้วยลายน้ำรูปภาพ">}}
        ```csharp {style=abap}
        // โหลดเอกสารต้นฉบับไปยัง Watermarker
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // ระบุเส้นทางไปยังภาพลายน้ำ
            using (ImageWatermark watermark = new ImageWatermark("watermark.jpg"))
            {
                // ปกป้องไฟล์และบันทึก
                watermarker.Add(watermark);

                watermarker.Save("result.pdf");
            }
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "ค้นหาและแก้ไขลายน้ำที่มีอยู่"
      content: |
        GroupDocs.Watermark สามารถ [แก้ไขลายน้ำ](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/) ที่นำเสนอไว้ในเอกสารแล้วค้นหารายการที่ต้องการและอัปเดตคุณสมบัติ
        {{< landing/code title="การค้นหาและแก้ไขลายน้ำ">}}
        ```csharp {style=abap}   
        // โหลดเอกสารต้นทาง
        using (Watermarker watermarker = new Watermarker("document.pdf"))
        {
            // ค้นหาลายน้ำที่จะอัปเดต
            TextSearchCriteria searchCriteria = new TextSearchCriteria("test", false);
            PossibleWatermarkCollection watermarks = watermarker.Search(searchCriteria);
            foreach (PossibleWatermark watermark in watermarks)
            {
                // อัปเดตคุณสมบัติที่ต้องการ
                watermark.Text = "New Text";
            }

            // บันทึกเอกสารที่แก้ไขไปยังเส้นทางที่ระบุ
            watermarker.Save("document.pdf");
        }
        ```
        {{< /landing/code >}}

---
