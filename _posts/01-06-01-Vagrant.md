---
isChild: true
---

## Vagrant {#vagrant_title}

การรันโปรแกรมที่คุณเขียนบนสภาพแวดล้อมที่แตกต่างกันระหว่างขณะกำลังพัฒนากับสภาพแวดล้อมจริง
อาจทำให้เกิดบั๊กแปลกๆ ที่พบเฉพาะเวลาใช้งานจริง การทำให้สภาพแวดล้อมในการพัฒนาของโปรแกรมเมอร์แต่ละคน
ตรงกัน ใช้ไลบรารีเดียวกัน เป็นเรื่องวุ่นวายไม่น้อย

ถ้าคุณพัฒนาโปรแกรมบน Windows แล้วต้องเอาไปรันบน Linux (หรืออะไรที่ไม่ใช่ Windows) หรือช่วยกันพัฒนาหลายคน
คุณควรจะทำงานบน virtual machine มากกว่า อาจจะฟังดูยุ่งยาก แต่ถ้าใช้ [Vagrant][vagrant] คุณสามารถเซต
virtual machine ขึ้นมาได้ในไม่กี่ขั้นตอน เครื่องที่สร้างขึ้นมานี้อาจสร้างขึ้นมาแบบ manual หรือให้โปรแกรมจัดให้
(provisioning) โดยใช้ [Puppet][puppet] หรือ [Chef][chef] ก็ได้ การสร้าง virtual machine ด้วยวิธีนี้
รับประกันได้ว่าเครื่องที่ถูกสร้างขึ้นจะออกมาเหมือนกัน และคุณไม่ต้องคอยจัดการขั้นตอนการติดตั้งที่ซับซ้อน
คุณยังสามารถทำลาย (destroy) เครื่องแล้วสร้างขึ้นมาใหม่ได้ง่ายๆ โดยไม่ต้องทำเองแบบ manual ทุกขั้นตอน
ทำให้การสร้าง "fresh" installation เป็นเรื่องง่ายดาย

Vagrant ใช้ shared folders สำหรับแชร์ไฟล์ระหว่างเครื่องของคุณกับ virtual machine 
นั่นคือ คุณสามารถสร้างหรือแก้ไขไฟล์บนเครื่องของคุณ แล้วรันโค้ดจากใน virtual machine ได้ทันที

### ความช่วยเหลือเล็กๆ น้อยๆ

ถ้าคุณต้องการความช่วยเหลือในการเริ่มใช้งาน Vagrant มีบริการที่มีประโยชน์อยู่สามตัว:

- [Rove][rove]: บริการสำหรับสร้าง Vagrant build แบบเลือกโปรแกรมใช้งานได้เอง มี PHP ให้เลือกด้วย
  ตัวติดตั้งเป็น Chef
- [Puphpet][puphpet]: เว็บสำหรับสร้าง virtual machine สำหรับพัฒนาโปรแกรมด้วย PHP **โฟกัสกับ PHP เป็นพิเศษ**
  ตัวติดตั้งเป็น Puppet นอกจากใช้สร้าง local VM แล้วยังสามารถนำไปติดตั้งลง cloud service ได้ด้วย
- [Protobox][protobox]: is a layer on top of vagrant and a web GUI to setup virtual machines for web development. A single YAML document controls everything that is installed on the virtual machine.

[vagrant]: http://vagrantup.com/
[puppet]: http://www.puppetlabs.com/
[chef]: http://www.opscode.com/
[rove]: http://rove.io/
[puphpet]: https://puphpet.com/
[protobox]: http://getprotobox.com/
