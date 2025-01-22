# Nmap-Prompt
#Prompt/Command	Fungsi
nmap <IP>	                      Melakukan scan port default pada target.
nmap -sS <IP>	                  Melakukan Stealth Scan (SYN scan).
nmap -sT <IP>	                  Melakukan TCP Connect Scan (alternatif jika SYN scan tidak tersedia).
nmap -sU <IP>	                  Melakukan UDP Scan pada target.
nmap -p <port> <IP>	            Scan port tertentu saja.
nmap -p- <IP>	                  Scan semua port (1–65535).
nmap -A <IP>	                  Scan lengkap dengan deteksi OS, versi, script, dan traceroute.
nmap -O <IP>	                  Deteksi sistem operasi (OS detection).
nmap -sV <IP>	                  Mendeteksi versi layanan yang berjalan di port terbuka.
nmap -Pn <IP>	                  Scan tanpa melakukan ping. Berguna jika ping diblokir.
nmap -T4 <IP>	                  Mempercepat proses scanning (agresif).
nmap -T0 <IP>	                  Memperlambat proses scanning untuk stealth (very slow).
nmap -sC <IP>	                  Menjalankan skrip default pada target.
nmap --script=<script> <IP>	    Menjalankan skrip spesifik (NSE Script).
nmap -oN output.txt <IP>	      Menyimpan hasil scan dalam format teks biasa.
nmap -oX output.xml <IP>	      Menyimpan hasil scan dalam format XML.
nmap -oG output.grep <IP>      	Menyimpan hasil scan dalam format grepable.
nmap --top-ports <number> <IP>	Scan sejumlah port yang paling umum digunakan.
nmap -6 <IPv6>	                Scan target dengan alamat IPv6.
nmap --traceroute <IP>	        Melacak jalur paket ke target.
nmap -v <IP>	                  Menampilkan hasil scanning secara rinci (verbose mode).
nmap -sW <IP>                  	Melakukan Window Scan untuk mendeteksi port terbuka.
nmap -sI <zombie_host> <IP>	    Melakukan Idle Scan (stealthy and untraceable).
nmap -D RND:10 <IP>	            Menggunakan decoy scan dengan 10 IP palsu untuk menyamarkan identitas.
nmap -f <IP>	                  Mengaktifkan fragmentasi paket untuk melewati firewall.
nmap --script=vuln <IP>        	Mendeteksi kerentanan yang diketahui pada target.
