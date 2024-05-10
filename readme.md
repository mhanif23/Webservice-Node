# Webservice Node.js

Webservice ini dibuat menggunakan Node.js untuk menyediakan data produk laptop kepada aplikasi klien.

## Instalasi

Pastikan Anda telah menginstal Node.js di sistem Anda. Jika belum, Anda dapat mengunduhnya dari [situs web resmi Node.js](https://nodejs.org/).

### Langkah-langkah Instalasi

1. Unduh atau salin repositori ini ke sistem Anda.

2. Buka terminal atau command prompt, dan navigasikan ke direktori webservice.

3. Jalankan perintah berikut untuk menginstal dependensi yang diperlukan:

   ```bash
   npm install

4. Setelah dependensi terinstal, Anda dapat menjalankan webservice dengan perintah:

   ```bash
   npm start

Webservice akan berjalan di port default 3000.

## Penggunaan

Webservice ini menyediakan endpoint RESTful API untuk mengakses data produk laptop. Berikut adalah beberapa endpoint yang tersedia:

- `GET /products`: Mengembalikan daftar semua produk laptop.

Anda dapat menggunakan perangkat lunak seperti [Postman](https://www.postman.com/) atau [Insomnia](https://insomnia.rest/) untuk mengakses endpoint tersebut dan menguji webservice.

## Struktur Data DB


    ```bash
    -- Create table untuk produk laptop
    CREATE TABLE laptops (
        id INT AUTO_INCREMENT PRIMARY KEY,
        brand VARCHAR(255) NOT NULL,
        model VARCHAR(255) NOT NULL,
        processor VARCHAR(255) NOT NULL,
        ram VARCHAR(50) NOT NULL,
        storage VARCHAR(50) NOT NULL,
        display_size DECIMAL(5, 2) NOT NULL,
        graphics_card VARCHAR(255) NOT NULL,
        price DECIMAL(10, 2) NOT NULL
    );

    -- Insert data 20 laptop
    INSERT INTO laptops (brand, model, processor, ram, storage, display_size, graphics_card, price) VALUES
    ('Acer', 'Aspire 5', 'Intel Core i5', '8GB', '512GB SSD', 15.6, 'Intel UHD Graphics 620', 599.99),
    ('ASUS', 'VivoBook 15', 'AMD Ryzen 5', '8GB', '512GB SSD', 15.6, 'AMD Radeon Vega 8', 649.99),
    ('Dell', 'Inspiron 15', 'Intel Core i7', '16GB', '512GB SSD', 15.6, 'Intel UHD Graphics', 899.99),
    ('HP', 'Pavilion x360', 'Intel Core i3', '8GB', '256GB SSD', 14, 'Intel UHD Graphics', 499.99),
    ('Lenovo', 'IdeaPad 3', 'AMD Ryzen 3', '4GB', '128GB SSD', 14, 'AMD Radeon Graphics', 329.99),
    ('Apple', 'MacBook Air', 'Apple M1', '8GB', '256GB SSD', 13.3, 'Apple M1', 999.99),
    ('Microsoft', 'Surface Laptop 4', 'Intel Core i5', '8GB', '256GB SSD', 13.5, 'Intel Iris Xe Graphics', 1299.99),
    ('Samsung', 'Galaxy Book Flex', 'Intel Core i7', '16GB', '512GB SSD', 15.6, 'Intel UHD Graphics', 1399.99),
    ('Google', 'Pixelbook Go', 'Intel Core i5', '8GB', '128GB SSD', 13.3, 'Intel UHD Graphics 615', 649.99),
    ('Razer', 'Blade 15', 'Intel Core i7', '16GB', '512GB SSD', 15.6, 'NVIDIA GeForce RTX 3060', 1799.99),
    ('MSI', 'GS66 Stealth', 'Intel Core i9', '32GB', '1TB SSD', 15.6, 'NVIDIA GeForce RTX 3080', 2999.99),
    ('LG', 'Gram 17', 'Intel Core i7', '16GB', '1TB SSD', 17, 'Intel Iris Xe Graphics', 1499.99),
    ('Huawei', 'MateBook X Pro', 'Intel Core i7', '16GB', '1TB SSD', 13.9, 'NVIDIA GeForce MX250', 1499.99),
    ('Xiaomi', 'Mi Notebook Pro', 'Intel Core i5', '8GB', '512GB SSD', 15.6, 'NVIDIA GeForce MX250', 899.99),
    ('Sony', 'VAIO S', 'Intel Core i7', '8GB', '256GB SSD', 13.3, 'Intel HD Graphics 620', 1199.99),
    ('Toshiba', 'Dynabook Tecra', 'Intel Core i5', '8GB', '256GB SSD', 14, 'Intel UHD Graphics 620', 799.99),
    ('Fujitsu', 'Lifebook U', 'Intel Core i5', '8GB', '256GB SSD', 13.3, 'Intel UHD Graphics 620', 899.99),
    ('Alienware', 'M15 R5', 'AMD Ryzen 7', '16GB', '512GB SSD', 15.6, 'NVIDIA GeForce RTX 3070', 2199.99),
    ('Gateway', 'Creator Series', 'Intel Core i5', '16GB', '512GB SSD', 15.6, 'Intel UHD Graphics 620', 999.99),
    ('Panasonic', 'Toughbook 55', 'Intel Core i7', '16GB', '512GB SSD', 14, 'Intel UHD Graphics 620', 2499.99);
