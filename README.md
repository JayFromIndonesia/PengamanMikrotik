# PengamanMikrotik

Mengamankan Mikrotik dari serangan luar pakai ip publik.<br>
Target : BruteForces, DDOS, dll.<br>

Silakan Copy/Salin script yang ada di SCRIPT-TERMINAL kedalam terminal di mikrotik anda.<br>
Kemudian lanjut ke step Keempat<br>

Pertama : <br>
Copy Paste script ini ke terminal mikrotik <br>
/system logging action add name=failedauth target=memory <br>
/system logging add action=failedauth topics=critical,system,error

Kedua : <br>
Copy Paste script ini ke terminal mikrotik <br>
/ip firewall filter add action=drop chain=input comment="Drop Attempt Login User" disabled=no src-address-list="IP-DDOS-BLOCKED"

Ketiga : <br>
Buka Mikrotik <br>
=> System => Scheduler  <br>
Tambah Schedule baru, name = IP-DDOS-BLOCKED <br>
Sesuaikan interval nya, rekomendasi per 5 menit. <br>
Buka file SCHEDULER-IP-DDOS.txt <br>
Copy Paste ke Source pada SCHEDULER-IP-DDOS <br>
Apply/simpan

Keempat : <br>
Silakan test pakai IP GSM, <br>
biar mudah gonta ganti ip nya, <br>
cukup dengan mode pesawat on terus mode pesawat off <br>
biar ip GSM berubah lagi. <br>

TAMBAHAN :  <br>
Segala resiko di tanggung sendiri ya, <br>
saya sarankan untuk bagian  <br>
<b>failthreshold 0</b> nya agar lebih banyak,  <br>
untuk menghindari kalo kita gagal input password.

Info lebih lanjut hubungi via WA https://wa.me/6287776319666 (Jay Nudin)
