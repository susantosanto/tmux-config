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

## Status Bar
- Status bar berada di posisi atas
- Menampilkan nama sesi, daftar window, serta informasi CPU dan waktu
- Warna status berubah sesuai tingkat penggunaan CPU
- Background status bar transparan

## Konfigurasi Tambahan
- Mouse support: Aktif
- 256 color mode: Aktif
- Base window index: 1 (bukan 0)
- History limit: 1000 baris