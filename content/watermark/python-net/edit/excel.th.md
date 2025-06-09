
---
############################# Static ############################
layout: "format"
date:  2025-06-09T18:08:16
draft: false
lang: th
format: Excel
product: "Watermark"
product_tag: "watermark"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "แก้ไขลายน้ำในไฟล์ Excel"
head_description: "ด้วย GroupDocs.Watermark for Python via .NET คุณสามารถปรับการตั้งค่าลายน้ำเพื่อปกป้องและปรับแต่งเอกสารของคุณ."

############################# Header ############################
title: "อัปเดตลายน้ำในสเปรดชีต Excel โดยใช้ Python" 
description: "ปกป้องสเปรดชีต Excel ของคุณด้วยเครื่องมือแก้ไขลายน้ำที่ยืดหยุ่นของเรา."
subtitle: "GroupDocs.Watermark for Python via .NET API" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดฟรีที่ PyPi"
      link: "https://releases.groupdocs.com/watermark/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for Python via .NET ไลบรารี"
    link: "/watermark/python-net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       **แก้ไขลายน้ำใน Excel ได้อย่างรวดเร็ว:** GroupDocs.Watermark for Python via .NET มอบเครื่องมือทั้งหมดที่จำเป็นสำหรับนักพัฒนา Python ในการจัดการลายน้ำอย่างมีประสิทธิภาพ ยกระดับกระบวนการทำงานเอกสารและความปลอดภัยของคุณ.

############################# Steps ############################
steps:
    enable: true
    title: "แก้ไขลายน้ำในเอกสาร Excel ด้วย Python"
    content: |
      **[GroupDocs.Watermark for Python via .NET](https://products.groupdocs.com/watermark/python-net/)** ช่วยนักพัฒนา Python ในการอัปเดตลายน้ำในไฟล์ Excel ต่างๆ อย่างมีประสิทธิภาพ นี่คือวิธีการใช้ในโปรเจคของคุณ:
      
      1. เริ่มต้นด้วยการเปิดไฟล์ Excel ของคุณโดยการส่งไปยังตัวสร้าง **Watermarker** คุณสามารถใช้ที่อยู่ไฟล์ สตรีมไบต์ หรือสตรีมไฟล์ได้.
      2. จากนั้น ค้นหาลายน้ำที่คุณต้องการเปลี่ยนโดยใช้ **SearchCriteria** ซึ่งจะช่วยให้คุณค้นหาข้อความหรือลักษณะของลายน้ำ.
      3. เมื่อพบแล้ว คุณสามารถเปลี่ยนรายละเอียดต่างๆ เช่น ข้อความ ฟอนต์ ขนาด ตำแหน่ง สี และอื่นๆ นี่จะทำให้คุณควบคุมรูปลักษณ์ของลายน้ำได้เต็มที่.
      4. หลังจากทำการเปลี่ยนแปลงแล้ว ให้บันทึกเอกสาร คุณสามารถเขียนผลลัพธ์ลงไปยังสตรีมหรือที่อยู่ไฟล์.
   
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
        # อัปเดตข้อความลายน้ำใน EXCEL
        import groupdocs.watermark as gw
        import groupdocs.watermark.search.searchcriteria as gwss

        # สร้าง Watermarker โดยใช้ไฟล์ EXCEL
        with gw.Watermarker("input.xslx") as watermarker:

            # ตั้งค่า TextSearchCriteria เพื่อค้นหาข้อความลายน้ำ
            search_criteria = gwss.TextSearchCriteria("test", False)

            possible_watermarks = watermarker.search(search_criteria)
                for watermark in possible_watermarks:
                    try:
                        # แก้ไขข้อความลายน้ำ
                        watermark.text = "passed"
                    except Exception as e:
                        pass
            
            watermarker.save("output.xslx")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ค้นพบวิธีการเพิ่มเติมในการอัปเดตลายน้ำ"
  description: "ด้วยไลบรารีของเรา Python แอพสามารถเพิ่ม ค้นหา แก้ไข หรือ ลบลายน้ำในหลายประเภทไฟล์."
  image: "/img/watermark/features_edit.webp" # 500x500 px
  image_description: "การแก้ไขลายน้ำ"
  features:
    # feature loop
    - title: "ทำลายน้ำในไฟล์ของคุณได้อย่างมีประสิทธิภาพ"
      content: "ใช้ GroupDocs.Watermark for Python via .NET ในการเพิ่มและจัดการลายน้ำในเอกสารของคุณ ค้นหา อัปเดต หรือ ลบลายน้ำตามต้องการด้วย API ที่เรียบง่าย."

    # feature loop
    - title: "ปรับแต่งลายน้ำให้เหมาะกับความต้องการของคุณ"
      content: "ปรับการตั้งค่าลายน้ำ เช่น ฟอนต์ ขนาด ทิศทาง และสี โดยใช้ API ที่ยืดหยุ่นเพื่อให้ได้ผลลัพธ์ที่คุณต้องการ."

    # feature loop
    - title: "ใช้คุณลักษณะเฉพาะของรูปแบบไฟล์"
      content: "ขึ้นอยู่กับรูปแบบไฟล์ คุณสามารถใช้คุณลักษณะเฉพาะเช่น ส่วนหัว ส่วนท้าย หมายเหตุ หรือพื้นที่พื้นหลังเป็นเขตลายน้ำ."
      
  code_samples:
    # code sample loop
    - title: "แก้ไขข้อความลายน้ำใน Excel"
      content: |
        โค้ดนี้แสดงวิธีเปลี่ยนข้อความลายน้ำในสเปรดชีต Excel.
        {{< landing/code title="Python">}}
        ```python {style=abap}
        # เปิดไฟล์ XLSX
        import groupdocs.watermark as gw
        import groupdocs.watermark.watermarks as gww
        import groupdocs.watermark.search.searchcriteria as gwss
        import groupdocs.watermark.options.spreadsheet as gwos

        # อ่านข้อมูลสเปรดชีต
        with gw.Watermarker("source.xlsx") as watermarker:

            search_criteria = gwss.TextSearchCriteria("test", False)
            search_criteria.pages = [1,3]

            # เปลี่ยนข้อความลายน้ำ
            watermarks = watermarker.search(search_criteria)
            for watermark in watermarks:
                try:
                    watermark.formatted_text_fragments.clear()
                    watermark.formatted_text_fragments.add(
                       "passed", 
                        gww.Font("Calibri", 19.0, gww.FontStyle.bold), 
                        gww.Color.red, 
                        gww.Color.aqua
                    )
                except Exception as e:
                    pass
        
            # บันทึกผลลัพธ์
            watermarker.save("output.xlsx")
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
    title: "อัปเดตลายน้ำในรูปแบบอื่นๆ"
    exclude: "EXCEL"
    description: "ปรับแต่งการตั้งค่าลายน้ำได้อย่างสะดวกในหลายรูปแบบไฟล์โดยใช้ GroupDocs.Watermark for Python via .NET."
    items: 
        # format loop 1
        - name: "ลายน้ำ PDF"
          format: "PDF"
          link: "/watermark/python-net/edit//pdf/"
          description: "รูปแบบเอกสาร Adobe Portable"

        # format loop 2
        - name: "ลายน้ำ Word"
          format: "WORD"
          link: "/watermark/python-net/edit//word/"
          description: "MS Word และเอกสาร Open Office"
          
        # format loop 3
        - name: "ลายน้ำ Excel"
          format: "EXCEL"
          link: "/watermark/python-net/edit//excel/"
          description: "MS Excel และสเปรดชีตโอเพ่นออฟฟิศ"

        # format loop 4
        - name: "ลายน้ำ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/python-net/edit//powerpoint/"
          description: "MS PowerPoint และงานนำเสนอแบบโอเพ่นออฟฟิศ"

        # format loop 5
        - name: "ลายน้ำ DOCX"
          format: "DOCX"
          link: "/watermark/python-net/edit//docx/"
          description: "ไมโครซอฟท์ Word เปิดเอกสาร XML"
          
        # format loop 6
        - name: "ลายน้ำ PPTX"
          format: "PPTX"
          link: "/watermark/python-net/edit//pptx/"
          description: "PowerPoint เปิดการนำเสนอ XML"
          
        # format loop 7
        - name: "ลายน้ำ XLSX"
          format: "XLSX"
          link: "/watermark/python-net/edit//xlsx/"
          description: "ไมโครซอฟท์ Excel เปิดสเปรดชีต XML"

        # format loop 8
        - name: "ลายน้ำ DOC"
          format: "DOC"
          link: "/watermark/python-net/edit//doc/"
          description: "ไมโครซอฟท์ Word 97 - เอกสาร 2007"

        # format loop 9
        - name: "ลายน้ำ XLS"
          format: "XLS"
          link: "/watermark/python-net/edit//xls/"
          description: "ไมโครซอฟท์ Excel สมุดงาน 97-2003"

        # format loop 10
        - name: "ลายน้ำ PPT"
          format: "PPT"
          link: "/watermark/python-net/edit//ppt/"
          description: "PowerPoint การนำเสนอ 97-2003"

        # format loop 11
        - name: "ลายน้ำ RTF"
          format: "RTF"
          link: "/watermark/python-net/edit//rtf/"
          description: "รูปแบบข้อความที่หลากหลาย"

---