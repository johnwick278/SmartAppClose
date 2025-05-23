![SmartAppClose Logo](./smarappcloselogos.png)

## Smart App Close (Gaming Mode)

## Apa Fungsi Modul Ini?

Smart App Close adalah modul berbasis Magisk/KernelSU yang dirancang khusus untuk **memaksimalkan performa gaming** di perangkat Android dengan cara **menutup aplikasi-aplikasi latar belakang secara otomatis saat kamu membuka game**. Modul ini sangat berguna untuk pengguna dengan RAM terbatas yang ingin menghindari lag atau delay saat bermain game.

Modul ini bekerja secara otomatis tanpa perlu aplikasi tambahan atau task killer, cukup edit file konfigurasi whitelist dan gamelist sesuai kebutuhanmu.

---

## Bagaimana Cara Kerjanya?

1. **Deteksi Game Aktif**  
   Modul memonitor aplikasi foreground dan membandingkannya dengan daftar package di `gamelist.txt`.

2. **Filter Aplikasi Penting**  
   Aplikasi yang ada di `whitelist.txt` tidak akan di-close, sehingga app penting tetap aman.

3. **Force-Close App Latar Belakang**  
   Saat game dari gamelist aktif, modul akan menutup semua aplikasi lain yang tidak termasuk whitelist untuk membebaskan RAM dan resource.

4. **Loop Aktif 24/7**  
   Modul terus berjalan di background melalui script `service.sh`, dan akan auto-reload konfigurasi pada versi terbaru tanpa butuh reboot.

---

## Kelebihan:
- Performa gaming meningkat signifikan
- RAM jadi lebih lega tanpa bloatware
- Ringan dan tidak memerlukan akses UI
- Bisa digunakan di semua jenis ROM: AOSP, MIUI, HyperOS, dll

---

## Cara Penggunaan
1. Flash modul via Magisk / KernelSU / KernelSU Next
2. Reboot device
3. Akses:
   ```
   /data/adb/modules/smartappclose/system/etc/smartappclose/
   ```
4. Edit file:
   - `whitelist.txt`: aplikasi yang tidak ingin ditutup
   - `gamelist.txt`: aplikasi game yang memicu clean
5. Enjoying Gaming

---

## Info:
- `whitelist.txt` = Daftar app yang **tidak ingin di-kill**
- `gamelist.txt` = Daftar game yang **akan memicu pembersihan**

---

## ⚠️ Untuk Android 11 Users ⚠️
Jika mengalami error saat install, [klik di sini](./for_Android_11.md)

---

## Download

Kamu bisa mengunduh semua versi modul dari halaman rilis resmi berikut:  
[**DOWNLOAD**](https://github.com/johnwick278/SmartAppClose/releases)

---

## Dibuat oleh
[@unknuw](https://t.me/unknuw) x [ChatGPT](https://chat.openai.com/)
