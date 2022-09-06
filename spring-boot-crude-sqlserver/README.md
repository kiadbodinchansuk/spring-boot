<img src="https://seeklogo.com/images/M/microsoft-sql-server-logo-96AF49E2B3-seeklogo.com.png" width="150"/>

# spring boot connect sqlserver
# วิธีการตั้งค่าเปิดพอร์ตเพื่อให้ MS SQL Server เพื่อให้สามารถเชื่อมต่อกับภายเครื่องได้ หรือ บน Server 
ดูตัวอย่าง <a href="https://docs.microsoft.com/th-th/sql/database-engine/configure-windows/configure-a-server-to-listen-on-a-specific-tcp-port?view=sql-server-2017"> TCP PORT </a>
# ตัวอย่าง
ในตัวอย่างนี้จะใช้ JpaRepository เป็นตัวดำเนินการ sql query ข้อมูล โดยไม่ต้องเขียนคำสั่ง  insert , update ,delete ของ statement sql
* การเพิ่ม Add
* แก้ไข  Update
* ลบข้อมูล Delete

# เริ่มต้นใน Eclipse ดังนี้
# 1. กำหนด Config ใน application.properties
# 2. กำหนด dependencies ในไฟล์ pom.xml  
# 3. เขียน Entity ในของ Table ให้ตรงกับชื่อ ตารางใน sqlserver
# 4. เขียน JpaRepository โดยสร้าง Interface ของ Repo เชื่อมต่อ JpaRepository ในแพจเกจ Repository
# 5. เขียน Service ในการเรียกใช้ Interface Repository กำหนด method ต่างๆ เช่น Add , findAll, delete เป็นต้น
# 6. เขียน Controller เพื่อกำหนด Mapping path url
# 7. รัน Project ทดสอบการใช้งาน
