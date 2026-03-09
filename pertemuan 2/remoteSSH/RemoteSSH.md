# Remote Instances with SSH Putty

1. Install Putty dan pasang putty
   ![alt text](image.png)
   ![alt text](image-1.png)

2. Konversi file public key dari .pem menjadi .ppk do Putty
   - buka puttyGen ![alt text](image-4.png)
   - load data file key.pem ![alt text](image-2.png)
   - Save File File key .ppk ![alt text](image-3.png)

3. Set Up Putty untuk remote SSH
   - Buka apps Putty ![alt text](image-5.png)
   - Isi IP public innstances ![alt text](image-8.png)
   - Isi port untuk SSH sesuai Security Group ![alt text](image-6.png)
   - Isi nama session agar saat connect lagi tinggal load saya ![alt text](image-7.png)
   - Load .ppk (Klik SSH -> Klik Auth -> Klik Gredential -> Load data ) ![alt text](image-9.png)
   - Kembali ke sessions Klik save ![alt text](image-10.png)
   - Klik Open dan masukan User name sesuai intences ![alt text](image-11.png)
   
4. Update
   - sudo apt-get update ![alt text](image-12.png)
   - sudo apt-get upgrade ![alt text](image-13.png)

5. Pembuktian remote SSH secara visual
   - Copy Public ip adress instance paste ke browser ![alt text](image-14.png)
   - install web server seperti Apache/Nginx
   - sudo install apt install apache2
   - reload browser ![alt text](image-15.png)

6. Matikan Instance agar tidak kena tagihan
   - sudo shutdown now ![alt text](image-16.png) 
   - cek di awas instance ![alt text](image-17.png)

