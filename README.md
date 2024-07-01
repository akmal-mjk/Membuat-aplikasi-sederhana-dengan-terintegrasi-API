---

# Aplikasi Absensi Kepegawaian

Aplikasi Absensi Kepegawaian adalah aplikasi berbasis Flutter yang dirancang untuk membantu perusahaan dalam mengelola kehadiran pegawai. Aplikasi ini memiliki fitur-fitur yang memungkinkan Anda untuk melihat daftar pegawai, menambah, mengedit, dan menghapus pegawai, serta melakukan check-in dan check-out menggunakan QR code.

## Fitur

### 1. Daftar Pegawai

- Menampilkan daftar semua pegawai yang terdaftar dalam sistem.

### 2. Daftar Pegawai di Kantor

- Menampilkan daftar pegawai yang saat ini berada di kantor.

### 3. Tambah Pegawai

- Menambahkan pegawai baru ke dalam sistem.

### 4. Edit Pegawai

- Mengedit informasi pegawai yang sudah terdaftar.

### 5. Hapus Pegawai

- Menghapus pegawai dari sistem.

### 6. Check-In Pegawai

- Menghasilkan QR code untuk pegawai yang melakukan check-in.
- QR code dapat dipindai oleh HP pegawai.
- Setelah QR code dipindai, pegawai akan dimasukkan ke dalam daftar pegawai yang ada di kantor.

### 7. Check-Out Pegawai

- Menghasilkan QR code untuk pegawai yang melakukan check-out.
- QR code dapat dipindai oleh HP pegawai.
- Setelah QR code dipindai, pegawai akan dihapus dari daftar pegawai yang ada di kantor.

## Instalasi

1. Clone repositori ini
   ```bash
   git clone https://github.com/!!!GANTI!!!/!!!GANTI!!!.git
   ```
2. Masuk ke direktori proyek
   ```bash
   cd !!!GANTI!!!
   ```
3. Instal dependensi
   ```bash
   flutter pub get
   ```
4. Jalankan aplikasi
   ```bash
   flutter run
   ```

## Konfigurasi

Pastikan Anda telah mengkonfigurasi izin internet di `AndroidManifest.xml` untuk memungkinkan aplikasi mengakses API.

```xml
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="com.example.your_project_name">

    <uses-permission android:name="android.permission.INTERNET"/>

    <application
        android:name=".MainApplication"
        android:label="your_project_name"
        android:icon="@mipmap/ic_launcher">
        <activity
            android:name=".MainActivity"
            android:label="your_project_name"
            android:configChanges="keyboard|keyboardHidden|orientation|screenSize"
            android:launchMode="singleTop"
            android:theme="@style/LaunchTheme"
            android:windowSoftInputMode="adjustResize">
            <meta-data
                android:name="flutterEmbedding"
                android:value="2" />
            <intent-filter>
                <action android:name="android.intent.action.MAIN"/>
                <category android:name="android.intent.category.LAUNCHER"/>
            </intent-filter>
        </activity>
    </application>

</manifest>
```

## Penggunaan

### Menambahkan Pegawai

1. Navigasikan ke halaman tambah pegawai dengan klick floating buttom di pojok kanan bawah.
2. Isi formulir dengan informasi pegawai.
3. Tekan tombol "Tambahkan" untuk menambahkan pegawai ke sistem.

### Mengedit Pegawai

1. Navigasikan ke halaman daftar pegawai.
2. Pilih pegawai yang ingin diedit.
3. Tekan pegawai yang ingin diedit.
4. Tekan tombol "Edit" dan lakukan perubahan yang diperlukan.
5. Tekan tombol "Simpan" untuk memperbarui informasi pegawai.

### Menghapus Pegawai

1. Navigasikan ke halaman daftar pegawai.
2. Pilih pegawai yang ingin dihapus.
3. Tekan pegawai yang ingin dihapus.
4. Tekan tombol "Hapus" untuk menghapus pegawai dari sistem.

### Check-In Pegawai

1. Navigasikan ke halaman absen.
2. Pilih pegawai yang ingin melakukan check-in.
3. Tekan "Checkin".
4. QR code akan dihasilkan.
5. Pegawai memindai QR code menggunakan HP mereka.
6. Setelah dipindai, pegawai akan masuk ke daftar pegawai yang ada di kantor.

### Check-Out Pegawai

1. Navigasikan ke halaman kantor.
2. Pilih pegawai yang ingin melakukan check-out.
3. Tekan "Checkout".
4. QR code akan dihasilkan.
5. Pegawai memindai QR code menggunakan HP mereka.
6. Setelah dipindai, pegawai akan dihapus dari daftar pegawai yang ada di kantor.
