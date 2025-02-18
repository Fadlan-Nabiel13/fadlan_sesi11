# fadlan_sesi11
project dapat dilihat pada google collab dengan link terlampir sebagai berikut : https://colab.research.google.com/drive/1NM-h0wpgAeess0zrQXNzuLytM7ku1ML5?authuser=0#scrollTo=wtbZOutUsWPe 

Hasil analisa yang didapat :
1. Gambar Input : Menampilkan citra asli dalam skala keabuan (grayscale). Citra ini merupakan input awal untuk proses segmentasi.
2. Gambar Tepi : Menampilkan hasil deteksi tepi menggunakan operator Sobel. Operator Sobel menghitung gradien intensitas piksel pada arah horizontal (sobel_x) dan vertikal (sobel_y). Gambar_tepi merepresentasikan magnitude gradien, menunjukkan seberapa kuat perubahan intensitas pada setiap titik di citra. Daerah dengan tepi akan memiliki nilai magnitude gradien yang tinggi (terlihat lebih terang pada gambar), sedangkan daerah yang homogen akan memiliki nilai rendah (terlihat lebih gelap).
3. Hasil Segmentasi: Menampilkan hasil segmentasi setelah menerapkan thresholding pada gambar_tepi. Thresholding membagi piksel menjadi dua kelas: objek dan latar belakang. Piksel dengan magnitude gradien di atas threshold (50 dalam kasus ini) diklasifikasikan sebagai tepi objek (bernilai True, ditampilkan putih), sedangkan piksel di bawah threshold diklasifikasikan sebagai latar belakang (bernilai False, ditampilkan hitam). Hasilnya adalah citra biner yang menunjukkan segmentasi objek dari latar belakang.

Analisis Lebih Lanjut :
- Kualitas Segmentasi : Kualitas segmentasi bergantung pada pemilihan threshold yang tepat. Nilai threshold yang terlalu rendah dapat menghasilkan banyak noise, sedangkan nilai yang terlalu tinggi dapat menghilangkan detail tepi objek.
- Kompleksitas Objek : Metode ini efektif untuk objek dengan tepi yang jelas. Objek dengan tepi yang kabur atau tekstur yang kompleks mungkin memerlukan metode segmentasi yang lebih canggih.
