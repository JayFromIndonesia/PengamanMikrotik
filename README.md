# PengamanMikrotik

Mengamankan Mikrotik dari serangan luar pakai ip publik.
BruteForces, DDOS, Dll.

Pertama : <br>
Buka file Konfigurasi <br>
Copy paste ke terminal mikrotik.

Kedua : <br>
Buka Mikrotik <br>
=> System => Scheduler  <br>
Tambah Schedule baru (CekUserGagalLogin) <br>
Sesuaikan interval nya, rekomendasi per 5 menit. <br>
Buka file CekUserGagalLogin <br>
Copy Paste ke Source pada CekUserGagalLogin <br>
Apply/simpan <br>

Ketiga : <br>
Copy Paste script ini ke terminal mikrotik <br>
/ip firewall filter add action=drop chain=input comment="Drop Attempt Login User" disabled=no src-address-list=IP_BlackList

KeEmpat : <br>
Silakan test pakai IP GSM, <br>
biar mudah gonta ganti ip nya, <br>
cukup dengan mode pesawat on terus mode pesawat off <br>
biar ip GSM berubah lagi. <br>

Info lebih lanjut hubungi via WA https://wa.me/6287776319666 (Jay Nudin)
