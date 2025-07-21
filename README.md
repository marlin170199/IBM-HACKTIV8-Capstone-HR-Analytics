# Diagnosis Budaya Perusahaan: Analisis Ulasan Karyawan Menggunakan AI untuk Menghasilkan Rekomendasi Strategis

**Oleh: Fauzi Noorsyabani - Universitas Siliwangi**
*Proyek Capstone - IBM SkillsBuild Student Development Initiative*

---

## Latar Belakang & Masalah (Project Overview)

Di tengah era persaingan talenta global yang ketat, saya mengamati bahwa banyak perusahaan, terutama di industri teknologi, menghadapi tantangan besar dalam mempertahankan talenta terbaik mereka. Fenomena 'Great Resignation' menjadi bukti nyata dari tantangan ini. Biaya yang timbul akibat turnover karyawan yang tinggi sangat signifikan, mencakup biaya rekrutmen, pelatihan, dan hilangnya produktivitas. Saya percaya bahwa akar masalah dari fenomena ini seringkali bersifat kualitatif dan tersembunyi di dalam ribuan ulasan anonim yang ditinggalkan oleh karyawan di platform publik seperti Glassdoor. Data ini, meskipun sangat berharga, seringkali tidak termanfaatkan karena volumenya yang masif dan sifatnya yang tidak terstruktur.

Proyek ini saya ajukan untuk memecahkan masalah tersebut dengan sebuah pendekatan analitis yang ditenagai oleh Kecerdasan Buatan. Tujuan saya adalah untuk mengubah "kebisingan" dari ribuan ulasan kualitatif menjadi sinyal strategis yang jernih dan dapat ditindaklanjuti.

### Tujuan Utama Proyek Saya:
1.  **Mengidentifikasi dan Mengklasifikasikan Pendorong Utama Ketidakpuasan:** Saya akan secara otomatis mengkategorikan ribuan keluhan karyawan ke dalam tema-tema bisnis yang spesifik untuk menemukan akar masalah yang paling dominan.
2.  **Menghasilkan Ringkasan Eksekutif yang Actionable:** Saya akan meringkas ratusan keluhan dalam satu tema menjadi beberapa poin strategis yang dapat dipahami dan digunakan oleh level manajemen untuk pengambilan keputusan.
3.  **Mendemonstrasikan Kekuatan IBM Granite sebagai Alat Strategis:** Saya akan menunjukkan bagaimana saya, sebagai seorang analis, dapat menggunakan model AI canggih sebagai partner strategis bagi departemen Sumber Daya Manusia (SDM) untuk melakukan diagnosis budaya perusahaan secara efisien, objektif, dan berbasis data.

---

## Proses Analisis & Peran Strategis AI

Untuk mencapai tujuan tersebut, saya menerapkan alur kerja yang sistematis dan dapat direproduksi. Setiap langkah saya rancang untuk memastikan integritas data dan validitas hasil analisis.

### Alur Kerja Proyek Saya:
1.  **Akuisisi & Pemuatan Data:** Saya menggunakan dataset publik dari Kaggle yang berisi 838.566 ulasan karyawan.
2.  **Pembersihan & Pra-pemrosesan Teks:** Saya melakukan pembersihan data secara ekstensif, termasuk penanganan nilai yang hilang dan standardisasi teks untuk meningkatkan akurasi analisis AI.
3.  **Analisis Sampel Representatif:** Saya melakukan analisis awal pada 200 sampel data untuk memvalidasi metode dan prompt AI sebelum diterapkan pada skala yang lebih besar.
4.  **Klasifikasi Tema dengan IBM Granite:** Saya menggunakan model `ibm-granite/granite-3.3-8b-instruct` untuk mengklasifikasikan setiap keluhan ke dalam lima kategori bisnis yang telah saya tentukan.
5.  **Analisis & Visualisasi Hasil:** Saya menganalisis distribusi tema yang dihasilkan oleh AI dan memvisualisasikannya untuk mengidentifikasi tren utama.
6.  **Summarisasi Otomatis dengan IBM Granite:** Saya menggunakan kemampuan summarization model untuk meringkas semua keluhan dalam tema yang paling dominan.
7.  **Formulasi Kesimpulan & Rekomendasi:** Saya menarik kesimpulan dari seluruh analisis dan merumuskan rekomendasi strategis.

### Dukungan AI (IBM Granite): Mengapa Saya Menggunakan AI?
Saya menyadari bahwa analisis manual terhadap hampir satu juta ulasan tidak hanya tidak efisien, tetapi juga sangat rentan terhadap bias subjektif. Penggunaan AI IBM Granite dalam proyek ini sangat relevan dan krusial karena:

-   **Skalabilitas & Konsistensi:** AI memungkinkan saya untuk memproses volume data yang masif dengan aturan yang sama persis untuk setiap baris data, memastikan hasil klasifikasi yang konsisten dan objektif.
-   **Pemahaman Kontekstual:** Saya memanfaatkan kemampuan model LLM seperti Granite untuk memahami nuansa dalam teks keluhan, sehingga dapat mengidentifikasi tema utama bahkan dari kalimat yang kompleks.
-   **Efisiensi Waktu:** Tugas yang mungkin memakan waktu berbulan-bulan untuk tim analis dapat saya selesaikan dalam hitungan jam, memungkinkan perusahaan untuk merespons masalah dengan lebih cepat.
-   **Transformasi Data:** AI memungkinkan saya untuk mengubah data kualitatif (teks ulasan) yang sulit diukur menjadi data kuantitatif (distribusi tema) dan insight kualitatif yang ringkas (ringkasan eksekutif).

---

## Temuan Kunci & Insight (Hasil Analisis)

Analisis saya pada sampel representatif sebanyak 200 ulasan menghasilkan beberapa temuan kunci yang signifikan dan terkadang berlawanan dengan intuisi.

### A. Distribusi Tema Keluhan Utama: Apa yang Sebenarnya Dikeluhkan Karyawan?
*Visualisasi dan grafik detail dapat dilihat pada notebook analisis.*

Dari analisis, saya dapat menarik insight berikut:
-   **Masalah Fundamental:** Keluhan yang paling dominan adalah seputar **Compensation & Benefits** (58 ulasan). Ini menunjukkan bahwa isu-isu mendasar terkait gaji, tunjangan, dan kompensasi masih menjadi sumber utama ketidakpuasan.
-   **Ambisi yang Terhalang:** Di posisi kedua adalah **Career Opportunities** (45 ulasan). Ini menandakan bahwa karyawan tidak hanya peduli pada gaji saat ini, tetapi juga pada masa depan mereka di perusahaan. Kurangnya jenjang karir yang jelas adalah faktor demotivasi yang sangat kuat.
-   **Pentingnya Lingkungan Kerja:** Tema **Culture & Values** dan **Senior Management** juga memiliki porsi yang signifikan, menunjukkan bahwa lingkungan kerja dan kualitas kepemimpinan tetap menjadi faktor penting yang tidak bisa diabaikan.

### B. Menggali Lebih Dalam: Ringkasan Eksekutif dari Masalah Utama
Untuk memahami apa saja masalah spesifik di dalam kategori *Compensation & Benefits*, saya memerintahkan AI untuk bertindak sebagai konsultan dan meringkas 58 keluhan tersebut. Hasilnya adalah sebuah memo strategis yang siap saya sajikan kepada manajemen:

> ### Memo Eksekutif: Analisis Keluhan Kompensasi & Tunjangan
> **Untuk:** Manajemen Senior  
> **Dari:** Fauzi Noorsyabani, Analis Data Strategis  
> **Subjek:** Tiga Masalah Utama Terkait Kompensasi Berdasarkan Ulasan Karyawan
>
> Berdasarkan analisis komprehensif terhadap keluhan karyawan, tiga masalah utama yang paling sering muncul telah teridentifikasi:
>
> 1.  **Gaji yang Tidak Memadai & Jenjang Karir yang Lambat:** Keluhan yang paling konsisten adalah mengenai tingkat gaji yang dianggap di bawah rata-rata industri. Karyawan merasa bahwa bahkan dengan adanya promosi dan penambahan tanggung jawab, peningkatan gaji yang diterima sangat minimal atau tidak ada sama sekali.
> 2.  **Kurangnya Pelatihan & Pengembangan:** Karyawan menyuarakan ketidakpuasan terhadap minimnya program pelatihan yang memadai, terutama untuk peran-peran yang membutuhkan keahlian spesifik. Tidak adanya struktur jenjang gaji yang transparan memperburuk masalah, menciptakan persepsi ketidakadilan.
> 3.  **Praktik Manajemen yang Buruk & Budaya Kerja Toksik:** Keluhan juga menyoroti pola manajemen yang buruk, termasuk micro-management dan favoritisme, yang pada akhirnya berdampak negatif pada moral dan kepuasan kerja karyawan.

---

## Kesimpulan & Rekomendasi Strategis

### Kesimpulan
Proyek ini berhasil membuktikan bahwa dengan memanfaatkan kekuatan AI canggih seperti IBM Granite, saya dapat mengubah data kualitatif yang masif dan "berisik" menjadi insight strategis yang jernih. Analisis saya menunjukkan bahwa ketidakpuasan karyawan tidak disebabkan oleh satu faktor tunggal, melainkan oleh interaksi kompleks antara kompensasi yang tidak memadai, peluang karir yang terbatas, dan kualitas manajemen yang perlu ditingkatkan.

### Rekomendasi Strategis (Actionable)
Berdasarkan temuan dan ringkasan yang dihasilkan, berikut adalah tiga rekomendasi konkret yang saya ajukan:
1.  **Lakukan Audit dan Penyesuaian Struktur Gaji:** Saya merekomendasikan perusahaan untuk segera membentuk tim guna melakukan audit kompensasi internal dan membandingkannya dengan standar industri terkini, terutama untuk posisi level junior dan menengah yang paling rentan.
2.  **Luncurkan Program Pengembangan Karir Terstruktur:** Saya menyarankan agar perusahaan mengalokasikan anggaran khusus untuk program pelatihan dan sertifikasi yang relevan, serta membuat jalur karir (career path) yang jelas untuk setiap peran.
3.  **Implementasikan Pelatihan Kepemimpinan Wajib:** Mengingat banyaknya keluhan terkait manajemen, saya merekomendasikan agar semua pemimpin tim dan manajer diwajibkan untuk mengikuti pelatihan kepemimpinan yang berfokus pada komunikasi, empati, dan manajemen kinerja yang adil.

---

## Detail Teknis Proyek
- **Dataset:** [Glassdoor Job Reviews on Kaggle](https://www.kaggle.com/datasets/davidgauthier/glassdoor-job-reviews)
- **Tools & Library:** Python, Google Colab, Pandas, Matplotlib, Seaborn, LangChain, Replicate
- **Model AI:** `ibm-granite/granite-3.3-8b-instruct` via Replicate API
