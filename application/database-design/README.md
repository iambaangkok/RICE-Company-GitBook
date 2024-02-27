# 📋 Database Design

@Database Team: Za, Pond, Meen

<details>

<summary>ภาพรวมของฐานข้อมูล</summary>

<img src="https://media1.tenor.com/m/x8v1oNUOmg4AAAAd/rickroll-roll.gif" alt="" data-size="original">

ลิงก์ดาวน์โหลดแผนภาพในรูปแบบ svg

</details>

การออกแบบฐานข้อมูลส่วนใหญ่จะใช้หลักการออกแบบฐานข้อมูลแบบ [Third normal form (3NF)](https://en.wikipedia.org/wiki/Third\_normal\_form), โดยที่ฐานข้อมูลต่างๆจะอยู่แยกกันตามแต่ละ[ระบบ](../../infrastructure/system-design/system-design-diagram.md) (บางระบบจะไม่มีฐานข้อมูลเนื่องจากใช้บริการจากภายนอกทั้งหมด)

แต่ละบริการจะแยกฐานข้อมูลออกจากกันอย่างชัดเจนโดยไม่มีการจัดกลุ่มย่อย อย่างไรก็ตาม ผู้จัดทำได้แบ่งเป็นกลุ่มคร่าวๆ เพื่อให้ง่ายต่อการอ่าน ดังนี้

* [ผู้ใช้งาน (User)](user/)
* [ร้านค้าและการสั่งซื้อ (Shop & Transaction)](shop-and-transaction/)
* [จิปาถะ (Miscellaneous)](miscellaneous/)

