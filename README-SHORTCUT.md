# Tmux Shortcut Guide

Dokumentasi ini menjelaskan shortcut tmux yang telah dikonfigurasi dalam sistem Anda.

## Prefix Key

- **F1** - Prefix key utama (menggantikan Ctrl+b)

## Session Management

- **F1 + Shift + S** - Manual save session sebelum shutdown/restart

## Window dan Pane Management

- **F1 + c** - Buat window baru
- **F1 + |** - Split window horizontal
- **F1 + -** - Split window vertikal
- **F1 + n** - Window berikutnya
- **F1 + p** - Window sebelumnya
- **F1 + h/j/k/l** - Navigasi pane (kiri/bawah/atas/kanan)
- **F1 + t** - Toggle zoom pane
- **F1 + x** - Kill pane
- **F1 + X** - Kill window

## Resize Pane

- **F1 + H/J/K/L** - Resize pane ke kiri/bawah/atas/kanan
- **F1 + Ctrl + H/J/K/L** - Resize pane dengan ukuran besar

## Custom Path Management

- **F1 + Shift + P** - Buka pane horizontal dengan custom path (relatif terhadap home, misal: `.config/nvim`)
- **F1 + Ctrl + P** - Buka pane vertikal dengan custom path (gunakan ~ untuk home, misal: `~/projects/myproject`)
- **F1 + Shift + W** - Buka window baru dengan custom path (gunakan ~ untuk home, misal: `~/documents`)

## Session dan Window Tree

- **F1 + s** - Lihat tree session
- **F1 + w** - Lihat tree window

## Command dan Menu

- **F1 + r** - Reload konfigurasi tmux
- **F1 + F1** - Buka menu (dengan tmux-which-key)
- **F1 + m** - Buka tmux-menus
- **F1 + BSpace** - Buka command palette

## Navigasi dan Copy Mode

- **F1 + [** - Masuk copy mode
- **Copy mode vi**: Gunakan h/j/k/l untuk navigasi, v untuk select, y untuk copy
- **F1 + /** - Cari teks dalam session

## Custom Commands

- **F1 + q** - Buka pane baru dengan perintah `qwen`
- **F1 + Q** - Buka window baru dengan perintah `qwen`
- **F1 + e** - Buka pane baru dengan perintah `opencode`
- **F1 + E** - Buka window baru dengan perintah `opencode`

## Informasi Tambahan

- `qwen` adalah perintah terminal untuk Qwen Code
- `opencode` adalah perintah terminal untuk OpenCode
- Kedua perintah ini akan dijalankan di path yang sama dengan pane/window saat ini

## Lainnya

- **F1 + Tab** - Pindah ke pane sebelumnya
- **F1 + d** - Detach dari session

## Note

- Gunakan `~` untuk merujuk ke home directory (`/home/xcode`)
- Path relatif dihitung dari home directory (misal: `.config/nvim` = `~/config/nvim`)
- Fungsi session persistence otomatis berjalan setiap 15 menit