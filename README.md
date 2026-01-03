# Kelengkapan Kode Program
dokumen ini berisi mengenai cara menjalankan kode program dan penjelasan struktur folder yang telah dibuat (tidak menjelaskan kode program secara terperinci)  
![PySpark](https://img.shields.io/badge/PySpark-3.5.7-orange?logo=apachespark&logoColor=white)  
![Python](https://img.shields.io/badge/Python-3.9-blue?logo=python&logoColor=white)  
![Java](https://img.shields.io/badge/Java%20JDK-11-red?logo=openjdk&logoColor=white)  
![Hadoop](https://img.shields.io/badge/Apache%20Hadoop-3.x-yellow?logo=apachehadoop&logoColor=black)

### Struktur Folder
```sh
UAS/
│
├── dataset/
│   ├── cooked/     
│   │   └── (berisi dataset setengah matang)                
│   └── raw/ 
│       └── (berisi dataset yang baru saja diunduh)
│  
├── notebook/
│   ├── 0-preprocessing.ipynb   
│   ├── 1-engineering.ipynb   
│   └── 2-modelling.ipynb 
│   
├── spark39        
│   └── (berisi kebutuhan env)           
│
├── data/                     
│   ├── raw/                  
│   ├── processed/            
│   └── external/             
│
├── .gitignore
├── README.md 
└── requirements.txt   
```

### Panduan Menjalankan Kode Program

kloning projek dari tautan yang ada dibawah ini
```sh
git clone https://github.com/Codex2142/Prediksi-Rata-rata-Penjualan-dengan-GBTRegressor.git
```

masuk ke direktori yang telah di kloning, misalnya
```sh
cd UAS
```

gunakan `venv` untuk mengunduh lib-lib yang akan dibutuhkan
```sh
spark39/Scripts/activate
```

tampilan bila berhasil mengaktifkan `venv` seperti dibawah ini
```sh
(spark39) PS E:\Riwayat Kuliah\Semester 7\Big Data dan AI\UAS>
```

jika sudah tampil seperti diatas, unduh lib lib yang akan digunakan dengan cara dibawah ini
```sh
pip install -r requirements.txt
```

### Testing Kernel
buka file `0-preprocessing.ipynb`, `1-engineering.ipynb`, `2-modelling.ipynb` kemudian pada sebelah pojok kanan atas terdapat opsi pemilihan kernel, silahkan ganti dengan venv yang telah dibuat yaitu `spark39`