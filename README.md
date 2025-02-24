# Indihome Hash Decrypter Generator

> **Peringatan:** :red_circle: Aplikasi ini dibuat khusus untuk keperluan pendidikan dan penelitian. Penulis tidak bertanggung jawab atas segala bentuk penyalahgunaan atau kerusakan yang mungkin timbul dari penggunaan program ini. Harap gunakan dengan bijak dan hanya di lingkungan di mana Anda memiliki izin eksplisit.

Aplikasi Indihome Hash Decrypter Generator adalah perangkat lunak yang dapat digunakan untuk menghasilkan (generate) atau mencoba membalikkan (decrypt) hash menjadi teks asli lewat tekhnik Brute Force. Fungsi aplikasi ini dibagi menjadi dua bagian utama:

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
~ (v1.0.0.2) Selasa 25 Februari 2025 - Update SecretKey Algoritms (Juniper Network)

#
<b>[ Cara Menggunakan Indihome Hash Decrypter Generator ]</b>

1. Download IHDG via: https://codeload.github.com/MichaelJorky/Indihome-Hash-Decrypter-Generator/zip/refs/heads/main
2. Pastikan ketika menggunakan aplikasi IHDG sedang terhubung ke jaringan yang sedang di Testing
3. Masukan Device SN, Device Mac, TR089 Mac (Optional) dan WPA Key lalu klik "Generating Hash Encryption" setelah keluar hasilnya lalu silahkan klik "BruteForce Hash Decryption!"
4. Jika hasil log menampilkan status Found maka itu adalah salah satu kunci yang bisa digunakan untuk login admin ke Router ZTE contohnya dalam pengujian Saya menggunakan ZTE F670L
5. Tingkat keberhasilan cara ini tergantung wordlist.txt seberapa besar database hash yang digunakan untuk melakukan brute force hash tersebut.

#
Just tested on ZTE F670L Software Version: V9.0.11P1N15 and V9.0.11P1N84A
