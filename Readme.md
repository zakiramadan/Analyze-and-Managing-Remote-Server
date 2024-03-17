# Praktek Dipandu: Menganalisis dan Mengelola Server Remote pada Desktop Linux Ubuntu

## Tujuan

Latihan ini bertujuan untuk memberikan pemahaman praktis tentang bagaimana menganalisis dan mengelola server remote menggunakan desktop Linux Ubuntu. Peserta akan menggunakan serangkaian perintah dan alat bawaan untuk mencapai tujuan ini.

## Deskripsi

Latihan ini memandu peserta melalui proses menganalisis dan mengelola server remote menggunakan desktop Linux Ubuntu. Peserta akan menggunakan perintah seperti `ssh`, `ping`, `traceroute`, dan `netstat` untuk memeriksa konektivitas, melacak rute paket, dan mengevaluasi status server remote.

### Langkah-langkah

1. **Membuat Koneksi SSH ke Server Remote**

   - Gunakan perintah `ssh` untuk terhubung ke server remote.
     ```bash
     ssh username@remote_server_ip
     ```

2. **Memeriksa Konektivitas Jaringan**

   - Gunakan perintah `ping` untuk memeriksa konektivitas dengan server remote.
     ```bash
     ping remote_server_ip
     ```
   - Gunakan perintah `traceroute` untuk melacak rute paket menuju server remote.
     ```bash
     traceroute remote_server_ip
     ```

3. **Meninjau Status Port pada Server Remote**
   - Gunakan perintah `netstat` untuk melihat status port pada server remote.
     ```bash
     netstat -tuln
     ```
   - Identifikasi port yang sedang mendengarkan dan layanan yang berjalan.

## Penilaian

- Keberhasilan dalam membuat koneksi SSH ke server remote.
- Kemampuan menggunakan perintah `ping` dan `traceroute` untuk memeriksa konektivitas jaringan.
- Kemampuan menggunakan `netstat` untuk menganalisis status port pada server remote.
- Kemampuan untuk menganalisis informasi yang diperoleh dan mengevaluasi status server remote.

## Catatan Tambahan

- Pastikan untuk menggunakan perintah dengan hati-hati dan hanya pada server yang Anda miliki atau dengan izin yang sesuai.
- Latihan ini bertujuan untuk memberikan pemahaman praktis tentang menganalisis dan mengelola server remote, yang merupakan keterampilan yang penting dalam administrasi sistem Linux.
