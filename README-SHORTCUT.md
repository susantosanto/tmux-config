# Tmux Shortcut Guide

Dokumentasi ini menjelaskan shortcut tmux yang telah dikonfigurasi dalam sistem Anda.

## Prefix Key

- **F1** - Prefix key utama (menggantikan Ctrl+b)

## Session Management

- **F1 + C** - Buat session baru (dengan prompt)
- **F1 + Ctrl + r** - Restore session dari tmux-resurrect
- **F1 + Ctrl + s** - Simpan session secara manual dengan tmux-resurrect
- **F1 + Shift + S** - Simpan session secara manual sebelum shutdown/restart
- **F1 + X** - Hapus session saat ini (dengan prompt)
- **F1 + d** - Detach dari session saat ini

## Window Management

- **F1 + c** - Buat window baru
- **F1 + '** - Pindah ke window tertentu (dengan prompt)
- **F1 + o** - Pindah ke window sebelumnya (previous window)
- **F1 + p** - Pindah ke window berikutnya (next window)
- **F1 + 0-9** - Pindah ke window dengan nomor tertentu
- **F1 + Ctrl + n** - Pindah ke window berikutnya (next window)
- **F1 + ,** - Tukar window dengan yang sebelumnya (swap window -1)
- **F1 + .** - Tukar window dengan yang berikutnya (swap window +1)

## Pane Management

- **F1 + |** - Split window horizontal (pane kiri/kanan)
- **F1 + -** - Split window vertikal (pane atas/bawah)
- **F1 + h/j/k/l** - Navigasi pane (kiri/bawah/atas/kanan)
- **F1 + Up/Down/Left/Right** - Navigasi pane (menggunakan arrow keys)
- **F1 + Tab** - Pindah ke pane sebelumnya
- **F1 + t** - Toggle zoom pane
- **F1 + z** - Toggle zoom pane (juga fungsi lainnya)
- **F1 + x** - Kill pane
- **F1 + {** - Tukar pane dengan yang sebelumnya (swap pane -U)
- **F1 + }** - Tukar pane dengan yang berikutnya (swap pane -D)

## Resize Pane

- **F1 + H/J/K/L** - Resize pane ke kiri/bawah/atas/kanan (5 karakter)
- **F1 + Ctrl + H/J/K/L** - Resize pane ke kiri/bawah/atas/kanan (1 karakter)
- **F1 + Shift + H/J/K/L** - Refresh client (bukan resize)

## Custom Path Management

- **F1 + P** - Buka pane horizontal dengan custom path (dengan prompt)
- **F1 + Ctrl + P** - Buka pane vertikal dengan custom path (dengan prompt)
- **F1 + W** - Buka window baru dengan custom path (dengan prompt)

## Session dan Window Tree

- **F1 + s** - Lihat dan pilih session dari tree
- **F1 + w** - Lihat dan pilih window dari tree

## Command dan Menu

- **F1 + r** - Reset kursor ke line style (bukan reload config)
- **F1 + ?** - Buka menu bantuan (tmux-which-key)
- **F1 + m** - Buka tmux-menus
- **F1 + F1** - Tampilkan menu (tmux-which-key)
- **F1 + BSpace** - Buka command palette
- **F1 + f** - Cari window dari semua window yang terbuka
- **F1 + :** - Command prompt

## Copy Mode

- **F1 + [** - Masuk copy mode
- **Mouse wheel** - Scroll dalam pane
- **Copy mode vi**: Gunakan h/j/k/l untuk navigasi, v untuk select, y untuk copy
- **F1 + /** - Cari teks dalam session (dengan prompt)

## Custom Commands

- **F1 + n** - Buka neovim di window baru (dengan path saat ini)
- **F1 + Ctrl + n** - Buka neovim di pane horizontal (dengan path saat ini)
- **F1 + Ctrl + v** - Buka neovim di pane vertikal (dengan path saat ini)
- **F1 + q** - Buka pane baru dengan perintah `qwen` (dengan path saat ini)
- **F1 + Q** - Buka window baru dengan perintah `qwen` (dengan path saat ini)
- **F1 + e** - Buka pane baru dengan perintah `opencode` (dengan path saat ini)
- **F1 + E** - Buka window baru dengan perintah `opencode` (dengan path saat ini)
- **F1 + g** - Buka lazygit di window baru (dengan path saat ini)
- **F1 + G** - Buka lazygit di pane horizontal (dengan path saat ini)

## Scratch Window

- **F1 + b** - Buka scratch window kecil (80x10)
- **F1 + B** - Buka scratch window besar (100x20)
- **F12** - Buka scratch window dari root (bukan dengan prefix key)

## Navigation dan Window

- **F1 + <** - Menu tindakan window (swap, rename, new, dll)
- **F1 + >** - Menu tindakan pane (swap, zoom, kill, dll)

## Join Window

- **F1 + Ctrl + j** - Gabung pane dari session lain (horizontal)
- **F1 + Ctrl + Shift + j** - Gabung pane dari session lain (vertikal)

## Mouse Support

- **Mouse Left Click** - Pilih pane
- **Mouse Wheel** - Scroll dan navigasi window (jika dalam mode)
- **Mouse Right Click** - Paste dari buffer

## Informasi Tambahan

- `qwen` adalah perintah terminal untuk Qwen Code
- `opencode` adalah perintah terminal untuk OpenCode
- `lazygit` adalah perintah terminal untuk interface Git
- Semua perintah ini akan dijalankan di path yang sama dengan pane/window saat ini

## Lainnya

- **F1 + &** - Konfirmasi sebelum kill window
- **F1 + !** - Pindahkan pane ke window baru (break pane)
- **F1 + ]** - Paste dari buffer
- **F1 + y** - Copy current line dari pane ke buffer
- **F1 + Y** - Copy current working directory (pwd) ke buffer

## Note

- Gunakan `~` untuk merujuk ke home directory (`/home/xcode`)
- Path relatif dihitung dari home directory (misal: `.config/nvim` = `~/config/nvim`)
- Fungsi session persistence otomatis berjalan setiap 15 menit (tmux-continuum)
- Plugin tmux-resurrect menyimpan dan memulihkan session, termasuk pane dan isi dari window