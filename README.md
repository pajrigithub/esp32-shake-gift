
# 🎁 esp32-shake-gift

**esp32-shake-gift** adalah proyek berbasis **ESP32** yang menampilkan gambar-gambar lucu pada **layar TFT ST7789** saat perangkat digoyangkan. Cocok sebagai hadiah unik dan interaktif yang memberikan kejutan menyenangkan setiap kali digoyang!

## ✨ Fitur

- Menggunakan sensor **MPU6050** untuk mendeteksi gerakan atau getaran.
- Menampilkan gambar secara acak di **layar TFT 240x240 ST7789**.
- Desain sederhana, cocok sebagai hadiah digital kreatif.

## 🧰 Komponen yang Digunakan

- ESP32
- MPU6050 (Accelerometer & Gyroscope)
- TFT LCD ST7789 240x240 (SPI interface)
- Breadboard dan kabel jumper
- File gambar dalam format `.h`

## ⚙️ Cara Kerja

1. Saat perangkat diam, layar menampilkan gambar standby.
2. Ketika ESP32 digoyangkan, sensor MPU6050 mendeteksi perubahan akselerasi.
3. Gambar-gambar lucu akan langsung muncul dan berganti secara acak di layar TFT.

## 🔌 Wiring

| ESP32 Pin | Komponen         |
|-----------|------------------|
| 3.3V      | VCC MPU6050 & VCC TFT |
| GND       | GND MPU6050 & GND TFT |
| SDA (21)  | SDA MPU6050      |
| SCL (22)  | SCL MPU6050      |
| GPIO 5    | CS TFT           |
| GPIO 18   | SCL TFT          |
| GPIO 23   | MOSI TFT         |
| GPIO 2    | DC TFT           |
| GPIO 4    | RESET TFT        |

> ⚠️ Pastikan pin sesuai dengan konfigurasi library TFT_eSPI Anda.

## 🚀 Instalasi

1. Clone repositori ini:
   ```bash
   git clone https://github.com/username/esp32-shake-gift.git
   ```
2. Buka folder proyek di Arduino IDE atau PlatformIO.
3. Pastikan library berikut telah terinstal:
   - TFT_eSPI
   - Wire
   - MPU6050 (by Ewan Leng)
4. Upload ke ESP32 dan sambungkan sesuai wiring.

## 📸 Contoh Gambar

Tambahkan gambar-gambar favorit Anda dalam format header `.h`, kemudian sertakan dalam kode untuk ditampilkan saat digoyangkan.


## 📄 Lisensi

Proyek ini menggunakan lisensi MIT. Silakan gunakan, modifikasi, dan distribusikan dengan bebas.

---

Made with ❤️ for fun and surprise!
