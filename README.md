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

## Sürümler
- **v1.6** — Telefonda da bilgisayardaki gibi halkalı klasör görünümü; parmakla sayfa çevirme; her zaman açık renkli kâğıt.
- **v1.5** — claude.ai'daki ilk sürümün tasarımı: lacivert klasör, renkli bölüm ayraçları, sade beyaz sayfalar.
- **v1.4** — Gerçek A4 düzeni: sayfa içi kaydırma yok; belgeler kendi sayfasında; belge ekleme penceresi.
- **v1.3** — Yeni tasarım: 13 bölüm, numaralı bölüm kapakları, otomatik işaretlenen kutucuklar, Türk Bayrağı sayfası.
- **v1.2** — Drive belgeleri sayfa içinde önizlenir.
- **v1.1** — Dosyayı görmek için giriş zorunlu; Firestore yalnızca sahibine açık.
- **v1.0** — İlk sürüm: Firebase bağlantılı, sayfa sayfa çevrilen öğretmen dosyası.

Her değişiklikte `index.html` içindeki `VERSION` artırılır ve buraya satır eklenir.
