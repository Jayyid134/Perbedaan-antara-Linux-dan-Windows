# Bagian yang dapat dikontrol pada unit kontrol Mikrokontroler(ESP32)
![image](https://github.com/user-attachments/assets/a26c3b9e-6c53-4d95-9aea-683a114dff0e)

Berikut adalah beberapa hal yang dapat dikontrol oleh Control Unit dalam ESP (ESP8266/ESP32):

## 1. CPU (Central Processing Unit)
Kecepatan clock CPU: Control Unit mengatur frekuensi clock CPU untuk mengoptimalkan kinerja dan konsumsi daya. Pada ESP32, CPU memiliki dua core yang dapat bekerja secara paralel, dan Anda dapat mengatur bagaimana keduanya beroperasi.
Mode operasi CPU: Mengatur apakah CPU beroperasi dalam mode aktif atau mode tidur (sleep mode) untuk menghemat daya.
## 2. Memori
RAM (Random Access Memory): Control Unit mengelola akses ke memori internal seperti SRAM (yang digunakan untuk penyimpanan data sementara selama proses berjalan).
Flash memory: Mengelola akses ke Flash memory eksternal yang digunakan untuk menyimpan program (firmware) dan data lainnya.
Pengaturan Cache: Mengelola pengaturan cache untuk mempercepat akses ke memori yang sering digunakan.
## 3. Mode Daya (Power Management)
Mode tidur (sleep modes): ESP memiliki beberapa mode tidur untuk menghemat daya, seperti deep sleep dan light sleep. Control Unit mengatur transisi antara mode tidur dan mode aktif berdasarkan kebutuhan.
Pengaturan daya untuk peripheral: Mengontrol konsumsi daya oleh peripheral seperti Wi-Fi, Bluetooth, GPIO, dan lainnya.
## 4. Wi-Fi dan Bluetooth (Jaringan)
Wi-Fi Management: Mengatur pengaturan Wi-Fi pada ESP32, termasuk penghubungan ke jaringan, pengaturan IP address, keamanan jaringan (WPA2, dll.), dan pengaturan mode (Access Point / Station).
Bluetooth: Pada ESP32, kontrol Bluetooth memungkinkan pengelolaan penghubungan perangkat Bluetooth dan komunikasi data melalui Bluetooth Classic atau Bluetooth Low Energy (BLE).
Pengaturan kanal dan frekuensi: Control Unit juga mengatur kanal Wi-Fi yang digunakan dan pengaturan frekuensi untuk transmisi data.
## 5. GPIO (General Purpose Input/Output)
Pengendalian GPIO: Control Unit mengelola pin GPIO yang digunakan untuk input atau output digital (misalnya untuk menghubungkan sensor atau aktuator).
PWM (Pulse Width Modulation): Mengontrol penggunaan PWM pada pin GPIO untuk mengatur kekuatan sinyal (misalnya untuk motor atau pengaturan kecerahan LED).
ADC (Analog to Digital Converter): Mengontrol pembacaan sinyal analog melalui pin ADC untuk membaca sensor atau sinyal analog lainnya.
I2C, SPI, UART: Control Unit mengelola komunikasi antar perangkat menggunakan antarmuka I2C, SPI, dan UART. Ini termasuk pengaturan kecepatan komunikasi, mode, dan pengelolaan buffer data.
## 6. Timer dan Interrupts
Pengaturan Timer: Control Unit dapat mengatur timer untuk operasi berulang, atau untuk mengatur waktu tunda (delays).
Interrupt Handling: Mengelola interrupts (sinyal atau event yang membutuhkan perhatian segera), memungkinkan eksekusi kode ketika terjadi event tertentu, misalnya sensor mendeteksi perubahan atau sinyal dari perangkat eksternal.
## 7. Sistem Jaringan dan Pengaturan Protokol
TCP/IP Stack: Mengatur komunikasi jaringan berbasis TCP/IP, yang memungkinkan ESP untuk berkomunikasi dengan server atau perangkat lain di jaringan.
Protokol komunikasi: Mengelola berbagai protokol komunikasi seperti HTTP, MQTT, WebSockets, dan lainnya yang digunakan untuk aplikasi IoT.
## 8. Pengaturan Periferal Lainnya
DAC (Digital to Analog Converter): Pada beberapa model ESP32, terdapat DAC yang memungkinkan mengubah sinyal digital menjadi sinyal analog (misalnya untuk pengontrol suara atau output audio).
Sensor & Aktuator: Control Unit mengelola komunikasi dan pengaturan sensor (seperti suhu, kelembaban, gerak, dll.) serta aktuator (motor, servo, dll.) yang terhubung ke perangkat.
## 9. Keamanan
Enkripsi: Control Unit dapat mengelola enkripsi untuk komunikasi aman melalui jaringan (misalnya TLS/SSL untuk komunikasi Wi-Fi).
Bootloader dan Firmware: Mengatur proses booting, serta update firmware (pembaruan perangkat lunak) secara aman melalui metode seperti OTA (Over-The-Air).
