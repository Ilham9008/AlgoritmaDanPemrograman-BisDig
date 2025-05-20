 NOMOR 1
nput dari pengguna

Program mulai dengan meminta pengguna memasukkan jumlah total belanja.

Ini penting agar program tahu berapa yang akan dihitung.

Pengecekan syarat diskon

Program mengecek apakah total belanja lebih dari Rp500.000.

Jika iya, maka pengguna memenuhi syarat untuk mendapat diskon 10%.

Perhitungan diskon

Jika berhak, diskon dihitung dengan mengalikan total belanja × 10%.

Total bayar dikurangi dengan diskon tersebut.

Jika tidak memenuhi syarat

Jika belanja kurang dari atau sama dengan Rp500.000, maka tidak ada diskon.
NOMOR 2 
Input Nilai dari Pengguna
Program meminta pengguna memasukkan tiga nilai.
Ini dilakukan dengan:

python
Copy
Edit
nilai1 = float(input("Masukkan nilai pertama: "))
nilai2 = float(input("Masukkan nilai kedua: "))
nilai3 = float(input("Masukkan nilai ketiga: "))
Setiap nilai dikonversi ke tipe float karena bisa saja berupa angka desimal.

Menghitung Rata-Rata Nilai
Setelah ketiga nilai dimasukkan, program menghitung rata-rata menggunakan rumus:

python
Copy
Edit
rata_rata = (nilai1 + nilai2 + nilai3) / 3
Menentukan Kelulusan
Program lalu mengecek apakah rata-rata nilai tersebut lebih dari atau sama dengan 75:

Jika ya → tampilkan “Lulus”

Jika tidak → tampilkan “Tidak Lulus”

Ini dilakukan dengan struktur:

python
Copy
Edit
if rata_rata >= 75:
    print("Lulus")
else:
    print("Tidak Lulus")

NOMOR 3 

ujuan Program
Program ini dibuat untuk menghitung faktorial dari sebuah angka yang dimasukkan oleh pengguna. Faktorial adalah hasil perkalian dari suatu bilangan dengan semua bilangan bulat positif di bawahnya.
Contohnya:

5! = 5 × 4 × 3 × 2 × 1 = 120

3! = 3 × 2 × 1 = 6

🧭 Alur Program dan Penjelasannya
Membuat fungsi faktorial

python
Copy
Edit
def faktorial(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * faktorial(n - 1)
Program membuat fungsi bernama faktorial untuk menghitung nilai faktorial secara rekursif.

Jika angka yang dimasukkan adalah 0 atau 1, hasil faktorialnya langsung 1 (karena itu memang aturan faktorial).

Untuk angka selain itu, fungsi akan memanggil dirinya sendiri hingga mencapai 1.

Mengambil input dari pengguna

python
Copy
Edit
angka = int(input("Masukkan angka: "))
Program meminta pengguna memasukkan sebuah angka bulat.

Nilai ini disimpan dalam variabel angka.

Menampilkan hasil

python
Copy
Edit
print(f"Faktorial dari {angka} adalah {faktorial(angka)}")
Program mencetak hasil perhitungan faktorial dengan memanggil fungsi yang sudah dibuat.

Hasilnya ditampilkan ke layar.

💡 Kenapa pakai cara ini?
Fungsi rekursif dipakai karena cara ini sangat cocok dan umum untuk menghitung faktorial. Pendek, rapi, dan mengikuti definisi matematika faktorial.

Struktur if dalam fungsi memastikan bahwa program tahu kapan harus berhenti (kasus dasar: n == 0 atau n == 1).

input() dan int() digunakan supaya program bisa membaca angka dari pengguna dan memprosesnya sebagai bilangan bulat.

Contoh Jalannya Program:
yaml
Copy
Edit
Masukkan angka: 4
Faktorial dari 4 adalah 24
N0M0R 4

Program ini digunakan untuk:

Mencatat nilai dari 5 siswa

Menentukan siapa yang memiliki nilai tertinggi

Menampilkan nilai tertinggi dan posisi siswa yang mendapatkannya

🧭 Alur Program dan Penjelasannya
Inisialisasi list kosong

python
Copy
Edit
nilai_siswa = []
Di awal, dibuat list kosong untuk menyimpan nilai-nilai yang dimasukkan oleh pengguna.

List digunakan karena bisa menampung banyak nilai dan memudahkan proses pencarian nilai tertinggi.

Input nilai dengan perulangan

python
Copy
Edit
for i in range(5):
    nilai = int(input(f"Masukkan nilai siswa ke-{i+1}: "))
    nilai_siswa.append(nilai)
Program meminta pengguna memasukkan nilai sebanyak 5 kali (untuk 5 siswa).

Nilai dimasukkan satu per satu dan langsung disimpan ke dalam list menggunakan .append().

Menentukan nilai tertinggi

python
Copy
Edit
nilai_tertinggi = max(nilai_siswa)
Fungsi max() digunakan untuk mencari nilai tertinggi dari semua nilai yang sudah dimasukkan.

Menentukan posisi siswa yang mendapat nilai tertinggi

python
Copy
Edit
siswa_tertinggi = nilai_siswa.index(nilai_tertinggi) + 1
Fungsi index() mencari posisi dari nilai tertinggi dalam list.

Ditambah 1 karena index di Python dimulai dari 0, sedangkan urutan siswa dimulai dari 1.

Menampilkan hasil

python
Copy
Edit
print(f"Nilai tertinggi adalah: {nilai_tertinggi}")
print(f"Didapatkan oleh siswa ke-{siswa_tertinggi}")
Hasil akhir ditampilkan, berupa nilai tertinggi dan siswa ke berapa yang mendapat nilai tersebut.

🔍 Kenapa cara ini digunakan?
List digunakan agar bisa menyimpan banyak data dengan rapi.

Perulangan for memudahkan input banyak data tanpa menulis kode berulang.

Fungsi max() dan index() memudahkan pencarian nilai tertinggi dan posisi siswa, tanpa perlu logika rumit.

Pendek, efisien, dan mudah dipahami oleh pemula.

Contoh Output:
yaml
Copy
Edit
Masukkan nilai siswa ke-1: 78
Masukkan nilai siswa ke-2: 85
Masukkan nilai siswa ke-3: 90
Masukkan nilai siswa ke-4: 88
Masukkan nilai siswa ke-5: 90
Nilai tertinggi adalah: 90
Didapatkan oleh siswa ke-3

NOMOR 5
