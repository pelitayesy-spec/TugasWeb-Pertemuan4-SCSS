# Tugas Rutin 4: Konversi CSS ke SCSS (7-1 Pattern)

Sumber: Tugas Pertemuan 2 (index.html + style.css), HTML tidak diubah
kecuali link `style.css` diganti dengan script Vite.

## Menjalankan
    npm install
    npm run dev       # buka alamat di terminal
    npm run build     # hasil di dist/

Letakkan foto di `images/MyPhoto.jpeg`.

## Struktur
    src/
    ├── main.js              (import main.scss)
    └── scss/
        ├── main.scss
        ├── abstracts/       variables, functions, mixins
        ├── vendors/
        ├── base/            root (CSS variables), reset
        ├── layout/          header, main, section, footer
        ├── components/      details, card, profile-card, contact-item
        ├── pages/           home, about, contact
        └── themes/          dark (prefers-color-scheme)

## Pemenuhan ketentuan
1. Konversi CSS existing ke SCSS: semua rule style.css dipindah
2. Variables colors & spacing: abstracts/_variables.scss
3. Nesting maks 3 level: semua file
4. Minimal 3 mixins: respond-down, flex, card-surface, hover-lift, icon-box, section-label
5. Struktur 7-1: 7 folder + main.scss
6. @use (bukan @import): semua file
7. @each: components/_card.scss (map $card-hover)
8. Compile dengan Vite / Dart Sass: package.json
