---
isChild: true
---

## การติดตั้งบน Mac  {#mac_setup_title}

OSX จะแถม PHP มาให้ในตัวด้วยอยู่แล้ว แต่จะเก่ากว่าเวอร์ชันล่าสุดอยู่เล็กน้อย
Lion จะให้ PHP 5.3.6, Mountain Lion ให้ PHP 5.3.10 และ Maverick ให้ PHP 5.4.17

คุณสามารถอัปเดตรุ่นของ PHP บน OS X ได้โดยใช้ [โปรแกรมจัดการแพคเกจ][mac-package-managers] 
บน Mac ซึ่งมีให้เลือกหลายตัว ที่แนะนำคือ [php-osx by Liip][php-osx-downloads]

วิธีอัปเดตแบบอื่นก็มีเช่น [คอมไพล์ด้วยตัวเอง][mac-compile] ซึ่งในเครื่องต้องติดตั้ง Xcode หรือ 
[Command Line Tools for Xcode][apple-developer] ไว้ด้วย สามารถโหลดได้จากหน้า 
Mac Developer Center ของ Apple

สำหรับแพคเกจแบบรวมที่มีทั้ง PHP, เว็บเซิร์ฟเวอร์ Apache และฐานข้อมูล MySQL มีตัวควบคุม
แบบกราฟิกสวยงาม ให้ลอง [MAMP][mamp-downloads] หรือ [XAMPP][xampp]

[mac-package-managers]: http://www.php.net/manual/en/install.macosx.packages.php
[mac-compile]: http://www.php.net/manual/en/install.macosx.compile.php
[xcode-gcc-substitution]: https://github.com/kennethreitz/osx-gcc-installer
[apple-developer]: https://developer.apple.com/downloads
[mamp-downloads]: http://www.mamp.info/en/downloads/index.html
[php-osx-downloads]: http://php-osx.liip.ch/
[xampp]: http://www.apachefriends.org/en/xampp.html
