## Membuat Database MySql di AWS EC2

1. Aktifkan instance ![alt text](image.png)

2. Remote SSH via Terminal 
   - Masuk ke folder penyimpanan private Key 
   (Cari folder klik kanan-pilih terminal sambil klik shift dan ctrl) ![alt text](image-1.png)
   - Masukan comman ssh -i key_2388010052.pem ubuntu@13.236.178.230 
   - Tekan enter

3. Lakukan Pathching OS
   - sudo apt-get update && sudo apt-get upgrade ![alt text](image-2.png)

4. Install MariaDB
   - sudo apt-get install mariadb-server ![alt text](image-3.png)
   - sudo system start mariadb
   - sudo system status mariadb ![alt text](image-4.png)
   - coba apakah default setting yang berlaku (sudo mysql -u root -p)
   - cek apakah masih ada database dummy (show databases;) ![alt text](image-5.png)

5. Kita lakukan Hardening Security
   - Masukan Command sudo mysql_secure_installation 
   - Switch to unix_socket authentication : Y
   - Change the root password? : Y
   - Remove anonymous users? : Y
   - Disallow root login remotely? : Y
   - Remove test database and access to it? : Y
   - Reload privilege tables now? : Y
   ![alt text](image-6.png)
   - Cek kembali apakah masih bisa login tanpa pw ![alt text](image-7.png) dan ternyata tidak bisa (berhasil)

6. Membuat database dan User
   - membuat database untuk web company profile (create database dbCompro;)
   - membuat user untuk web company profile (create user 'userCompro'@'localhost' identified by '*********';)
   - Memberikan Hak akses user untuk web company profile (grant all privileges on dbCompro.* to userCompro'@'localhost';)
   - flush privileges ![alt text](image-8.png)

7. Login menggunakan akun database yang sudah di buat
   - login menggunakan username (sudo mysql -u userCompro -p)
   - enter password yang sudah di buat (passwordCompro)
   - lihat database yang sudah dibuat (show databases;) 
![alt text](image-9.png)

