# ⚡ Dönüştürücü 1.0

Sıfır bağımlılık, tek dosya dosya dönüştürücü. GitHub Pages ile saniyeler içinde yayınla.

## 🔄 Desteklenen Dönüşümler

| Kaynak | Hedef | Açıklama |
|--------|-------|----------|
| XLSX   | PDF   | Excel tabloları → görsel belge |
| DOCX   | PDF   | Word belgeleri → taşınabilir PDF |
| PDF    | XLSX  | PDF tabloları → Excel'e aktar |
| PDF    | DOCX  | PDF metni → düzenlenebilir Word |
| CSV    | XLSX  | Ham veri → formatlanmış Excel |
| XLSX   | CSV   | Excel → evrensel CSV (UTF-8 BOM) |
| TXT    | DOCX  | Düz metin → Word belgesi |
| DOCX   | TXT   | Word → sade metin çıkarımı |

## ✨ Özellikler

- **Türkçe karakter desteği** — ş, ı, ğ, ç, ö, ü tam desteklenir (UTF-8, Windows-1254, ISO-8859-9 otomatik algılama)
- **Akıllı hata konsolu** — hata türü, satır numarası, stack trace + tek tıkla kopyala
- **Sıfır kurulum** — sadece `index.html`, hiçbir paket/bağımlılık yok
- **Sürükle-bırak** dosya yükleme
- **Canlı log konsolu** — işlem adımlarını anlık izle
- **Global hata yakalayıcı** — beklenmeyen hatalar da yakalanır
- **Duyarlı tasarım** — mobil ve masaüstü uyumlu

## 🚀 GitHub Pages'e Yayınlama

### 1. Repo oluştur

```bash
git init donusturucu
cd donusturucu
cp /indirilen/index.html .
git add index.html README.md
git commit -m "feat: Donusturucu v1.0"
git remote add origin https://github.com/KULLANICI_ADI/donusturucu.git
git push -u origin main
```

### 2. GitHub Pages'i aktifleştir

- Repo → **Settings** → **Pages**
- Source: `Deploy from a branch` → `main` / `/ (root)`
- **Save** — birkaç dakika içinde yayında!

### Yayın URL'si

```
https://KULLANICI_ADI.github.io/donusturucu/
```

## 🧩 API Gereksinimleri

| Dönüşüm | Gereksinim |
|---------|-----------|
| CSV ↔ XLSX | Offline, API gerekmez |
| TXT ↔ DOCX | Offline, API gerekmez |
| XLSX/DOCX ↔ PDF | Claude API (otomatik kullanılır) |

## 🐛 Hata Bildirimi

1. Uygulamada ⛔ HATA paneli açıldığında **📋 Kopyala** butonuna tıkla
2. Bu repoyu fork et, Issue aç, kopyalanan metni yapıştır

## 📄 Lisans

MIT License
