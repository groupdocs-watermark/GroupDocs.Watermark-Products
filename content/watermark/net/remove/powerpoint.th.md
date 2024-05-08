
---
############################# Static ############################
layout: "format"
date:  2024-05-08T17:25:19
draft: false
lang: th
format: Powerpoint
product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "ล้างลายน้ำใน Powerpoint ด้วย C# .NET API"
head_description: "ลบและจัดการลายน้ำในสไลด์ Powerpoint ได้อย่างง่ายดายโดยใช้ API C# .NET ของเราเพื่อให้แน่ใจว่ามีการนำเสนอที่ชัดเจนและเป็นมืออาชีพ"

############################# Header ############################
title: "C# .NET Powerpoint น้ำยาล้างลายน้ำ" 
description: "ใช้พลังของ GroupDocs.Watermark for .NET C# API เพื่อลบลายน้ำออกจากงานนำเสนอ Powerpoint ได้อย่างมีประสิทธิภาพ รักษาความสวยงามของสไลด์ในขณะที่ยังคงความสมบูรณ์ของเนื้อหา"
subtitle: "GroupDocs.Watermark for .NET C# เอพีอี" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Nuget ดาวน์โหลด"
      link: "https://releases.groupdocs.com/watermark/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Watermark for .NET C# ห้องสมุด"
    link: "/watermark/net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_watermark.svg" # 480 X 400
    content: |
       ไลบรารี GroupDocs.Watermark for .NET C# นำเสนอเครื่องมือที่ซับซ้อนในการลบลายน้ำออกจากงานนำเสนอ Powerpoint มีฟังก์ชั่นสำหรับการลบลายน้ำอย่างราบรื่น ทำให้มั่นใจได้ว่าการนำเสนอของคุณยังคงมีผลกระทบและไม่ยุ่งยากเหมาะสำหรับสภาพแวดล้อมทางธุรกิจ การศึกษา และการฝึกอบรมที่ภาพที่สะอาดและชัดเจนเป็นสิ่งจำเป็น

############################# Steps ############################
steps:
    enable: true
    title: "ลบลายน้ำออกจากเอกสาร Powerpoint โดยใช้ .NET"
    content: |
      **[GroupDocs.Watermark](https://products.groupdocs.com/watermark/net/)** ช่วยให้งานลบลายน้ำออกจากเอกสารทางธุรกิจง่ายขึ้น เพิ่มประสิทธิภาพให้กับแอปพลิเคชัน .NET ของคุณด้วยการผสานรวมไลบรารีของเราและทำตามขั้นตอนง่ายๆ เหล่านี้:
      
      1. เริ่มต้นด้วยการสร้างอินสแตนซ์คลาสหลัก **Watermarker** ด้วยเอกสาร Powerpoint API ของเรารองรับการประมวลผลเอกสารที่เป็นสตรีมหรือเส้นทางในเครื่อง
      2. ใช้ **SearchCriteria** เพื่อจำกัดชุดลายน้ำที่จะประมวลผลให้แคบลง คุณสามารถใช้พารามิเตอร์ต่างๆ เช่น รูปภาพ ข้อความ หรือคุณลักษณะการจัดรูปแบบ ยิ่งคุณระบุพารามิเตอร์การค้นหาที่เฉพาะเจาะจงมากเท่าไร ผลลัพธ์ที่คุณได้รับก็จะยิ่งแม่นยำมากขึ้นเท่านั้น
      3. ประมวลผลรายการลายน้ำเอกสารที่ได้รับเป็นผลการค้นหา และลบออกจากเอกสาร
      4. หลังจากลบลายน้ำแล้ว ให้บันทึกเอกสารผลลัพธ์เป็นไฟล์ในเครื่องหรือสตรีมไบต์
   
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
        // ลบลายน้ำข้อความออกจากเอกสาร Powerpoint

        // จัดเตรียมอินสแตนซ์ Watermarker สำหรับเอกสารต้นฉบับ Powerpoint
        using (Watermarker watermarker = new Watermarker("input.พีพีทีเอ็กซ์"))
        {
            // ลบลายน้ำที่เลือกออกจากเอกสาร
            TextFormattingSearchCriteria criteria = new TextFormattingSearchCriteria();
            criteria.ForegroundColorRange = new ColorRange();
            criteria.FontBold = true;
            PossibleWatermarkCollection watermarks = watermarker.Search(criteria);
            watermarks.Clear();

            // บันทึกไฟล์ไปยังเส้นทางที่ให้ไว้
            watermarker.Save("output.พีพีทีเอ็กซ์");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ปรับปรุงการกำจัดลายน้ำด้วย C# .NET API"
  description: "ค้นพบความสามารถในการกำจัดลายน้ำอันทรงพลังของ API C# .NET ของเราที่ออกแบบมาเพื่อผสานรวมกับแอปพลิเคชัน .NET ของคุณได้อย่างราบรื่นลบหรือล้างลายน้ำจาก PDF และเอกสารสำนักงานอย่างมีประสิทธิภาพในขณะที่รักษาคุณภาพของไฟล์ต้นฉบับ"
  image: "/img/watermark/features_remove.webp" # 500x500 px
  image_description: "ลบลายน้ำ"
  features:
    # feature loop
    - title: "การล้างลายน้ำที่แม่นยำ"
      content: "API .NET ของเราให้เครื่องมือที่แม่นยำในการลบลายน้ำออกจากเอกสารใด ๆ ได้อย่างสะอาดคุณลักษณะนี้เหมาะสำหรับนักพัฒนา ช่วยให้มั่นใจได้ว่าการลบลายน้ำจะไม่ส่งผลต่อคุณภาพของเอกสารหรือเค้าโครง"

    # feature loop
    - title: "การกำจัดลายน้ำจำนวนมากโดยอัตโนมัติ"
      content: "ทำกระบวนการลบลายน้ำออกจากชุดเอกสารขนาดใหญ่โดยอัตโนมัติ ด้วย API .NET ของเราเหมาะสำหรับธุรกิจที่จัดการเอกสารจำนวนมาก ช่วยเพิ่มประสิทธิภาพและความปลอดภัยของเอกสาร"

    # feature loop
    - title: "คุณสมบัติการแก้ไขลายน้ำขั้นสูง"
      content: "ใช้ประโยชน์จากคุณลักษณะขั้นสูงเพื่อเลือกแก้ไขหรือแก้ไขลายน้ำAPI ของเรารองรับการปรับเปลี่ยนโดยละเอียดเพื่อให้แน่ใจว่าเอกสารของคุณคงรูปลักษณ์อย่างมืออาชีพในขณะที่รักษาความปลอดภัยข้อมูลที่ละเอียดอ่อน"
      
  code_samples:
    # code sample loop
    - title: "ลบลายน้ำข้อความสเปรดชีต"
      content: |
        วิธีลบลายน้ำข้อความด้วยการจัดรูปแบบพิเศษใน Excel เอกสาร
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        
            //  โหลดสมุดงาน Excel
            var loadOptions = new SpreadsheetLoadOptions();
            using (Watermarker watermarker = new Watermarker("source.xlsx", loadOptions))
            {
                //  รับเนื้อหาและค้นหาลายน้ำที่เหมาะสม
                SpreadsheetContent content = watermarker.GetContent<SpreadsheetContent>();
                foreach (SpreadsheetWorksheet section in content.Worksheets)
                {
                    for (int i = section.Shapes.Count - 1; i >= 0; i--)
                    {
                        foreach (FormattedTextFragment fragment in section.Shapes[i].FormattedTextFragments)
                        {
                            if (fragment.ForegroundColor.Equals(Color.Red) && fragment.Font.FamilyName == "Arial")
                            {
                                //  ลบลายน้ำข้อความ
                                section.Shapes.RemoveAt(i);
                                break;
                            }
                        }
                    }
                }

                //  บันทึกการประมวลผล XLSX
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
    title: "การเพิ่มประสิทธิภาพการนำเสนอ Powerpoint ใน .NET"
    exclude: "POWERPOINT"
    description: "ค้นพบวิธีใช้ API GroupDocs.Watermark for .NET C# สำหรับการนำเสนอ Powerpoint ที่สะอาดและเป็นมืออาชีพ โดยปราศจากองค์ประกอบลายน้ำที่ทำให้เสียสมาธิ"
    items: 
        # format loop 1
        - name: "ลายน้ำ PDF"
          format: "PDF"
          link: "/watermark/net/remove//pdf/"
          description: "รูปแบบเอกสาร Adobe Portable"

        # format loop 2
        - name: "ลายน้ำ Word"
          format: "WORD"
          link: "/watermark/net/remove//word/"
          description: "MS Word และเอกสาร Open Office"
          
        # format loop 3
        - name: "ลายน้ำ Excel"
          format: "EXCEL"
          link: "/watermark/net/remove//excel/"
          description: "MS Excel และสเปรดชีตโอเพ่นออฟฟิศ"

        # format loop 4
        - name: "ลายน้ำ PowerPoint"
          format: "POWERPOINT"
          link: "/watermark/net/remove//powerpoint/"
          description: "MS PowerPoint และงานนำเสนอแบบโอเพ่นออฟฟิศ"

        # format loop 5
        - name: "ลายน้ำ DOCX"
          format: "DOCX"
          link: "/watermark/net/remove//docx/"
          description: "ไมโครซอฟท์ Word เปิดเอกสาร XML"
          
        # format loop 6
        - name: "ลายน้ำ PPTX"
          format: "PPTX"
          link: "/watermark/net/remove//pptx/"
          description: "PowerPoint เปิดการนำเสนอ XML"
          
        # format loop 7
        - name: "ลายน้ำ XLSX"
          format: "XLSX"
          link: "/watermark/net/remove//xlsx/"
          description: "ไมโครซอฟท์ Excel เปิดสเปรดชีต XML"

        # format loop 8
        - name: "ลายน้ำ DOC"
          format: "DOC"
          link: "/watermark/net/remove//doc/"
          description: "ไมโครซอฟท์ Word 97 - เอกสาร 2007"

        # format loop 9
        - name: "ลายน้ำ XLS"
          format: "XLS"
          link: "/watermark/net/remove//xls/"
          description: "ไมโครซอฟท์ Excel สมุดงาน 97-2003"

        # format loop 10
        - name: "ลายน้ำ PPT"
          format: "PPT"
          link: "/watermark/net/remove//ppt/"
          description: "PowerPoint การนำเสนอ 97-2003"

        # format loop 11
        - name: "ลายน้ำ RTF"
          format: "RTF"
          link: "/watermark/net/remove//rtf/"
          description: "รูปแบบข้อความที่หลากหลาย"

---