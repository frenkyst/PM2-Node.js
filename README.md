# PM2-Node.js

Menggunakan PM2+LocalTunnel untuk menjalankan Aplikasi
1. Download dan Install pm2 dengan command berikut

        npm install pm2@latest -g

![image](https://user-images.githubusercontent.com/40049149/186715154-02621ce9-255c-4572-b789-796a53c3ba33.png)

2. Jalankan command berikut untuk memastikan pm2 sudah terinstall

        pm2

![image](https://user-images.githubusercontent.com/40049149/186715238-ceb91c65-fa77-4eec-adf1-840390cad18c.png)

3. Jalankan aplikasi node yang sudah dibuat sebelumnya dengan command berikut

        pm2 start index.js

![image](https://user-images.githubusercontent.com/40049149/186715898-f0755a27-d0eb-49e6-9265-e50a599268a9.png)

4. Jalankan aplikasi python yang sudah dibuat sebelumnya dengan command berikut

        pm2 start index.py --interpreter python3

![image](https://user-images.githubusercontent.com/40049149/186716169-bb5fab90-5f69-45ef-8c83-670ce699eda6.png)

5. Untuk melihat process pm2 yang sudah perjalan, gunakan command berikut

        pm2 list

![image](https://user-images.githubusercontent.com/40049149/186716312-cf0df2aa-c77b-4969-aa5a-25f5d7f2dd94.png)

6. Cek melalui browser untuk mengecek apakah aplikasi sudah berjalan ( sesuikan ip local milik kalian )

        http://192.168.89.29:3000/
        
![image](https://user-images.githubusercontent.com/40049149/186716033-f7ce3dff-87e6-4eb2-8304-23bc5739dc3a.png)
        
        http://192.168.89.29:5000/

![image](https://user-images.githubusercontent.com/40049149/186716388-5e462058-96db-41ad-89aa-da7922d45b2f.png)

7. Jalankan command berikut untuk melakukan local tunnel ke port 3000 aplikasi nodejs dan port 5000 aplikasi python yang sudah di jalankan dengan pm2 sebelumnya (dijalankan bergantian)

        lt -p 3000

        lt -p 5000
