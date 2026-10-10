# Pertemuan 06 Nested Loop Python

Nama: Sekar Wahyuningrum

NIM: 2225250095

Kelas: 3E

## Tujuan

Menggunakan nested loop, pola, akumulasi, dan pencacahan.

## Cara Menjalankan

Jalankan program menggunakan Python:

```bash
python latihan/01_pasangan_indeks.py
python latihan/02_pola_segitiga.py
python latihan/03_jumlah_per_baris.py
python latihan/04_hitung_pasangan.py
python tugas/tabel_perkalian_dan_statistik.py
```

## Algoritma Tugas 3

- **Loop luar (`i`)** digunakan untuk menentukan baris pada tabel perkalian.
- **Loop dalam (`j`)** digunakan untuk menghitung setiap hasil perkalian pada baris.
- **Akumulator (`total_baris` dan `total_semua`)** digunakan untuk menjumlahkan hasil perkalian.
- **Counter (`count_genap`)** digunakan untuk menghitung banyaknya hasil perkalian yang bernilai genap.
- Setiap hasil perkalian dihitung dengan `hasil = i * j`.
- Jika hasil perkalian genap, maka `count_genap` ditambah 1.

## Hasil Pengujian

| Input `n` | Banyak Pasangan | Total Seluruh Hasil | Banyak Hasil Genap | Status |
|---:|---:|---:|---:|---|
| 1 | 1 | 1 | 0 | Berhasil |
| 2 | 4 | 9 | 3 | Berhasil |
| 3 | 9 | 36 | 5 | Berhasil |

### Contoh Hasil Tabel Perkalian untuk `n = 3`

| `i \ j` | 1 | 2 | 3 | Jumlah Baris |
|---:|---:|---:|---:|---:|
| 1 | 1 | 2 | 3 | 6 |
| 2 | 2 | 4 | 6 | 12 |
| 3 | 3 | 6 | 9 | 18 |
| **Total** | | | | **36** |

## Analisis Efisiensi

Untuk input `n`, loop luar berjalan sebanyak `n` kali dan loop dalam juga berjalan sebanyak `n` kali.

Jadi, badan loop dalam berjalan:

**n × n = n² kali**

Contoh:
- `n = 1` → 1² = **1 kali**
- `n = 2` → 2² = **4 kali**
- `n = 3` → 3² = **9 kali**
- `n = 5` → 5² = **25 kali**

Semakin besar nilai `n`, semakin banyak iterasi yang dilakukan program.

## Refleksi

Kesalahan yang ditemukan adalah kesalahan indentasi pada nested loop. Jika `print()` diletakkan pada posisi yang salah, pola atau hasil program dapat menjadi tidak sesuai.

Perbaikannya adalah memastikan indentasi menunjukkan bagian mana yang termasuk loop luar dan loop dalam.
