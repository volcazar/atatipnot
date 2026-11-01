# Atatürk Üniversitesi Tıp Fakültesi Notları Arşivi

Atatürk Üniversitesi Tıp Fakültesi kurumsal renkleriyle (`#0B1934` Derin Lacivert & `#C5A059` / `#D4AF37` Altın Sarısı) tasarlanmış, slaytlar ne notlar arşivi.

## Dosya Yapısı

- `index.html`: Tek sayfalık (Single Page) kurumsal arayüz.
- `stajlar.json`: Tüm stajların isimlerini, kısaltmalarını (`ATA4...` / `ATA5...`), sürelerini, `slaytLink` ve `notLink` Google Drive bağlantılarını barındıran veri dosyası.

## Staj Linkleri Nasıl Güncellenir?

Kod bilgisine ihtiyaç duymadan sadece **`stajlar.json`** dosyasını düzenleyerek `slaytLink` ve `notLink` alanlarını güncelleyebilirsiniz:

```json
{
  "id": "d5-ortopedi",
  "donem": 5,
  "ad": "Ortopedi ve Travmatoloji",
  "kisaltma": "ATA5ORT",
  "sure": "3 Hafta",
  "ikon": "bone",
  "slaytLink": "https://drive.google.com/drive/folders/YENI_SLAYT_LINKI",
  "notLink": "https://drive.google.com/drive/folders/YENI_NOT_LINKI",
  "etiketler": ["Ortopedi", "Travmatoloji", "ORT"]
}
```

## Dosya İsimlendirme Sistemi

- **Format:** `ATA[Sınıf][Staj]-[Tür] ([Sene]) [[Yazar/Editör]]` (Örnek: `ATA5ORT-Ço (23-26) [ASG]`)
- **ATA:** Atatürk Üniversitesi Tıp Fakültesi
- **Sınıf:** `4` (4. sınıf), `5` (5. sınıf)
- **Staj Kısaltmaları:** `BC` (Beyin cerrahisi), `D` (Dermatoloji), `EH` (Enfeksiyon), `G` (Göz), `GH` (Göğüs), `KAR` (Kardiyoloji), `KBB` (Kulak burun boğaz), `KDC` (Kalp damar cerrahisi), `NÖR` (Nöroloji), `ORT` (Ortopedi), `RSH` (Psikiyatri), `Ü` (Üroloji) vb.
- **Tür:** `Ç` (Sözlü çıkmışı), `Ço` (Cevaplı sözlü), `Çx` (Cevapsız sözlü), `Y` (Yazılı çıkmışları), `Yo` (Cevaplı yazılı), `Yx` (Cevapsız yazılı), `S` (Slayt), `N` (Not), `Z` (Anamnez)
- **Sene/Grup:** `(23-26)`, `(23-24)` vb.
- **Editör/Kısaltmalar:** `[ASG]`, `[EBA]`, `[FK]`, `[RÖ]`, `[EH]`, `[G]` vb.
