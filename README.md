### Beberapa Konsep Dasar Statistika
Populasi, sampel dan observasi/pengamatan
Observasi: Adalah suatu unit yang diukur dengan data. Beberapa contoh diantaranya adalah:

Siswa
Warga negara
Hewan
Kendaraan
Populasi: Adalah koleksi dari keseluruhan observasi. Beberapa contoh diantaranya adalah:

Semua siswa yang ada di sekolah
Semua warga negara Indonesia,
Semua hewan yang ada di hutan lindung,
Semua kendaraan di Jakarta
Sampel: Adalah sub koleksi dari populasi. Beberapa contoh diantaranya adalah:

5 siswa dari masing-masing kelas di suatu sekolah
100 warga negara Indonesia yang diambil dari beberapa wilayah
Beberapa species hewan tertentu di suatu hutan lindung
3 jenis kendaraan di Jakarta

Parameter adalah penjelasan atas populasi sedangkan statistik hanya menjelaskan sampel dari populasi. Untuk kasus terkait segmentasi pasar, mengukur revenue dari setiap orang di dalam segmen adalah parameter sedangkan jika kita hanya mengambil 20% dari tiap segmen hal ini dikatakan sebagai statistik.

### Data Kualitatif dan Data Kuantitatif
Terdapat dua kategori data yang terdapat pada populasi atau sampel, yaitu data kualitatif dan data kuantitatif.

Data kualitatif adalah data yang diperoleh dari mengkategorikan atau menjelaskan suatu atribut dari populasi atau sampel. Biasanya disebut juga sebagai data kategorik. Beberapa contoh data kualitatif misalnya warna rambut, golongan darah, nama jalan, nama produk yang digunakan dan lain sebagainya.Biasanya data kualitatif selalu disebutkan dalam bentuk kata ataupun simbol.

Data kuantitatif adalah data yang diperoleh dari ukuran atau hitungan di suatu populasi atau sampel. Data kuantitatif selalu berbentuk angka. Data seperti gaji, berat badan, populasi di suatu negara, dan jumlah pelanggan yang dimiliki suatu e-commerce termasuk data kuantitatif. Data kuantitatif sendiri dapat dibagi menjadi dua yaitu data diskrit dan data kontinu.

Data yang diperoleh dari hasil perhitungan adalah data diskrit: jumlah pelanggan, jumlah produk, dan jumlah telefon yang diterima oleh customer service per harinya adalah beberapa contoh data diskrit.

Data yang diperoleh dari hasil perhitungan namun dapat memuat rasio, desimal, atau bilangan irasional adalah data kontinu: berat badan, tinggi badan, waktu, dan gaji adalah beberapa contoh data kontinu.

### Tipe Statistika
Statistika deskriptif digunakan untuk melakukan eksplorasi pada data, biasanya menggunakan teknik visualisasi data sebagai alat bantu untuk memahami bagaimana bentuk distribusi dan hubungan antara satu titik data dengan titik data lainnya.

Statistika inferensial digunakan untuk melakukan pemgambilan keputusan atas suatu simpulan terkait dengan data yang sedang dianalisa. Statistika inferensi memungkinkan kita mengambil kesimpulan dari suatu populasi dengan menggunakan sampel yang diambil dari populasi tersebut.

download.png

### Skala Pengukuran - Data Kategorikal
Ada beberapa skala pengukuran sebagaimana ada beberapa cara kita dapat mengelompokkan objek yang ingin kita ukur. Beberapa tingkatan tersebut adalah:
download (1).png

Skala Nominal
Skala nominal adalah skala yang digunakan untuk mengkategorikan suatu objek pengamatan dengan objek pengamatan lainnya. Sebagai contoh yang termasuk skala nominal seperti gender, kategori barang, ras, status pernikahan dan lain sebagainya

Skala Ordinal
Skala ordinal adalah skala yang digunakan untuk mengurutkan suatu objek pengamatan dimana suatu titik pengamatan memiliki nilai yang lebih rendah atau tinggi dibanding nilai lainnya. Sebagai contoh yang termasuk skala nominal adalah kelas, jabatan, tingkat pendidikan, dan sebagainya


### Skala Pengukuran - Data Numerikal
Ada beberapa skala pengukuran sebagaimana ada beberapa cara kita dapat mengelompokkan objek yang ingin kita ukur. Beberapa tingkatan tersebut adalah:
download (2).png
Skala Interval
Skala interval adalah skala yang digunakan untuk tidak hanya untuk mengklasifikasikan maupun memberikan tingkatan pada suatu titik pengamatan, namun kita dapat mengukur seberapa besar nilai antara suatu titik pengamatan dengan titik pengamatan lainnya. Beberapa contoh yang termasuk skala interval diantaranya adalah suhu tubuh dan jarak

Skala Rasio
Skala rasio memiliki kemiripan dengan skala interval, perbedaannya terletak pada nilai 0 pada skala rasio. Berbeda dengan skala interval yang tidak memiliki nilai 0 yang tidak pasti.


### Package Statistika di Python
Untuk melakukan perhitungan statistika, kita dapat menggunakan beberapa package atau library berikut yang tersedia di Python. Diantaranya adalah:

numpy: digunakan untuk melakukan analisa data numerik dan perhitungan berbasis vektor atau matriks
pandas: digunakan untuk melakukan pengolahan data tabular
matplotlib: digunakan untuk melakukan ploting atau penggambaran grafik, dapat digunakan sebagai alat bantu dalam analisa data
statsmodels: digunakan untuk melakukan uji hipotesa, eksplorasi data maupun pemodelan statistika
scipy: digunakan untuk melakukan uji statistika, juga dapat digunakan untuk melakukan pemodelan statistika
Sebenarnya masih banyak lagi library python untuk pengolahan data statistika, namun untuk materi ini cukup 4 atau 5 library di atas saja yang akan kita gunakan.

### Pengenalan Numpy dan Pandas
Kedua library ini, numpy dan pandas, adalah library yang umum digunakan untuk melakukan pengolahan data, mulai dari membaca data dalam format tertentu (csv, xlsx, xls, tsv) atau dari sumber tertentu (RDBMS, No-SQL), melakukan inspeksi (mengecek data yang hilang, inkonsistensi pada data) dan pengolahan data (transformasi nilai, encoding, normalisasi) sampai visualisasi data untuk membuat laporan atau mempersiapkan data untuk membuat model.

Numpy adalah library yang biasanya digunakan untuk manipulasi array atau vektor. Perhitungan yang melibatkan operasi pada objek berbentuk matriks, vektor atau bahkan multidimensi vektor (misalnya data gambar dengan skema warna RGB) dapat kita lakukan dengan menggunakan numpy.

Pandas adalah library yang biasanya digunakan untuk analisa data atau biasa disebut sebagai data wrangling. Biasanya data yang diolah oleh pandas berbentuk tabular atau tabel layaknya spreadsheet di Excel. Pandas menggunakan numpy sebagai back-end sehingga beberapa fungsi atau method dari numpy dapat digunakan di objek pandas.

### Load Library
Biasanya pada awal mula sebelum melakukan pengolahan data kita memanggil library yang diinginkan untuk digunakan dalam analisa data, dalam hal ini kita akan memuat numpy dan pandas.
sou :
# memuat numpy sebagai np
import numpy as np
# memuat pandas sebagai pd
import pandas as pd

### Load Dataset
Pada tahap pertama ketika ingin menganalisa data kita biasanya memuat data yang disimpan di salah satu folder untuk dimuat ke IDE atau interactive notebook seperti Jupyter. Untuk memuat data dalam format csv kita dapat menggunakan method .read_csv() dari pandas sebagaimana contoh berikut:

sou :
# memuat data bernama 'dataset_statistics.csv' dan memasukkan hasilnya ke dalam 'raw_data'
raw_data = pd.read_csv("https://storage.googleapis.com/dqlab-dataset/dataset_statistic.csv", sep=';')

### Inspeksi Data
Untuk melihat keseluruhan data cukup memanggil nama variabelnya dengan fungsi :


sou :
print (raw_data)
# melihat 10 data pada baris pertama
print (raw_data.head(10))
# melihat 5 data pada baris terakhir
print (raw_data.tail())

out:
   ID Pelanggan     Nama  Jenis Kelamin  Pendapatan Produk   Harga  Jumlah   \
0              1     Arif              1      600000      A  100000        4   
1              2     Dian              2     1200000      D  250000        4   
2              3    Dinda              2      950000      D  250000        3   
3              4    Fajar              1      400000      A  100000        2   
4              5      Ika              2     1200000      D  250000        4   
5              6    Ilham              1      800000      B  150000        4   
6              7    Indra              1      950000      B  150000        5   
7              8  Kartika              2     1100000      E  300000        3   
8              9  Lestari              2      800000      E  300000        2   
9             10      Lia              2     1700000      E  300000        5   
10            11    Maria              2      600000      A  100000        4   
11            12     Maya              2      950000      B  150000        5   
12            13     Mila              2      400000      C  200000        1   
13            14    Nurul              2     6450000      D  250000        5   
14            15    Retno              2     1000000      C  200000        4   
15            16     Rini              2      800000      B  150000        4   
16            17    Rizki              1     1200000      C  200000        5   
17            18     Sari              2      700000      D  250000        2   
18            19     Tyas              2      600000      A  100000        4   
19            20    Wahyu              1      800000      C  200000        3   

      Total  Tingkat Kepuasan  
0    400000                 2  
1   1000000                 2  
2    750000                 3  
3    200000                 3  
4   1000000                 2  
5    600000                 3  
6    750000                 1  
7    900000                 3  
8    600000                 1  
9   1500000                 1  
10   400000                 3  
11   750000                 3  
12   200000                 2  
13  1250000                 1  
14   800000                 2  
15   600000                 1  
16  1000000                 3  
17   500000                 1  
18   400000                 3  
19   600000                 1  
   ID Pelanggan     Nama  Jenis Kelamin  Pendapatan Produk   Harga  Jumlah   \
0             1     Arif              1      600000      A  100000        4   
1             2     Dian              2     1200000      D  250000        4   
2             3    Dinda              2      950000      D  250000        3   
3             4    Fajar              1      400000      A  100000        2   
4             5      Ika              2     1200000      D  250000        4   
5             6    Ilham              1      800000      B  150000        4   
6             7    Indra              1      950000      B  150000        5   
7             8  Kartika              2     1100000      E  300000        3   
8             9  Lestari              2      800000      E  300000        2   
9            10      Lia              2     1700000      E  300000        5   

     Total  Tingkat Kepuasan  
0   400000                 2  
1  1000000                 2  
2   750000                 3  
3   200000                 3  
4  1000000                 2  
5   600000                 3  
6   750000                 1  
7   900000                 3  
8   600000                 1  
9  1500000                 1  
    ID Pelanggan   Nama  Jenis Kelamin  Pendapatan Produk   Harga  Jumlah   \
15            16   Rini              2      800000      B  150000        4   
16            17  Rizki              1     1200000      C  200000        5   
17            18   Sari              2      700000      D  250000        2   
18            19   Tyas              2      600000      A  100000        4   
19            20  Wahyu              1      800000      C  200000        3   

      Total  Tingkat Kepuasan  
15   600000                 1  
16  1000000                 3  
17   500000                 1  
18   400000                 3  
19   600000                 1  

### Metode Shape
sou :
#melihat dimensi dari raw_data
print (raw_data.shape)
#mengambil jumlah data
print (raw_data.shape[0])

ou :
(20, 9)
20

### Melihat Kolom Dalam Dataset
Kolom apa saja yang terdapat dalam dataset?

Untuk melihat kolom apa saja yang terdapat pada dataset cukup menggunakan method columns: 


sou :
print (raw_data)
print (raw_data.columns)

out:
ID Pelanggan     Nama  Jenis Kelamin  Pendapatan Produk   Harga  Jumlah   \
0              1     Arif              1      600000      A  100000        4   
1              2     Dian              2     1200000      D  250000        4   
2              3    Dinda              2      950000      D  250000        3   
3              4    Fajar              1      400000      A  100000        2   
4              5      Ika              2     1200000      D  250000        4   
5              6    Ilham              1      800000      B  150000        4   
6              7    Indra              1      950000      B  150000        5   
7              8  Kartika              2     1100000      E  300000        3   
8              9  Lestari              2      800000      E  300000        2   
9             10      Lia              2     1700000      E  300000        5   
10            11    Maria              2      600000      A  100000        4   
11            12     Maya              2      950000      B  150000        5   
12            13     Mila              2      400000      C  200000        1   
13            14    Nurul              2     6450000      D  250000        5   
14            15    Retno              2     1000000      C  200000        4   
15            16     Rini              2      800000      B  150000        4   
16            17    Rizki              1     1200000      C  200000        5   
17            18     Sari              2      700000      D  250000        2   
18            19     Tyas              2      600000      A  100000        4   
19            20    Wahyu              1      800000      C  200000        3   

      Total  Tingkat Kepuasan  
0    400000                 2  
1   1000000                 2  
2    750000                 3  
3    200000                 3  
4   1000000                 2  
5    600000                 3  
6    750000                 1  
7    900000                 3  
8    600000                 1  
9   1500000                 1  
10   400000                 3  
11   750000                 3  
12   200000                 2  
13  1250000                 1  
14   800000                 2  
15   600000                 1  
16  1000000                 3  
17   500000                 1  
18   400000                 3  
19   600000                 1  
Index(['ID Pelanggan', 'Nama', 'Jenis Kelamin', 'Pendapatan', 'Produk',
       'Harga', 'Jumlah ', 'Total', 'Tingkat Kepuasan'],
      dtype='object')
      

### Metode Isna
Ada berapa banyak data yang hilang dari dataset?

Untuk melihat data dari dataset bisa menggunakan method isna: 

sou :
print (raw_data.isna())
print (raw_data.isna().sum())


out :
ID Pelanggan   Nama  Jenis Kelamin  Pendapatan  Produk  Harga  Jumlah   \
0          False  False          False       False   False  False    False   
1          False  False          False       False   False  False    False   
2          False  False          False       False   False  False    False   
3          False  False          False       False   False  False    False   
4          False  False          False       False   False  False    False   
5          False  False          False       False   False  False    False   
6          False  False          False       False   False  False    False   
7          False  False          False       False   False  False    False   
8          False  False          False       False   False  False    False   
9          False  False          False       False   False  False    False   
10         False  False          False       False   False  False    False   
11         False  False          False       False   False  False    False   
12         False  False          False       False   False  False    False   
13         False  False          False       False   False  False    False   
14         False  False          False       False   False  False    False   
15         False  False          False       False   False  False    False   
16         False  False          False       False   False  False    False   
17         False  False          False       False   False  False    False   
18         False  False          False       False   False  False    False   
19         False  False          False       False   False  False    False   

    Total  Tingkat Kepuasan  
0   False             False  
1   False             False  
2   False             False  
3   False             False  
4   False             False  
5   False             False  
6   False             False  
7   False             False  
8   False             False  
9   False             False  
10  False             False  
11  False             False  
12  False             False  
13  False             False  
14  False             False  
15  False             False  
16  False             False  
17  False             False  
18  False             False  
19  False             False  
ID Pelanggan        0
Nama                0
Jenis Kelamin       0
Pendapatan          0
Produk              0
Harga               0
Jumlah              0
Total               0
Tingkat Kepuasan    0
dtype: int64

### Metode Describe
Untuk bisa melihat ringkasan dari data misalnya rerata, jumlah, nilai maksimum-minimum dan ukuran lainnya, kita dapat menggunakan method .describe():

sou :
print (raw_data.describe())

# Mencari nilai maksimum dari tiap kolom
raw_data.max()

# Mencari nilai maksimum dari kolom 'Harga'
raw_data['Harga'].max()

# Mencari nilai minimum dari kolom 'Harga'
raw_data['Harga'].min()

out:
ID Pelanggan  Jenis Kelamin    Pendapatan          Harga    Jumlah   \
count      20.00000      20.000000  2.000000e+01      20.000000  20.000000   
mean       10.50000       1.700000  1.160000e+06  197500.000000   3.650000   
std         5.91608       0.470162  1.282842e+06   69726.910912   1.182103   
min         1.00000       1.000000  4.000000e+05  100000.000000   1.000000   
25%         5.75000       1.000000  6.750000e+05  150000.000000   3.000000   
50%        10.50000       2.000000  8.750000e+05  200000.000000   4.000000   
75%        15.25000       2.000000  1.125000e+06  250000.000000   4.250000   
max        20.00000       2.000000  6.450000e+06  300000.000000   5.000000   

              Total  Tingkat Kepuasan  
count  2.000000e+01         20.000000  
mean   7.100000e+05          2.050000  
std    3.338768e+05          0.887041  
min    2.000000e+05          1.000000  
25%    4.750000e+05          1.000000  
50%    6.750000e+05          2.000000  
75%    9.250000e+05          3.000000  
max    1.500000e+06          3.000000  
Out[7]:
100000

### Metode Sum
Jumlah dari semua nilai pada kolom dengan method .sum() agar menghasilkan :

sou :
# menghitung jumlah dari semua kolom
print (raw_data.sum())

# menghitung jumlah dari semua kolom bertipe data numerik saja
raw_data.sum(numeric_only=True)

# menghitung jumlah dari kolom 'Harga' dan 'Pendapatan'
raw_data[['Harga', 'Pendapatan']].sum()

out :
ID Pelanggan                                                      210
Nama                ArifDianDindaFajarIkaIlhamIndraKartikaLestariL...
Jenis Kelamin                                                      34
Pendapatan                                                   23200000
Produk                                           ADDADBBEEEABCDCBCDAC
Harga                                                         3950000
Jumlah                                                             73
Total                                                        14200000
Tingkat Kepuasan                                                   41
dtype: object

Harga          3950000
Pendapatan    23200000
dtype: int64

### Manipulasi Dataframe - Memilih Kolom dan Baris
Terkadang kita hanya ingin melakukan analisa sebagian kecil dari data atau hanya beberapa kolom saja, untuk itu kita dapat melakukan slice-and-dice pada data yang kita punya.

Untuk memilih kolom untuk dianalisa, kita dapat memanggil objek dataframe yang sudah dibuat dan menggunakan tanda ['nama_kolom'] untuk memilih satu kolom atau [['nama_kolom_1', 'nama_kolom_2', ..., 'nama_kolom_n']] untuk memilih lebih dari 1 kolom

sou :
# Memilih kolom 'Pendapatan' saja
print (raw_data['Pendapatan'])

# Memilih kolom 'Jenis Kelamin' dan 'Pendapatan'
print (raw_data[['Jenis Kelamin', 'Pendapatan']])

out :
0      600000
1     1200000
2      950000
3      400000
4     1200000
5      800000
6      950000
7     1100000
8      800000
9     1700000
10     600000
11     950000
12     400000
13    6450000
14    1000000
15     800000
16    1200000
17     700000
18     600000
19     800000
Name: Pendapatan, dtype: int64
    Jenis Kelamin  Pendapatan
0               1      600000
1               2     1200000
2               2      950000
3               1      400000
4               2     1200000
5               1      800000
6               1      950000
7               2     1100000
8               2      800000
9               2     1700000
10              2      600000
11              2      950000
12              2      400000
13              2     6450000
14              2     1000000
15              2      800000
16              1     1200000
17              2      700000
18              2      600000
19              1      800000


### Metode Loc
Untuk memilih baris, kita dapat menggunakan [m:n] untuk mengambil baris data ke-m sampai ke-(n-1) atau bisa juga menggunakan method loc untuk pemilihan baris yang lebih spesifik.

sou :
# mengambil data dari baris ke-0 sampai baris ke-(10-1) atau baris ke-9
print (raw_data[:10])

# mengambil data dari baris ke-3 sampai baris ke-(5-1) atau baris ke-4
print (raw_data[3:5])

# mengambil data pada baris ke-1, ke-3 dan ke-10
print (raw_data.loc[[1,3,10]])

# Mengambil kolom 'Jenis Kelamin' dan 'Pendapatan' dan ambil baris ke-1 sampai ke-9
print (raw_data[['Jenis Kelamin', 'Pendapatan']][1:10])

# Mengambil kolom 'Harga' dan 'Tingkat Kepuasan' dan ambil baris ke-1, ke-10 dan ke-15
print (raw_data[['Harga', 'Tingkat Kepuasan']].loc[[1,10,15]])

out:
ID Pelanggan     Nama  Jenis Kelamin  Pendapatan Produk   Harga  Jumlah   \
0             1     Arif              1      600000      A  100000        4   
1             2     Dian              2     1200000      D  250000        4   
2             3    Dinda              2      950000      D  250000        3   
3             4    Fajar              1      400000      A  100000        2   
4             5      Ika              2     1200000      D  250000        4   
5             6    Ilham              1      800000      B  150000        4   
6             7    Indra              1      950000      B  150000        5   
7             8  Kartika              2     1100000      E  300000        3   
8             9  Lestari              2      800000      E  300000        2   
9            10      Lia              2     1700000      E  300000        5   

     Total  Tingkat Kepuasan  
0   400000                 2  
1  1000000                 2  
2   750000                 3  
3   200000                 3  
4  1000000                 2  
5   600000                 3  
6   750000                 1  
7   900000                 3  
8   600000                 1  
9  1500000                 1  
   ID Pelanggan   Nama  Jenis Kelamin  Pendapatan Produk   Harga  Jumlah   \
3             4  Fajar              1      400000      A  100000        2   
4             5    Ika              2     1200000      D  250000        4   

     Total  Tingkat Kepuasan  
3   200000                 3  
4  1000000                 2  
    ID Pelanggan   Nama  Jenis Kelamin  Pendapatan Produk   Harga  Jumlah   \
1              2   Dian              2     1200000      D  250000        4   
3              4  Fajar              1      400000      A  100000        2   
10            11  Maria              2      600000      A  100000        4   

      Total  Tingkat Kepuasan  
1   1000000                 2  
3    200000                 3  
10   400000                 3  
   Jenis Kelamin  Pendapatan
1              2     1200000
2              2      950000
3              1      400000
4              2     1200000
5              1      800000
6              1      950000
7              2     1100000
8              2      800000
9              2     1700000
     Harga  Tingkat Kepuasan
1   250000                 2
10  100000                 3
15  150000                 1


### Ukuran Pusat (Measures of Central Tendency)
Ukuran pusat (measures of central tendency) adalah statistika deskriptif yang dapat digunakan untuk membantu kita mengidentifikasi kasus-kasus tipikal di dalam sebuah sampel atau populasi

Terdapat beberapa jenis ukuran pusat yang dapat digunakan untuk menganalisa data, diantaranya:

Mean atau rerata
Median
Modus

### Rata-rata (Mean)
Rata-rata atau mean adalah salah satu ukuran pusat yang nilainya diperoleh dengan cara menjumlahkan semua nilai titik data yang ada lalu dibagi oleh jumlah data. 
Kita dapat menghitung nilai rata-rata menggunakan method .mean() pada numpy atau pandas sebagaimana pada contoh berikut:

sou :
# mengambil hanya data untuk produk 'A'
produk_A = raw_data[raw_data['Produk'] == 'A']
# menghitung rerata pendapatan menggunakan method .mean pada objek pandas DataFrame
print (produk_A['Pendapatan'].mean())
# menghitung rerata pendapatan menggunakan method .mean pada objek pandas DataFrame dengan numpy

out:
550000.0
550000.0

### Median
Median adalah salah satu ukuran pusat yang nilainya terletak di tengah titik data. Sebagai gambaran, jika kita memiliki titik data bernilai 1, 2, 3, 4, 4, 5, 6 maka median dari sekumpulan titik data tersebut adalah 4.

sou :
print (raw_data)
# Hitung median dari pendapatan menggunakan pandas
print (produk_A['Pendapatan'].median())

# Hitung median dari pendapatan menggunakan numpy
print (np.median(produk_A['Pendapatan']))

out :
ID Pelanggan     Nama  Jenis Kelamin  Pendapatan Produk   Harga  Jumlah   \
0              1     Arif              1      600000      A  100000        4   
1              2     Dian              2     1200000      D  250000        4   
2              3    Dinda              2      950000      D  250000        3   
3              4    Fajar              1      400000      A  100000        2   
4              5      Ika              2     1200000      D  250000        4   
5              6    Ilham              1      800000      B  150000        4   
6              7    Indra              1      950000      B  150000        5   
7              8  Kartika              2     1100000      E  300000        3   
8              9  Lestari              2      800000      E  300000        2   
9             10      Lia              2     1700000      E  300000        5   
10            11    Maria              2      600000      A  100000        4   
11            12     Maya              2      950000      B  150000        5   
12            13     Mila              2      400000      C  200000        1   
13            14    Nurul              2     6450000      D  250000        5   
14            15    Retno              2     1000000      C  200000        4   
15            16     Rini              2      800000      B  150000        4   
16            17    Rizki              1     1200000      C  200000        5   
17            18     Sari              2      700000      D  250000        2   
18            19     Tyas              2      600000      A  100000        4   
19            20    Wahyu              1      800000      C  200000        3   

      Total  Tingkat Kepuasan  
0    400000                 2  
1   1000000                 2  
2    750000                 3  
3    200000                 3  
4   1000000                 2  
5    600000                 3  
6    750000                 1  
7    900000                 3  
8    600000                 1  
9   1500000                 1  
10   400000                 3  
11   750000                 3  
12   200000                 2  
13  1250000                 1  
14   800000                 2  
15   600000                 1  
16  1000000                 3  
17   500000                 1  
18   400000                 3  
19   600000                 1  
600000.0
600000.0

### Modus
Modus didefinisikan sebagai data yang memiliki frekuensi kemunculan terbanyak/terbesar. Sebagai contoh, jika terdapat titik data seperti berikut: 1, 1, 1, 1, 2, 3, 3, 4 maka modus dari data tersebut adalah 1 karena 1 muncul sebanyak 4 kali, lebih banyak dibanding titik data lainnya.

Kita dapat menggunakan method .count_values() pada pandas sebagaimana contoh berikut:

sou :
# Melihat jumlah dari masing-masing produk
print (raw_data['Produk'].value_counts())


out :
D    5
B    4
A    4
C    4
E    3
Name: Produk, dtype: int64

### Kuantil
Kuantil adalah nilai-nilai data yang membagi data yang telah diurutkan sebelumnya menjadi beberapa bagian yang sama besar ukurannya. Beberapa ukuran fraktil ini diantaranya adalah:

Kuartil: Adalah kuantil yang membagi data menjadi empat bagian sama besar. Kuartil ke-2 dari adalah median dari data tersebut.
Desil: Adalah kuantil yang membagi data menjadi 10 bagian sama besar.
Persentil: Adalah kuantil yang membagi data menjadi 100 bagian sama besar.
Untuk mencari fraktil dari data, kita dapat menggunakan method .quantile dari pandas atau numpy sebagaimana contoh berikut:


sou :
# mencari median atau 50% dari data menggunakan pandas
print (raw_data['Pendapatan'].quantile(q = 0.5))

# mencari median atau 50% dari data menggunakan pandas
print (np.quantile(raw_data['Pendapatan'], q=0.5))

out:
875000.0
875000.0

### Agregasi Data dengan method .agg()
Ada kalanya kita ingin menghitung sekaligus beberapa ukuran, misalnya menghitung nilai mean sekaligus menghitung nilai median. Kita dapat melakukan kedua hal tersebut dengan menggunakan method .agg() pada objek pandas DataFrame sebagaimana contoh berikut:

sou :
# menghitung rerata dan median usia (age) dan insulin (insu)
print (raw_data[['Pendapatan', 'Harga']].agg([np.mean, np.median]))

# menghitung rerata dan median Pendapatan dan Harga dari tiap produk
print (raw_data[['Pendapatan', 'Harga', 'Produk']].groupby('Produk').agg([np.mean, np.median]))

out:
 Pendapatan     Harga
mean     1160000.0  197500.0
median    875000.0  200000.0
       Pendapatan            Harga        
             mean   median    mean  median
Produk                                    
A          550000   600000  100000  100000
B          875000   875000  150000  150000
C          850000   900000  200000  200000
D         2100000  1200000  250000  250000
E         1200000  1100000  300000  300000


### Ukuran Sebaran (Measures of Dispersion)
Ukuran sebaran (measure of dispersion) adalah statistika deskriptif yang digunakan untuk membantu kita memahami sebaran titik data di dalam sebuah sampel ataupun populasi.

Terdapat beberapa ukuran sebaran yang biasanya digunakan tergantung pada jenis atau tipe datanya, yaitu:

Tipe Data Nominal dan Ordinal
Proporsi Kategori (Categorical Proportion)
Persen Proporsi (Percent Proportion)
Rasio Variasi (Variation Ratio)
Tipe Data Interval dan Rasio
Rentang (Range)
Variansi (Variance)
Deviasi Baku (Standard Deviation)

### Proporsi Kategori
Proporsi kategori adalah ukuran sebaran yang paling sederhana dari ukuran sebaran pada data nomisal dan ordinal. 

sou:
# cari proporsi tiap Produk
print (raw_data['Produk'].value_counts()/raw_data.shape[0])

out :
D    0.25
B    0.20
A    0.20
C    0.20
E    0.15
Name: Produk, dtype: float64

### Ukuran Sebaran pada Data Interval dan Rasio
Rentang (range)
Rentang adalah jarak antara nilai maksimum dengan nilai minimum. Semakin besar jarang antara nilai maksimum dan minimum semakin besar pula sebaran datanya. Secara matematis dapat dituliskan sebagai berikut:

 

Range=max(X)−min(X)
 

Dengan X adalah sampel atau populasi yang sedang diamati.

sou :
# Cari nilai rentang dari kolom 'Pendapatan'
print (raw_data['Pendapatan'].max() - raw_data['Pendapatan'].min())

ou :
6050000

### Variansi
Variansi adalah ukuran sebaran pusat yang diperoleh dengan cara menghitung jarak antara tiap titik data pada sampel atau populasi dengan nilai mean.

sou :
# menghitung variansi umur menggunakan method .var() dari pandas
print (raw_data['Pendapatan'].var())
# menghitung variansi umur menggunakan method .var() dari numpy
print (np.var(raw_data['Pendapatan']))
# mengatur variansi populasi dengan method `.var()` dari pandas
print (raw_data['Pendapatan'].var(ddof = 0))

ou :
1645684210526.3157
1563400000000.0
1563400000000.0

### Deviasi Baku (Standard Deviation)
Deviasi baku adalah ukuran sebaran pusat yang diperoleh dengan cara menarik akar kuadrat dari hasil perhitungan variansi. Hal ini dilakukan karena nilai variansi umumnya memiliki nilai yang lebih besar daripada nilai aslinya sebagai efek dari pengkuadratan dan ini menjadikan variansi sulit untuk diinterpretasikan.
Kita dapat menghitung deviasi baku menggunakan method .std dari numpy maupun pandas.

sou:
#menghitung deviasi baku sampel pendapatan menggunakan method std() dari pandas
print (raw_data['Pendapatan'].std())
#menghitung deviasi baku pendapatan menggunakan method std() dari numpy
print (np.std(raw_data['Pendapatan'], ddof = 1))

ou: 
1282842.2391417876
1282842.2391417876

### Korelasi
Korelasi adalah salah satu metode statistika yang dapat digunakan untuk mengukur seberapa besar hubungan antara satu variabel dengan variabel lainnya. Sebagai contoh, misalnya mencari hubungan antara tinggi badan dengan berat badan, mencari hubungan antara gender dengan penghasilan dan masih banyak aplikasi penggunaan korelasi.

Terdapat beberapa metode yang dapat digunakan untuk menghitung korelasi antara sepasang variabel tergantung tipe dari sepasang variabel tersebut. Diantaranya adalah:

Korelasi Pearson
Korelasi Spearman
Korelasi Kendall

### Menghitung Korelasi
# menghitung korelasi dari setiap pasang variabel pada raw_data
print (raw_data.corr())

# mencari korelasi 'kendall' untuk tiap pasang variabel
print (raw_data.corr(method='kendall'))

# mencari korelasi 'spearman' untuk tiap pasang variabel
print (raw_data.corr(method='spearman'))

out:

ID Pelanggan  Jenis Kelamin  Pendapatan     Harga   Jumlah   \
ID Pelanggan          1.000000       0.151375    0.110958 -0.028707  0.011289   
Jenis Kelamin         0.151375       1.000000    0.192849  0.457555 -0.104168   
Pendapatan            0.110958       0.192849    1.000000  0.322443  0.399825   
Harga                -0.028707       0.457555    0.322443  1.000000 -0.138883   
Jumlah                0.011289      -0.104168    0.399825 -0.138883  1.000000   
Total                -0.039968       0.238051    0.592044  0.645455  0.636097   
Tingkat Kepuasan     -0.245717      -0.088339   -0.312663 -0.380798  0.017568   

                     Total  Tingkat Kepuasan  
ID Pelanggan     -0.039968         -0.245717  
Jenis Kelamin     0.238051         -0.088339  
Pendapatan        0.592044         -0.312663  
Harga             0.645455         -0.380798  
Jumlah            0.636097          0.017568  
Total             1.000000         -0.268345  
Tingkat Kepuasan -0.268345          1.000000  
                  ID Pelanggan  Jenis Kelamin  Pendapatan     Harga   Jumlah   \
ID Pelanggan          1.000000       0.126650   -0.054998 -0.005753  0.024016   
Jenis Kelamin         0.126650       1.000000    0.190245  0.415339 -0.090299   
Pendapatan           -0.054998       0.190245    1.000000  0.523053  0.501925   
Harga                -0.005753       0.415339    0.523053  1.000000 -0.098450   
Jumlah                0.024016      -0.090299    0.501925 -0.098450  1.000000   
Total                -0.065998       0.190245    0.988506  0.535078  0.501925   
Tingkat Kepuasan     -0.183817      -0.085796   -0.165588 -0.325659 -0.028923   

                     Total  Tingkat Kepuasan  
ID Pelanggan     -0.065998         -0.183817  
Jenis Kelamin     0.190245         -0.085796  
Pendapatan        0.988506         -0.165588  
Harga             0.535078         -0.325659  
Jumlah            0.501925         -0.028923  
Total             1.000000         -0.165588  
Tingkat Kepuasan -0.165588          1.000000  
                  ID Pelanggan  Jenis Kelamin  Pendapatan     Harga   Jumlah   \
ID Pelanggan          1.000000       0.151375   -0.063711 -0.039149  0.046356   
Jenis Kelamin         0.151375       1.000000    0.219508  0.463635 -0.098864   
Pendapatan           -0.063711       0.219508    1.000000  0.640000  0.607110   
Harga                -0.039149       0.463635    0.640000  1.000000 -0.130749   
Jumlah                0.046356      -0.098864    0.607110 -0.130749  1.000000   
Total                -0.069779       0.219508    0.998470  0.646194  0.607110   
Tingkat Kepuasan     -0.238890      -0.090784   -0.192463 -0.378933 -0.023874   

                     Total  Tingkat Kepuasan  
ID Pelanggan     -0.069779         -0.238890  
Jenis Kelamin     0.219508         -0.090784  
Pendapatan        0.998470         -0.192463  
Harga             0.646194         -0.378933  
Jumlah            0.607110         -0.023874  
Total             1.000000         -0.192463  
Tingkat Kepuasan -0.192463          1.000000  

