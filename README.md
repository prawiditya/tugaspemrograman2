# Program Kalkulator Sederhana
Program kalkulator sederhana untuk menghitung inputan dari user.

## Deskripsi Program
Program kalkulator sederhana yang mampu melakukan operasi dasar matematika dengan dua bilangan, user bisa memilih operasi yang ingin mereka lakukak (+,-.x.\).

## Flowchaart Kalkulator
![image](https://github.com/user-attachments/assets/8bc14701-d9fa-4677-83e7-cdb615e4b366)
## kode program
```Python
ef kalkulator(a, b, operator):
    if operator == '+':
        return a + b
    elif operator == '-':
        return a - b
    elif operator == '*':
        return a * b
    elif operator == '/':
        return a / b
    else:
        print("Input tidak valid")
        exit()

a = int(input("Masukkan angka pertama: "))
b = int(input("Masukkan angka kedua: "))
operator = input("Masukkan operator '+', '-', '*', atau '/': ")

hasil = kalkulator(a, b, operator)
print(f"Hasilnya adalah {hasil}")
```
```Python
## contoh output program
Masukkan angka pertama: 9
Masukkan angka kedua: 8
Masukkan operator '+', '-', '*', atau '/': +
Hasilnya adalah 17
## Cara Kerja Program:
1. Program menentukan harga awal:
   - Tiket VIP: Rp 100.000
   - Tiket Reguler: Rp 50.000

2. User diminta memilih jenis tiket:
   - Jika memilih "vip", harga diset Rp 100.000
   - Jika memilih "reguler", harga diset Rp 50.000
   - Jika input selain keduanya, program berhenti dengan pesan "Input tidak valid"

3. User diminta konfirmasi kepemilikan kartu member:
   - Jika memiliki kartu member (input "ya"), akan mendapat diskon 20%
   - Jika tidak memiliki (input "tidak"), tidak ada diskon

4. Program menampilkan harga akhir setelah perhitungan diskon
```

## Sistem Pembelian Tiket
Program sederhana untuk menghitung harga tiket berdasarkan jenis tiket dan status member.

## Deskripsi Program
Program ini memungkinkan pengguna untuk:

Memilih jenis tiket (VIP/Reguler)
Menentukan status member
Mendapatkan perhitungan harga tiket final dengan diskon jika memiliki kartu member

## Flowchart Ticket
![image](https://github.com/user-attachments/assets/3b2b2174-9393-4415-aafa-451b9404eb08)
## kode program
```Python
vip = 100000
reguler = 50000

jenis = input("Pilih jenis ticket anda (vip/reguler): ")

if jenis == "vip":
    harga_ticket = vip
elif jenis == "reguler":
    harga_ticket = reguler
else:
    print("Input tidak valid")
    exit()

member = input("Apakah anda punya kartu member (ya/tidak): ")
harga_ticket -= harga_ticket * 0.20 if member == "ya" else 0

print(f"Harga ticket anda {int(harga_ticket)}")
```
```Python
## contoh output program
Pilih jenis ticket anda (vip/reguler): vip
Apakah anda punya kartu member (ya/tidak): ya
Harga ticket anda 80000
## Cara Kerja Program:

1. Program menentukan harga awal:
   - Tiket VIP: Rp 100.000
   - Tiket Reguler: Rp 50.000

2. User diminta memilih jenis tiket:
   - Jika memilih "vip", harga diset Rp 100.000
   - Jika memilih "reguler", harga diset Rp 50.000
   - Jika input selain keduanya, program berhenti dengan pesan "Input tidak valid"

3. User diminta konfirmasi kepemilikan kartu member:
   - Jika memiliki kartu member (input "ya"), akan mendapat diskon 20%
   - Jika tidak memiliki (input "tidak"), tidak ada diskon

4. Program menampilkan harga akhir setelah perhitungan diskon

Contoh perhitungan:
- Jika pilih VIP dan punya member:
  Rp 100.000 - (20% × Rp 100.000) = Rp 80.000
- Jika pilih Reguler dan punya member:
  Rp 50.000 - (20% × Rp 50.000) = Rp 40.000
```
