# รายงานวิชา CN210

## สรุปเนื้อหา


#### Computer Organization
   - ส่วนประกอบของ Computer 
     ~~~~ 
     1. CPU (Central Processing Unit) 
     2. I/O (Input,Output) 
     3. Main Memory
     ~~~~ 
   - ส่วนประกอบของ CPU      
     ~~~
     1. ALU (Arithmetic Logic Unit) 
     2. Control Unit 
     3. Register
     ~~~
#### Von Neuman & Harvard Architectures
   - Von Neuman Architecture : มี Memory ที่เก็บทั้ง Instruction และ Data อยู่ภายใน Memory เดียวกันทำให้มีพื้นที่ในการเก็บข้อมูลมาก
   - Harvard Architecture    : มี Memory ที่เก็บ Instruction และ Data แยกกัน ไม่ได้อยู่ภายใน Memory เดียวกันทำให้มีประสิทธิภาพในการรับส่งข้อมูลที่รวดเร็ว
   
#### MIPS 
  - MIPS มีคำสั่ง 3 คำสั่งคือ
     ~~~
     1. R-format
     ![image1]( https://drive.google.com/drive/u/0/folders/1w0vSdX_HcPCu6YNymyqS10r3wl_KZTS2 )
     2. I-format
     ![image2](  )
     3. J-format
     ![image3](  )
     ~~~

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
    
![image4](  )

#### Multi-cycle
   Multi-cycle processor  : เป็นคอมพิวเตอร์ที่มีการประมวลผลคำสั่งแต่ละคำสั่งไม่ได้จบใน 1 รอบ หรือ 1 Clock cycle ซึ่งแต่ละคำสั่งใช้เวลาในการประมวลผล หรือ Clock cycle ไม่เท่ากัน 
   
![image4](  )

#### Pipe lining
 - เป็นการลดระยะเวลาที่ใช้ในการทำงานลงโดยเมื่อมีอุปกรณ์ที่ว่างก้จะนำคำสั่งต่อไปมาทำงานทันที

## Homework
* [งานครั้งที่ 1](https://drive.google.com/open?id=1JahkkOSXNiXsl_ZzBNgzGbNgR5M7mhUK)

* [งานครั้งที่ 2](https://drive.google.com/file/d/1EP2tqjhE2Gw8tjX2D7x8oRSfundzdQIQ/view?usp=drivesdk)

* [งานครั้งที่ 3](https://youtu.be/K4fZwQTjtdc)
  
* [งานครั้งที่ 4](https://youtu.be/c3uKJYdjnJM)

* [งานครั้งที่ 5](https://youtu.be/gJ6TK7mZDMQ)

* [งานครั้งที่ 6](https://youtu.be/xfQPSRIEDAk)

* [งานครั้งที่ 7]
