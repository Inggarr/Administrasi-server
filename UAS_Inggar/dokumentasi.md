## DOKUMENTASI UAS MMUHAMMAD INGGAR A S (2388010052) - INFORMATIKA 6B

membuat instance baru 
![alt text](image-21.png)
![alt text](image-22.png)
1. Proses Upload File Folder komdis-app
   ![alt text](image.png)
   ![alt text](image-1.png)
   ![alt text](image-2.png)
   ![alt text](image-3.png)

2. Mebuat database di mariadb
   ![alt text](image-4.png)
   - create database dbkomdis; ![alt text](image-5.png)
   - CREATE USER 'userkomdis'@'localhost' IDENTIFIED BY 'passwordkomdis';
   - grant all privileges on dbkommdis.* to 'userkomdis'@'localhost';
   ![alt text](image-6.png)
   ![alt text](image-7.png)

3. Export dbcompro dari localhost dari database phpmyadmin dalam bentuk sql
   ![alt text](image-8.png)

=======================================================================================================

4. instaall docker di ssh
   - ![alt text](image-9.png)

5. buka https//docker.com
   - buat repositori baru ![alt text](image-10.png)
   - Create Token Access ![alt text](image-11.png) ![alt text](image-12.png)
   - Buat repositori github ![alt text](image-13.png)

=======================================================================================================

6. Moderenisasi CI/CD
   - Mengisi Secrets Variable di Github Actions ![alt text](image-14.png)
   - build and deploy ![alt text](image-15.png) ![alt text](image-16.png)
   - cek web ![alt text](image-17.png)

=======================================================================================================

7. Deploy Multi Apps CI/CD Docker
   - uninstall apache dan mariadb
   ![alt text](image-18.png)
   - Create user baru bukan root di BMS (Laragon) ![alt text](image-19.png)
   - edit privilages ![alt text](image-20.png)
   
8. Docker compose
   - repo docker baru 
   - bikin repo github baru
   - deploy ![alt text](image-23.png)

struktur folder
![alt text](image-24.png)