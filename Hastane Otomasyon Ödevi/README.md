# 🏥 Hastane Otomasyonu Veri Tabanı Tasarımı

Bu proje, bir hastane otomasyonu prototipi için tasarlanmış ilişkisel veri tabanı yapısını ve Varlık-İlişki (ER) modelini içermektedir.

---

## 📐 Chen Gösterimi ER Diyagramı

Sistem tasarımı **Chen Gösterimi** (Chen Notation) prensiplerine uygun olarak kurgulanmıştır:

- **Varlık Kümeleri (Entities):** Dikdörtgen simgeleri ile temsil edilir (`Doktor`, `Poliklinik`, `Hasta`, `Servis`, `Hemşire`, `Laboratuvar`, `Tahlil`).
- **Öznitelikler (Attributes):** Elips simgeleri ile gösterilir; birincil anahtarların (Primary Key) altı çizilidir.
- **İlişkiler (Relationships):** Baklava (eşkenar dörtgen) simgeleri ile ifade edilir.
- **Kardinalite (Derecelendirme):**
  - **1:N İlişkiler:** `Poliklinik` ➔ `Doktor`, `Poliklinik` ➔ `Servis`, `Servis` ➔ `Hemşire`, `Laboratuvar` ➔ `Tahlil`
  - **N:M İlişkiler:** `Hasta` ➔ `Poliklinik` (Muayene) ve `Hasta` ➔ `Doktor` ➔ `Tahlil` (Tahlil İstem)

---

## 🗄️ Veri Tabanı Tablo Yapıları

1. **Poliklinik:** Hastanedeki polikliniklerin temel kimlik, ad ve kat bilgilerini saklar.
2. **Doktor:** Doktorların kişisel bilgilerini, uzmanlık alanlarını ve çalıştıkları polikliniği kaydeder.
3. **Servis:** Hastane servislerinin adını, kat konumunu ve bağlı olduğu polikliniği tutar.
4. **Hemşire:** Hemşirelerin kimlik bilgilerini ve görevli oldukları servisi takip eder.
5. **Laboratuvar:** Tahlillerin yapıldığı laboratuvar birimlerinin adını ve kat bilgilerini saklar.
6. **Tahlil:** Hastanede uygulanan tahlil türlerini, açıklamalarını ve ilgili laboratuvar birimini belirtir.
7. **Hasta:** Hastaların sistemdeki temel kimlik, ad, soyad ve T.C. Kimlik No kayıtlarını tutar.
8. **Muayene:** Hastaların polikliniklerdeki muayene süreçlerini çözen N:M ilişki tablosudur.
9. **Hasta Tahlil:** Hangi hastaya, hangi doktor tarafından, hangi tahlilin istendiğini bağlayan N:M ilişki tablosudur.

---

## 👥 Hazırlayanlar

- **Berra Atakan** - 455090
- **Beyan Alalı** - 458136
- ---

> **Not:** Ödevi 17.10.2026'da ayrı bir repo olarak kaydetmiştik ama yanlış yaptığımızı anlayınca ödevi bir daha gözden geçirip bu repoya attık.
