Generalization Abstraction
    private 
    protected 
    public

Association Abstraction 
    relationship 
    role

Generalization Abstraction
คือกระบวนการในการนํา Class ที่มีลักษณะเหมือนหรือคล้ายกันหรือมีคุณสมบัติอย่างใดอย่างหนึ่งร่วมกัน (General) มาจัดหมวดหมู่ไว ้เป็น Class เดียวกัน 

    Private
        คือ Attributes และ Functions ที่ไม่สามารถเห็นได้จากภายนอก
            -การเข ้าถึง Attribute เหล่านี้ได้ต้องผ่าน Function ที่มีไว ้เท่านั้น
            -จะใช้เครื่องหมาย (-) กํากับไว ้หน้า Private Attribute และ Private Function
        เช่น อายุของคน

    protected 
        คือ Attributes และ Functions             ที่ไม่สามารถเห็นได้ได้จากภายนอกแต่เป็นส่วนที่สามารถส่งต่อให้ Inherited Class ได้เท่านั้น
            -จะใช้เครื่องหมาย (#) กํากับไว้หน้า Protected Attribute และ Protected Function
        เช่น ลักษณะทางกรรมพันธ์ที่ลูกสืบทอดมาจากพ่อแม่
    
    public 
        คือ Attributes และ Functions ที่สามารถมองเห็นได้และสามารถเรียกใช้ได้โดยตรงจากภายนอก
            -จะใชเครื่องหมาย ้ (+) กํากับไว ้หน้า Public Attribute และ Public Function
        เช่น สีผม สีผิว

    Association Abstraction
    คือ กระบวนการในการสร้างความสัมพันธ์ ระหว่าง class ต่าง  ๆ ใน Problem domain ที่เราสนใจ โดยเป็นการอธิบายความสัมพันธ์ ของ class ในเชิงกิจกรรม

    เป็นความสัมพันธ์ขั้นพื้นฐาน คือ สิ่งของทั้งสองสิ่งที่มีความสัมพันธ์กันเป็นสิ่งที่มีความสำคัญเท่าเทียมกัน ไม่ใช่องค์ประกอบของกันเช่น คนเป็นเจ้าของรถยนต์  แม่มีลูก  สามีรักภรรยา  ดินสออยู่ในกระเป๋า

    ในทาง OO เรียกความสัมพันธ์เรียกความสัมพันธ์ในลักษณะนี้ว่า Association Relationship และเรียกกระบวนการค้นหาความสัมพันธ์ลักษณะนี้ ว่า Association Abstraction

    role หมายถึง ชื่อที่กําหนดให้กับด้านปลายของ association ซึ่งระบุวิธีการในการที่คลาสมีส่วนร่วมใน association
        -ปกติชื่อของ role มักเกิดขึ้นเป็นคู่ (เช่นทั้งสองด้านของ association จะมีชื่อของ role
        -บังคับให ้กําหนดชื่อของ Role กับ associations แบบ reflexive (Reflexive associations : ย้อนกลับ)

