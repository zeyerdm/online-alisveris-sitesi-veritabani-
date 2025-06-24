Nisa Hobi Evim SQL Veritabanı Projesi
Bu depo, Nisa Hobi Evim'in çevrimiçi satış ve envanter yönetimi ihtiyaçları için tasarlanmış SQL Server veritabanı projesini içermektedir.
Proje, ürün kategorizasyonu, müşteri yönetimi, sipariş takibi ve ödeme işlemlerini kapsayan bir veritabanı şeması sunar.

🎯 Proje Amacı
Bu projenin temel amacı, Nisa Hobi Evim için aşağıdaki işlevleri destekleyecek temel bir veritabanı altyapısı oluşturmaktır:

Ürün ve kategori bilgilerinin yönetimi
Müşteri kayıtlarının ve adres bilgilerinin saklanması
Siparişlerin detaylı takibi ve yönetimi
Ödeme bilgilerinin güvenli bir şekilde işlenmesi
Kargo firmaları ve yönetici hesaplarının entegrasyonu

🛠️ Kullanılan Teknolojiler
Veritabanı Sistemi: Microsoft SQL Server
Veritabanı Tasarım Aracı: SQL Server Management Studio (SSMS)

📄 Veritabanı Şeması
Projenin ana veritabanı şeması aşağıdaki varlıkları ve aralarındaki ilişkileri içermektedir:

Urunler: Ürün bilgilerini (ad, fiyat, açıklama, model) tutar.
Kategoriler: Ürün kategorilerini (ad, açıklama) tanımlar.
Urunler_Ve_Kategoriler: Ürünler ve kategoriler arasındaki çok-çok ilişkiyi yönetir.
Musteriler: Müşteri bilgilerini (ad, soyad, e-posta, telefon) saklar.
Adresler: Müşterilerin adres bilgilerini (il, ilçe, mahalle, cadde, sokak) tutar.
Sepet: Müşterilerin alışveriş sepeti bilgilerini içerir.
Sepetteki_Urunler: Sepetlerdeki ürünlerin adet bilgilerini tutar.
Siparisler: Müşterilerin verdiği siparişlerin genel bilgilerini (tarih, durum, toplam fiyat) kaydeder.
Odemeler: Siparişlere ait ödeme bilgilerini (kart numarası, son kullanma tarihi) içerir.
Admin: Yönetim paneli erişimi için yönetici hesaplarını tutar.
Kargo_Firmalari: Kargo firmalarının bilgilerini (ad, ücret, teslim süresi) saklar.
Görsel Şema:
Projenin görsel veritabanı şeması için lütfen Diagrams/image_a04802.png dosyasına bakınız.

