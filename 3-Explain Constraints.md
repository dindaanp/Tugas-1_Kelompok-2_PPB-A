# Explain Constraints

Dalam konteks pengembangan aplikasi **Layanan Musik Global (Enterprise)** seperti Spotify, terdapat sejumlah batasan (*constraints*) yang mempengaruhi keputusan pemilihan teknologi. Constraints ini selaras dengan harapan pengguna, kebutuhan bisnis, serta strategi investasi jangka panjang perusahaan.

---

## 1. Performance & Reliability Constraint

Sebagai aplikasi streaming musik global dengan jutaan pengguna aktif harian, sistem harus mampu memberikan:

- Streaming tanpa jeda (*no buffering*)
- Minim crash
- Respons UI yang cepat
- Konsumsi memori dan baterai yang efisien

Aplikasi harus tetap stabil bahkan ketika berjalan di background, saat perangkat berpindah jaringan (WiFi ke data seluler), atau ketika pengguna membuka aplikasi berat lainnya.

Constraint ini membatasi pilihan teknologi pada solusi yang memiliki kontrol penuh terhadap resource perangkat, sehingga pendekatan Native menjadi lebih relevan dalam konteks enterprise.

---

## 2. Device Integration Constraint

Pengguna mengharapkan pengalaman yang menyatu dengan ekosistem perangkat, seperti:

- Kontrol musik dari lockscreen
- Integrasi dengan smartwatch
- Dukungan Android Auto / CarPlay
- Notifikasi interaktif
- Background audio service yang stabil

Fitur-fitur ini membutuhkan akses mendalam terhadap API sistem operasi (Android dan iOS). Tidak semua framework cross-platform mampu mengakomodasi integrasi kompleks ini tanpa penyesuaian tambahan atau custom native bridge.

Artinya, terdapat batasan teknis yang mengharuskan teknologi memiliki fleksibilitas penuh terhadap sistem operasi.

---

## 3. Scalability & Load Constraint

Sebagai layanan global, sistem harus mampu:

- Menangani jutaan concurrent users
- Mendukung update fitur secara berkala
- Mengelola berbagai tipe perangkat (low-end hingga flagship)

Semakin besar skala pengguna, semakin kecil toleransi terhadap bug atau penurunan performa. Arsitektur yang dipilih harus mendukung pengembangan modular dan scalable tanpa mengorbankan stabilitas.

Constraint ini membatasi penggunaan teknologi yang belum terbukti stabil di skala enterprise besar.

---

## 4. Brand Reputation Constraint

Dalam model bisnis berbasis langganan, kualitas aplikasi secara langsung mempengaruhi:

- Retention rate
- Subscription renewal
- Brand perception

Jika aplikasi terasa lambat atau sering bermasalah, pengguna dapat dengan mudah berpindah ke kompetitor.

Karena itu, constraint bisnis menuntut standar kualitas yang sangat tinggi, yang sering kali lebih mudah dicapai melalui pendekatan Native yang memberikan optimasi maksimal.

---

## 5. Long-Term Investment Constraint

Sebagai perusahaan besar, keputusan teknologi bukan hanya soal cepat rilis, tetapi juga:

- Maintainability jangka panjang  
- Keamanan sistem  
- Stabilitas update OS  
- Dukungan komunitas dan developer ecosystem  

Kesalahan memilih teknologi dapat menyebabkan technical debt yang besar dan biaya maintenance yang tinggi di masa depan.

Constraint ini mendorong pemilihan teknologi yang matang, stabil, dan memiliki roadmap pengembangan jangka panjang yang jelas.

---

# Kesimpulan Constraints

Berdasarkan introduction dan context assumption, dapat disimpulkan bahwa batasan utama dalam studi kasus ini adalah:

- Tidak boleh ada kompromi terhadap performa  
- Integrasi perangkat harus maksimal  
- Sistem harus scalable dan stabil di skala global  
- Kualitas aplikasi berpengaruh langsung terhadap bisnis  

Dengan constraints tersebut, pilihan teknologi bukan sekadar pertimbangan teknis, melainkan keputusan strategis yang berdampak pada keberlanjutan perusahaan secara keseluruhan.
