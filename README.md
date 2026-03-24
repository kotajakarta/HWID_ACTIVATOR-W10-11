# Windows 10/11 HWID Activation (Standalone & Improved)

Alat aktivasi Windows berbasis Batch dan PowerShell yang menggunakan metode **HardwareID (HWID)**. Metode ini memberikan aktivasi permanen yang tetap bertahan meskipun Anda melakukan instalasi ulang Windows (Digital License), karena lisensi terikat pada hardware komputer Anda.

## ✨ Fitur Utama
- **Permanen**: Aktivasi tetap ada setelah instalasi ulang.
- **Aman & Bersih**: Tidak memerlukan KMS atau crack eksternal, hanya menggunakan metode native Windows.
- **Cepat**: Proses otomatis dalam satu klik melalui skrip `.cmd`.
- **Tanpa File Eksternal**: Skrip berjalan secara mandiri (Standalone) dan mengeksekusi perintah langsung di memori.

## 📋 Edisi Windows yang Didukung
Skrip ini mendukung berbagai edisi Windows 10 dan 11, antara lain:
- **Professional / Professional N**
- **Enterprise / Enterprise N**
- **Education / Education N**
- **Core (Home) / Core N**
- **Core Single Language / Country Specific**
- **Pro for Workstations / Pro Education**

## 🚀 Cara Penggunaan
1. Unduh atau salin file `Hwid.cmd`.
2. Klik kanan pada file `Hwid.cmd`.
3. Pilih **Run as Administrator**.
4. Tunggu proses pendeteksian OS dan penginstalan kunci produk selesai.
5. Skrip akan otomatis membuat `GenuineTicket.xml` dan melakukan aktivasi ke server Microsoft.
6. Selesai! Windows Anda sekarang teraktivasi secara permanen.

## 🛠️ Cara Kerja
1. **Hak Akses**: Memastikan skrip berjalan dengan hak Administrator.
2. **Deteksi SKU**: Mengidentifikasi edisi Windows yang sedang digunakan menggunakan CIM/WMI.
3. **Pemasangan Key**: Memasukkan *Generic Product Key* yang sesuai dengan edisi OS.
4. **Generate Tiket**: Membuat tiket lisensi hardware (`GenuineTicket.xml`) menggunakan injeksi RSA.
5. **Aktivasi**: Memicu layanan `ClipSVC` dan `clipup.exe` untuk mendaftarkan lisensi ke Microsoft.

## ⚠️ Catatan
- Pastikan koneksi internet aktif untuk proses aktivasi ke server Microsoft.
- Skrip ini ditujukan untuk tujuan edukasi dan penggunaan pribadi.