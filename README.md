# ANALISIS KOMPLEKSITAS ALGORITMA ITERATIF DAN REKURSIF PADA APLIKASI “KALKULATOR HOKI”

Nama Anggota :
1. I Kadek Rio Adi Pranata K_103132400029_SD-04-01
2. Maysa Azhra Fauziyyah_103132430005_SD-04-01 
3. Raymundus Ariel Abas_103132430021_SD-04-01

# Studi Kasus
Kalkulator Hoki merupakan sebuah program berbasis Python yang dirancang untuk menghitung nilai keberuntungan seseorang berdasarkan nama panggilan dan tanggal lahir. Perhitungan dilakukan dengan mengonversi setiap huruf dalam nama menjadi nilai numerik sesuai urutan alfabet (A=1, B=2, ..., Z=26), kemudian menjumlahkannya dan mengombinasikannya dengan nilai tanggal, bulan, dan tahun kelahiran untuk menghasilkan skor hoki akhir.

Program ini dikembangkan sebagai studi kasus untuk menganalisis dan membandingkan efisiensi dua pendekatan algoritma, yaitu iteratif dan rekursif, dalam menyelesaikan permasalahan yang sama. Fokus utama dari studi kasus ini adalah membandingkan running time serta menentukan kelas kompleksitas waktu dari kedua algoritma tersebut berdasarkan hasil pengujian.

# Deskripsi Program
- Input Pengguna
Pengguna diminta untuk memasukkan:
1. Nama panggilan
2. Tanggal lahir dengan format YYYY-MM-DD
- Proses Perhitungan
1. Setiap huruf pada nama panggilan dikonversi menjadi nilai numerik sesuai alfabet.
2. Seluruh huruf pada nama diproses tanpa batasan jumlah karakter.
3. Nilai huruf dijumlahkan menggunakan dua pendekatan algoritma: Algoritma iteratif dan Algoritma rekursif
4. Nilai hoki dihitung dengan menambahkan nilai tanggal, bulan, dan tahun kelahiran, kemudian dimodulus 100.
- Output
Program menampilkan:
1. Nilai hoki pengguna
2. Waktu eksekusi algoritma iteratif
3. Waktu eksekusi algoritma rekursif
4. Tabel hasil pengujian
5. Grafik perbandingan running time kedua algoritma

# Struktur Program
File Notebook
Notebook utama berisi seluruh implementasi program, mulai dari pendefinisian fungsi, proses input data pengguna, perhitungan nilai hoki, penyimpanan hasil pengujian, hingga visualisasi grafik perbandingan running time algoritma iteratif dan rekursif.
Library yang Digunakan, Program memanfaatkan beberapa library pendukung, yaitu:
1. datetime untuk pengolahan tanggal lahir
2. time untuk pengukuran waktu eksekusi
3. matplotlib untuk visualisasi grafik
4. tabulate untuk menampilkan tabel hasil pengujian

## Flowchart Program

![FlowChart] (https://github.com/maysaazhra/TugasBesarAnalisisKompleksitasAlgoritma-KalkulatorHoki/edit/main/README.md/Flowchart Struktur Program.png)

# Deskripsi Algoritma yang Dipilih
- Algoritma Iteratif
Algoritma iteratif menghitung total nilai nama menggunakan perulangan. Setiap huruf diproses satu per satu dan nilainya ditambahkan ke dalam variabel akumulator. Pendekatan ini sederhana dan efisien dalam penggunaan memori karena tidak melibatkan pemanggilan fungsi berulang. Kompleksitas waktu algoritma iteratif adalah O(n), dengan n merupakan jumlah huruf pada nama.
- Algoritma Rekursif
Algoritma rekursif menghitung nilai nama dengan memanggil fungsi secara berulang. Setiap pemanggilan fungsi memproses satu huruf dan memanggil dirinya sendiri untuk sisa nama hingga kondisi dasar tercapai.Kompleksitas waktu algoritma rekursif juga O(n), namun memiliki overhead memori tambahan akibat penggunaan call stack.

# Grafik Perbandingan Running Time
Grafik perbandingan running time menunjukkan bahwa waktu eksekusi kedua algoritma meningkat seiring bertambahnya panjang nama. Pola pertumbuhan waktu eksekusi algoritma iteratif dan rekursif relatif serupa karena keduanya memproses jumlah karakter yang sama. Perbedaan waktu yang muncul disebabkan oleh perbedaan mekanisme eksekusi dan overhead fungsi pada algoritma rekursif.

# Analisis Perbandingan Iteratif & Rekursif
Berdasarkan hasil pengujian, kedua algoritma memiliki kompleksitas waktu yang sama, yaitu O(n). Algoritma iteratif lebih unggul dalam efisiensi memori karena tidak menggunakan call stack, sedangkan algoritma rekursif menawarkan struktur kode yang lebih modular dan mudah dikembangkan. Dalam konteks program ini, perbedaan performa tidak terlalu signifikan karena ukuran input relatif kecil.

# Hasil dan Manfaat
Program Kalkulator Hoki memberikan beberapa manfaat, antara lain:
1. Interaksi Pengguna: Program bersifat interaktif karena pengguna dapat memasukkan data nama dan tanggal lahir secara langsung.
2. Analisis Algoritma: Program memungkinkan perbandingan performa antara algoritma iteratif dan rekursif secara nyata.

# Kesimpulan
Dari hasil analisis yang dilakukan, dapat disimpulkan bahwa algoritma iteratif dan rekursif sama-sama efektif untuk digunakan dalam program Kalkulator Hoki. Keduanya memiliki kompleksitas waktu O(n) karena memproses seluruh huruf pada nama pengguna. Pemilihan algoritma terbaik bergantung pada kebutuhan aplikasi, apakah mengutamakan efisiensi memori atau kejelasan struktur kode.

# Referensi
1. T. H. Cormen et al., Introduction to Algorithms, MIT Press, 2009.
2. D. E. Knuth, The Art of Computer Programming, Addison-Wesley, 1973.
3. R. Sedgewick and K. Wayne, Algorithms, Addison-Wesley, 2011.
4. Visualisasi Data: Hasil pengukuran waktu eksekusi ditampilkan dalam bentuk tabel dan grafik sehingga lebih mudah dianalisis.
5. Pembelajaran Konsep Algoritma: Program membantu memahami perbedaan implementasi iteratif dan rekursif dalam kasus sederhana.
