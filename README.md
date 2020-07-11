# PengamanMikrotik

Mengamankan Mikrotik dari serangan luar pakai ip publik.

Pertama :
Buka file Konfigurasi
Copy paste ke terminal mikrotik.

Kedua :
Buka Mikrotik
> System > Scheduler 
Tambah Schedule baru (CekUserGagalLogin)
Sesuaikan interval nya, rekomendasi per 5 menit.
Buka file CekUserGagalLogin
Copy Paste ke Source pada CekUserGagalLogin
Apply/simpan

Ketiga :
Copy Paste script ini ke terminal mikrotik
/ip firewall filter add action=drop chain=input comment="Drop Attempt Login User" disabled=no src-address-list=IP_BlackList

KeEmpat :
Silakan test pakai IP GSM,
biar mudah gonta ganti ip nya,
cukup dengan mode pesawat on terus mode pesawat off
biar ip GSM berubah lagi.

Info lebih lanjut hubungi via WA https://wa.me/6287776319666 (Jay Nudin)
