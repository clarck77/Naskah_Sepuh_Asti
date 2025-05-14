# Naskah_Sepuh_Asti

---

### **Materi 1 & 2 – Membuat Akun GitHub (Selesai)**

1. Buka website GitHub: [https://github.com](https://github.com)
2. Klik **Sign up for GitHub**.
3. Isi **username**, **email**, dan **password**.
4. Setelah selesai, klik **Sign up** untuk membuat akun.
5. Cek email untuk proses verifikasi, lalu ikuti instruksinya.

---

### **Materi 3 – Download Git (Selesai)**

**Git** adalah *version control system* yang digunakan untuk mengelola versi kode, baik untuk kerja individu maupun kolaborasi tim.

1. Buka website [https://git-scm.com](https://git-scm.com)
2. Klik tombol **Download for Windows**.
3. Proses unduhan akan berjalan otomatis. Jika tidak, pilih versi yang sesuai secara manual.

---

### **Materi 4 & 5 – (Dilewati, karena menggunakan Windows)**

---

### **Materi 6 – Instalasi Git di Windows (Selesai)**

**Cek apakah Git sudah terinstal:**

* Buka **CMD**, lalu ketik:
  `git --version`

**Langkah instalasi Git:**

1. Jalankan file instalasi `.exe` sebagai administrator.
2. Klik **Next** terus hingga proses instalasi selesai (pengaturan default saja).
3. Tunggu sampai proses instalasi selesai.

---

### **Materi 7 – Konfigurasi Git (Selesai)**

**Pastikan sudah login ke akun GitHub.**

1. Buka **CMD**, lalu pastikan Git sudah terinstal:
   `git --version`

2. **Set email Git:**

   ```bash
   git config --global user.email "email_github"
   ```

3. **Set nama pengguna Git:**

   ```bash
   git config --global user.name "username_github"
   ```

4. Cek konfigurasi:

   * Email: `git config --global user.email`
   * Nama: `git config --global user.name`

---

### **Materi 8 – Git Init, Status, Add, Commit, Log (Selesai)**

1. Buat folder project dan buka di text editor.

2. Buka **CMD** dan masuk ke folder:

   ```bash
   cd "alamat_folder"
   ```

3. Inisialisasi Git:

   ```bash
   git init
   ```

4. Buat file `index.html`, isi dengan kode HTML.

5. Cek status file:

   ```bash
   git status
   ```

6. Tambahkan file ke staging:

   * Semua file: `git add .`
   * Satu file: `git add nama_file`

7. Simpan perubahan dengan commit:

   ```bash
   git commit -m "pesan_commit"
   ```

8. Lihat riwayat commit:

   ```bash
   git log
   git log --oneline
   ```

---

### **Materi 9 – Branch: Membuat, Menghapus, Berpindah (Selesai)**

1. Lihat daftar branch:

   ```bash
   git branch
   ```

2. Buat branch baru:

   ```bash
   git branch nama_branch
   ```

3. Pindah ke branch:

   ```bash
   git checkout nama_branch
   ```

4. Hapus branch:

   ```bash
   git branch -d nama_branch
   ```

5. Buat dan langsung pindah ke branch:

   ```bash
   git checkout -b nama_branch
   ```

---

### **Materi 10 – Checkout Berdasarkan Commit ID (Selesai)**

1. Lihat commit ID:

   ```bash
   git log --oneline
   ```

2. Kembali ke versi tertentu:

   ```bash
   git checkout commit_id -- nama_file
   ```

---

### **Materi 11 – Git Reset (Selesai)**

1. Reset commit ke versi sebelumnya (hanya commit dan pesan):

   ```bash
   git reset commit_id
   ```

2. Reset seluruh perubahan termasuk isi file:

   ```bash
   git reset --hard commit_id
   ```

---

### **Materi 12 – Git Merge (Selesai)**

1. Gabungkan branch ke branch aktif:

   ```bash
   git merge nama_branch
   ```

2. Jika ada konflik:

   ```bash
   git merge --abort
   ```

---

### **Materi 13 – Git Conflict (Selesai)**

**Konflik Git** terjadi saat dua perubahan berbenturan.

* Tentukan kode mana yang ingin digunakan.
* Hapus bagian yang tidak diperlukan.
* Simpan kembali dan lakukan commit.

---

### **Materi 14 – GitHub Clone & Push (Selesai)**

1. Login ke GitHub, buat repository baru, centang opsi **README**.

2. Salin URL repo dari tombol **<> Code**.

3. Di CMD, clone repo:

   ```bash
   git clone https://github.com/username/nama-repo.git
   ```

4. Masuk ke folder hasil clone, buat file `index.html`.

5. Tambahkan dan commit:

   ```bash
   git add .
   git commit -m "menambahkan index.html"
   ```

6. Push ke GitHub:

   ```bash
   git push
   ```

---

### **Materi 15 – Git Push dengan Branch Baru (Selesai)**

1. Buat dan pindah ke branch baru:

   ```bash
   git checkout -b nama_branch
   ```

2. Setelah commit, push branch:

   ```bash
   git push origin nama_branch
   ```

3. Agar ke depannya cukup pakai `git push`:

   ```bash
   git push --set-upstream origin nama_branch
   ```

---

### **Materi 16 – Git Pull (Selesai)**

**Pull** = Mengambil perubahan dari GitHub ke lokal.

1. Setelah update file di GitHub dan commit, gunakan:

   ```bash
   git pull origin nama_branch
   ```

---

### **Materi 17 – Git Fetch (Selesai)**

**Fetch** = Mengambil semua branch dari repo GitHub.

1. Ambil semua branch lalu pindah ke branch tertentu:

   ```bash
   git fetch
   git checkout nama_branch
   ```

---

### **Materi 18 – Pull Request & Merge (Selesai)**

**Pull Request (PR)** = Mengusulkan penggabungan branch ke branch utama.

1. Di GitHub, klik **Pull Request** > **New Pull Request**
2. Pilih branch sumber dan target.
3. Klik **Create Pull Request**
4. Setelah disetujui, lakukan merge.

---

### **Materi 19 – Fork Repository (Selesai)**

**Fork** = Menyalin repo orang lain ke akun pribadi.

1. Buka repo target, klik **Fork**.
2. Repo akan muncul di akun GitHub pribadi.
3. Clone ke lokal:

   ```bash
   git clone link_forked_repo
   ```
---
