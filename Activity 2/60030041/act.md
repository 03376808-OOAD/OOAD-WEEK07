>classification, abstraction, states and behavious 

>Aggregation,Abstraction, Cardinallity, Regurired and optional

**classification, abstraction, states and behavious**

    - classification คือการจำนำแนก ประกอบด้วย state(สถานะ) behavior(พฤติกรรม)
    - abstraction คือการให้นิยามให้กับวัตถุ เช่น
    มองว่า ชาเขียวนมไขมุก เป็นสิ่งที่อยู่ในโลกแห่งความเป็นจริง จะทำการแยกประเภทออกมาได้ดังนี้
    state
        -หลอด
        -ผงชาเขียว
        -น้า
        -แก้ว
    behavior
    -สามารถดื่มได้

**Aggregation,Abstraction, Cardinallity, Regurired, Ptinal**

    Aggregation คือ การบอกส่วนประกอบ เช่น Concep ของวัตถุ ประโยชน์ในหารทำ Reuse
    เป็นความสัมพันธ์ระหว่าง Object หรือ Class โดยจะมี Class ที่ใหญ่ที่สุดที่เป็น Object หลัก และมี Class
    เช่น class หลอด, class ผงชาเขียว, class น้ำ, class แก้ว มีความสำพันธ์กัน อย่างไร
    จะสร้่าง class ของผงชงออกมา เป็น class ผมชาเขียว, class กาแฟ มีความสัมพันธ์ สามาผสมกับน้ำได้

     การประกอบกันของclass หรือความสมพันธ์เชิง is part of นั้นอาจจะเกิดกรณีที่ class หลัก (main class) ประกอบด้วย class ย่อยComposite class ) ชนิดที่หรือ เพียงชนิดหรือเพียงชิ้นเดียวแต่ประกอบด้วย class ชนิดที่สอง จํานวน 4 ชนขึ้นไป และอาจจะประกอบไปด้วยชนิดที่สาม ไม่จํากัดจํานวน หรืออาจไม่มีเลยก็ได้
     ซึ่งสิ่งที่ใช้ในการแสดงความสัมพันธ์ ดังกล่าวนี้เรียกว่า Cardinality ประกอบด้วย min Cardinality และ max Cardinality