# Daftar Test Cases - SauceDemo

Berikut adalah skenario pengujian untuk fungsionalitas Login.

| Test Case ID | Fitur | Judul Test Case | Langkah-langkah | Hasil yang Diharapkan |
| :--- | :--- | :--- | :--- | :--- |
| TC-L-001 | Login | **Positif** - Login dengan kredensial valid | 1. Buka halaman Login (https://www.saucedemo.com/) <br> 2. Masukkan username: `standard_user` <br> 3. Masukkan password: `secret_sauce` <br> 4. Klik tombol "Login" | Pengguna berhasil login dan diarahkan ke halaman Beranda (Inventory) di URL: `https://www.saucedemo.com/inventory.html` |
| TC-L-002 | Login | **Negatif** - Login dengan password salah | 1. Buka halaman Login <br> 2. Masukkan username: `standard_user` <br> 3. Masukkan password: `password_salah` <br> 4. Klik tombol "Login" | Pengguna gagal login. <br> Pesan error "Epic sadface: Username and password do not match any user in this service" muncul di bawah tombol Login. |
| TC-L-003 | Login | **Negatif** - Login dengan username salah | 1. Buka halaman Login <br> 2. Masukkan username: `username_salah` <br> 3. Masukkan password: `secret_sauce` <br> 4. Klik tombol "Login" | Pengguna gagal login. <br> Pesan error "Epic sadface: Username and password do not match any user in this service" muncul. |
| TC-L-004 | Login | **Negatif** - Login tanpa memasukkan password | 1. Buka halaman Login <br> 2. Masukkan username: `standard_user` <br> 3. Biarkan kolom password kosong <br> 4. Klik tombol "Login" | Pengguna gagal login. <br> Pesan error "Epic sadface: Password is required" muncul. |
| TC-L-005 | Login | **Negatif** - Login tanpa memasukkan username | 1. Buka halaman Login <br> 2. Biarkan kolom username kosong <br> 3. Masukkan password: `secret_sauce` <br> 4. Klik tombol "Login" | Pengguna gagal login. <br> Pesan error "Epic sadface: Username is required" muncul. |
| TC-L-006 | Login | **Fungsional** - Validasi *user* yang terkunci | 1. Buka halaman Login <br> 2. Masukkan username: `locked_out_user` <br> 3. Masukkan password: `secret_sauce` <br> 4. Klik tombol "Login" | Pengguna gagal login. <br> Pesan error "Epic sadface: Sorry, this user has been locked out." muncul. 


### Skenario Pengujian Visual (UI/UX & Responsiveness)

| Test Case ID | Fitur | Judul Test Case | Langkah-langkah | Hasil yang Diharapkan |
| :--- | :--- | :--- | :--- | :--- |
| TC-UI-001 | UI/Layout | Validasi tampilan Grid Produk | 1. Login ke aplikasi. <br> 2. Amati halaman Inventory. <br> 3. Cek tata letak gambar, judul, dan harga. | Semua kartu produk harus sejajar (aligned), gambar tidak tumpang tindih, dan font konsisten. |
| TC-UI-002 | Responsiveness | Validasi tampilan Mobile (iPhone 12/13) | 1. Buka DevTools (F12). <br> 2. Aktifkan "Device Toolbar". <br> 3. Pilih dimensi iPhone 12 Pro. | Layout harus menyesuaikan layar kecil (responsif). Tidak ada elemen yang terpotong atau *scroll* horizontal yang tidak perlu. |
| TC-UI-003 | Typography | Cek Konsistensi Font | 1. Inspeksi elemen judul produk. <br> 2. Bandingkan dengan standar desain (jika ada). | Jenis font, ukuran, dan ketebalan huruf harus konsisten di setiap kartu produk. |


