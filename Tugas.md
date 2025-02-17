## Control Unit pada Raspberry Pi (SoC - System on Chip)
Raspberry Pi menggunakan SoC (System on Chip), yang menggabungkan CPU, GPU, RAM, dan berbagai komponen lain dalam satu chip. SoC yang umum digunakan adalah Broadcom BCM2711 (untuk Raspberry Pi 4).

Arsitektur Control Unit di Raspberry Pi
CPU (Central Processing Unit)

Menggunakan arsitektur ARM Cortex-A72 (pada Raspberry Pi 4) atau sebelumnya ARM Cortex-A53 (Raspberry Pi 3).
Control Unit di CPU menangani eksekusi instruksi, pengelolaan register, dan komunikasi dengan perangkat lain.
Bekerja dengan pipeline execution untuk meningkatkan efisiensi pemrosesan.
Memory Management Unit (MMU)

Mengelola alokasi memori antara CPU, GPU, dan perangkat eksternal.
Berbasis paging dan caching untuk efisiensi akses data.
GPU (Graphics Processing Unit)

Menggunakan VideoCore IV (Raspberry Pi 3) atau VideoCore VI (Raspberry Pi 4).
Bertindak sebagai kontrol unit untuk pemrosesan grafis dan akselerasi multimedia.
Peripheral Control Unit

Raspberry Pi memiliki beberapa pengontrol untuk komunikasi dengan perangkat eksternal:
I2C, SPI, UART untuk komunikasi sensor.
GPIO (General Purpose Input/Output) untuk kontrol perangkat fisik.
USB Controller untuk perangkat input/output seperti keyboard dan mouse.
Real-Time Clock (RTC) & Power Management

Mengelola waktu dan konsumsi daya, meskipun Raspberry Pi tidak memiliki RTC bawaan (bisa menggunakan modul tambahan).


## Arsitektur Control Unit pada ESP (ESP8266 & ESP32)
ESP adalah mikrokontroler berbasis RISC yang lebih hemat daya dibanding Raspberry Pi. ESP8266 dan ESP32 dibuat oleh Espressif Systems dan dirancang khusus untuk aplikasi IoT.

### Komponen Utama Control Unit di ESP

#### 1. CPU – Xtensa (ESP8266) & Dual-Core Xtensa (ESP32)
- ESP8266 memiliki satu core Xtensa LX106.
- ESP32 memiliki dual-core Xtensa LX6, sehingga bisa melakukan multitasking lebih efisien.
- Control Unit dalam CPU menangani eksekusi instruksi dan mengatur pipeline processing.

#### 2. Memory & Cache Controller
- ESP memiliki SRAM terbatas (~520 KB di ESP32), sehingga sering menggunakan Flash eksternal.
- Memori dikontrol menggunakan cache untuk meningkatkan efisiensi akses data.

#### 3. Wi-Fi & Bluetooth Controller
- ESP8266 hanya mendukung Wi-Fi, sementara ESP32 mendukung Wi-Fi + Bluetooth.
- Modul komunikasi ini memiliki dedicated control unit untuk menangani koneksi jaringan.

#### 4. GPIO & Peripheral Control Unit
- Seperti Raspberry Pi, ESP memiliki GPIO, I2C, SPI, dan UART.
- ESP32 memiliki lebih banyak peripheral, termasuk DAC, ADC, dan PWM untuk kontrol sensor dan aktuator.

#### 5. Power Management Unit (PMU)
- ESP dirancang untuk aplikasi low power, sehingga memiliki berbagai mode hemat daya seperti Deep Sleep dan Light Sleep.
