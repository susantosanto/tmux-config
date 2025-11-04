# Dokumentasi Pintasan Tmux

Dokumentasi ini berisi semua pintasan keyboard untuk konfigurasi tmux Anda yang saat ini menggunakan tema Oasis.

## Prefix Key
- `F1` - Prefix key (menggantikan Ctrl-b)

## Navigasi dan Manipulasi Window/Pane

### Membagi Window
- `F1` + `|` - Membagi window secara horizontal
- `F1` + `-` - Membagi window secara vertikal

### Navigasi Pane
- `F1` + `h` - Pindah ke pane kiri
- `F1` + `j` - Pindah ke pane bawah
- `F1` + `k` - Pindah ke pane atas
- `F1` + `l` - Pindah ke pane kanan

### Resize Pane
- `F1` + `H` - Resize pane ke kiri
- `F1` + `J` - Resize pane ke bawah
- `F1` + `K` - Resize pane ke atas
- `F1` + `L` - Resize pane ke kanan

### Copy Mode
- `F1` + `[` - Masuk ke copy mode
- Dalam copy mode vi:
  - `v` - Mulai seleksi teks
  - `y` - Copy seleksi dan keluar dari copy mode
  - `C-j` - Scroll page down
  - `C-k` - Scroll page up
  - `C-d` - Scroll half page down
  - `C-u` - Scroll half page up
  - `/` - Cari teks

### Manipulasi Window
- `F1` + `c` - Buat window baru
- `F1` + `x` - Kill pane
- `F1` + `X` - Kill window
- `F1` + `n` - Pindah ke window berikutnya
- `F1` + `p` - Pindah ke window sebelumnya
- `F1` + `C-h` - Pindahkan window ke kiri
- `F1` + `C-l` - Pindahkan window ke kanan

## Plugin dan Fungsi Lainnya

### Plugin Manager (TPM)
- `F1` + `I` - Install plugin
- `F1` + `U` - Update plugin
- `F1` + `C` - Clean plugin yang tidak digunakan

### Menu dan Command Palette
- `F1` + `m` - Buka tmux-menus
- `F1` + `P` - Buka command palette
- `F1` + `?` - Buka prefix command palette

### Fungsi Lainnya
- `F1` + `s` - Pilih sesi
- `F1` + `w` - Pilih window
- `F1` + `r` - Reload konfigurasi
- `F1` + `t` - Toggle zoom pada pane

## Plugin Produktivitas Baru

### tmux-yank
Plugin untuk copy ke clipboard sistem dari dalam tmux.

- `F1` + `y` - Copy teks yang diseleksi ke clipboard sistem
- `F1` + `Y` - Copy seluruh baris yang dipilih ke clipboard sistem
- Dalam copy mode vi:
  - `Y` - Copy seleksi ke clipboard sistem

### tmux-prefix-highlight
Plugin untuk menyorot status prefix key agar jelas kapan Anda dalam mode perintah tmux.

- Tidak memiliki shortcut spesifik, tetapi akan menyorot status bar saat prefix key aktif
- Warna foreground: white
- Warna background: red
- Juga menyorot saat dalam copy mode

### tmux-better-mouse-mode
Plugin untuk mengelola mouse di tmux dengan lebih baik, termasuk emulasi mouse untuk program fullscreen seperti less dan kemampuan untuk keluar dari copy-mode dengan scrolling.

- Fungsi utama berjalan secara otomatis saat plugin aktif
- Memungkinkan penggunaan mouse untuk seleksi teks dan navigasi
- Mengaktifkan scrolling dalam buffer dan keluar dari copy mode saat scroll ke bawah

### tmux-which-key
Plugin untuk menampilkan semua pintasan keyboard yang tersedia setelah menekan prefix key tertentu.

- `Ctrl` + `a` - Menampilkan daftar semua pintasan (prefix table)
- `Ctrl` + `Shift` + `2` - Menampilkan daftar semua pintasan (root table)
- Tampilan daftar pintasan otomatis akan hilang setelah beberapa detik
- Warna border untuk tampilan: #859900 (hijau lembut)
- Posisi tampilan: atas
- Label pintasan akan dibungkus (wrap) jika terlalu panjang

### tmux-neolazygit
Plugin untuk mengintegrasikan lazygit ke dalam tmux, menyediakan antarmuka Git yang ramah pengguna secara visual.

- `F1` + `g` - Membuka lazygit dalam pane baru
- Secara default akan membuka lazygit di posisi kanan dengan lebar 80% dan tinggi 80%
- Jika lazygit tidak terinstal di sistem, plugin ini akan menampilkan pesan kesalahan



## Status Bar
- Status bar berada di posisi atas
- Menampilkan nama sesi, daftar window, serta informasi CPU dan waktu
- Warna status berubah sesuai tingkat penggunaan CPU
- Background status bar transparan
- Highlight prefix akan muncul saat prefix key aktif

## Konfigurasi Tambahan
- Mouse support: Aktif
- 256 color mode: Aktif
- Base window index: 1 (bukan 0)
- History limit: 1000 baris

## Shortcut Kustom Terbaru

### Fungsi Qwen dan Opendcode
- `F1` + `q` - Membuka pane baru secara horizontal (vertical split) dan menjalankan perintah `qwen`
- `F1` + `Q` - Membuka window baru dan menjalankan perintah `qwen`
- `F1` + `e` - Membuka pane baru secara horizontal (vertical split) dan menjalankan perintah `opencode`
- `F1` + `E` - Membuka window baru dan menjalankan perintah `opencode`

### Fungsi Tambahan
- `F1` + `Tab` - Pindah ke pane sebelumnya
- `F1` + `/` - Mencari teks dalam pane