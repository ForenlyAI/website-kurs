# Website Yapımı 101 — Lab deposu

[Forenly Academy](https://academy.forenly.ai) · **Website Yapımı 101** kursunun uygulama dosyaları.
Kurs boyunca kurgusal bir Eskişehir kafesinin sitesi, **Kahve Durağı**, Astro ile yapılır, derlenir ve
Cloudflare Pages'e yüklenmeye hazır hâle getirilir.

[![GitHub Codespaces'te aç](https://github.com/codespaces/badge.svg)](https://codespaces.new/ForenlyAI/website-kurs?quickstart=1)

## En hızlı yol: tarayıcıda (kurulum yok)

1. Yukarıdaki **Open in GitHub Codespaces** düğmesine basılır (GitHub hesabı yeterli; kişisel hesaplarda aylık ücretsiz kullanım vardır).
2. Ortam 1–2 dakikada açılır; Node.js 22 ve paketler hazır kurulur.
3. Alttaki terminalde:

```bash
cd kahve-duragi
npm run dev        # önizleme: 4321 portu otomatik açılır
```

## Kendi bilgisayarınızda

Node.js **22 LTS** (en az 22.12) ve VS Code (Astro eklentisiyle) kurulur, sonra:

```bash
cd kahve-duragi
npm ci             # package-lock.json'daki sabit sürümler
npm run dev        # http://localhost:4321
npm run build      # yayına hazır dosyalar: dist/
npm run preview    # derlenmiş siteyi yerelde aç
```

## Klasörler

| Klasör | Ne |
|---|---|
| `kahve-duragi/` | Bitmiş site (2.3 → 4.x derslerinin sonu) |
| `asamalar/1.3-bos-proje/` | Ders 1.3 sonu: boş Astro projesi |
| `asamalar/2.1-duzen/` | Ders 2.1 sonu: ortak düzen (üst menü, alt bilgi, stil) |
| `asamalar/2.2-icerik/` | Ders 2.2 sonu: menü, hakkımızda ve ana sayfa içerikleri |

Bir derste takılındığında kendi projeniz o dersin klasörüyle karşılaştırılabilir
(VS Code: iki dosyayı seçip sağ tık → “Compare Selected”). Ayrıntı: [`asamalar/README.md`](asamalar/README.md).

> Kafenin adı, adresi, telefonu (0222 000 00 00) ve e-postası (merhaba@example.com) kurgusaldır.
> Görseller bu kurs için çizilmiş SVG'lerdir; fotoğraf ya da telifli içerik yoktur.
