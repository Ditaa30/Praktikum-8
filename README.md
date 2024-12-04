# Praktikum-8

# PERTEMUAN 11

# Soal

![Screenshot 2024-11-29 130143](https://github.com/user-attachments/assets/b2a572b9-928a-4d3d-9a24-878ea9859596)

## Customer

![customer](https://github.com/user-attachments/assets/7a02a8ae-6a73-4025-aa0b-a79db9999d8f)

Penjelasan :
- Atribut:
  - name: Nama customer.
  - address: Alamat customer.
- Konstruktor: Menginisialisasi name dan address.
- Getter: Memberikan akses ke nama dan alamat customer.

## Order

![Order](https://github.com/user-attachments/assets/6dcc79b5-0457-4707-8b97-39127a1a6372)


Penjelasan : 
- Atribut:
  - date: Tanggal pesanan.
  - status: Status pesanan (misalnya: "Processed").
  - orderDetails: List yang berisi objek OrderDetail.
- Metode:
  - calcSubTotal(): Menghitung total semua subtotal dari setiap barang.
  - calcTax(): Menghitung total pajak dari semua barang.
  - calcTotal(): Menghitung total keseluruhan (subtotal + pajak).
  - calcTotalWeight(): Menghitung total berat semua barang.
  - 
## OrderDetail

![OrderDetail](https://github.com/user-attachments/assets/6317f498-ca26-4e19-9581-eec026fb94fd)

penjelasan :
- Atribut:
  - quantity: Jumlah barang dalam pesanan.
  - taxStatus: Status pajak barang.
  - item: Objek dari kelas Item.
- Metode:
  - calcSubTotal(): Menghitung subtotal dengan mengalikan harga barang dengan jumlah.
  - calcTax(): Menghitung pajak dari subtotal.
  - calcWeight(): Menghitung total berat barang yang dipesan.

## Item

![item](https://github.com/user-attachments/assets/5b911c2a-3385-44c6-b8b8-5eb2e14ce8b9)

Penjelasan :
- Atribut:
  - shippingWeight: Berat barang yang akan dikirim.
  - description: Deskripsi barang.
- Metode:
  - getPriceForQuantity(): Mengembalikan harga barang per unit (contoh: 1000).
  - inStock(): Mengembalikan status stok (asumsi selalu tersedia).
    
## Payment (abstrac)

![payment](https://github.com/user-attachments/assets/c3bb1267-4270-4ef5-8ac8-2db87f73c92d)

penjelasan : 
- Atribut:
  - amount: Jumlah pembayaran.
- Metode abstrak:
  - authorized(): Harus diimplementasikan oleh kelas turunan (misalnya Cash, Check, atau Credit).
    
## Cash

![cash](https://github.com/user-attachments/assets/0df1590e-e8ce-4a74-b637-b1aa6af41387)

Penjelasan :
- Atribut:
cashTendered: Jumlah uang tunai yang diterima.
- Metode:
authorized(): Mengecek apakah uang tunai cukup.

## Check

![check](https://github.com/user-attachments/assets/87a256c1-3572-4ef8-a27c-85c043b598c5)


Penjelasan : 
- Atribut:
  - name: Nama pada cek.
  - bankID: ID bank.
- Metode:
authorized(): Mengecek validitas ID bank.

## Credit

![credit](https://github.com/user-attachments/assets/8504151e-e98f-4e02-b205-12885c5379d2)


Penjelasan :
- Atribut:
  - number: Nomor kartu kredit.
  - type: Jenis kartu (Visa, MasterCard, dll.).
  - expDate: Tanggal kedaluwarsa.
- Metode:
authorized(): Mengecek apakah nomor kartu memiliki panjang 16 digit.

## Main

![main1](https://github.com/user-attachments/assets/f295c1a7-b356-4d22-8a8d-6dc4937d5396)

![main2](https://github.com/user-attachments/assets/3f30c7bd-0173-445d-9a6c-362159e31187)

## Output

![OutPut8](https://github.com/user-attachments/assets/61f48720-cc52-4763-98de-1e83aeb2a6e2)

# Selesai
