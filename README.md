# labpy03

# LATIHAN 1

![Screenshot (73)](https://github.com/user-attachments/assets/fa209f1f-8e81-4a81-a4e8-d83d1e2e4444)

![Screenshot (72)](https://github.com/user-attachments/assets/a297d51f-df72-45bb-8b58-c13541efa20f)


# PENJELASANNYA

Kode pada tangkapan layar di atas menghasilkan angka acak dan mencetaknya jika angkanya di bawah 0,5. Berikut penjelasan masing-masing bagian:

1. Mengimpor random fungsi :

        from random import random
   
Ini mengimpor random fungsi dari random modul, yang memungkinkan Anda menghasilkan nilai float acak antara 0 dan 1.

2. Mendefinisikan generate_random_numbers fungsi :

        def generate_random_numbers():

Baris ini mendefinisikan fungsi bernama generate_random_numbers yang berisi logika untuk menghasilkan dan mencetak angka acak.

3. Mendapatkan Masukan Pengguna :

        n = int(input("Masukkan nilai N: "))
   
Baris ini meminta pengguna untuk memasukkan bilangan bulat N, yang menentukan berapa banyak angka acak yang akan dihasilkan program.

4. Menyiapkan loop :

        count = 1
        while count <= n:

countdiinisialisasi ke 1, dan whileloop diatur untuk terus berlanjut selama countkurang dari atau sama dengan N.

5. Membuat dan Memeriksa Nilai Acak :

        value = random()
        if value < 0.5:
            print(f"data ke: {count} => {value}")
        
Di dalam lingkaran:
value = random()menghasilkan angka acak antara 0 dan 1.
if value < 0.5memeriksa apakah nilai ini kurang dari 0,5. Jika ya, kode akan mencetak nilai beserta jumlahnya.

    
6. Menambah Penghitung :

        count += 1
    
Nilai tersebut countbertambah 1 untuk berpindah ke iterasi berikutnya.

7. Pesan Penyelesaian :

        print("Selesai")
        
Setelah loop selesai, "Selesai" dicetak untuk menunjukkan bahwa program telah selesai.

8. Memanggil Fungsi :

        generate_random_numbers()
    
Baris ini memanggil fungsi dan memulai proses.


Contoh Keluaran

Jika pengguna memasukkan N = 5, program akan menghasilkan dan mencetak hingga 5 angka acak (jika kurang dari 0,5).

Misalnya:

    Masukkan nilai N: 5
    data ke: 1 => 0.4304522641343549
    data ke: 2 => 0.3824479399818994
    data ke: 3 => 0.10742157983454792
    data ke: 4 => 0.3512501306810244
    data ke: 5 => 0.021373204187890127
    Selesai
    
Kode ini hanya akan menampilkan angka acak yang memenuhi kondisi ( < 0.5). Jika angka acak yang dihasilkan adalah 0,5 atau lebih tinggi, angka tersebut akan dilewati dalam output.


# LATIHAN 2

![Screenshot (75)](https://github.com/user-attachments/assets/1f589eb3-1fc0-44b6-961c-07ca835039a6)

![Screenshot (74)](https://github.com/user-attachments/assets/797fea2e-bd38-4e3f-ae0e-486f87761484)


# PENJELASAN 

Kode di atas adalah program Python yang menghitung laba investasi setiap bulannya.

Berikut penjelasannya:

1. Definisi Variabel Awal:

        modal_awal: Menyimpan nilai modal awal investasi (100.000.000).
        
        laba_bulanan: List kosong untuk menyimpan laba setiap bulannya.
        
        total_laba: Variabel untuk menampung total laba hingga saat ini, diinisialisasi dengan nilai 0.
        
2. Perulangan untuk Menghitung Laba:
   
       Kode menggunakan perulangan for untuk menghitung laba setiap bulan selama 8 bulan (range(1, 9)).

4. Logika Penghitungan Laba:

        Bulan 1-2: Tidak ada laba (laba = 0).
        Bulan 3-4: Laba 1% dari modal awal.
        Bulan 5-7: Laba 5% dari modal awal.
        Bulan 8: Laba 2% dari modal awal.
   
5. Menambahkan Laba ke List:

        laba_bulanan.append(laba): Menambahkan nilai laba ke dalam list 
        laba_bulanan untuk menyimpan riwayat laba bulanan.
        total_laba += laba: Menambahkan nilai laba saat ini ke variabel total_laba.

6. Menampilkan Hasil:

  Kode mencetak hasil perhitungan laba untuk setiap bulan menggunakan
  
      print(f"laba bulan ke- {bulan} sebesar: {laba}").
  Terakhir, kode mencetak total laba hingga akhir bulan ke-8 dengan
      
      print(f"Total laba adalah: {total_laba}").
      
  Kode ini mendemonstrasikan bagaimana menghitung laba investasi secara sederhana dengan persentase yang berbeda untuk periode waktu tertentu.


# LATIHAN 3

![Screenshot (79)](https://github.com/user-attachments/assets/676ef1c5-239e-4b8b-b5d7-4f233ca9488e)

![Screenshot (78)](https://github.com/user-attachments/assets/5deb1c35-c7fa-47f8-a7cb-75c4eb66f1cf)

# PENJELASAN

Kode di atas adalah fungsi yang mensimulasikan mesin ATM sederhana.

Berikut Penjelasannya:

1.      'def atm_simulator():'
   
   Baris ini mendefinisikan fungsi bernama atm_simulator(). Ini berarti bahwa kode di dalam fungsi ini akan dieksekusi saat fungsi ini dipanggil.

  
2.     'saldo = 1000000'
   
   Baris ini menetapkan variabel saldo dengan nilai 1000000, yang menunjukkan saldo awal akun di ATM.

3.     'while True:'
   
   Baris ini memulai loop while yang akan terus berulang selama kondisinya (True) bernilai benar. Ini berarti bahwa kode di dalam loop akan terus berulang hingga secara eksplisit       dihentikan.

4.     'print(f"\nSaldo saat ini: Rp {saldo}")'

    Baris ini mencetak teks ke layar yang menunjukkan saldo akun saat ini. \n digunakan untuk menambahkan baris baru sebelum pesan saldo.

5.     'print("1. Tarik Uang")'

    Baris ini mencetak pilihan menu pertama di ATM, yaitu "Tarik Uang".

6.     'print("2. Keluar")'

    Baris ini mencetak pilihan menu kedua di ATM, yaitu "Keluar".

7.     'pilihan = input("Pilih menu (1/2): ")'

    Baris ini meminta input dari pengguna untuk memilih menu yang ingin digunakan. Input pengguna disimpan di variabel pilihan.

8.     'if pilihan == "1":'

   Baris ini memulai pernyataan if yang memeriksa apakah input pengguna (pilihan) sama dengan "1". Jika benar, maka kode di dalam blok if akan dieksekusi.

9.     'jumlah = int(input("Masukkan jumlah penarikan: "))'

    Baris ini meminta input dari pengguna untuk memasukkan jumlah uang yang ingin ditarik. Input pengguna kemudian diubah ke tipe data integer dan disimpan dalam variabel jumlah.

10.     'if jumlah > saldo:'

    Baris ini memulai pernyataan if yang memeriksa apakah jumlah yang ingin ditarik (jumlah) lebih besar daripada saldo akun (saldo). Jika benar, maka kode di dalam blok if akan dieksekusi.

11.     'print("Maaf, saldo tidak mencukupi!")'
    Baris ini mencetak pesan ke layar yang memberitahu








