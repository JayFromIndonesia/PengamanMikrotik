# PengamanMikrotik

Mengamankan Mikrotik dari serangan luar pakai ip publik.<br>
Target : BruteForces, DDOS, dll.<br>

Silakan Copy/Salin script yang ada di SCRIPT-TERMINAL kemudian Paste/Tempel ke dalam Terminal di mikrotik anda.<br>
Kemudian lanjut ke step yang keempat, jika masih kurang paham ikuti perintah dibawah ini.<br>

<b>Pertama</b> : <br>
Copy Paste script ini ke terminal mikrotik <br>
/system logging action add name=failedauth target=memory <br>
/system logging add action=failedauth topics=critical,system,error

<b>Kedua :</b> <br>
Copy Paste script ini ke terminal mikrotik <br>
/ip firewall filter add action=drop chain=input comment="Drop Attempt Login User" disabled=no src-address-list="IP-DDOS-BLOCKED"

<b>Ketiga :</b> <br>
Buka Mikrotik <br>
<b><i>=> System => Scheduler</i></b>  <br>
Tambah Schedule baru, name = <i>IP-DDOS-BLOCKED</i> <br>
Sesuaikan interval nya, rekomendasi per 5 menit. <br>
Buka file <i>SCHEDULER-IP-DDOS.txt</i> <br>
Copy Paste ke Source pada <i>SCHEDULER-IP-DDOS</i> <br>
Apply/simpan<br>
<b><i>=> System => Scripts</i></b>  <br>
Tambah Scripts baru, name = <i>FUNCTIONS</i> <br>
Buka file <i>FUNCTIONS.txt</i> <br>
Copy Paste ke Source pada <i>FUNCTIONS</i> <br>
Apply/simpan<br>

<b>Keempat :</b> <br>
Silakan test pakai IP GSM, <br>
biar mudah gonta ganti ip nya, <br>
cukup dengan mode pesawat on terus mode pesawat off <br>
biar ip GSM berubah lagi. <br>

TAMBAHAN :  <br>
Segala resiko di tanggung sendiri ya, <br>
saya sarankan untuk bagian  <br>
<b>failthreshold 0</b> nya agar lebih banyak,  <br>
untuk menghindari kalo kita gagal input password.

Info lebih lanjut hubungi via WA https://wa.me/6281914005555 (RADITEK GROUP)
