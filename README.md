# Man In The Middle Attack dengan Wireshark

Dalam bug bounty ini, saya menemukan kerentanan pada fitur login sebuah website yang rentan terhadap serangan Man-In-The-Middle (MITM). Website tersebut belum menggunakan certificate SSL, sehingga data yang dikirimkan antara pengguna dan server tidak terenkripsi dan berpotensi diintersepsi oleh penyerang. Solusi yang direkomendasikan adalah memasang certificate SSL agar semua informasi terenkripsi sebelum dikirimkan ke server. Berikut adalah langkah-langkah penyerang dalam menjalankan aksinya:

1. Hubungkan PC atau laptop ke jaringan, di sini saya menggunakan jaringan WiFi.
2. Buka aplikasi monitoring jaringan, seperti Wireshark. Pilih koneksi WiFi yang telah disediakan sebelumnya, lalu klik start capturing untuk mulai memantau aktivitas pada jaringan tersebut.
![Picture1](https://github.com/user-attachments/assets/103ef687-62ca-4fac-9fca-6b726663e4af)
3. Hubungkan perangkat korban ke jaringan WiFi yang sama.
Setelah terhubung, kunjungi website target dan lakukan login. Misalnya dengan email: 2******_a@stu**.****.ac.id dan password yang sesuai.
4. Kembali ke aplikasi Wireshark dan filter menggunakan http.host untuk memantau aktivitas POST request pada jaringan. Pada tabel, dapat ditemukan informasi login korban, termasuk username dan password.
![Picture3](https://github.com/user-attachments/assets/8b58324b-b36e-484d-968e-b90598a63aa3)
5. Untuk melihat detail lebih lanjut, buka HTTP Stream untuk melihat informasi sensitif yang dikirimkan.
![Picture4](https://github.com/user-attachments/assets/60f0c0bf-1102-4a6f-bb00-d02b41e793ba)

Namun, perlu diingat bahwa segala bentuk peretasan tanpa izin adalah tindakan ilegal dan dapat menimbulkan konsekuensi hukum yang serius. Oleh karena itu, semua risiko yang terkait dengan aktivitas ini sepenuhnya menjadi tanggung jawab individu. Mari kita gunakan keterampilan ini dengan bijak dan etis. Jika Anda memiliki pertanyaan atau ingin berdiskusi santai, jangan ragu untuk menghubungi saya. Saya senang dapat berbagi pengetahuan dan berdiskusi lebih lanjut.
<ul>
<li class="has-line-data" data-line-start="20" data-line-end="21">Instagram: <a href="https://www.instagram.com/_dhan.i/">_dhan.i</a></li>
<li class="has-line-data" data-line-start="22" data-line-end="23">LinkedIn: <a href="https://www.linkedin.com/in/ramadhani-aulia/">Aulia Ramadhani</a></li>
</ul>
