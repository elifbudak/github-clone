# GitHub Profil Sayfası Klonu

HTML, CSS ve SCSS kullanılarak oluşturulmuş bir GitHub profil sayfası arayüz klonu.

## 📸 Önizleme

Proje, GitHub'ın kullanıcı profil sayfasını taklit eden statik bir web arayüzüdür. Header navigasyonu, kullanıcı bilgi kartı ve sabitlenmiş proje kartlarını içerir.

## 🚀 Özellikler

- GitHub tarzı üst navigasyon çubuğu (arama, bildirim, menü ikonları)
- Kullanıcı profil kartı (avatar, isim, kullanıcı adı, açıklama)
- Sabitlenmiş repo kartları (proje adı, dil bilgisi, ikon)
- SVG sprite ile inline ikonlar
- SCSS ile modüler stil yapısı
- Google Fonts entegrasyonu (Maven Pro)

## 🗂️ Dosya Yapısı

```
├── index.html           # Ana HTML dosyası
├── main.css             # Derlenmiş CSS çıktısı
├── main.css.map         # Source map dosyası
└── scss/
    ├── main.scss        # Ana SCSS giriş noktası (tüm parçaları import eder)
    ├── _normalize.scss  # Tarayıcı sıfırlama stilleri
    ├── _formalize.scss  # Temel form ve genel sıfırlama stilleri
    ├── _variables.scss  # SCSS değişkenleri (renkler, fontlar)
    ├── _header.scss     # Header bileşeni stilleri
    └── _content.scss    # Ana içerik ve proje kartı stilleri
```

## 🛠️ Kullanılan Teknolojiler

| Teknoloji | Amaç |
|-----------|------|
| HTML5 | Sayfa yapısı |
| SCSS | Modüler stil yazımı |
| CSS3 | Derlenmiş stiller |
| Google Fonts | Maven Pro yazı tipi |
| SVG Sprite | İkon sistemi |

## ⚙️ Kurulum ve Kullanım

### Projeyi Görüntüleme

`index.html` dosyasını doğrudan tarayıcıda açarak projeyi çalıştırabilirsiniz.

### SCSS Derleme

SCSS dosyalarını düzenledikten sonra CSS'e derlemek için:

```bash
# sass CLI ile
sass scss/main.scss main.css

# watch modunda (değişiklikleri otomatik derler)
sass --watch scss/main.scss:main.css
```

> **Not:** Sass'ın yüklü olması gerekir. `npm install -g sass` komutuyla kurabilirsiniz.

## 🎨 SCSS Değişkenleri

`_variables.scss` içinde tanımlanan değişkenler:

```scss
$header-bg: #24292e;          // Header arka plan rengi
$my-font: 'Maven Pro', sans-serif;  // Genel yazı tipi
```

## 📌 Notlar

- Proje tamamen statik olup herhangi bir JavaScript framework'ü kullanmamaktadır.
- Responsive tasarım henüz eklenmemiştir; masaüstü görünüm için optimize edilmiştir.
- Avatar görseli bir GitHub hesabının gerçek profil fotoğrafından çekilmektedir.
