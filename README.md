# experiment

Folder `experiment` berisi beberapa proof-of-concept dan skrip HTA/Powershell yang digunakan untuk pengujian atau eksploitasi pada lingkungan Windows.




## Isi folder

- `cobalagi.hta` - skrip VBScript HTA yang membuka file lokal dan mengirimkan isinya ke server web melalui HTTP GET.
- `revshell.hta` - HTA yang menjalankan `powershell` untuk mendownload dan menjalankan `shell.ps1` dari server jarak jauh.
- `shell.ps1` - skrip Powershell reverse shell yang membuka koneksi ke server dan menyediakan shell interaktif balik.
- `test.hta` - HTA sederhana yang menampilkan pesan `Halo! Ini dijalankan via mshta.exe` sebagai PoC.
- `coba/` - subfolder yang berisi file tambahan terkait eksperimen.
  - `coba/baka.hta` - HTA dengan VBScript untuk membaca file lokal dan mengekfiltrasi data ke server.
  - `coba/note.txt` - catatan atau informasi tambahan terkait eksperimen.

## Catatan penting

- Skrip ini ditujukan untuk tujuan riset, pengujian, atau pembelajaran.
- Skrip hanya bisa bekerja jika realtime protection windows defender dimatikan
- Jangan menjalankan file-file ini pada sistem produksi atau tanpa izin yang jelas.
- Beberapa file menggunakan koneksi jaringan ke alamat IP yang tersimpan secara hardcoded; sesuaikan atau nonaktifkan bila diperlukan.
