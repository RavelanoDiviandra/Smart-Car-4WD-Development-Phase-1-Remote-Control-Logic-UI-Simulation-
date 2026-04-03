# ESP32 WebSocket GPIO Controller (Proof of Concept)

Sistem ini dirancang untuk melakukan kendali perangkat keras jarak jauh secara real-time melalui jaringan nirkabel lokal menggunakan protokol WebSockets. 

### Development Status: Phase 1
Proyek saat ini berada pada tahap **Validasi Komunikasi Real-Time**. 
- **Physical Output:** Disimulasikan menggunakan LED pada GPIO 16 & 17 (Logika Maju/Mundur).
- **UI/UX Simulation:** Fitur 'Speed Control' dan tombol arah lainnya pada antarmuka web telah diimplementasikan sebagai bagian dari pengembangan UI masa depan (Phase 2), namun saat ini belum terhubung ke beban aktuator mekanis.

## Arsitektur Sistem
Sistem beroperasi pada Mode Station (STA) dan mendelegasikan perintah dari antarmuka web (HTML/JS) ke GPIO ESP32 tanpa jeda (zero latency).
