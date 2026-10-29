# Haftalık otomatik yazı görevi

Bu dosya, her hafta çalışan otomatik görevin talimatlarıdır.

## Görev
1. `_posts/` klasöründeki mevcut yazıları oku. Aynı konuyu tekrar yazma.
2. Bu hafta için **2 yeni yazı** yaz. Konu türleri sırayla dönsün:
   - "X mi Y mi?" karşılaştırması
   - "Nasıl yapılır" rehberi (aranan pratik bir problem)
   - Satın alma rehberi ("... alırken nelere dikkat edilmeli")
   - Kategori listesi ("... için ilk alışveriş listesi")
3. Kategoriler: Mutfak, Ev, Temizlik, Teknoloji, Kişisel Bakım, Evcil Hayvan.
4. Ürün bağlantıları için yalnızca `_data/products.yml` içindeki ASIN'leri kullan. Ürün eklemek için `{% include product.html name="..." asin="..." meta="..." good="..." bad="..." %}`.

## Kurallar
- Türkçe, sade, faydalı. 450-800 kelime.
- **Fiyat yazma.** Fiyat ve indirim oranı belirtme.
- Uydurma özellik, test sonucu veya kişisel deneyim yazma ("denedik", "3 ay kullandık" deme). Puan, yorum sayısı ve sıralama `_data/products.yml`'deki verilerden alınır.
- Sağlık ve tıbbi iddia yok. Evcil hayvan ve kişisel bakım yazılarında "veterinerinize/uzmanınıza danışın" notu ekle.
- Her yazıda ürünün kime uygun **olmadığını** da yaz.
- Dosya adı: `_posts/YYYY-MM-DD-ascii-slug.md`, tarih bugünün tarihi (Europe/Istanbul).
- Front matter: `layout: post`, `title`, `category`, `summary`.

## Bitirince
`git add -A && git commit -m "Haftalık yazılar: <başlıklar>" && git push`
