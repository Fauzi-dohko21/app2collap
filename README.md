# Project Kolaborasi Android

Ini adalah proyek sederhana untuk belajar kolaborasi menggunakan Git & Android Studio

## 👥 Tim
-	M Alfian Fauzi 1 : Inisialisasi & Merge PR
-	Sabila Zahrani 2 : Fitur TextView
-	Meutya Candra Dewi 3 : Fitur Button
  
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

<img width="4604" height="6904" alt="activity main xml" src="https://github.com/user-attachments/assets/546dcd9e-a587-4917-bfad-c7317c9c6653" /> 
(Activity.main.xml)
<img width="4064" height="4300" alt="MainActivity" src="https://github.com/user-attachments/assets/571bbd5c-95f3-4d8d-a093-5479e50f8f28" />
(MainActivity)
<img width="3384" height="2536" alt="Splash" src="https://github.com/user-attachments/assets/f936a0f4-6fe7-4d9d-b776-aba10d6fb99a" />
(splash)
<img width="2920" height="3712" alt="activity splash xml" src="https://github.com/user-attachments/assets/39c45a41-ecf5-4a33-a2e9-ae64bebbfdca" />
(Activity.splash.xml)

<img width="269" height="480" alt="Screenshot 2025-07-31 132729" src="https://github.com/user-attachments/assets/b8deecf5-2a32-45c0-8672-665edf8adca6" />
<img width="173" height="313" alt="Screenshot 2025-07-31 132834" src="https://github.com/user-attachments/assets/6f5c9c38-9858-44cd-a685-8af0011feb8e" />








  
