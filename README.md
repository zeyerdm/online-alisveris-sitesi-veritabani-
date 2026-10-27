# 🛍️ Nisa Hobi Evim — Online Alışveriş Sitesi Veritabanı

> Bir hobi ürünleri mağazasının çevrimiçi satış ve envanter yönetimi için tasarlanmış ilişkisel SQL Server veritabanı.
>
> *A relational Microsoft SQL Server database designed for the online store and inventory management of a hobby shop.*

![Veritabanı](https://img.shields.io/badge/Veritaban%C4%B1-Microsoft%20SQL%20Server-CC2927?logo=microsoftsqlserver&logoColor=white)
![Araç](https://img.shields.io/badge/Ara%C3%A7-SSMS-5C2D91)

## 📌 Proje Hakkında

Bu proje, **Nisa Hobi Evim** adlı hobi mağazası için ürün kataloğu, müşteri yönetimi, sepet, sipariş, ödeme ve kargo süreçlerini kapsayan bir veritabanı şeması sunar. Tablolar arasındaki bire-çok ve çoka-çok ilişkiler normalizasyon kurallarına uygun şekilde modellenmiştir.

## 🎯 Kapsanan İşlevler

- Ürün ve kategori yönetimi (çoka-çok ilişki)
- Müşteri ve adres kayıtları
- Alışveriş sepeti ve sepetteki ürünler
- Sipariş takibi (tarih, durum, toplam tutar)
- Ödeme kayıtları
- Kargo firmaları ve yönetici hesapları

## 🗄️ Veritabanı Şeması

| Tablo | Açıklama |
| --- | --- |
| `Urunler` | Ürün adı, fiyatı, açıklaması ve modeli |
| `Kategoriler` | Kategori adı ve açıklaması |
| `Urunler_Ve_Kategoriler` | Ürün–kategori çoka-çok ilişki tablosu |
| `Musteriler` | Ad, soyad, e-posta, telefon |
| `Adresler` | İl, ilçe, mahalle, cadde, sokak |
| `Sepet` | Müşterinin alışveriş sepeti |
| `Sepetteki_Urunler` | Sepetteki ürünler ve adetleri |
| `Siparisler` | Sipariş tarihi, durumu ve toplam fiyatı |
| `Odemeler` | Siparişe ait ödeme bilgileri |
| `Admin` | Yönetim paneli kullanıcıları |
| `Kargo_Firmalari` | Kargo firması adı, ücreti ve teslim süresi |

## 📁 Proje Yapısı

```
.
└── database/
    └── NisaHobiEvim-veritabani.rar   # SQL Server yedeği (.bak) ve veritabanı dosyaları (.mdf / .ldf)
```

## 🚀 Kurulum

1. `database/NisaHobiEvim-veritabani.rar` arşivini açın (`NisaHobievim.bak`, `NisaHobievim.mdf`, `NisaHobievim_log.ldf`).
2. SQL Server Management Studio'da **Databases → Restore Database…** adımından `NisaHobievim.bak` dosyasını seçin
   *veya* **Databases → Attach…** ile `NisaHobievim.mdf` dosyasını ekleyin.
3. Tabloları ve ilişkileri **Database Diagrams** bölümünden inceleyebilirsiniz.

## 🛠️ Kullanılan Teknolojiler

- Microsoft SQL Server
- SQL Server Management Studio (SSMS)

## 👩‍💻 Geliştirici

**Zeynep Erdem** — [github.com/zeyerdm](https://github.com/zeyerdm)
