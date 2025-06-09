
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:28
draft: false
lang: th
format: Tiff
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "เพิ่มลายน้ำใน TIFF ด้วย Python"
head_description: "สร้างและเพิ่มลายน้ำในภาพ TIFF ใน Python เพื่อปกป้องไฟล์ดิจิทัลของคุณ"

############################# Header ############################
title: "สร้างลายน้ำสำหรับ TIFF ด้วย Python" 
description: "เพิ่มลายน้ำที่แข็งแรงและกำหนดเองในไฟล์ TIFF ใน Python — เหมาะสำหรับการจัดทำเอกสารดิจิทัลและช่างภาพ"
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดฟรีที่ PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET เป็นเครื่องมือ Python สำหรับการเพิ่มลายน้ำในไฟล์ TIFF เลือกลายน้ำข้อความหรือภาพ ตั้งค่าความโปร่งแสง ขนาด และตำแหน่ง และเก็บรักษาภาพของคุณให้ปลอดภัย ด้วยฟีเจอร์การเลเยอร์ลายน้ำและการจัดรูปแบบอย่างชาญฉลาด GroupDocs.Watermark เป็นเครื่องมือที่จำเป็นสำหรับผู้ที่ต้องการปกป้องคลังภาพของตน

############################# Steps ############################
steps:
    enable: true
    title: "เพิ่มลายน้ำลงในไฟล์ Tiff อย่างรวดเร็ว"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/):** ไลบรารี Python ที่ทรงพลังที่ช่วยให้คุณสามารถเพิ่มลายน้ำลงในเอกสารได้
      
      1. **คลาสหลัก: Watermarker.** เริ่มโดยการสร้างวัตถุ **Watermarker** โดยให้ไฟล์ Tiff ของคุณเป็นพาธไฟล์หรือสตรีม
      2. **สร้างลายน้ำของคุณ.** ต่อไป สร้างวัตถุ Watermark ประเภทที่คุณต้องการ คุณสามารถวางมันบนหน้าใดก็ได้หรือแม้กระทั่งในองค์ประกอบเอกสาร เช่น รูปภาพหรือหัวข้อ
      3. **ปรับแต่งรูปลักษณ์.** ตั้งค่าขนาด ตำแหน่ง ฟอนต์ และสีของลายน้ำให้ตรงตามความต้องการของคุณ
      4. **เพิ่มและบันทึก.** ใช้เมธอด **Watermarker** เพื่อนำลายน้ำของคุณไปใส่ เพิ่มได้ตามต้องการ แล้วบันทึกไฟล์ไปที่ที่ที่คุณต้องการ
   
    code:
      platform: "python-net"
      copy_title: "คัดลอก"
      install:
        command: |
        command: "pip install groupdocs-watermark-net"
        copy_tip: "คลิกเพื่อคัดลอก"
        copy_done: "คัดลอก"
      links:
        #  loop
        - title: "ตัวอย่างเพิ่มเติม"
          link: "https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET/"
        #  loop
        - title: "เอกสาร"
          link: "https://docs.groupdocs.com/watermark/python-net/"
          
      content: |
        ```python {style=abap}
        # เพิ่มลายน้ำภาพลงในไฟล์ TIFF
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # ส่งพาธไฟล์ไปยังตัวสร้าง Watermarker
        with gw.Watermarker("input.tiff") as watermarker:

            # สร้างลายน้ำภาพโดยใช้ไฟล์ภาพของคุณ
            watermark = gww.ImageWatermark("watermark.png")

            watermarker.add(watermark)

            # บันทึกไฟล์ TIFF ที่มีลายน้ำ
            watermarker.save("output.tiff")
        ```  

############################# More features ############################
more_features:
  enable: true
  title: "ค้นพบเครื่องมือการทำลายน้ำเพิ่มเติม"
  description: "GroupDocs.Watermark for Python via .NET มอบตัวเลือกขั้นสูงสำหรับการเพิ่มและกำหนดค่าลายน้ำในหลายประเภทไฟล์ ปกป้องเอกสารและภาพของคุณด้วยฟีเจอร์ที่ยืดหยุ่นและใช้งานง่าย"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "เครื่องมือทำลายน้ำแบบครบวงจร"
  features:
    # feature loop
    - title: "การปูพื้นเต็มหน้า"
      content: "ครอบคลุมเอกสารทั้งหมดด้วยลายน้ำที่ปูพื้น ทำให้ลายน้ำยากต่อการลบและปกป้องไฟล์ของคุณโดยไม่ทำให้รูปแบบเสีย"

    # feature loop
    - title: "สีที่ปรับแต่งได้"
      content: "เลือกสีใดก็ได้สำหรับลายน้ำของคุณให้ตรงกับแบรนด์หรือสไตล์เอกสารของคุณ ทำให้ลายน้ำของคุณโดดเด่นหรือกลมกลืนตามต้องการ"

    # feature loop
    - title: "ตัวเลือกความปลอดภัยเพิ่มเติม"
      content: "เพิ่มความปลอดภัยให้เอกสารของคุณด้วยลายน้ำหลายชั้น รวมลายน้ำที่มองเห็นได้และซ่อนไว้เพื่อป้องกันการคัดลอกและให้แน่ใจว่ามีแค่คนที่ถูกต้องเข้าถึงไฟล์ของคุณ"
      
  code_samples:
    # code sample loop
    - title: "เพิ่มลายน้ำลงใน PowerPoint"
      content: |
        ตัวอย่างนี้แสดงให้เห็นถึงวิธีการวางลายน้ำในพื้นหลังของสไลด์ PPTX
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.presentation as gwop

        # เปิดไฟล์ PPTX
        load_options = gwop.PresentationLoadOptions()
        with gw.Watermarker("source.pptx", load_options) as watermarker:

            # ตั้งค่ารายละเอียดลายน้ำ
            with TextWatermark("Protected image", gww.Font("Arial", 8.0)) as watermark:

                watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
                watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
                watermark.rotate_angle = 45
                watermark.scale_factor = 1

                # ใช้ลายน้ำกับพื้นหลังของสไลด์
                watermarker.add(watermark)

                # บันทึกการนำเสนอที่ปรับปรุงแล้ว
                watermarker.save("result.pptx")
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "พร้อมที่จะเริ่มแล้วหรือยัง?"
  description: "ลองใช้คุณสมบัติ GroupDocs.Watermark ฟรีหรือขอใบอนุญาต"
  items:
    #  loop
    - title: "PyPi ดาวน์โหลด"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      color: "red"
        #  loop
    - title: "การออกใบอนุญาต"
      link: "https://purchase.groupdocs.com/pricing/watermark/python-net/"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "รักษาความปลอดภัยภาพ TIFF ด้วยลายน้ำ Python"
    exclude: "TIFF"
    description: "เพิ่มและจัดการลายน้ำในไฟล์ TIFF ใน Python เพื่อปกป้องภาพของคุณและควบคุมงานสร้างสรรค์ของคุณ"
    items: 
        # format loop 1
        - name: "ลายน้ำ PDF"
          format: "PDF"
          link: "/watermark/python-net/add//pdf/"
          description: "รูปแบบเอกสาร Adobe Portable"

        # format loop 2
        - name: "ลายน้ำ Word"
          format: "WORD"
          link: "/watermark/python-net/add//word/"
          description: "MS Word และเอกสาร Open Office"
          
        # format loop 3
        - name: "ลายน้ำ Excel"
          format: "EXCEL"
          link: "/watermark/python-net/add//excel/"
          description: "MS Excel และสเปรดชีตโอเพ่นออฟฟิศ"

        # format loop 4
        - name: "ภาพลายน้ำ"
          format: "IMAGE"
          link: "/watermark/python-net/add//image/"
          description: "รูปแบบภาพยอดนิยม"

        # format loop 5
        - name: "ภาพลายน้ำ"
          format: "PHOTO"
          link: "/watermark/python-net/add//photo/"
          description: "รูปแบบภาพถ่าย"

        # format loop 6
        - name: "ลายน้ำ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/add//powerpoint/"
          description: "MS PowerPoint และงานนำเสนอแบบโอเพ่นออฟฟิศ"

        # format loop 7
        - name: "ลายน้ำ DOCX"
          format: "DOCX"
          link: "/watermark/python-net/add//docx/"
          description: "ไมโครซอฟท์ Word เปิดเอกสาร XML"
          
        # format loop 8
        - name: "ลายน้ำ PPTX"
          format: "PPTX"
          link: "/watermark/python-net/add//pptx/"
          description: "PowerPoint เปิดการนำเสนอ XML"
          
        # format loop 9
        - name: "ลายน้ำ XLSX"
          format: "XLSX"
          link: "/watermark/python-net/add//xlsx/"
          description: "ไมโครซอฟท์ Excel เปิดสเปรดชีต XML"

        # format loop 10
        - name: "ลายน้ำ JPEG"
          format: "JPEG"
          link: "/watermark/python-net/add//jpeg/"
          description: "JPEG รูปภาพ"

        # format loop 11
        - name: "ลายน้ำ PNG"
          format: "PNG"
          link: "/watermark/python-net/add//png/"
          description: "Portable กราฟิกเครือข่าย"

        # format loop 12
        - name: "ลายน้ำ TIFF"
          format: "TIFF"
          link: "/watermark/python-net/add//tiff/"
          description: "รูปแบบไฟล์รูปภาพแท็ก"

        # format loop 13
        - name: "ลายน้ำ WEBP"
          format: "WEBP"
          link: "/watermark/python-net/add//webp/"
          description: "รูปภาพเว็บ"

        # format loop 14
        - name: "ลายน้ำ DOC"
          format: "DOC"
          link: "/watermark/python-net/add//doc/"
          description: "ไมโครซอฟท์ Word 97 - เอกสาร 2007"

        # format loop 15
        - name: "ลายน้ำ XLS"
          format: "XLS"
          link: "/watermark/python-net/add//xls/"
          description: "ไมโครซอฟท์ Excel สมุดงาน 97-2003"

        # format loop 16
        - name: "ลายน้ำ PPT"
          format: "PPT"
          link: "/watermark/python-net/add//ppt/"
          description: "PowerPoint การนำเสนอ 97-2003"

        # format loop 17
        - name: "ลายน้ำ RTF"
          format: "RTF"
          link: "/watermark/python-net/add//rtf/"
          description: "รูปแบบข้อความที่หลากหลาย"

---