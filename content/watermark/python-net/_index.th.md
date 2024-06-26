---
############################# Static ############################
layout: "landing"
date: 2024-06-26T07:20:49
draft: false

lang: th
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

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
    # supported_platforms loop
    - title: "Python"
      tag: "python-net"

############################# Head ############################
head_title: "Python ไลบรารีลายน้ำ | ลายน้ำเอกสาร"
head_description: "Python ปกป้องเอกสารทางธุรกิจด้วยลายน้ำข้อความและรูปภาพ รองรับรูปแบบไฟล์เช่น PDF, Word, Excel และ PowerPoint"

############################# Header ############################
title: "เข้าถึงเทคโนโลยีลายน้ำของ Python via .NET"
description: "ปกป้องข้อมูลของคุณและป้องกันการคัดลอกโดยไม่ได้รับอนุญาตด้วยโซลูชัน Python นี้ เพิ่มลายน้ำให้กับเอกสารทางธุรกิจในรูปแบบต่าง ๆ ได้อย่างง่ายดาย รวมถึง PDF, Word, Excel, PowerPoint, รูปภาพ ฯลฯ"
words:
  for: "สำหรับ"

actions:
  main: "PyPi ดาวน์โหลดฟรี"
  main_link: "https://pypi.org/project/groupdocs-watermark-net/"
  alt: "การออกใบอนุญาต"
  alt_link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
  title: "พร้อมที่จะเริ่มแล้วหรือยัง?"
  description: "ลองใช้คุณสมบัติ GroupDocs.Watermark ฟรีหรือขอใบอนุญาต"

release:
  title: "เวอร์ชัน {0} เผยแพร่"
  notes: "ดูว่ามีอะไรใหม่"
  downloads: "ดาวน์โหลด"
  link: "https://releases.groupdocs.com/watermark/python-net/"

code:
  title: "เพิ่มลายน้ำให้กับ PDF โดยใช้ Python"
  more: "ตัวอย่างเพิ่มเติม"
  more_link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
  install: "pip install groupdocs-watermark-net"
  content: |
    ```python {style=abap}

    import groupdocs.watermark as gw
    import groupdocs.watermark.watermarks as gww
    import groupdocs.watermark.options.pdf as gwop
    import groupdocs.watermark.common as gwc

    # ใช้เครื่องหมายน้ำแบบทันทีที่ผ่านเส้นทาง PDF
    pdf_lo = gwop.PdfLoadOptions()
    with gw.Watermarker("source.pdf", pdf_lo) as watermarker:
        options = gwop.PdfArtifactWatermarkOptions()

        # ปรับแต่งตัวเลือกลายน้ำ
        text_watermark = 
            gww.TextWatermark("Approved", gww.Font("Arial", 8.0))
        text_watermark.horizontal_alignment = 
            gwc.HorizontalAlignment.RIGHT

        # ใช้ลายน้ำกับเอกสาร PDF
        watermarker.add(text_watermark, options)

        # บันทึกเอกสารผลลัพธ์
        watermarker.save("result.pdf")

    ```

############################# Overview ############################
overview:
  enable: true
  title: "สรุปภาพ GroupDocs.Watermark"
  description: "Python ไลบรารีสำหรับลายน้ำ"
  features:
    # feature loop
    - title: "Python ลายน้ำเอกสาร"
      content: "รักษาความปลอดภัยข้อมูลที่ละเอียดอ่อนของคุณด้วย GroupDocs.Watermark for Python via .NET ใส่ข้อความหรือรูปภาพลงในไฟล์รูปแบบต่างๆเป็นลายน้ำ"

    # feature loop
    - title: "ปรับแต่งลายน้ำ"
      content: "ตัวเลือกการปรับแต่งมากมายมีอยู่ใน GroupDocs.Watermark for Python via .NET ตั้งค่าลักษณะข้อความ (ตัวหนา ตัวเอียง แบบอักษร) หรือคุณสมบัติของรูปภาพ เช่น ขนาดหรือการหมุน เพื่อปรับแต่งลายน้ำในเอกสาร"

    # feature loop
    - title: "รองรับรูปแบบไฟล์ยอดนิยม"
      content: "GroupDocs.Watermark for Python via .NET รองรับรูปแบบไฟล์ที่หลากหลาย รวมถึง PDF, เอกสาร MS Office เช่น Word, Excel, PowerPoint และรูปภาพ เช่น JPEG, PNG, GIF, BMP, ไดอะแกรม Visio, อีเมล ฯลฯ เพิ่มประสิทธิภาพการประมวลผลเอกสารให้ตอบโจทย์ธุรกิจ เป้าหมาย"

    # feature loop
    - title: "ค้นหาและอัปเดตลายน้ำ"
      content: "ดึงและอัปเดตลายน้ำที่วางอยู่ในเอกสาร แก้ไขรูปแบบข้อความ เนื้อหารูปภาพ หรือลบออกทั้งหมด GroupDocs.Watermark for Python via .NET นำเสนอความสามารถในการประมวลผลลายน้ำที่หลากหลาย"

############################# Platforms ############################
platforms:
  enable: true
  title: "อิสระของแพลตฟอร์"
  description: "GroupDocs.Watermark for Python via .NET ทำงานร่วมกับระบบปฏิบัติการและตัวจัดการแพ็คเกจต่างๆ ได้อย่างราบรื่น"
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "รูปแบบไฟล์ที่รองรับ"
  description: |
    GroupDocs.Watermark for Python via .NET ช่วยให้คุณสามารถประมวลผลรูปแบบไฟล์ที่หลากหลาย [สำรวจรายการทั้งหมด](https://docs.groupdocs.com/watermark/net/supported-document-formats/)
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
  title: "คุณลักษณะของ GroupDocs.Watermark for Python via .NET"
  description: "เสริมสร้างความปลอดภัยของเอกสารผ่านลายน้ำแบบเป็นโปรแกรม ประมวลผลรูปแบบไฟล์ที่หลากหลาย รวมถึง PDF, DOCX, XLSX, PPTX และรูปแบบรูปภาพ (PNG, JPG ฯลฯ)"

  items:
    # feature loop
    - icon: "watermark_add"
      title: "การควบคุมลายน้ำที่แม่นยำ"
      content: "จัดการลายน้ำได้อย่างแม่นยำโดยการเพิ่มหรือลบลายน้ำออกจากส่วนเฉพาะ เอกสารทั้งหมด หรือไฟล์แนบและรูปร่างแต่ละรายการภายในรูปแบบไฟล์ที่แตกต่างกัน"

    # feature loop
    - icon: "watermark_style"
      title: "ปรับแต่งลักษณะลายน้ำ"
      content: "ควบคุมความสวยงามของลายน้ำอย่างละเอียดโดยการปรับเปลี่ยนคุณลักษณะ เช่น สี แบบอักษร ความทึบ การหมุน และการวางตำแหน่งภายในเอกสาร"

    # feature loop
    - icon: "hidden_print"
      title: "พิมพ์ลายน้ำ PDF"
      content: "เพิ่มลายน้ำที่ซ่อนอยู่ในเอกสารปกติซึ่งจะมองเห็นได้ในระหว่างขั้นตอนการพิมพ์เท่านั้น ช่วยเพิ่มความปลอดภัยของเอกสารอย่างรอบคอบ"

    # feature loop
    - icon: "image_only"
      title: "ลายน้ำภาพเฉพาะ"
      content: "ใส่ลายน้ำรูปภาพเฉพาะภายในเอกสารโดยใช้โซลูชันของเรา ฝังลายน้ำในส่วนที่กำหนด (เช่น หน้า สไลด์) หรือทั่วทั้งเอกสาร"

    # feature loop
    - icon: "image_frame"
      title: "ลายน้ำภาพหลายชั้น"
      content: "เพิ่มลายน้ำอย่างแม่นยำให้กับเฟรมที่ต้องการภายในรูปแบบภาพหลายเฟรม ช่วยให้สามารถควบคุมการวางตำแหน่งลายน้ำได้อย่างละเอียด"

    # feature loop
    - icon: "attachments"
      title: "การปกป้องเนื้อหาที่ครอบคลุม"
      content: "ขยายการป้องกันไปยังองค์ประกอบเอกสารต่างๆ เช่น ไฟล์แนบภายในเอกสาร Excel และรูปร่างของรูปภาพภายในงานนำเสนอ ซึ่งช่วยเพิ่มระดับความปลอดภัยอีกชั้นหนึ่ง"

    # feature loop
    - icon: "pdf_objects"
      title: "ลายน้ำ PDF ขั้นสูง"
      content: "ลายน้ำบนพื้นที่ต่างๆ ของ PDF รวมถึง Bleed Box, Art Box, Crop Box, Trim Box ฯลฯ"

    # feature loop
    - icon: "doc_background"
      title: "ลายน้ำภาพพื้นหลัง"
      content: "จัดการลายน้ำภายในภาพพื้นหลังของสเปรดชีตและงานนำเสนอ โดยเสนอตัวเลือกการปรับแต่งเพิ่มเติมสำหรับมาตรการรักษาความปลอดภัยด้วยภาพ"

    # feature loop
    - icon: "unreadable_characters"
      title: "ลายน้ำข้อความที่มีอักขระที่อ่านไม่ได้"
      content: "ใช้อักขระที่อ่านไม่ได้ภายในลายน้ำข้อความที่ฝังอยู่ในงานนำเสนอ เพิ่มความปลอดภัยโดยการทำให้การแยกลายน้ำโดยไม่ได้รับอนุญาตมีความท้าทายมากขึ้นอย่างมาก"

    # feature loop
    - icon: "watermark_text_search"
      title: "การค้นหาลายน้ำขั้นสูง"
      content: "ใช้คุณลักษณะการค้นหาที่ครอบคลุมเพื่อค้นหาลายน้ำในเอกสารตามพารามิเตอร์เฉพาะหรือโดยการรวมเกณฑ์ต่างๆ"

    # feature loop
    - icon: "watermark_image_search"
      title: "การตรวจจับลายน้ำภาพที่คล้ายกัน"
      content: "ค้นหารูปภาพลายน้ำที่คล้ายกันภายในเอกสารที่มีลักษณะคล้ายกับรูปภาพต้นฉบับ"

    # feature loop
    - icon: "document_info"
      title: "วิเคราะห์ข้อมูลเอกสาร"
      content: "แยกข้อมูลเอกสารที่จำเป็น เช่น การตั้งค่าหน้าเพื่อการวิเคราะห์เพิ่มเติม"

############################# Code samples ############################
code_samples:
  enable: true
  title: "ตัวอย่างรหัส"
  description: "สำรวจตัวอย่างโค้ดที่แสดงฟังก์ชันการทำงานทั่วไปของ GroupDocs.Watermark for Python via .NET"
  items:
    # code sample loop
    - title: "ลายน้ำเอกสารด้วยรูปภาพ"
      content: |
        ใช้ GroupDocs.Watermark for Python via .NET เพื่อปกป้องเอกสารโดยการเพิ่มลายน้ำรูปภาพ [เรียนรู้เพิ่มเติม](https://docs.groupdocs.com/watermark/net/adding-image-watermarks/#add-image-watermark-from-local-file/)
        {{< landing/code title="วิธีป้องกันไฟล์ด้วยลายน้ำรูปภาพ">}}
        ```python {style=abap}

        # โหลดเอกสารต้นฉบับไปยัง Watermarker
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # ระบุเส้นทางไปยังภาพลายน้ำ
            watermark = groupdocs.watermark.watermarks.ImageWatermark("watermark.jpg")
            watermark.horizontal_alignment = groupdocs.watermark.common.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwgroupdocs.watermark.common.VerticalAlignment.CENTER

            # ปกป้องไฟล์และบันทึก
            watermarker.add(watermark)
            watermarker.save("result.pdf")
       
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "ค้นหาและแก้ไขลายน้ำที่มีอยู่"
      content: |
        GroupDocs.Watermark for Python via .NET ช่วยให้คุณจัดการลายน้ำในเอกสารได้ เลือกลายน้ำและแก้ไขคุณสมบัติ [ค้นพบวิธีการ](https://docs.groupdocs.com/watermark/net/modifing-found-watermark-properties/#replacing-text/)
        {{< landing/code title="การค้นหาและแก้ไขลายน้ำ">}}
        ```python {style=abap}

        # โหลดเอกสารต้นทาง
        with groupdocs.watermark.Watermarker("document.pdf") as watermarker:

            # ค้นหาลายน้ำที่จะอัปเดต
            search_criteria = groupdocs.watermark.search.searchcriteria.TextSearchCriteria("annotation", False)
            watermarks = watermarker.search(search_criteria)
            
            # อัปเดตคุณสมบัติที่ต้องการ
            for watermark in watermarks:
                watermark.text = "passed"

            # บันทึกเอกสารที่แก้ไขไปยังเส้นทางที่ระบุ
            watermarker.save("result.pdf")


        ```
        {{< /landing/code >}}

---
