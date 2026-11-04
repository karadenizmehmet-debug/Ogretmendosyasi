# Öğretmen Dosyası 2026-2027

Karahüyük Ali Akkanat Ortaokulu, Bilişim Teknolojileri ve Yazılım öğretmen dosyası.
Mehmet Karadeniz, 2026-2027

## Yapı
- `index.html` — dosyanın tamamı (tek sayfa, sayfa sayfa çevrilir).
- `gorseller/` — varsayılan görseller (Atatürk portresi, çalışma takvimi).
- `firestore.rules` — Firebase Firestore kuralları (yalnızca sahibi okur ve yazar).

## Veriler (Firebase projesi: ogretmendosyam)
- `belgeler` koleksiyonu — sayfalara eklenen Drive bağlantıları.
- `gorseller/<anahtar>` — sayfadan yüklenen görseller (küçültülmüş JPEG, base64).
  Firestore'daki görsel, `gorseller/` klasöründeki varsayılanın yerine geçer.

Firebase Storage kullanılmaz (ücretsiz Spark planında yok).
