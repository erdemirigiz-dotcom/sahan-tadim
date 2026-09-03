# SAHAN — İlham Turu

Tarih: 2026-09-03. Konu: tava ciğeri fine-dining usulüyle sunan, boğaz kıyısı
havasında lüks/sofistike bir tadım mutfağı (kurgu marka SAHAN).

## Yöntem
- Ağ: telefon TR exit node, `socks5://127.0.0.1:1055` (bu makinenin normal çıkışı
  Romanya/M247 olduğu için Cloudflare 403 veriyor, proxy zorunlu).
- İndeks **yeniden taranmadı** — hazır kaynak `~/vyron/site-fabrikasi/data/
  godly-indeks.json` (**471 kayıt**, 03.09 kurulan aynı envanter, astro-kamp'ın
  da kullandığı kaynak). Bu turda astro-kamp'ın seçtiği 6 site (Astro Dither,
  21 Hrs on the Moon, White Desert, Tandjung Sari, The Pop-Up Hotel, Tengile
  MalaMala) **bilinçli olarak tekrar seçilmedi** — kategori/etiket araması
  `Food & Drink` / `Hotel / Restaurant` / `Luxury` / `Editorial` alanlarında
  farklı 6 site verdi.
- Awwwards kayıtlarının `url` alanı çoğu zaman awwwards.com'daki vitrin sayfası
  (gerçek site değil) — 3 kayıtta (Caffè Gilli, Moncalisse, Palazzo Sogni,
  De Groene Afslag) gerçek site adresi awwwards sayfasının HTML'i içinden
  (`curl` + proxy, harici link çıkarımı) bulundu; awwwards linki KULLANILMADI,
  gerçek canlı site ekran görüntüsü alındı.
- Masaüstü (1440×900, tam sayfa) + mobil (390×844) ekran görüntüsü, JPEG q70,
  `~/vyron/site-fabrikasi/data/ilham-ekranlar/sahan-*.jpg`.
- Kaba analiz Claude'da YAPILMADI — bedava `gemini-2.5-flash` (vision), anahtar
  `~/.hermes/.env`'den okundu, ekrana hiç basılmadı. Ham model çıktısı bu dosyaya
  doğrudan dökülmedi, kısaltılıp düzenlendi.
- Gerçek font aileleri `getComputedStyle` ile DOM'dan doğrulandı (Gemini'nin
  görsel tahminiyle YETİNİLMEDİ — aşağıda her sitede "Gerçek font (DOM)" satırı
  ayrı, Gemini'nin "tipografi izlenimi" görsel bir yorumdur).

---

## 1) Postevand
**URL:** https://postevand.com/ · **Kategori:** Food & Drink (recent.design —
Minimal, Clean, 3D, Large Type, Muted)
**Ekran:** `data/ilham-ekranlar/sahan-postevand-masaustu.jpg` / `-mobil.jpg`
**Gerçek font (DOM):** `"Nimbus Sans D OT", "Helvetica Neue", Helvetica, Arial, sans-serif`

- **Düzen:** Ferah, bol boşluklu, tek ürün etrafında kurulmuş hiyerarşik hero;
  sağa hizalı ince gezinme.
- **Tipografi (izlenim):** Logo/başlıkta kalın geometrik sans-serif, gövdede
  ince/okunaklı sans — marka odaklı ve çağdaş.
- **Renk:** gökyüzü mavisi `#7AB1D8`, açık bulut mavisi `#C2DAEB`, koyu metin
  `#1A1A1A`, beyaz `#F7F7F7`/`#FFFFFF`.
- **Hareket izlenimi:** hover'da ince renk/altçizgi değişimi, hero'da hafif
  paralaks beklentisi.
- **İmza öğe:** ürünün (şişe) gökyüzü fonuyla bütünleşmiş, marka adının devasa
  ama sakin tipografisi.
- **Kopyalanmayacak klişe:** newsletter pop-up'ı — SAHAN'da form dışında hiçbir
  bloke edici pop-up olmayacak.

## 2) Caffè Gilli
**URL:** https://www.caffegilli.com/en · **Kategori:** Food & Drink (awwwards —
Scrolling, Photo & Video, Animation; gerçek marka: 1733'ten beri Floransa'da
tarihi kahve/pasticceria)
**Ekran:** `data/ilham-ekranlar/sahan-caffe-gilli-masaustu.jpg` / `-mobil.jpg`
**Gerçek font (DOM):** başlık `greycliff-cf, sans-serif`, gövde `Cosen, sans-serif`

- **Düzen:** Tam genişlik görsel blokları dikey akış, ortalanmış logo + sol/sağ
  ince menü.
- **Tipografi (izlenim):** klasik/zarif serif logo + modern sans gövde —
  gelenek/modernlik kontrastı.
- **Renk:** beyaz `#FFFFFF`, koyu lacivert-füme `#1A233A`, altın-bej vurgu
  `#D9C48B`, açık gri `#F5F5F5`.
- **Hareket izlenimi:** hero'da video/slayt, scroll'da yumuşak fade-in.
- **İmza öğe:** markanın karakteristik klasik logo tipografisi.
- **Kopyalanmayacak klişe:** standart çerez onay banner'ı.

## 3) Moncalisse
**URL:** https://www.moncalisse.com/en · **Kategori:** Food & Drink / şarap
(awwwards — Clean, Navigation Menu, Photo & Video)
**Ekran:** `data/ilham-ekranlar/sahan-moncalisse-masaustu.jpg` / `-mobil.jpg`
**Gerçek font (DOM):** başlık `termina, sans-serif`, gövde `canto, serif`

- **Düzen:** Geniş boşluklu, asimetrik; metin blokları solda, yaş doğrulama
  modalı açılışta tam ekran.
- **Tipografi (izlenim):** ince/uzun zarif serif başlık + sade sans gövde —
  lüks/klasik.
- **Renk:** krem `#F9F7F1`, koyu kahve-gri metin `#4D4D4D`, bordo/şarap vurgu
  `#7C2A3C`, muted yeşil-gri modal `#6B6D66`.
- **Hareket izlenimi:** butonlarda ton geçişi, modallar yumuşak açılış.
- **İmza öğe:** zarif serif logo + havadar minimalist sayfa düzeni.
- **Kopyalanmayacak klişe:** bulanıklaştırılmış jenerik manzara hero fonu +
  yaş doğrulama pop-up'ı — SAHAN'da hero gerçek/net bir tabak/mekân fotoğrafı
  olacak, sahte doğa fonu yok.

## 4) Palazzo Sogni
**URL:** https://www.palazzosogni.com · **Kategori:** Hotel/Restaurant (awwwards
— Colorful, Scrolling, Typography, Footer Design)
**Ekran:** `data/ilham-ekranlar/sahan-palazzo-sogni-masaustu.jpg` / `-mobil.jpg`
**Gerçek font (DOM):** başlık `Sogo`, gövde `"Times New Roman"`

- **Düzen:** dikey bloklar, bol beyaz boşluk, ortalanmış/simetrik içerik.
- **Tipografi (izlenim):** klasik serif başlık + modern sans gövde — sofistike.
- **Renk:** krem `#F7F5F0`, soluk mavi-gri `#DDE5EA`, metalik altın `#A78C6E`,
  koyu lacivert metin `#3F5868`.
- **Hareket izlenimi:** bölümler arası yumuşak geçiş, galeri hover vurgusu.
- **İmza öğe:** tekrarlayan kavisli üst kenarlı geometrik görsel maskesi/ayırıcı.
- **Kopyalanmayacak klişe:** tam ekran açılış pop-up'ı + "scroll down" oku —
  SAHAN doğrudan içerikle açılacak.

## 5) De Groene Afslag
**URL:** https://www.degroeneafslag.nl/ · **Kategori:** Hotel/Restaurant
(awwwards — Webflow, Animation, Colorful, Copy design)
**Ekran:** `data/ilham-ekranlar/sahan-groene-afslag-masaustu.jpg` / `-mobil.jpg`
**Gerçek font (DOM):** `"Helvetica Neue", Arial, sans-serif` (başlıklarda kalın
kesim) + ikincil `"Times New Roman"` serif vurgu

- **Düzen:** geniş başlık alanı + görsel domine, orta kısımda nefes boşluğu.
- **Tipografi (izlenim):** kalın geniş-aralıklı modern sans başlık + zarif serif
  ikincil vurgu kontrastı.
- **Renk:** yeşil `#209559`, zeytin yeşili `#6F6D38`, magenta vurgu `#EC008C`,
  bej-gri zemin `#EDEBE8`, koyu gri metin `#333333`.
- **Hareket izlenimi:** düğme hover'ları, video oynat tetiği, içerik kaydırıcı okları.
- **İmza öğe:** başlık kelimesinin bir bölümünün ters/dikey konumlandırılması —
  tipografik oyun.
- **Kopyalanmayacak klişe:** bağlamdan kopuk "ilham" ikon/slogan köşesi (roket +
  "fly me to the moon" gibi) — SAHAN'da her öğe menü/mekân/rezervasyonla
  doğrudan ilişkili olacak, dekoratif/bağlamsız süs yok.

## 6) Schemas of Uncertainty
**URL:** https://schemasofuncertainty.com/ · **Kategori:** Editorial
(recent.design — Typographic, Experimental, Animation, Black & White)
**Ekran:** `data/ilham-ekranlar/sahan-schemas-uncertainty-masaustu.jpg` / `-mobil.jpg`
**Gerçek font (DOM):** `"Century Schoolbook"`

- **Düzen:** metin ağırlıklı, çok sütunlu grid; her sütun kendi başlık/önizleme
  bloğu.
- **Tipografi (izlenim):** keskin modern sans başlık + klasik okunaklı serif
  gövde — akademik/ciddi.
- **Renk:** beyaz `#FFFFFF`, siyah `#000000`, bordo etiket `#A00000`, açık gri
  çizgiler `#CCCCCC`.
- **Hareket izlenimi:** statik/sabit yapı, sade hover altçizgisi.
- **İmza öğe:** yoğun, grid tabanlı akademik dergi/gazete sütun düzeni.
- **Kopyalanmayacak klişe:** yok — bilinçli minimalist, jenerik süs içermiyor
  (bu turun tek "klişesiz" örneği).

---

## SAHAN İÇİN ÇIKARIM

1. **Bol beyaz boşluk + koyu blok kontrastı alınacak** — Postevand ve Palazzo
   Sogni'de içerik ferah, nefes alan bloklar halinde; SAHAN'da da zemin ağırlıklı
   açık (`--tuz #F2F0EB`) olacak, hero + tadım şeridi bilinçli olarak TAM
   GENİŞLİK koyu (`--is #1C1A17`) bir kontrast bloğu kuracak — Caffè Gilli'nin
   koyu lacivert + altın-bej vurgu ikilisi bu kontrastın nasıl "ucuz" değil
   "zengin" durabileceğini gösteriyor.
2. **Serif başlık + sade sans gövde kontrastı alınacak, ama didone değil** —
   Moncalisse ve Palazzo Sogni ikisi de zarif serif başlık kullanıyor; SAHAN'da
   Gambetta (hümanist kaligrafik serif) bu rolü üstlenecek, ama frontend-design
   skill'inin ölçtüğü "yüksek kontrast didone serif + krem + terrakota" AI
   varsayılanına düşülmeyecek — Gambetta yumuşak/kaligrafik, kontrast düşük.
3. **Tek tipografik oyun/detay imza olarak alınacak** — De Groene Afslag'daki
   kelime-ters-çevirme numarasının KENDİSİ değil, mantığı: SAHAN'da imza öğe
   TADIM ŞERİDİ'nin kendisi olacak (kurs numarası + tabak fotoğrafı + bakır
   ilerleme çizgisi), tipografi de ona hizmet edecek, ayrı bir süs numarası
   eklenmeyecek.
4. **Klişe reddi — bloke edici pop-up (yaş doğrulama / newsletter / tam ekran
   giriş) YASAK** — Moncalisse'nin yaş doğrulaması, Palazzo Sogni'nin açılış
   modalı, Postevand'ın newsletter pop-up'ı üçü de kullanıcıyı içerikten önce
   durduruyor; SAHAN doğrudan içerikle açılacak.
5. **Klişe reddi — bulanık/jenerik "atmosfer" fonu ve bağlamdan kopuk dekoratif
   ikon YASAK** — Moncalisse'nin bulanık manzara hero'su ve De Groene Afslag'ın
   "fly me to the moon" köşesi gibi öğeler SAHAN'da yok; her görsel gerçek
   tabak/mekân/malzeme fotoğrafı olacak, her öğe menü ya da rezervasyonla
   doğrudan ilişkili olacak.
6. **Schemas of Uncertainty'den alınan tek şey disiplin** — o sayfa hiç klişe
   içermiyor çünkü hiçbir öğe süs değil, hepsi içeriğin kendisi (sütun =
   makale). SAHAN'da da TADIM ŞERİDİ'ndeki her öğe (numara, fotoğraf, tek
   cümle, eşlik notu) gerçek bir kurs bilgisidir — dekoratif "01/02/03" değil.
