# Project Kolaborasi Android

Ini adalah proyek sederhana untuk belajar kolaborasi menggunakan Git & Android Studio

## 👥 Tim
- M.Alfian Fauzi: Inisialisasi & Merge PR
- Sabila Zahrani Fitur TextView
- Meutya Candra Dewi Fitur Button
  
## 📱 Fitur
- Menampilkan TextView
- Menampilkan Button yang dapat diklik

## 🔧 Teknologi
- Kotlin
- Android Studio
- Git + GitHub

## 📸 Penjelasan code penting
- import android.os.Bundle
  Fungsi: Mengimpor Bundle, yaitu objek yang digunakan untuk menyimpan data yang ingin dikirim antar activity atau saat memulihkan state Activity.
  
- import android.widget.Button
- import android.widget.EditText
- import android.widget.TextView
  Fungsi: Mengimpor kelas UI:
  - Button untuk tombol.
  - EditText untuk input teks.
  - TextView untuk menampilkan teks.
  Ini semua adalah komponen antarmuka pengguna (UI) dalam Android.

- import androidx.activity.enableEdgeToEdge
  - Fungsi: Mengaktifkan tampilan full screen atau edge-to-edge layout, agar konten bisa muncul di belakang sistem bar (status bar dan         navigation bar).
  - Biasanya dipakai agar aplikasi terlihat modern dan bersih.
  
- import androidx.appcompat.app.AppCompatActivity
  - Fungsi: Ini adalah kelas dasar untuk membuat Activity dengan dukungan dari AndroidX (modern Android libraries).
  - AppCompatActivity memungkinkan penggunaan fitur-fitur modern sambil tetap kompatibel dengan versi Android lama.
  
- import androidx.core.view.ViewCompat
- import androidx.core.view.WindowInsetsCompat
  - Fungsi: ViewCompat: Kelas pembantu agar kode bisa berjalan kompatibel di berbagai versi Android.
          WindowInsetsCompat: Digunakan untuk mengatur padding/layout agar tidak tertutup oleh status bar atau navigation bar. Berguna untuk UI responsif.

- private lateinit var inputName: EditText
- private lateinit var inputKelas: EditText
- private lateinit var btnSubmit: Button
- private lateinit var txtResult: TextView
  - Fungsi: - private
            Artinya properti ini hanya bisa diakses dari dalam class MainActivity.
            Ini adalah encapsulation: menyembunyikan detail internal agar tidak bisa diakses sembarangan dari luar.
          - lateinit
            Artinya: variabel ini akan di-inisialisasi nanti, bukan saat dibuat.
          - var
            Artinya: Menandakan ini adalah mutable variable — bisa diubah nilainya.
  - kesimpulan: private lateinit var namaVariabel: Tipe
              berarti:
              Inisialisasi variabel ini nanti (bukan saat deklarasi), dan variabel ini hanya bisa diakses dari dalam class

- override fun onCreate
  - Fungsi: - fun onCreate(...)
            Fungsi yang dipanggil satu kali saat activity diluncurkan (pertama kali dibuka).
          - override
            Menandakan bahwa fungsi ini mengganti (meng-override) versi aslinya dari AppCompatActivity.
            AppCompatActivity sudah punya onCreate() bawaan.
            Kita meng-override agar bisa menambahkan logika sendiri saat Activity dimulai.
  
- setContentView(R.layout.activity_main)
  - Fungsi: perintah untuk menampilkan layout XML ke layar saat aplikasi dibuka.
  
- inputName = findViewById(R.id.etNama)
- inputKelas = findViewById(R.id.etKelas)
- btnSubmit = findViewById(R.id.btnTampilkan)
- txtResult = findViewById(R.id.tvHasil)
  - Fungsi: untuk menghubungkan (menginisialisasi) variabel di Kotlin dengan komponen UI yang kamu buat di file XML (activity_main.xml).

- btnSubmit.setOnClickListener {
    val nama = inputName.text.toString().trim()
    var kelas = inputKelas.text.toString().trim()
    var hasil = "Nama: $nama\nKelas: $kelas"
    txtResult.text = hasil
  }
  - Fungsi: Menangani aksi saat tombol btnSubmit ditekan, lalu menampilkan hasil input ke layar.

## 📸 Screenshot


  
