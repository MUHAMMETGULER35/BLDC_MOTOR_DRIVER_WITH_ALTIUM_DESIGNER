  Bu projede BLDC motor sürücü kartı tasarımı, modellemesi, devre testleri yapılmıştır. Altium Designer ile  şematik ve PCB oluşturulmuştur.Yazılım kısmında STM32CubeIDE üzerinden HAL kütüphaneleriyle gömülü yazılımı oluşturulmuştur. Devre ile ilgili detaylar aşağıda belirtilmiştir.

  Tasarım sürecinde oluşturulan devreler LTspice'da simüle edilmiş ve breadboard üzerinde kurularak test edilmiştir. Devre protection, power, Feedback ve MCU kısımlarından oluşmaktadır. Devrenin protection kısmı reverse polarity, over voltage, under voltage ve thermal shutdown devrelerinden oluşmaktadır. Devrenin driver kısmında, IR2103 IC kullanılarak, bootstrap sürme tekniğiyle mosfetler hıgh side ve low sıde sürülmüştür. Devrenin feedback kısımlarında rotorun başlangıç konumunu tespit eden initial pozition detector(IPD) devre yapısı kullanılmıştır.  zero-crossıng detector devresi ile sıfır noktası ADC'ler ile tespit edilip fazlar PWM ile enerjilendirilerek algoritma oluşturulmuştur. Regülatör kısmında 24V-3.3V swıtchıng mod yüksek verimli buck converter tasarımı yapılmıştır. MCU olarak STM32F103C8T6 mikrodenetleyicisi tercih edilmiştir. UART ile akım gerilim ve sıcaklık verileri dışarı verilmiştir. ADC, DMA ve interrupt gibi çevresel birimleri algoritmanın diğer kısımlarında kullanılmıştır.

![28](https://github.com/MUHAMMETGULER35/BLDC_MOTOR_DRIVER_WITH_ALTIUM_DESIGNER/assets/156583959/9300c498-d545-419c-9a08-914b2014a111)
  
![58](https://github.com/MUHAMMETGULER35/BLDC_MOTOR_DRIVER_WITH_ALTIUM_DESIGNER/assets/156583959/6d2fe379-770a-40ee-a0e2-e542e5de2f4f)
![59](https://github.com/MUHAMMETGULER35/BLDC_MOTOR_DRIVER_WITH_ALTIUM_DESIGNER/assets/156583959/0bda92ca-d1b6-447b-a65a-639bc16304d9)
![60](https://github.com/MUHAMMETGULER35/BLDC_MOTOR_DRIVER_WITH_ALTIUM_DESIGNER/assets/156583959/13d51b87-6aaa-4d4d-a865-5715e8d140a5)
![57](https://github.com/MUHAMMETGULER35/BLDC_MOTOR_DRIVER_WITH_ALTIUM_DESIGNER/assets/156583959/237f13eb-dec8-4ee8-abd3-345ff2a02faf)
![56](https://github.com/MUHAMMETGULER35/BLDC_MOTOR_DRIVER_WITH_ALTIUM_DESIGNER/assets/156583959/f314d959-f9d0-40a2-b2df-5e9d68c3fbbe)
![55](https://github.com/MUHAMMETGULER35/BLDC_MOTOR_DRIVER_WITH_ALTIUM_DESIGNER/assets/156583959/4843a219-241d-4f5c-b5dd-dc97890c2284)
![54](https://github.com/MUHAMMETGULER35/BLDC_MOTOR_DRIVER_WITH_ALTIUM_DESIGNER/assets/156583959/8b6ebae4-5e27-4340-9ff8-7779b16f0068)
![62](https://github.com/MUHAMMETGULER35/BLDC_MOTOR_DRIVER_WITH_ALTIUM_DESIGNER/assets/156583959/7a7ca570-faf0-4e3e-85b5-f358405c89f9)
![61](https://github.com/MUHAMMETGULER35/BLDC_MOTOR_DRIVER_WITH_ALTIUM_DESIGNER/assets/156583959/c87e8b06-21c4-41c0-a980-67c47b55c391)



