# EVALUASI-DAN-PERTANYAAN
# 1. Tulis semua perintah-perintah SQL percobaan di atas beserta outputnya!
Jawaban :
1. Memasukkan data => INSERT
  • INSERT INTO <table_name> (field1, ..., fieldn) VALUE (val1, ..., valn)
2. Mengubah data => UPDATE
  • UPDTAE <table_name> SET [field1=val1, ,... fieldn=valn] WHERE <kondisi>
3. Menghapus data => DELETE
  • DELETE FROM <table_name> WHERE <kondisi>
4. Menampilkan data => SELECT
  • SELECT * FROM <table_name>
# 2. Apa bedanya penggunaan BETWEEN dan penggunaan operator >= dan <= ?
# • (misal: tgl_lahir BETWEEN '1990-10-10' AND '1992-10-11')
# • (misal: tgl_lahir >= '1990-10-10' AND tgl_lahir <= '1992-10-11')
Jawaban :
Perbedaan antara penggunaan BETWEEN dan penggunaan operator >= dan <= dalam konteks yang Anda berikan adalah:

1. **BETWEEN**: Dalam kasus ini, penggunaan BETWEEN akan memeriksa apakah nilai tgl_lahir berada di antara '1990-10-10' dan '1992-10-11', termasuk kedua tanggal tersebut. Jadi, jika tgl_lahir sama dengan '1990-10-10' atau '1992-10-11', data tersebut akan disertakan dalam hasil kueri.
   tgl_lahir BETWEEN '1990-10-10' AND '1992-10-11'
   
2. **Operator >= dan <=**: Dalam kasus ini, operator >= dan <= akan memeriksa apakah nilai tgl_lahir lebih besar dari atau sama dengan '1990-10-10' dan kurang dari atau sama dengan '1992-10-11'. Ini berarti data yang memiliki tgl_lahir sama dengan '1990-10-10' atau '1992-10-11' akan disertakan dalam hasil kueri hanya jika operator adalah <= atau >=. Ini menyebabkan perilaku sedikit berbeda dari penggunaan BETWEEN karena BETWEEN akan menyertakan kedua nilai batas, sedangkan operator >= dan <= akan memperlakukan kedua batas secara terpisah.
   tgl_lahir >= '1990-10-10' AND tgl_lahir <= '1992-10-11'
  
