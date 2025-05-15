# 🧠 100 Komend w Kali Linux (z opisem)

---

## 1️⃣ Podstawowe polecenia systemowe

1. `pwd` – pokaż bieżący katalog
2. `ls -la` – lista plików z ukrytymi
3. `cd folder` – przejdź do folderu
4. `mkdir folder` – stwórz katalog
5. `touch plik.txt` – stwórz pusty plik
6. `rm plik` – usuń plik
7. `rm -rf katalog` – usuń katalog i zawartość
8. `cp a.txt b.txt` – kopiuj plik
9. `mv a.txt b.txt` – przenieś/zmień nazwę
10. `file plik` – sprawdź typ pliku
11. `cat plik` – wyświetl zawartość
12. `less plik` – podgląd z przewijaniem
13. `head -n 10` – pierwsze 10 linii
14. `tail -n 10` – ostatnie 10 linii
15. `tree` – struktura katalogów
16. `find . -name "*.txt"` – szukaj plików
17. `locate passwd` – szybkie znajdowanie
18. `df -h` – przestrzeń dyskowa
19. `du -sh katalog` – rozmiar katalogu
20. `history` – historia poleceń

---

## 2️⃣ Zarządzanie użytkownikami i uprawnieniami

21. `whoami` – obecny użytkownik
22. `id` – UID, GID i grupy
23. `adduser test` – dodaj użytkownika
24. `passwd test` – zmień hasło
25. `usermod -aG sudo test` – dodaj do sudo
26. `su test` – przełącz użytkownika
27. `sudo su` – root jako sudo
28. `groups` – pokaż grupy
29. `chmod 755 plik` – zmień uprawnienia
30. `chown user:user plik` – zmień właściciela

---

## 3️⃣ Sieć i połączenia

31. `ip a` – adresy IP
32. `ip r` – trasy routingu
33. `ping 1.1.1.1` – sprawdź połączenie
34. `netstat -tulnp` – aktywne porty
35. `ss -tuln` – aktywne sockety
36. `ifconfig` – stare info o interfejsach
37. `iwconfig` – sieci Wi-Fi
38. `curl ifconfig.me` – sprawdź zewnętrzne IP
39. `host google.com` – rozwiązywanie DNS
40. `dig +short google.com` – szybkie DNS

---

## 4️⃣ Narzędzia bezpieczeństwa (część 1)

41. `nmap -sV -A IP` – skan usług i OS
42. `netcat -lvnp 4444` – nasłuch
43. `nc IP 4444` – połącz do portu
44. `hydra -l admin -P passlist.txt IP http-get` – brute force
45. `john hash.txt --wordlist=rockyou.txt` – łamanie haseł
46. `hash-identifier` – rozpoznanie hasha
47. `sqlmap -u URL --dbs` – SQLi automatycznie
48. `gobuster dir -u http://IP -w wordlist.txt` – brute katalogów
49. `wpscan --url http://site` – test WordPress
50. `nikto -h http://site` – skaner podatności HTTP

---

## 5️⃣ Narzędzia bezpieczeństwa (część 2)

51. `msfconsole` – uruchom metasploit
52. `searchsploit apache` – exploit-db lokalnie
53. `exploit-db` – katalog exploitów (strona)
54. `dirb http://site` – fuzzowanie katalogów
55. `burpsuite` – uruchom Burpa
56. `ftp IP` – połącz FTP
57. `telnet IP port` – połącz telnet
58. `rpcinfo -p IP` – info o usługach RPC
59. `enum4linux IP` – enumeracja SMB
60. `smbclient //IP/share` – dostęp do udziału

---

## 6️⃣ Procesy i usługi

61. `ps aux` – aktywne procesy
62. `top` – monitorowanie procesora
63. `htop` – lepsze `top`
64. `kill PID` – zakończ proces
65. `killall nazwa` – zakończ wszystkie z nazwą
66. `systemctl status` – status usług
67. `systemctl restart apache2` – restart usługi
68. `journalctl` – logi systemowe
69. `service ssh start` – uruchom SSH
70. `crontab -l` – lista zadań cron

---

## 7️⃣ Logi i monitoring

71. `dmesg` – log jądra
72. `tail -f /var/log/syslog` – obserwuj logi
73. `uptime` – ile system działa
74. `last` – historia logowań
75. `who` – kto jest zalogowany
76. `w` – aktywność użytkowników
77. `env` – zmienne środowiskowe
78. `alias` – pokaż aliasy
79. `uname -a` – wersja kernela
80. `lsb_release -a` – wersja systemu

---

## 8️⃣ Kali Linux – specjalistyczne

81. `airmon-ng` – Wi-Fi monitorowanie
82. `airodump-ng wlan0mon` – sniffer Wi-Fi
83. `aircrack-ng capture.cap -w wordlist.txt` – łamanie WPA
84. `ettercap -G` – sniffing GUI
85. `bettercap -iface wlan0` – sniffing CLI
86. `responder -I eth0` – ataki na sieć Windows
87. `tcpdump -i eth0` – przechwytywanie ruchu
88. `mitmproxy` – proxy MITM
89. `proxychains nmap -sT site.com` – przez proxy
90. `setoolkit` – ataki socjotechniczne

---

## 9️⃣ Przydatne tipy i narzędzia

91. `alias ll='ls -la'` – alias
92. `history | grep nmap` – filtruj historię
93. `!!` – ostatnie polecenie
94. `!n` – polecenie nr z historii
95. `Ctrl + R` – przeszukaj historię
96. `man nmap` – manual
97. `--help` – pomoc narzędzia
98. `clear` – wyczyść terminal
99. `exit` – wyjście z powłoki
100. `reboot` – restart systemu

