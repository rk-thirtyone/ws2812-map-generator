# LED Map Designer

Tool interaktif buat desain layout custom LED matrix (WS2812 / NeoPixel) langsung dari browser. Klik buat nandain bentuk panel, penomoran index dibuat otomatis mengikuti pola zigzag/ular sesuai wiring fisik strip LED — hasilnya langsung jadi array `map2D` yang siap paste ke kode Arduino.

🔗 **Demo:** https://rk-thirtyone.github.io/led-map-designer/

## Fitur

- **Ukuran custom** — atur jumlah baris & kolom sesuai bentuk panel LED kamu.
- **Klik buat nandain LED** — gak perlu klik berurutan, tinggal tandain bentuknya.
- **Penomoran zigzag otomatis** — pilih mode "Per Kolom" atau "Per Baris", plus titik mulai (atas/bawah, kiri/kanan) biar cocok sama arah solder fisik strip.
- **Preview animasi (chase)** — ngecek urutan nyala LED sebelum di-upload ke board.
- **Zoom grid** — perbesar/perkecil kotak biar tetap enak diklik di panel besar.
- **Export langsung** — output berupa `#define NUM_LEDS`, `#define ROWS/COLS`, dan array `map2D` siap copy-paste.

## Cara Pakai

1. Isi jumlah **ROWS** dan **COLS**, klik **Buat Grid Baru**.
2. Klik kotak-kotak sesuai bentuk panel LED kamu.
3. Pilih **Pola Zigzag** (Per Kolom / Per Baris) dan titik mulainya, sesuaikan sampai penomoran cocok dengan wiring fisik.
4. Tekan **▶ Play** buat preview animasi urutan nyala LED-nya.
5. Copy hasil di kotak **Output**, tempel ke kode `.ino` kamu.

## Teknis

Single-file HTML — tidak ada dependency eksternal (semua CSS & JS inline), jadi bisa langsung dibuka dari file lokal atau di-hosting di mana saja (GitHub Pages, dll).

---
Bagian dari [RK-Thirtyone Tools](https://rk-thirtyone.github.io/)
