# Armbian_Autorun_Verus_miner.sh
How to install
1. open terminal armbiannya.
2. type perintah dibawah 
```
wget -L https://raw.githubusercontent.com/psky/verus-auto-armbian/main/miner.sh
```
4. edit file miner.sh yang telah didownload sebelumnya.
```
nano miner.sh
```
  - wallet = ganti dengan wallet address verus kalian
  - workername = nama worker yang akan digunakan. Contoh : node-01
5. Save and quit
6. ketik command dibawah di terminal, untuk edit crontab
```
crontab -e
```
7. Tambahkan script dibawah
```
@reboot bash /root/miner.sh > /root/miner.log 2>&1
```
8. Save dan quit.

NB:Semua file Harus dlm posisi Root
