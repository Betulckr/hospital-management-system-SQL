# Hastane Yönetim Sistemi

MS SQL Server ile hazırlanmış bir hastane yönetim sistemi veritabanı projesi. Hastane, doktor, hasta, hasta kabul, randevu, tahlil ve muayene süreçlerini ilişkisel bir veritabanı şeması üzerinde modellemektedir.

> Not: Projedeki tüm hasta/doktor bilgileri (ad, TC No, telefon, e-posta vb.) ders projesi kapsamında oluşturulmuş **kurgusal (fictional) örnek verilerdir**, gerçek kişilere ait değildir.

## Dosyalar

- **SQLproje.sql** — Veritabanı şeması (tablo oluşturma, kısıtlar, ilişkiler) ve örnek veri girişleri
- **Sorgu.sql** — SELECT, UPDATE, LIKE, IN, agregat fonksiyonlar (COUNT, SUM, AVG, MIN, MAX) gibi çeşitli SQL sorgu örnekleri
- **Trigger.sql** — INSERT sonrası çalışan örnek trigger tanımları

## Veritabanı Şeması

| Tablo | Açıklama |
|---|---|
| `TBLHastane` | Hastane bilgileri |
| `TBLDoktor` | Doktor bilgileri (pozisyon, uzmanlık alanı, maaş) |
| `TBLHastalar` | Hasta bilgileri |
| `TBLHastaKabul` | Hasta kabul/şikayet kayıtları |
| `TBLRandevu` | Randevu kayıtları |
| `TBLTahliller` | Tahlil sonuçları |
| `TBLMuayeneler` | Muayene kayıtları |

Tablolar arasında `Hastane_ID`, `Doktor_ID`, `Hasta_ID`, `Hasta_Kabul_ID` üzerinden foreign key ilişkileri kurulmuştur.

## Kurulum

1. MS SQL Server (veya SQL Server Management Studio) üzerinde `Hastane` adında bir veritabanı oluşturun.
2. `SQLproje.sql` dosyasını çalıştırarak şemayı ve örnek verileri oluşturun.
3. `Sorgu.sql` içindeki örnek sorguları inceleyerek veritabanı üzerinde deneyler yapabilirsiniz.
