# Babalar Günü Resim Sergisi — bitirme & yayınlama

Etkileşimli bir hediye: açılış kartı → Porsche ile sür → 22 fotoğraflık bir
duvarda gez → parlayan 10 çerçeve mektupları, listeyi ve sözleri açar →
radyo "Bana Bir Masal Anlat Baba"yı çalar.

**22 fotoğrafın hepsi artık `index.html` dosyasının İÇİNE gömülü.** Yani fotoğraflar
her yerde görünür ve yayınlamak için tek dosya yeterli. Sadece metinleri
düzenliyorsun: `index.html` içindeki en üstteki CONFIG bloğu.

---

## 1. Dosyalar

```
fathers-day-gift/
├── index.html        ← TÜM site + 22 fotoğraf gömülü (CONFIG'i düzenle)
├── README.md
└── images/           ← fotoğrafların kaynak halleri (yayın için şart değil)
    ├── photo1.jpg ... photo22.jpg
    └── song.mp3      ← (opsiyonel) radyonun çaldığı şarkı
```

---

## 2. Doldurman gerekenler (hepsi CONFIG'de)

- `meName`, `sisterName`, `dadName` — isimler
- 7 adet `kind:"quote"` çerçevesinde `quote:"..."` — tatlı babalık sözlerin
- `letterMe.paragraphs` — senin mektubun
- `letterSister.paragraphs` — kız kardeşinin mektubu
- `list.items` — ondan öğrendiklerin
- Her çerçevenin `caption` (altyazı) ve `kind` (tür) alanını istediğin gibi
  değiştirebilir, sırayı değiştirebilirsin.

**Şarkı (opsiyonel):** `images/song.mp3` koy ve yayınlarken `index.html` ile
birlikte `images` klasörünü de yükle. Radyoya dokununca çalar, tekrar dokununca
durur.

---

## 3. Önizleme

`index.html`'e çift tıkla — tarayıcıda açılır, fotoğraflar görünür (gömülü
oldukları için klasöre gerek yok). Sadece mp3 için gerçek bir sunucu (GitHub
Pages) gerekir.

---

## 4. GitHub Pages ile ücretsiz yayınla

1. github.com → giriş → **New repository** → ad: `baba` → **Public** → Create.
2. **Add file → Upload files** → `index.html`'i sürükle. (Şarkı istiyorsan
   `images` klasörünü `song.mp3` ile birlikte de yükle.) Commit.
3. **Settings → Pages** → Source: **Deploy from a branch**, Branch: **main**,
   klasör **/(root)** → Save.
4. ~1 dakika sonra `https://KULLANICIADIN.github.io/baba/` bağlantısı çıkar.
   Babana gönder.

---

## 5. Notlar
- Porsche, Türk evi, radyo, güneş ve bulutlar `index.html` içinde SVG çizim.
- Fotoğrafı değiştirmek istersen: `images/` içindekini değiştir, sonra bana
  söyle yeniden gömeyim (gömülü oldukları için elle değiştirmek zor).
- Telefonda çalışır ve "hareketi azalt" ayarına saygı gösterir.
