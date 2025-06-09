
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:15
draft: false
lang: th
format: Image
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "เพิ่มลายน้ำให้กับภาพด้วย Python"
head_description: "เรียนรู้วิธีเพิ่มลายน้ำให้กับภาพใน Python ปกป้องภาพถ่ายของคุณโดยไม่สูญเสียคุณภาพ"

############################# Header ############################
title: "การเพิ่มลายน้ำภาพอย่างรวดเร็วด้วย Python" 
description: "เครื่องมือ Python ของเราช่วยให้คุณเพิ่มลายน้ำให้กับภาพได้อย่างรวดเร็ว รองรับหลายรูปแบบ ตั้งแต่ภาพถ่ายไปจนถึงศิลปะดิจิทัล"
subtitle: "GroupDocs.Watermark for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลด PyPi ฟรี"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET"
    link: "/watermark/python-net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       GroupDocs.Watermark for Python via .NET ช่วยให้คุณเพิ่มลายน้ำในภาพใน Python รองรับ JPEG, PNG, BMP, TIFF และอีกมากมาย คุณสามารถปรับความโปร่งใส ขนาด และตำแหน่งของลายน้ำให้เหมาะสมตามต้องการ ใช้เพื่อปกป้องภาพหรือเพิ่มการสร้างแบรนด์ โดยไม่สูญเสียคุณภาพต้นฉบับ

############################# Steps ############################
steps:
    enable: true
    title: "เพิ่มลายน้ำอย่างง่าย: การเพิ่มลายน้ำด้วย Python สำหรับ Image"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** เป็นไลบรารีที่ช่วยให้คุณสามารถเพิ่มลายน้ำในหลายประเภทไฟล์ธุรกิจได้อย่างรวดเร็ว ปฏิบัติตามขั้นตอนเหล่านี้เพื่อเพิ่มลายน้ำในเอกสารของคุณใน Python:
      
      1. **เริ่มต้นกับลายน้ำ:** เริ่มด้วยการสร้างตัวอย่างของคลาส **Watermarker** ส่งไฟล์ Image ของคุณ (เป็นพาธหรือสตรีม) ไปยังคอนสตรัคเตอร์เพื่อเปิดสำหรับการเพิ่มลายน้ำ
      2. **สร้างลายน้ำของคุณ:** สร้างวัตถุลายน้ำ **Watermark** พร้อมข้อความและการตั้งค่าที่คุณต้องการ คุณสามารถเพิ่มลายน้ำไปยังหน้าใดก็ได้หรือแม้แต่ไปยังองค์ประกอบเอกสารเช่นหัวเรื่องหรือไฟล์แนบ
      3. **ปรับแต่งลายน้ำ:** ปรับขนาด ตำแหน่ง ฟอนต์ สี และการจัดตำแหน่งของลายน้ำให้เหมาะสมตามต้องการ นี่จะช่วยให้ลายน้ำดูดีในเอกสารของคุณ
      4. **นำไปใช้และบันทึก:** ใช้เมธอด **Watermarker** เพื่อนำลายน้ำของคุณไปใช้ในเอกสาร บันทึกผลลัพธ์ โดยปกติให้บันทึกเป็นไฟล์ใหม่เพื่อความปลอดภัย
   
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
        # เพิ่มลายน้ำข้อความลงในไฟล์ IMAGE
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.common as gwс

        # เลือกไฟล์ที่คุณต้องการเพิ่มลายน้ำ
        with gw.Watermarker("input.jpeg") as watermarker:

            # สร้างวัตถุลายน้ำข้อความ
            font = gww.Font("Arial", 36.0)
            watermark = gww.TextWatermark("top secret", font)
            watermark.foreground_color = gww.Color.red
            watermark.horizontal_alignment = gwс.HorizontalAlignment.CENTER
            watermark.vertical_alignment = gwс.VerticalAlignment.CENTER
            watermark.opacity = 0.4

            watermarker.add(watermark)

            # บันทึกไฟล์ IMAGE ที่อัปเดตแล้ว
            watermarker.save("output.jpeg")
        ```            


############################# More features ############################
more_features:
  enable: true
  title: "สำรวจฟีเจอร์การเพิ่มลายน้ำเพิ่มเติม"
  description: "ใช้ API Python ของเราเพื่อเพิ่ม ดู แปลง และจัดการลายน้ำในเอกสาร สไลด์ แผนภาพ และอื่นๆ GroupDocs.Watermark for Python via .NET ช่วยให้คุณปกป้องไฟล์และเพิ่มข้อมูลลิขสิทธิ์ได้อย่างรวดเร็ว"
  image: "/img/watermark/features_add.webp" # 500x500 px
  image_description: "เพิ่มลายน้ำ"
  features:
    # feature loop
    - title: "เพิ่มลายน้ำได้อย่างรวดเร็ว"
      content: "GroupDocs.Watermark อนุญาตให้ผู้พัฒนา Python สามารถเพิ่มลายน้ำข้อความ รูปภาพ หรือแบบไดนามิกลงในเอกสารทางธุรกิจได้อย่างรวดเร็ว รักษาความปลอดภัยและภาพลักษณ์ของไฟล์ด้วยความพยายามน้อยที่สุด"

    # feature loop
    - title: "ลายน้ำที่ปรับแต่งได้ทั้งหมด"
      content: "เปลี่ยนขนาดลายน้ำ การหมุน ความโปร่งใส สี และฟอนต์ได้ด้วย GroupDocs.Watermark ทำให้ลายน้ำของคุณพอดีกับเอกสารของคุณและเก็บเนื้อหาสำคัญไว้อย่างชัดเจน"

    # feature loop
    - title: "ใช้ฟีเจอร์เอกสารสำหรับการเพิ่มลายน้ำ"
      content: "ใช้ประโยชน์จากฟีเจอร์เอกสารในตัว เช่น หมายเหตุ PDF พื้นหลัง Word หรือหัวเรื่อง Excel เพื่อเพิ่มลายน้ำ GroupDocs.Watermark ทำงานร่วมกับโครงสร้างของเอกสารเพื่อการเพิ่มลายน้ำที่มีประสิทธิภาพและไม่รบกวน"
      
  code_samples:
    # code sample loop
    - title: "เพิ่มลายน้ำรูปภาพลงใน DOCX"
      content: |
        ตัวอย่างนี้แสดงวิธีการใช้เอฟเฟกต์รูปภาพกับลายน้ำรูปทรง
        {{< landing/code title="Python">}}
        ```python {style=abap}
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.options as gwo
        import groupdocs.watermark.options.wordprocessing as gwow

        # เปิดเอกสาร Word
        load_options = gwow.WordProcessingLoadOptions()
        with gw.Watermarker("source.docx", load_options) as watermarker:

            # ตั้งค่าตัวเลือกลายน้ำ
            with gww.ImageWatermark("logo.png") as watermark:

                effects = gwow.WordProcessingImageEffects()
                effects.brightness = 0.7
                effects.contrast = 0.6
                effects.chroma_key = gww.Color.red

                options = gwow.WordProcessingWatermarkSectionOptions()
                options.Effects = effects;

                # สร้างลายน้ำ
                watermarker.add(watermark, options)

                # บันทึกเอกสารพร้อมลายน้ำ
                watermarker.save("result.docx")
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
    title: "เพิ่มลายน้ำให้กับภาพด้วย Python"
    exclude: "IMAGE"
    description: "ปกป้องภาพของคุณด้วยชุดเครื่องมือ Python ของเรา เพิ่มลายน้ำให้กับหลายรูปแบบภาพได้อย่างรวดเร็ว"
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