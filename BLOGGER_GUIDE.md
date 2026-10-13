# Panduan Blogger — kebun-digitalku

## Menambah Post Blog Baru

Buat file `.md` di `src/content/blog/`:

```markdown
---
title: "Judul Postingan"
description: "Deskripsi singkat untuk SEO"
pubDate: 2026-10-13
heroImage: ../../assets/nama-gambar.jpg
tags: ["teknologi", "opini"]
---

Tulis konten di sini pakai Markdown.
```

Field wajib: `title`, `description`, `pubDate`. Field opsional: `heroImage`, `tags`, `updatedDate`.

---

## Menambah Project Baru

Buat file `.md` di `src/content/projects/`:

```markdown
---
title: "Nama Project"
description: "Deskripsi singkat"
pubDate: 2026-10-13
heroImage: ../../assets/screenshot.jpg
tags: ["Python", "Streamlit"]
status: completed
---

Penjelasan lengkap project di sini.
```

Status bisa: `completed`, `in-progress`, `on-hold`.

---

## Mengubah Data Blog

Edit file `src/consts.ts`:

```ts
export const SITE_TITLE = 'Rahsan\'s Blog';
export const SITE_DESCRIPTION = 'Welcome to my website!';
```

---

## Mengubah Navigasi

Edit `src/components/Header.astro` — tambah/hapus `<HeaderLink>` di dalam `.internal-links`.

---

## Menambah Gambar

Letakkan gambar di `src/assets/`, lalu reference di frontmatter atau komponen dengan path `../../assets/nama-gambar.jpg`.

---

## Deploy ke Netlify

```bash
git add -A
git commit -m "deskripsi perubahan"
git push
```

Netlify otomatis build dan publish.

---

## Menambah Filter Kategori Project

Di `src/pages/projects.astro`, tambahkan tag baru di frontmatter project. Filter otomatis muncul berdasarkan tag dan status yang ada.

---

## Mengatur Jumlah Post per Halaman

Di `src/pages/blog/page/[page].astro`, ubah nilai `POSTS_PER_PAGE`:

```ts
const POSTS_PER_PAGE = 6;
```

---

## Menonaktifkan Dark Mode

Hapus komponen `<button id="theme-toggle">` di `src/components/Header.astro` dan hapus style `[data-theme="dark"]` di `src/styles/global.css`.
