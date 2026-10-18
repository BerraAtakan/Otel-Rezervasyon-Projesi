
# 🏨 Otel Rezervasyon ve Konaklama Yönetim Sistemi

Modern bir otel işletmesinin rezervasyon ve konaklama süreçlerini dijital ortamda yönetmek amacıyla geliştirilen bu proje, **Veritabanı Yönetim Sistemleri dersi** kapsamında hazırlanmaktadır.

Projenin temel amacı; misafirlerin rezervasyon işlemlerini kolaylaştırmak, otel personelinin operasyonlarını düzenlemek ve yöneticilerin oda, fiyatlandırma, ödeme ve raporlama süreçlerini tek bir sistem üzerinden yönetmesini sağlamaktır.

## 👥 Proje Ekibi

| Ad Soyad | Öğrenci Numarası |
|---|---|
| Berra Atakan | 455090 |
| Beyan Alalı | 458136 |

## 🛠️ Kullanılan Teknolojiler

- **Backend:** Python, Django
- **Veritabanı:** MySQL
- **Frontend:** HTML, CSS ve JavaScript (planlanan)
- **Versiyon Kontrolü:** Git ve GitHub

> **Teknoloji Notu:** Yukarıda belirtilen teknolojiler mevcut proje planını yansıtmaktadır. Geliştirme sürecinde ihtiyaçlara, teknik gereksinimlere ve ekip kararlarına bağlı olarak kullanılan teknolojilerde ve araçlarda değişiklik yapılabilir.

## ✨ Temel Özellikler

### 🧑‍💼 Misafir İşlemleri

- Kullanıcı kayıt ve giriş işlemleri
- Tarih aralığına ve oda tipine göre boş oda arama
- Rezervasyon oluşturma ve iptal etme
- Geçmiş konaklamaları görüntüleme

### 🛎️ Resepsiyon İşlemleri

- Günlük giriş ve çıkış listelerini görüntüleme
- Check-in ve check-out işlemlerini gerçekleştirme
- Konaklamaya ek hizmetler ekleme
- Ödeme alma ve konaklama hesabını yönetme

### ⚙️ Yönetici İşlemleri

- Oda ve oda tipi yönetimi
- Sezonluk fiyatlandırma işlemleri
- Ek hizmet ve personel yönetimi
- Aylık doluluk oranı ve gelir raporlarını görüntüleme

## 🗄️ Veritabanı Tasarımı

Projenin veritabanı, ilişkisel veritabanı tasarım ilkelerine uygun olarak ve en az üçüncü normal form (3NF) hedeflenerek oluşturulacaktır.

Planlanan temel tablolar şunlardır:

- OdaTipi
- Oda
- SezonFiyati
- Misafir
- Kullanici
- Personel
- Rezervasyon
- Konaklama
- EkHizmet
- KonaklamaHizmeti
- Odeme
- TemizlikKaydi
- IslemLog

Veritabanı tasarımı kapsamında ER diyagramı, tablolar arası ilişkiler ve gerekli SQL betikleri hazırlanacaktır.

## 🔍 Uygulanacak Veritabanı Özellikleri

Proje kapsamında aşağıdaki veritabanı kavramlarının uygulanması hedeflenmektedir:

- **CRUD:** Veri ekleme, okuma, güncelleme ve silme işlemleri
- **JOIN ve Gruplama:** İlişkili tablolardan veri alma ve raporlama
- **TRIGGER:** Rezervasyon çakışmalarını önleme, oda durumlarını güncelleme ve işlem geçmişini kaydetme
- **STORED PROCEDURE:** Boş oda arama, konaklama tutarı hesaplama ve aylık raporlama
- **VIEW:** Günlük giriş-çıkış listeleri ve oda durumlarının görüntülenmesi
- **TRANSACTION:** Check-out ve ödeme işlemlerinin tutarlı biçimde yürütülmesi
- **İndeksleme:** Sık sorgulanan alanlarda sorgu performansının iyileştirilmesi
- **Tarih Aralığı Kontrolü:** Aynı odanın çakışan tarihlerde birden fazla rezervasyona verilmesinin engellenmesi

## 🔐 API ve Güvenlik

Backend tarafında REST API uç noktalarının geliştirilmesi, katmanlı mimarinin uygulanması ve kullanıcı rollerine göre yetkilendirme yapılması planlanmaktadır.

Misafir, resepsiyon personeli ve yönetici rolleri için farklı erişim izinleri tanımlanacaktır. Ayrıca JWT tabanlı kimlik doğrulama mekanizmasının uygulanması hedeflenmektedir.

## 🧪 Test ve Raporlama

Projenin test ve değerlendirme aşamalarında:

- En az 20 oda, 50 misafir ve 200 rezervasyon içeren örnek veriler hazırlanacaktır.
- API uç noktaları Postman veya Swagger ile test edilecektir.
- Rezervasyon çakışması ve başarısız işlemlerde geri alma (ROLLBACK) senaryoları test edilecektir.
- İndeksli ve indekssiz sorguların performansları karşılaştırılacaktır.
- ER diyagramı, test senaryoları ve proje raporu hazırlanacaktır.

## 📁 Proje İçeriği

Geliştirme süreci boyunca bu GitHub deposunda aşağıdaki dosyaların yer alması planlanmaktadır:

- Django kaynak kodları
- Veritabanı oluşturma ve örnek veri SQL betikleri
- ER diyagramı
- Test senaryoları ve API test koleksiyonu
- Proje dokümantasyonu ve raporu

## 🎯 Projenin Amacı

Bu proje ile ilişkisel veritabanı tasarımı, normalizasyon, SQL programlama, backend geliştirme, API tasarımı ve kullanıcı arayüzü geliştirme konularında uygulamalı deneyim kazanılması amaçlanmaktadır.

---

**Proje Durumu:** Geliştirme aşamasında 🚧

