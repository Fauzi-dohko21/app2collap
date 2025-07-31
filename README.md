# Project Kolaborasi Android

Ini adalah proyek sederhana untuk belajar kolaborasi menggunakan Git & Android Studio

## 👥 Tim
⦁	M Alfian Fauzi 1 : Inisialisasi & Merge PR
⦁	Sabila Zahrani 2 : Fitur TextView
⦁	Meutya Candra Dewi 3 : Fitur Button
  
## 📱 Fitur
- Menampilkan TextView
- Menampilkan Button yang dapat diklik

## 🔧 Teknologi
- Kotlin : Kotlin adalah bahasa pemrograman modern yang digunakan untuk membuat aplikasi Android. 
- Android Studio : Android Studio adalah software resmi dari Google untuk mengembangkan aplikasi Android. Di dalamnya, kamu bisa menulis kode, mendesain tampilan, dan mengetes aplikasi.
- Git + GitHub : Git adalah alat untuk mencatat dan mengelola perubahan kode, sedangkan GitHub adalah tempat online untuk menyimpan dan membagikan project Git. Keduanya memudahkan kerja tim dan kolaborasi dari mana saja.

## 📸 Penjelasan code penting
- import android.os.Bundle
  Fungsi: Mengimpor Bundle, yaitu objek yang digunakan untuk menyimpan data yang ingin dikirim antar activity atau saat memulihkan state Activity.

- import android.widget.Button → Untuk menampilkan tombol pada UI.
- import android.widget.EditText → Untuk membuat kolom input teks dari pengguna.
- import android.widget.TextView → Untuk menampilkan teks ke layar.
  Ini semua adalah komponen antarmuka pengguna (UI) dalam Android.

- import androidx.activity.enableEdgeToEdge
Fungsi: Mengaktifkan tampilan layar penuh (full screen), supaya konten aplikasi bisa tampil sampai ke pinggir layar, termasuk di belakang status bar dan navigation bar.
Tujuan: Membuat tampilan aplikasi terlihat lebih modern, bersih, dan luas.
-import androidx.appcompat.app.AppCompatActivity
Fungsi: AppCompatActivity Digunakan sebagai dasar untuk membuat sebuah Activity (layar tampilan aplikasi).
 memberikan dukungan fitur-fitur modern dan tetap bisa dijalankan di Android versi lama.
-import androidx.core.view.ViewCompat
Fungsi: Membantu agar kode bisa berjalan lancar di berbagai versi Android.
Sederhananya: Biar aplikasi tetap kompatibel meskipun dijalankan di Android versi lama atau baru.
-import androidx.core.view.WindowInsetsCompat
Fungsi: Mengatur agar tampilan tidak tertutup oleh status bar atau navigation bar.
Gunanya: Biar layout aplikasi bisa menyesuaikan otomatis, jadi UI tetap rapi dan nyaman dilihat di semua perangkat.

- private lateinit var inputName: EditText → Kolom untuk mengetik nama.
- private lateinit var inputKelas: EditText → Kolom untuk mengetik kelas.
- private lateinit var btnSubmit: Button → Tombol untuk mengirim atau memproses data input.
- private lateinit var txtResult: TextView → Tempat menampilkan hasil output ke layar.

- override fun onCreate → Fungsi yang jalan pertama kali saat aplikasi dibuka.
- setContentView(R.layout.activity_main) → Perintah untuk menampilkan tampilan yang sudah dibuat di XML ke layar. Jadi, desain yang kamu buat di activity_main.xml akan langsung muncul saat aplikasi dibuka.
  
- inputName = findViewById(R.id.etNama) → Menghubungkan variabel inputName dengan kotak input nama di tampilan
- inputKelas = findViewById(R.id.etKelas) → Menghubungkan inputKelas dengan kotak input kelas di tampilan.
- btnSubmit = findViewById(R.id.btnTampilkan) → Menghubungkan btnSubmit dengan tombol yang akan ditekan oleh pengguna.
- txtResult = findViewById(R.id.tvHasil) → Menghubungkan txtResult dengan teks hasil yang akan ditampilkan di layar.
 
- btnSubmit.setOnClickListener {
    val nama = inputName.text.toString().trim()
    var kelas = inputKelas.text.toString().trim()
    var hasil = "Nama: $nama\nKelas: $kelas"
    txtResult.text = hasil
  }
  Fungsi: Kode ini akan menangani saat tombol ditekan, lalu mengambil input nama dan kelas, dan menampilkannya ke layar dalam format yang rapi.

## 📸 Screenshot

<img width="1255" height="543" alt="Screenshot 2025-07-31 122040" src="https://github.com/user-attachments/assets/65565586-58ba-4315-815f-156c0d5ba938" />
<img width="1215" height="626" alt="Screenshot 2025-07-31 122059" src="https://github.com/user-attachments/assets/4ac33458-1132-41e0-b626-96193e59d22c" />
<img width="945" height="592" alt="Screenshot 2025-07-31 122125" src="https://github.com/user-attachments/assets/21fdbcfb-bf9d-440b-a1da-7e6640c341af" />




  
