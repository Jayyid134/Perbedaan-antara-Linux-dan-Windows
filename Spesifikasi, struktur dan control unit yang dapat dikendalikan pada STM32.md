# Spesifikasi, struktur dan control unit yang dapat dikendalikan pada STM32

## 1. Spesifikasi Umum STM32
STM32 memiliki berbagai varian yang ditujukan untuk kebutuhan yang berbeda, mulai dari yang memiliki kemampuan rendah hingga yang lebih tinggi, dengan berbagai pilihan fitur dan performa. Beberapa spesifikasi umum yang dimiliki oleh STM32 antara lain:

### Core Processor: 
STM32 didasarkan pada ARM Cortex-M (M0, M0+, M3, M4, M7, M33, dan M55). Setiap varian memiliki kelebihan dalam hal kinerja dan kemampuan pengolahan sinyal.
### Kecepatan Clock: 
Kecepatan clock dapat bervariasi, biasanya antara 32 MHz hingga 400 MHz tergantung pada modelnya.
### Memori:
- Flash Memory: Biasanya memiliki kapasitas mulai dari 16 KB hingga beberapa MB, tergantung pada modelnya.
- RAM: Memori SRAM mulai dari 2 KB hingga 512 KB.
### Peripherals:
- GPIO (General Purpose Input/Output): Berfungsi untuk menghubungkan mikrokontroler dengan perangkat eksternal.
- ADC (Analog to Digital Converter): Biasanya dengan resolusi 12-bit atau 16-bit.
- DAC (Digital to Analog Converter): Digunakan untuk mengkonversi sinyal digital menjadi sinyal analog.
- Timers: Digunakan untuk berbagai aplikasi seperti pengaturan waktu, PWM, atau pengukuran frekuensi.
- USART, SPI, I2C: Antarmuka komunikasi yang mendukung berbagai protokol komunikasi serial.
- CAN (Controller Area Network): Digunakan dalam sistem komunikasi kendaraan dan industri.
- USB, Ethernet: Beberapa model memiliki dukungan untuk komunikasi USB dan Ethernet.
## 2. Struktur STM32
Struktur umum mikrokontroler STM32 terdiri dari beberapa komponen penting, seperti berikut:

### CPU (Central Processing Unit): 
Berdasarkan ARM Cortex-M core, bertanggung jawab untuk eksekusi instruksi dan pengendalian sistem.
### Memori:
  - Flash: Digunakan untuk menyimpan kode program (termasuk bootloader).
  - RAM: Digunakan untuk penyimpanan data sementara selama eksekusi program.
### Bus: 
STM32 menggunakan bus untuk komunikasi antara CPU, memori, dan periferal lainnya.
### Peripherals: 
Sebagian besar model STM32 memiliki berbagai periferal seperti ADC, DAC, timer, GPIO, dan lainnya.
### Power Management: 
Banyak model STM32 mendukung berbagai mode daya seperti mode tidur atau hibernasi untuk efisiensi energi.
## 3. Control Unit (Unit Kontrol) yang Dapat Dikendalikan pada STM32
Unit kontrol pada STM32 mengacu pada bagian sistem yang bertanggung jawab untuk mengelola eksekusi instruksi dan pengendalian periferal. Unit-unit kontrol ini dapat dikendalikan untuk berbagai aplikasi:

### Timer dan PWM (Pulse Width Modulation): 
Digunakan untuk menghasilkan sinyal waktu, kendali motor, atau pengaturan kecepatan perangkat.
### Interrupt Controller: 
Digunakan untuk mengelola dan merespons interupsi (peristiwa eksternal atau internal) yang memicu eksekusi kode tertentu.
### Clock Control: 
Mengatur sumber dan frekuensi clock untuk seluruh sistem, memungkinkan penghematan daya dengan mengubah kecepatan clock sesuai kebutuhan.
### DMA (Direct Memory Access): 
Memungkinkan data dipindahkan antara periferal dan memori tanpa intervensi CPU, meningkatkan kinerja dan efisiensi.
### Power Control: 
Mengatur mode daya dan pengelolaan konsumsi daya mikrokontroler, memungkinkan untuk bekerja pada mode daya rendah.

