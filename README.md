# Indihome Hash Decrypter Generator

> **Peringatan:** :red_circle: Aplikasi ini dibuat khusus untuk keperluan pendidikan dan penelitian. Penulis tidak bertanggung jawab atas segala bentuk penyalahgunaan atau kerusakan yang mungkin timbul dari penggunaan program ini. Harap gunakan dengan bijak dan hanya di lingkungan di mana Anda memiliki izin eksplisit.

Aplikasi Indihome Hash Decrypter Generator adalah perangkat lunak yang dapat digunakan untuk menghasilkan (generate) atau mencoba membalikkan (decrypt) hash menjadi teks asli. Fungsi aplikasi ini dibagi menjadi dua bagian utama:

1. Hash Generator
- Mengubah teks biasa (plaintext) menjadi hash menggunakan algoritma seperti MD5, SHA-1, SHA-256, SHA-512, CRC32, dan lainnya.
- Hash ini bersifat one-way (tidak bisa dikembalikan secara langsung), sering digunakan untuk keamanan seperti penyimpanan password atau verifikasi data.

2. Hash Decrypter
- Mencoba menemukan teks asli dari sebuah hash.
- Karena hashing adalah proses satu arah, "dekripsi" dalam konteks ini biasanya dilakukan dengan rainbow tables, dictionary attacks, atau brute-force.
- Beberapa aplikasi mencari hash yang cocok di database hash yang telah dikompilasi sebelumnya.

Contoh Penggunaan:

- Keamanan IT → Untuk memverifikasi integritas file atau password.
- Penetration Testing → Digunakan oleh pentester untuk menguji keamanan sistem.
- Forensik Digital → Menelusuri hash dari file atau password yang telah dienkripsi.

Aplikasi seperti Hashcat, John the Ripper, atau layanan online seperti CrackStation sering digunakan untuk mencoba membalikkan hash ke teks aslinya.

~ (v1.0.0.1) Kamis 6 Februari 2025 - First Release Indihome Hash Decrypter Generator by Xtreme's

#
<b>[ Cara Menggunakan Indihome Hash Decrypter Generator ]</b>

1. Download IHDG via: https://codeload.github.com/MichaelJorky/Indihome-Hash-Decrypter-Generator/zip/refs/heads/main
2. Kemudian silahkan akses IP Router misal: 192.168.1.1 lalu arahkan mouse pada kolom password lalu klik kanan pilih "Inspect" lalu copy element id misal:Frm_Password {ZTE}, Txt_Password {Huawei} lalu tekan CTRL+U lalu CTRL+F search misal: Frm_Password lalu temukan misal yang seperti ini: var SHA256Password =sha256(Password+xmlObj); maka diaplikasi IHDG yang dipilih harus "Enabled SHA256 Algoritms".
3. Petunjuk pengisian pada aplikasi
- Edit Unix Time misal: 59438044
- Edit Signature misal: F670L
- Edit Serial Number misal: ZTEGcanr9631
- Edit Mac Address misal: D7:4E:09:4C:57:F2
- Edit Public Key Misal: Telkomdso123
- Edit Customer ID misal: 124716254913
- Edit Secret Key misal: telkomselbrn5
4. Selanjutnya buka Aplikasi "Fiddler" (Cari di google), lalu pilih "Browse → Chrome" (tinggal disesuaikan dengan kebutuhan).
5. Dalam keadaan aplikasi IHDG terbuka silahkan login ke router misalkan IP Router 192.168.1.1 user: user password: user1234 (Tinggal disesuaikan untuk login usernya).
6. Selanjutnya perhatikan pada log Fiddler temukan URL misal: http://{router_ip}/?_type=loginData&_tag=login_token&_={Unix_Timestamp} lalu klik pada bagian "WebView" lalu copy angka yang muncul misal: 59438044 lalu silahkan paste di unix time pada aplikasi IHDG.
7. Masih di log Fiddler selanjutnya cari misal: http://{router_ip}/?_type=loginData&_tag=login_entry lalu copy password yang muncul pada bagian body misal: f6c1479b56ebe0345e1b370640b74d77e6b09c41c3c8412a542adc2167ec3b6e (SHA256Password =sha256(Password+xmlObj);) secara default {unix_time_algoritms} bisa didapat di http://{router_ip}/function_module/login_module/login_page/logintoken_lua.lua?_={unix_time}.
8. Selanjutnya klik "Generate Hash Encryption!" di Aplikasi IHDG lalu search f6c1479b56ebe0345e1b370640b74d77e6b09c41c3c8412a542adc2167ec3b6e pada aplikasi IHDG jika pencarian hash tidak ditemukan silahkan coba ulangi sampai mendapatkan hash yang cocok, jika sudah mendapatkan hash yang cocok silahkan klik "Generate Hash Decryption!".
9. MD5 Result & HMAC-MD5 Result ini adalah login level 2 {tergantung versi dan type}, SHA256 Result & HMAC-SHA256 Result ini adalah login level 1 {tergantung versi dan type serta secret key}.

#
Just tested on ZTE F670L Software Version: V9.0.11P1N15 and V9.0.11P1N84A
