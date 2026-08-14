# 🐚 Defne Derin · 1. Yaş Doğum Günü Davetiyesi

Deniz kızı / derin okyanus temalı, animasyonlu ve mobil uyumlu dijital doğum günü davetiyesi.

**Canlı davetiye:** https://aliiball.github.io/defne-derin/

---

## ✨ Nasıl çalışır?

1. **Açılış ekranı** — Sualtında bir istiridye belirir: *"Kabuğu açar mısın?"*
2. **Dokununca** — Kabuk açılır, inci yükselir ve ekran yumuşak bir geçişle (crossfade) davetiye kartına dönüşür.
3. **Davetiye kartı** — Defne Derin'in bilgileri, tarih/saat/yer ve aksiyon butonları.

## 🔘 Butonlar

| Buton | İşlevi |
|-------|--------|
| ✓ **Geliyoruz** | WhatsApp'ı hazır bir LCV mesajıyla açar |
| 📅 **Takvime ekle** | Etkinliği `.ics` dosyası olarak takvime ekler (iOS: Apple Takvim, Android: Google Takvim) |
| 🧭 **Yol tarifi** | Google Maps'te mekâna yol tarifi açar |

## 📱 Uyumluluk

- Tüm telefon, tablet ve masaüstü ekranlarında sorunsuz çalışır (320px → 1920px breakpoint seti).
- `dvh/svh` birimleri ve `safe-area` desteğiyle çentikli telefonlarda düzgün görünür.
- "Az hareket" (reduced motion) tercihi olan cihazlarda animasyonlar sadeleşir.

## 🛠️ Bilgileri düzenleme

Tüm davet bilgileri tek bir dosyada, `index.html` içindeki `<script>` bölümünde bulunan **`DAVET`** ayar bloğundadır:

```js
const DAVET = {
  telefon: "905383678276",                 // WhatsApp LCV numarası (90 ile, boşluksuz)
  mesaj:   "Merhaba! Defne Derin'in 1. yaş kutlamasına geliyoruz.",
  baslangic: "2026-10-10T16:00:00",        // etkinlik başlangıcı
  bitis:     "2026-10-10T18:00:00",        // etkinlik bitişi
  baslik:    "Defne Derin · 1. Yaş Doğum Günü",
  mekan: "Vefa 2 Konutları",
  adres: "Hadımköy Mah. Adnan Menderes Cad., Arnavutköy / İstanbul"
};
```

Kartta görünen Tarih / Saat / Yer / LCV yazıları da `index.html` içindeki kart bölümünde (`.rows` ve `.lcv`) düz metin olarak yer alır.

## 🚀 Yayınlama (GitHub Pages)

1. Dosyayı `index.html` adıyla bu repoya yükle.
2. **Settings → Pages → Source: Deploy from a branch → Branch: `main` / `(root)`** seç, **Save**.
3. 1–2 dakika içinde site şu adreste yayına girer: `https://aliiball.github.io/defne-derin/`

## 📄 Etkinlik bilgileri

- **Kim:** Defne Derin Durmuş — 1 yaşında 🎉
- **Ne zaman:** 10 Ekim 2026, Cumartesi · 16:00 – 18:00
- **Nerede:** Vefa 2 Konutları, Hadımköy, Arnavutköy / İstanbul
- **Aile:** Selin & Enes Durmuş