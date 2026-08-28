# Relasi dan Fungsi — Kelas XII

---

## 1. Pengertian Dasar

### 1.1 Relasi

**Relasi** adalah hubungan antara dua himpunan yang menghubungkan setiap elemen dari himpunan tertentu dengan elemen lainnya.

> **Analogi:** Bayangkan sebuah daftar nomor HP. Setiap nama (dari himpunan nama) dihubungkan ke nomor HP (dari himpunan nomor). Hubungan "nama → nomor HP" itu adalah relasi.

Notasi:

$$
R: A \rightarrow B \quad \text{atau} \quad (a, b) \in R
$$

Di mana $A$ adalah **domain** (himpunan asal) dan $B$ adalah **codomain** (himpunan tujuan).

### 1.2 Fungsi

**Fungsi** adalah relasi khusus di mana **setiap elemen** dalam himpunan asal dipetakan ke **tepat satu** elemen di himpunan tujuan.

> **Analogi:** Sebuah mesin vending. Masukkan uang Rp5.000 (input), keluar satu botol minum (output). Setiap uang yang dimasukkan selalu menghasilkan tepat satu hasil — tidak lebih, tidak kurang.

Notasi:

$$
f: A \rightarrow B, \quad f(x) = y
$$

### 1.3 Perbedaan Relasi dan Fungsi

| Ciri | Relasi | Fungsi |
|---|---|---|
| Setiap elemen domain harus punya pasangan? | Tidak wajib | **Wajib** |
| Satu elemen domain boleh punya lebih dari satu pasangan? | Boleh | **Tidak boleh** |
| Contoh | {(1,2), (1,3), (2,4)} | {(1,2), (2,4), (3,1)} |

---

## 2. Tipe-Tipe Relasi

### 2.1 Relasi Satu-ke-Satu (One-to-One / Injektif)

Setiap elemen $A$ dipetakan ke elemen unik di $B$, dan tidak ada dua elemen $A$ yang dipetakan ke elemen $B$ yang sama.

> **Analogi:** Satu kursi, satu orang. Tidak ada yang berdiri berdua di satu kursi.

$$
\text{Jika } f(a_1) = f(a_2), \text{ maka } a_1 = a_2
$$

### 2.2 Relasi Satu-ke-Banyak (One-to-Many)

Satu elemen $A$ dipetakan ke lebih dari satu elemen $B$.

> **Analogi:** Satu orang punya banyak akun media sosial. Tapi ini **bukan fungsi**, karena dari satu input menghasilkan banyak output.

Contoh: $\{(1,2), (1,3), (2,4)\}$ — elemen 1 punya dua pasangan.

### 2.3 Relasi Banyak-ke-Satu (Many-to-One / Non-Injektif)

Lebih dari satu elemen $A$ dipetakan ke elemen $B$ yang sama, tetapi tetap memenuhi syarat fungsi.

> **Analogi:** Banyak siswa dalam satu kelas, tetapi satu wali kelas. Banyak → satu.

Contoh: $\{(1,5), (2,5), (3,6)\}$ — elemen 1 dan 2 sama-sama menghasilkan 5. Ini **masih fungsi**.

### 2.4 Relasi Banyak-ke-Banyak (Many-to-Many)

> **Analogi:** Di media sosial, satu orang bisa follow banyak orang, dan di-follow balik oleh banyak orang.

### 2.5 Relasi Total (Totalitas)

Setiap elemen di $A$ memiliki pasangan di $B$. Jika ada elemen $A$ yang tidak memiliki pasangan, relasi tersebut tidak total.

### 2.6 Relasi Injektif, Surjektif, dan Bijections

| Tipe | Definisi | Analogi |
|---|---|---|
| **Injektif** (One-to-One) | Tiap elemen domain unik ke codomain | KTP: satu orang, satu nomor |
| **Surjektif** (Onto) | Semua elemen codomain terpakai | Setiap kursi di ruangan terisi |
| **Bijektif** (One-to-One & Onto) | Injektif + Surjektif | Satu pintu masuk, satu pintu keluar, semua terpakai |

---

## 3. Komposisi Fungsi

**Komposisi fungsi** adalah penggabungan dua fungsi: hasil fungsi pertama menjadi masukan fungsi kedua.

$$
(g \circ f)(x) = g(f(x))
$$

> **Analogi:** Di sebuah pabrik, barang melewati dua mesin. Mesin pertama ($f$) memotong, mesin kedua ($g$) mengecat. Hasil akhir = $g(f(\text{barang}))$.

### Contoh:

$$
f(x) = 2x + 1, \quad g(x) = x^2
$$

$$
(g \circ f)(3) = g(f(3)) = g(7) = 49
$$

$$
(f \circ g)(3) = f(g(3)) = f(9) = 19
$$

> ⚠️ Perhatikan: $g \circ f \neq f \circ g$ dalam kebanyakan kasus!

---

## 4. Fungsi Invers (Fungsi Balikan)

Fungsi invers $f^{-1}$ membalik pemetaan: jika $f(a) = b$, maka $f^{-1}(b) = a$.

> **Analogi:** Lift di gedung. Jika tombol lantai 3 mengantar ke lantai 3, maka tombol invers dari lantai 3 kembali ke lobby.

$$
f(f^{-1}(x)) = x \quad \text{dan} \quad f^{-1}(f(x)) = x
$$

### Syarat fungsi memiliki invers:
Fungsi harus **bijektif** (injektif + surjektif).

### Contoh:

$$
f(x) = 3x - 5
$$

Cari $f^{-1}(x)$:

$$
y = 3x - 5 \Rightarrow x = \frac{y + 5}{3}
$$

$$
f^{-1}(x) = \frac{x + 5}{3}
$$

---

## 5. Fungsi Linear, Kuadrat, dan Eksponensial

### 5.1 Fungsi Linear

$$
f(x) = ax + b, \quad a \neq 0
$$

Grafik: garis lurus.

> **Analogi:** Gaji tetap = gaji pokok + bonus tetap per jam.

### 5.2 Fungsi Kuadrat

$$
f(x) = ax^2 + bx + c, \quad a \neq 0
$$

Grafik: parabola. Titik puncak:

$$
x_p = -\frac{b}{2a}, \quad y_p = f(x_p)
$$

> **Analogi:** Lemparan bola ke atas. Tinggi bola mengikuti kurva parabola.

### 5.3 Fungsi Eksponensial

$$
f(x) = a \cdot b^x, \quad a \neq 0, \; b > 0, \; b \neq 1
$$

> **Analogi:** Bunga bank berbunga majemuk. Uangmu tumbuh cepat seiring waktu.

---

## 6. Contoh Soal

### Contoh 1 (Mudah)

Diketahui $A = \{1, 2, 3\}$ dan $B = \{4, 5, 6\}$. Tentukan apakah $R = \{(1,4), (2,5), (3,6)\}$ adalah fungsi.

**Jawab:**
Setiap elemen $A$ memiliki tepat satu pasangan di $B$. → **Ya, ini fungsi.**

---

### Contoh 2 (Sedang)

$$
f(x) = 2x^2 - 8x + 3
$$

Tentukan titik puncak parabola.

**Jawab:**

$$
x_p = -\frac{-8}{2(2)} = \frac{8}{4} = 2
$$

$$
y_p = f(2) = 2(4) - 8(2) + 3 = 8 - 16 + 3 = -5
$$

Titik puncak: $(2, -5)$

---

### Contoh 3 (Sulit)

Tentukan fungsi invers dari $f(x) = \dfrac{2x + 3}{x - 1}$.

**Jawab:**

$$
y = \frac{2x + 3}{x - 1}
$$

$$
y(x - 1) = 2x + 3
$$

$$
xy - y = 2x + 3
$$

$$
xy - 2x = y + 3
$$

$$
x(y - 2) = y + 3
$$

$$
x = \frac{y + 3}{y - 2}
$$

$$
f^{-1}(x) = \frac{x + 3}{x - 2}, \quad x \neq 2
$$

---

## 7. Latihan Soal (20 Soal)

### Soal 1 — Mudah

Tentukan apakah relasi berikut adalah fungsi:

$$
R = \{(1,2), (2,3), (3,4), (4,5)\}
$$

---

### Soal 2 — Mudah

Tentukan apakah relasi berikut adalah fungsi:

$$
R = \{(1,1), (1,2), (2,3), (3,4)\}
$$

---

### Soal 3 — Mudah

Diketahui $f(x) = 3x - 7$. Tentukan nilai $f(4)$.

---

### Soal 4 — Mudah

Diketahui $f(x) = x^2 + 1$. Tentukan nilai $f(-3)$.

---

### Soal 5 — Mudah

Fungsi $f(x) = 5x + 2$. Tentukan $f^{-1}(x)$.

---

### Soal 6 — Mudah

Diketahui himpunan $A = \{a, b, c\}$ dan $B = \{1, 2, 3, 4\}$. Berapa banyak fungsi dari $A$ ke $B$?

---

### Soal 7 — Sedang

Diketahui $f(x) = 2x + 1$ dan $g(x) = x^2 - 3$. Tentukan $(g \circ f)(2)$.

---

### Soal 8 — Sedang

Diketahui $f(x) = 3x - 2$. Tentukan nilai $x$ jika $f(x) = 13$.

---

### Soal 9 — Sedang

Tentukan titik puncak dari fungsi $f(x) = -2x^2 + 8x - 3$.

---

### Soal 10 — Sedang

Diketahui $f(x) = \dfrac{x + 2}{3}$. Tentukan $f^{-1}(x)$.

---

### Soal 11 — Sedang

Diketahui $f(x) = 4x - 1$ dan $g(x) = x + 5$. Tentukan $(f \circ g)(x)$ dan $(g \circ f)(x)$.

---

### Soal 12 — Sedang

Fungsi $f: \mathbb{R} \to \mathbb{R}$ didefinisikan oleh $f(x) = x^2 - 4$. Apakah $f$ adalah fungsi bijektif? Jelaskan.

---

### Soal 13 — Sedang

Tentukan domain dan range dari $f(x) = \sqrt{x - 3}$.

---

### Soal 14 — Sedang

Diketahui relasi $R = \{(x,y) \mid y = 2x + 1, \; x \in \{0,1,2,3\}\}$. Tuliskan $R$ dalam bentuk himpunan pasangan terurut.

---

### Soal 15 — Sulit

Diketahui $f(x) = \dfrac{3x + 2}{x - 4}$. Tentukan $f^{-1}(x)$ dan nyatakan domain $f^{-1}$.

---

### Soal 16 — Sulit

Diketahui $f(x) = 2^x + 1$. Tentukan $f^{-1}(x)$.

---

### Soal 17 — Sulit

Diketahui $f(x) = x^2 - 6x + 8$ untuk $x \geq 3$. Tentukan $f^{-1}(x)$.

---

### Soal 18 — Sulit

Sebuah fungsi $f$ didefinisikan dari $\mathbb{R}$ ke $\mathbb{R}$ dengan $f(x) = ax + b$. Jika $f(1) = 5$ dan $f(3) = 11$, tentukan nilai $a$ dan $b$.

---

### Soal 19 — Sulit

Diketahui $f(x) = \dfrac{x - 1}{x + 2}$ dan $g(x) = \dfrac{2x + 1}{x - 3}$. Tentukan $(f \circ g)(x)$.

---

### Soal 20 — Sulit

Fungsi $f: \mathbb{R} \setminus \{2\} \to \mathbb{R}$ didefinisikan oleh $f(x) = \dfrac{3x + 1}{x - 2}$.

a) Buktikan bahwa $f$ adalah fungsi injektif.
b) Tentukan $f^{-1}(x)$.
c) Jika $f(a) = 4$, tentukan nilai $a$.

---

## 8. Pembahasan Latihan Soal

### Pembahasan Soal 1

$$
R = \{(1,2), (2,3), (3,4), (4,5)\}
$$

Setiap elemen domain $\{1,2,3,4\}$ memiliki tepat satu pasangan di codomain. Tidak ada elemen yang memiliki lebih dari satu pasangan.

**→ Ya, ini fungsi.**

---

### Pembahasan Soal 2

$$
R = \{(1,1), (1,2), (2,3), (3,4)\}
$$

Elemen $1$ memiliki dua pasangan: $1$ dan $2$.

**→ Bukan fungsi** (satu input menghasilkan dua output).

---

### Pembahasan Soal 3

$$
f(4) = 3(4) - 7 = 12 - 7 = 5
$$

**→ $f(4) = 5$**

---

### Pembahasan Soal 4

$$
f(-3) = (-3)^2 + 1 = 9 + 1 = 10
$$

**→ $f(-3) = 10$**

---

### Pembahasan Soal 5

$$
y = 5x + 2
$$

$$
x = \frac{y - 2}{5}
$$

$$
f^{-1}(x) = \frac{x - 2}{5}
$$

---

### Pembahasan Soal 6

Setiap elemen di $A$ (3 elemen) dapat dipetakan ke salah satu dari 4 elemen di $B$.

$$
4^3 = 64 \text{ fungsi}
$$

---

### Pembahasan Soal 7

$$
f(2) = 2(2) + 1 = 5
$$

$$
g(5) = 5^2 - 3 = 25 - 3 = 22
$$

**→ $(g \circ f)(2) = 22$**

---

### Pembahasan Soal 8

$$
4x - 1 = 13
$$

$$
4x = 14
$$

$$
x = \frac{14}{4} = 3{,}5
$$

**→ $x = \frac{7}{2}$**

---

### Pembahasan Soal 9

$$
x_p = -\frac{8}{2(-2)} = -\frac{8}{-4} = 2
$$

$$
y_p = f(2) = -2(4) + 8(2) - 3 = -8 + 16 - 3 = 5
$$

**→ Titik puncak: $(2, 5)$**

---

### Pembahasan Soal 10

$$
y = \frac{x + 2}{3}
$$

$$
3y = x + 2
$$

$$
x = 3y - 2
$$

$$
f^{-1}(x) = 3x - 2
$$

---

### Pembahasan Soal 11

$$
(f \circ g)(x) = f(g(x)) = f(x + 5) = 4(x + 5) - 1 = 4x + 20 - 1 = 4x + 19
$$

$$
(g \circ f)(x) = g(f(x)) = g(4x - 1) = (4x - 1) + 5 = 4x + 4
$$

**→ $(f \circ g)(x) = 4x + 19$ dan $(g \circ f)(x) = 4x + 4$**

---

### Pembahasan Soal 12

$f(x) = x^2 - 4$:

- **Injektif?** Tidak. $f(2) = 0$ dan $f(-2) = 0$. Dua input berbeda menghasilkan output sama.
- **Surjektif?** Ya, untuk codomain $\mathbb{R}_{\geq -4}$.
- Karena tidak injektif, **tidak bijektif**.

**→ Fungsi tidak bijektif karena tidak injektif.**

---

### Pembahasan Soal 13

$$
f(x) = \sqrt{x - 3}
$$

Domain: $x - 3 \geq 0 \Rightarrow x \geq 3$

$$
\text{Domain} = [3, \infty)
$$

Range: $\sqrt{\text{bilangan} \geq 0}$ selalu $\geq 0$

$$
\text{Range} = [0, \infty)
$$

---

### Pembahasan Soal 14

Substitusi setiap nilai $x \in \{0, 1, 2, 3\}$ ke $y = 2x + 1$:

- $x = 0 \Rightarrow y = 1$
- $x = 1 \Rightarrow y = 3$
- $x = 2 \Rightarrow y = 5$
- $x = 3 \Rightarrow y = 7$

$$
R = \{(0,1), (1,3), (2,5), (3,7)\}
$$

---

### Pembahasan Soal 15

$$
y = \frac{3x + 2}{x - 4}
$$

$$
y(x - 4) = 3x + 2
$$

$$
yx - 4y = 3x + 2
$$

$$
yx - 3x = 4y + 2
$$

$$
x(y - 3) = 4y + 2
$$

$$
x = \frac{4y + 2}{y - 3}
$$

$$
f^{-1}(x) = \frac{4x + 2}{x - 3}
$$

Domain $f^{-1}$: $x \neq 3$

---

### Pembahasan Soal 16

$$
y = 2^x + 1
$$

$$
y - 1 = 2^x
$$

$$
x = \log_2(y - 1)
$$

$$
f^{-1}(x) = \log_2(x - 1)
$$

---

### Pembahasan Soal 17

Karena $x \geq 3$, kita harus memilih cabang positif akar:

$$
y = x^2 - 6x + 8 = (x-3)^2 - 1
$$

$$
y + 1 = (x - 3)^2
$$

$$
x - 3 = \sqrt{y + 1} \quad (\text{karena } x \geq 3, \text{ ambil positif})
$$

$$
x = 3 + \sqrt{y + 1}
$$

$$
f^{-1}(x) = 3 + \sqrt{x + 1}, \quad x \geq -1
$$

---

### Pembahasan Soal 18

$$
\begin{cases} a(1) + b = 5 \\ a(3) + b = 11 \end{cases}
$$

$$
\begin{cases} a + b = 5 \quad \ldots(1) \\ 3a + b = 11 \quad \ldots(2) \end{cases}
$$

(2) − (1):

$$
2a = 6 \Rightarrow a = 3
$$

Substitusi ke (1):

$$
3 + b = 5 \Rightarrow b = 2
$$

**→ $a = 3, \; b = 2$**, sehingga $f(x) = 3x + 2$

---

### Pembahasan Soal 19

$$
g(x) = \frac{2x + 1}{x - 3}
$$

$$
f(g(x)) = \frac{g(x) - 1}{g(x) + 2}
$$

$$
= \frac{\dfrac{2x+1}{x-3} - 1}{\dfrac{2x+1}{x-3} + 2}
$$

$$
= \frac{\dfrac{2x+1 - (x-3)}{x-3}}{\dfrac{2x+1 + 2(x-3)}{x-3}}
$$

$$
= \frac{2x + 1 - x + 3}{2x + 1 + 2x - 6}
$$

$$
= \frac{x + 4}{4x - 5}
$$

**→ $(f \circ g)(x) = \dfrac{x + 4}{4x - 5}$, $x \neq 3, \; x \neq \dfrac{5}{4}$**

---

### Pembahasan Soal 20

**Bagian (a):**

Untuk membuktikan injektif, misalkan $f(a) = f(b)$:

$$
\frac{3a + 1}{a - 2} = \frac{3b + 1}{b - 2}
$$

$$
(3a + 1)(b - 2) = (3b + 1)(a - 2)
$$

$$
3ab - 6a + b - 2 = 3ab - 6b + a - 2
$$

$$
-6a + b = -6b + a
$$

$$
7b = 7a
$$

$$
a = b
$$

Karena $f(a) = f(b) \Rightarrow a = b$, fungsi **injektif**.

---

**Bagian (b):**

$$
y = \frac{3x + 1}{x - 2}
$$

$$
y(x - 2) = 3x + 1
$$

$$
xy - 2y = 3x + 1
$$

$$
xy - 3x = 2y + 1
$$

$$
x(y - 3) = 2y + 1
$$

$$
f^{-1}(x) = \frac{2x + 1}{x - 3}, \quad x \neq 3
$$

---

**Bagian (c):**

$$
f(a) = 4
$$

$$
\frac{3a + 1}{a - 2} = 4
$$

$$
3a + 1 = 4(a - 2)
$$

$$
3a + 1 = 4a - 8
$$

$$
a = 9
$$

**→ $a = 9$** (verifikasi: $f(9) = \frac{28}{7} = 4$ ✓)

---

*Selesai. Semoga membantu dalam memahami Relasi dan Fungsi!*
