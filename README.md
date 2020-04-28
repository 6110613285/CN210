# รายงานวิชา CN210

## สรุปเนื้อหา


#### Computer Organization
   - ส่วนประกอบของ Computer 
     1. CPU (Central Processing Unit) 
     2. I/O (Input,Output) 
     3. Main Memory
    
   - ส่วนประกอบของ CPU      
     1. ALU (Arithmetic Logic Unit) 
     2. Control Unit 
     3. Register
     
#### Von Neuman & Harvard Architectures
   - Von Neuman Architecture : มี Memory ที่เก็บทั้ง Instruction และ Data อยู่ภายใน Memory เดียวกันทำให้มีพื้นที่ในการเก็บข้อมูลมาก
   - Harvard Architecture    : มี Memory ที่เก็บ Instruction และ Data แยกกัน ไม่ได้อยู่ภายใน Memory เดียวกันทำให้มีประสิทธิภาพในการรับส่งข้อมูลที่รวดเร็ว
   
#### MIPS 
  - MIPS มีคำสั่ง 3 คำสั่งคือ
     * R-format
     
     ![image](http://4.bp.blogspot.com/-Ui0mt4h44s8/Up2nvk3iU3I/AAAAAAAAAPY/sF4haVYx6BE/s1600/1.png)
     
     * I-format
      
      ![image](http://4.bp.blogspot.com/-SrDyDKDbxJ8/Up2oHmwtNEI/AAAAAAAAAPg/9i686ypFdCg/s1600/3.png)
     
     * J-format
   
      ![image](http://1.bp.blogspot.com/-MqcOl_V2rSw/Up2okUK7aNI/AAAAAAAAAPo/R5iPs60F8Y0/s1600/2.png)
     

#### CISC & RISC
  - CISC ย่อมาจาก Complex instruction set computer : เป็นคอมพิวเตอร์ที่มีชุดคำสั่งซับซ้อน
      * ทุกชุดคำสั่งจะต้องมี Reference ถึง Memory
      * Program code มีขนาดเล็ก
      * รูปแบบชุดคำสั่งมีหลากหลาย
      * มี Register ชุดเดียว
      * ชุดคำสั่งเป็นแบบ Multi-cycle
   - RISC ย่อมาจาก Reduced instruction set computer : เป็นคอมพิวเตอร์ที่มีชุดคำสั่งน้อย
      * มีเพียงคำสั่ง Load และ Store ที่มี Reference ถึง Memory
      * Program code มีขนาดใหญ่
      * รูปแบบชุดคำสั่งตายตัว
      * มี Register ชุดเดียว
      * ชุดคำสั่งเป็นแบบ Single-cycle

#### Single-cycle
   Single-cycle processor : เป็นคอมพิวเตอร์ที่มีการประมวลผลคำสั่งแต่ละคำสั่งจบใน 1 รอบ หรือ 1 Clock cycle ซึ่งทุกคำสั่งจะใช้เวลาในการประมวลผลเท่ากัน
    
![image](http://drive.google.com/uc?export=view&id=1GIYTId6ZYovkSXrQ31STBv3uLl52b8g9)

#### Multi-cycle
   Multi-cycle processor  : เป็นคอมพิวเตอร์ที่มีการประมวลผลคำสั่งแต่ละคำสั่งไม่ได้จบใน 1 รอบ หรือ 1 Clock cycle ซึ่งแต่ละคำสั่งใช้เวลาในการประมวลผล หรือ Clock cycle ไม่เท่ากัน 
   
![image](http://drive.google.com/uc?export=view&id=19A9x3-tvJNARLM_pqO3fG_Zm3eLgdx-S)

#### Pipe lining
 - เป็นการลดระยะเวลาที่ใช้ในการทำงานลงโดยเมื่อมีอุปกรณ์ที่ว่างก้จะนำคำสั่งต่อไปมาทำงานทันที

## Homework
#### การบ้านครั่งที่1
* [งานครั้งที่ 1](https://drive.google.com/open?id=1JahkkOSXNiXsl_ZzBNgzGbNgR5M7mhUK) เป็นการอธิบายคำสั่ง J-format หรือคำสั่ง jump โดย คำสั่งนี้จะเป็นการสั่งให้ CPU ข้ามไปทำคำสั่งในอีก address ที่เป็นเป้าหมายของคำสั่ง มี 2 ส่วน คือ 
  1. **Op Code (Operation Code)** : มีความยาว *6 bits* และ สำหรับ J-Format จะใช้ Op Code คือ `000010`
  2. **Address (Jump Target Address)** : มีความยาว *26 bits* 
* [งานครั้งที่ 2](https://drive.google.com/file/d/1EP2tqjhE2Gw8tjX2D7x8oRSfundzdQIQ/view?usp=drivesdk) เป็นการอธิบายตัวอย่างการทำงานของระบบคอมพิวเตอร์ในภาษาขั้นสูง โดยภายในคลิปจะพูดถึงการทำงานของคำสั่งต่างๆตั้งแต่การย้ายตำแหน่งในการทำงาน(jump) การดึงข้มูลในชุดคำสั่ง(lw) การเก็บข้อมูล(sw) และการคำนวณคำสั่ง add ในรูปแบบของbinary

* [งานครั้งที่ 3](https://youtu.be/K4fZwQTjtdc) เป็นการอธิบายความแตกต่างระหว่างการทำงานแบบ single cycle และ multi cycle โดยเนื้อหาภายในคลิปจะเป็นการอธิบายการทำงานของ Single cycle และ Multi cycle เพื่อเปรียบเทียบว่าการทำงานแบบ Single cycle และ Multi cycleมีความแตกต่างกันยังไง
  
* [งานครั้งที่ 4](https://youtu.be/c3uKJYdjnJM) อธิบายตัวอย่างการทำงานของคำสั่ง lw ในการทำงานแบบ multi cycle โดยเนื้อหาภายในคลิปจะเป็นการอธิบายขั้นตอนต่างๆในการทำงานของคำสั่ง lw ว่าแต่ละขั้นตอนในการทำงานในแบบ Multi cycle มีการทำงานยังไง ซึ่งจะมีการแบ่งขั้นตอนต่างๆเป็น T1-T5

* [งานครั้งที่ 5](https://youtu.be/gJ6TK7mZDMQ) อธิบายการทำงานของคำสั่ง beq ในการทำงานแบบ multi cycle โดยเนื้อหาภายในคลิปจะเป็นการอธิบายขั้นตอนต่างๆในการทำงานของคำสั่ง beq ว่าแต่ละขั้นตอนในการทำงานแบบ Multi cycle มีการทำงานยังไง ซึ่งจะมีการแบ่งขั้นตอนต่างๆ เป็น T1-T3

* [งานครั้งที่ 6](https://youtu.be/xfQPSRIEDAk) อธิบายวิธีในการทำงานของคำสั่ง r-type ใน multi cycle โดยเนื้อหาภายในคลิปจะเป็นการอธิบายขั้นตอนต่างๆในการทำงานของคำสั่งในรูปแบบ R-format ว่าแต่ละขั้นตอนในการทำงานแบบ Multi cycle มีการทำงานยังไง ซึ่งจะมีการแบ่งขั้นตอนต่างๆ ออกเป็น T1-T4 และจะแสดงการทำงานในรูปแบบของสัญญาณ

* [งานครั้งที่ 7]()การทำงานแบบ pipelining โดยเนื้อหาภายในคลิปจะเป็นการอธิบายความแตกต่างระหว่างการทำงานของ Single ,Multi cycle และ pipelining เพื่อจะได้เห็นว่าการทำงานแบบ pipelining นั้นมีความเร็วมากกว่าแบบ Single และ Multi cycle ยังไง และภายในคลิปก้จะมีการพูดถึงข้อเสียของการทำงานแบบ pipelining อยู่ช่วงท้ายคลิป
