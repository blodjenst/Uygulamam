# Ne Açsam

Oyun, müzik ya da film seçip birkaç soruya cevap verince sana uygun öneriler çıkaran tek sayfalık site. Telefona ya da bilgisayara uygulama gibi kurulabilir (PWA).

## Dosyalar

- `index.html`: site (tasarım ve listeler içinde)
- `manifest.json`: uygulama adı, renkler, başlangıç adresi, görüntüleme modu ve ikonlar
- `sw.js`: service worker, siteyi çevrim dışı da açılır yapar
- `icons/`: uygulama ikonları (192 ve 512 piksel, maskable ve Apple ikonu, SVG)

## GitHub'a yükleme ve yayınlama

1. GitHub'da yeni bir depo oluştur (örneğin `ne-acsam`).
2. Bu klasördeki tüm dosyaları ve `icons` klasörünü deponun ana dizinine yükle. `index.html` ana dizinde, yani en üstte olmalı.
3. Depoda **Settings > Pages** bölümüne git. **Source** olarak **Deploy from a branch** seç, dalı `main`, klasörü `/ (root)` yap ve kaydet.
4. Birkaç dakika sonra site `https://kullaniciadin.github.io/ne-acsam/` adresinde açılır.

Dosya yollarının hepsi göreli olduğu için site bir alt klasörde (`/ne-acsam/`) de, kendi alan adında da çalışır.

## Kurulum denemesi

- Chrome ve Edge: adres çubuğunda "Yükle" simgesi çıkar.
- Android: menüden "Ana ekrana ekle".
- iPhone (Safari): Paylaş, ardından "Ana Ekrana Ekle".

PWA olarak kurulması için sitenin HTTPS ile açılması gerekir. GitHub Pages bunu kendiliğinden sağlar.

## Siteyi güncellersen

`sw.js` içindeki `CACHE` değerini değiştir (örneğin `ne-acsam-v1` yerine `ne-acsam-v2`). Böylece kurulu uygulamaların eski kopyası silinir ve yeni sürüm yüklenir.

## Not

Film IMDb puanları ve Steam etiketleri elle girilmiş yaklaşık değerlerdir ve zamanla değişir.
