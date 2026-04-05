# Smart Car 4WD - Phase 1: Logic & UI Simulation

Bagian ini merupakan tahap awal pengembangan sistem kendali mobil pintar 4WD. Fokus utama fase ini adalah membangun antarmuka pengguna (UI) yang responsif dan memverifikasi logika kendali sebelum diimplementasikan ke perangkat keras (ESP32).

## 🎮 Antarmuka Kendali (UI)
Simulasi ini menggunakan dashboard berbasis web untuk mengirimkan instruksi ke sistem. Berikut adalah visualisasi status sistem:

| Status: OFF | Status: ON |
|---|---|
| ![Sistem Matikan](./Saat%20tombol%20OFF.jpeg) | ![Sistem Hidup](./Saat%20Tombol%20ON.jpeg) |

### Penjelasan Logika:
1. **Status OFF:** Sistem dalam keadaan *idle*. Semua output GPIO pada simulasi disetel ke logika `LOW`.
2. **Status ON:** Menandakan koneksi WebSockets aktif. Antarmuka siap mengirimkan data koordinat atau perintah pergerakan ke motor driver.

## 🛠️ Teknologi yang Digunakan
* **Web Interface:** HTML5 & CSS3 (Dashboard Design).
* **Protocol:** WebSockets (Experimental) untuk komunikasi data dua arah.
* **Simulation Environment:** Perancangan logika UI sebelum *deployment* ke ESP32.

---
*Proyek ini masih dalam tahap pengembangan (Work In Progress).*
