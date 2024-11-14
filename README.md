# lapby04

# praktikum 4 

# Tugas Praktikum
Buatlah program sederhana untuk menambahkan data kedalam sebuah list dengan rincian sebagai berikut : 
1.	Program meminta memasukkan data sebanyak-banyakanya (gunakan perulangan)
2.	Tampilkan pertanyaan untuk menambahkan data (y/t?), apabila jawaban t (tidak), maka program akan menampilkan daftar datanya
3.	Nilai akhir diambil dari perhitungan 3 komponen nilai (tugas: 30%, uts:35%, uas:35%)
4.	Buat flowchart 

        # Inisialisasi list untuk menyimpan data
        data_mahasiswa = []

        while True:
          # Input data mahasiswa
          nama = input("Nama mahasiswa: ")
          tugas = float(input("Nilai tugas: "))
          uts = float(input("Nilai UTS: "))
          uas = float(input("Nilai UAS: "))
    
          # Hitung nilai akhir
          nilai_akhir = (tugas * 0.3) + (uts * 0.35) + (uas * 0.35)
    
          # Simpan data ke dalam list
          data_mahasiswa.append({
              'nama': nama,
              'tugas': tugas,
              'uts': uts,
              'uas': uas,
              'nilai_akhir': nilai_akhir
        })
    
        # Tanyakan apakah ingin menambah data
        tambah_data = input("Apakah ada data yang ingin ditambahkan? (y/t): ")
        if tambah_data.lower() == 't':
            break
  
        # Tampilkan daftar data
        print("\nDaftar Data Mahasiswa:")
        for mahasiswa in data_mahasiswa:
            print(f"Nama: {mahasiswa['nama']}, Tugas: {mahasiswa['tugas']}, UTS: {mahasiswa['uts']}, UAS: {mahasiswa['uas']}, Nilai Akhir: {mahasiswa['nilai_akhir']:.2f}")


        print("================================================")
        print("| No | Nama | Tugas | UTS | UAS | Akhir |")
        print("================================================")
        for i, mahasiswa in enumerate(data_mahasiswa):
            print(f"| {i+1} | {mahasiswa['nama']} | {mahasiswa['tugas']} | {mahasiswa['uts']} | {mahasiswa['uas']} | {mahasiswa['nilai_akhir']:.2f} |")
        print("================================================")

PROSES INPUT DATA 
![kode 1](https://github.com/user-attachments/assets/e5d4f6d8-17fb-4422-aee7-faba6c5d4ffa)
![kode 2](https://github.com/user-attachments/assets/38ad1c6c-324b-4905-8390-e931caba24bf)

PROSES OUTPUT HASIL 
![hasil praktikum](https://github.com/user-attachments/assets/21d2f2ad-c64d-4805-bf05-3246be919eae)

PENJELASAN : 
1. Penggunaan while True berguna untuk terus meminta input dari pengguna atau pengulangan sampai diputuskan untuk berhenti oleh sang pengguna dengan menjawab antara 'y' atau 't'
2. Penginputan data mahasiswa yang berisi nama, nilai tugas, UTS, UAS, bertipe float yang memungkinkan pengguna memasukkan angka desimal
3. Penghitungan nilai akhir berdasarkan bobot yang telah ditentukan seperti, tugas:30%, UTS35%, UAS35% dan hasil penghitungan nilai akhir disimpan kedalam variable nilai_akhir
4. Penyimpanan data kedalam list dengan menggunakan metode append()
5. Menanyakan apakah ada data yang ingin ditambahkan atau tidak. Jika jawabannya 't' maka program akan berhenti dan mengeluarkan hasil penghitungan
6. Menampilkan data yang telah selesai diolah

FLOWCHART : 

![flowchart](https://github.com/user-attachments/assets/06e94ebd-b023-4561-9482-b85af296a77d)

# Latihan 

Buat sebuah list sebanyak 5 elemen dengan nilai bebas
1. akses list: tampilkan elemen ke 3, ambil nilai elemen ke 2 sampai elemen ke 4, ambil elemen terakhir
2. ubah elemen list: ubah elemen ke 4 dengan nilai lainnya, ubah elemen ke 4 sampai dengan elemen terakhir
3. tambah elemen list: ambil 2 bagian dari list pertama (A) dan jadikan list ke 2 (B), tambah list B dengan nilai string, tambah list B dengan 3 nilai, gabungkan list B dengan list A

        # Membuat list dengan 5 elemen
        A = [10, 20, 30, 40, 50]

        # Akses list
        print("List A:", A)

        # Tampilkan elemen ke-3
        print("Elemen ke-3:", A[2])

        # Ambil nilai elemen ke-2 sampai elemen ke-4
        print("Elemen ke-2 sampai ke-4:", A[1:4])

        # Ambil elemen terakhir
        print("Elemen terakhir:", A[-1])

        # Ubah elemen list
        # Ubah elemen ke-4 dengan nilai lainnya
        A[3] = 100
        print("Setelah mengubah elemen ke-4:", A)

        # Ubah elemen ke-4 sampai dengan elemen terakhir
        A[3:] = [200, 300]
        print("Setelah mengubah elemen ke-4 sampai terakhir:", A)

        # Tambah elemen list
        # Ambil 2 bagian dari list pertama (A) dan jadikan list ke-2 (B)
        B = A[1:3]
        print("List B (dari A):", B)

        # Tambah list B dengan nilai string
        B.append("String")
        print("Setelah menambah string ke B:", B)

        # Tambah list B dengan 3 nilai
        B.extend([400, 500, 600])
        print("Setelah menambah 3 nilai ke B:", B)

        # Gabungkan list B dengan list A
        C = A + B
        print("List C (gabungan A dan B):", C)

PROSES INPUT DATA
![Screenshot 2024-11-14 131534](https://github.com/user-attachments/assets/5520dd56-8f65-459f-8ac8-7209b829789b)
![Screenshot 2024-11-14 131624](https://github.com/user-attachments/assets/f4f949c2-3ebc-4d36-8f9d-e636092026ec)

HASIL OUTPUT 
![Screenshot 2024-11-14 131741](https://github.com/user-attachments/assets/0b266eed-ba9a-4a28-81de-0656e6a8d99f)

PENJELASAN : 
1. Di sini, kita membuat sebuah list bernama A yang berisi 5 elemen dengan nilai bebas: 10, 20, 30, 40, dan 50.
2. Mengakses elemen ke-3 dari list A. Dalam Python, indeks dimulai dari 0, jadi A[2] merujuk pada elemen ketiga, yaitu 30.
3. Mengambil elemen dari indeks 1 sampai 3 (indeks 4 tidak termasuk). Ini akan menghasilkan list baru yang berisi [20, 30, 40].
4. Mengakses elemen terakhir dari list A menggunakan indeks negatif. A[-1] merujuk pada elemen terakhir, yaitu 50.
5. Mengubah elemen ke-4 (indeks 3) menjadi 100. Setelah perubahan, list A menjadi [10, 20, 30, 100, 50].
6. Mengubah elemen dari indeks 3 hingga akhir list menjadi [200, 300]. List A sekarang menjadi [10, 20, 30, 200, 300].
7. Membuat list baru B yang berisi elemen dari A mulai dari indeks 1 sampai 2, yaitu [20, 30].
8. Menambahkan string "String" ke dalam list B. List B sekarang menjadi [20, 30, 'String'].
9. Menambahkan tiga nilai (400, 500, 600) ke dalam list B. List B sekarang menjadi [20, 30, 'String', 400, 500, 600].
10. Menggabungkan list A dan B menjadi list baru C. List C berisi semua elemen dari A diikuti oleh semua elemen dari B. Hasilnya adalah [10, 20, 30, 200, 300, 20, 30, 'String', 400, 500, 600].










