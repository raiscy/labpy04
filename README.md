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





