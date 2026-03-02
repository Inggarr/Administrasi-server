# Membuat EC2 / Instance /VM

1. Pilih menu All Services  -> Ec2
   ![alt text](image-3.png)

2. Di dalam menu EC2 pilih instances
   ![alt text](image-4.png)

3. dalam instances Pilih menu Launch Intences
   ![alt text](image-5.png)

4. Beri nama Instance dengan format Nim_server
   ![alt text](image-6.png)

5. Pilih OS Server untuk Instances
   ![alt text](image-7.png)

6. Pilih Resource Instaances T3.,icro (2VCPU, 1GB Memory)
   ![alt text](image-8.png)

7. Membuat Key Pair, Pilih Menu create new key pair, Isi nama Key Pair, Pilih RSA, Format file .pem,   Klik Create New Key
   ![alt text](image-9.png)

8. Setting kebijakan keamanan atau privasi / security group
    - Allow SSH   -> Artinya membolehkan Remote SSH dari luar
    - Allow HTTPS -> Artinya Instances bisa di akses dari protokol HTTPS
    -Allow HTTPS  -> Artinya Instances bisa di akses dari Protokol HTTP
   ![alt text](image-10.png)

9. Selesai Setup pilih Launc Instances
   ![alt text](image-11.png)
   ![alt text](image-12.png)

10. Pastikan Launch Instances Sukses
    ![alt text](image-13.png)

11. EC2 berhasil terbuat
    ![alt text](image-14.png)
    




