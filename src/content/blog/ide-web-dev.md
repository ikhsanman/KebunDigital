---
title: "Ide Pertamaku tentang Web Dev"
description: "Catatan awal belajar Astro dan Netlify."
pubDate: "2026-07-07"
heroImage: "../../assets/blog-placeholder-3.jpg"
---

# Rencana penelitian

<aside>
📖

**Peta Jalan Penelitian (Research Roadmap)**
Pengerjaan model *Fractional Partial Differential Equation* (FPDE) memerlukan pendekatan yang bertahap agar kamu tidak kewalahan. Kita akan membaginya menjadi 4 fase utama.

</aside>

## **Fase 1: Fondasi dan Formulasi Model (Minggu 1)**

Fokus di fase ini adalah membangun persamaan matematis yang merepresentasikan semua kondisi ekologis.

- **Langkah 1:** Susun model dasar predator-prey orde integer (turunan biasa) yang menyertakan fungsi ketakutan, *prey refuge* (sebagian mangsa sembunyi sehingga tidak bisa dimakan), dan *harvesting* (pemanenan pada mangsa atau predator).
- **Langkah 2:** Ubah turunan waktu menjadi turunan fraksional Caputo ($^C D^\alpha_t$).
- **Langkah 3:** Tambahkan operator Laplacian ($\Delta$) untuk mewakili difusi spasial (pergerakan acak) pada mangsa dan pemangsa.
- **Target Luaran:** Mendapatkan sistem persamaan FPDE yang utuh beserta penjelasan biologis untuk setiap parameter.

## **Fase 2: Analisis Dinamika Tanpa Ruang / Homogen Spasial (Minggu 2)**

Sebelum menganalisis ruang, wajib membuktikan kestabilan model jika hewan tersebut tidak bergerak (koefisien difusi = 0).

- **Langkah 1:** Cari semua Titik Kesetimbangan (*Equilibrium Points*), seperti titik kepunahan total, titik kepunahan predator, dan titik koeksistensi (keduanya hidup).
- **Langkah 2:** Lakukan analisis kestabilan lokal menggunakan matriks Jacobian di setiap titik kesetimbangan.
- **Langkah 3:** Gunakan kriteria stabilitas Routh-Hurwitz yang dimodifikasi untuk sistem fraksional (memperhatikan nilai eigen dan syarat sudut orde fraksional $\alpha$).

## **Fase 3: Analisis Dinamika Spasial dan Ketidakstabilan Turing (Minggu 3)**

Ini adalah "jantung" dari kebaruan skripsi.

- **Langkah 1:** Aktifkan koefisien difusi ($d_1$ dan $d_2$).
- **Langkah 2:** Lakukan analisis **Ketidakstabilan Turing**. Harus membuktikan kondisi matematis di mana titik ekuilibrium yang awalnya stabil di Fase 2, tiba-tiba menjadi *tidak stabil* hanya karena adanya pergerakan (difusi).
- **Target Luaran:** Mendapatkan himpunan parameter bersyarat (misal: "Pola spasial akan muncul jika laju pemanenan $h < 0.5$ dan tingkat ketakutan $k > 0.1$").

## **Fase 4: Diskritisasi, Simulasi Komputer, dan Ekologi (Minggu 4-5)**

Karena FPDE tidak bisa diselesaikan di atas kertas untuk mendapatkan solusi pastinya, harus menggunakan komputasi.

- **Langkah 1:** Pilih skema numerik. Biasanya yang paling aman adalah **Skema Beda Hingga (*Finite Difference*)** untuk memotong-motong ruang, dan **Aproksimasi L1** untuk menghitung turunan fraksional Caputo terhadap waktu.
- **Langkah 2:** Lakukan *coding* (MATLAB atau Python sangat disarankan) untuk merender visualisasinya.
- **Langkah 3:** Hasilkan plot 2D atau 3D yang menunjukkan pola Turing (seperti pola bintik-bintik atau labirin yang merepresentasikan distribusi populasi hewan).
- **Langkah 4:** Interpretasikan hasil grafiknya secara biologis. Apa artinya jika polanya terputus-putus? Bagaimana efek memori (orde $\alpha$) menunda kepunahan akibat pemanenan berlebih?