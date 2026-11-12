# SF Siparişler (mobil)

Sunucu Modu panelindeki siparişlerin telefondan görülebilen, **salt okunur** görünümü.
Veri Supabase `sf_store` tablosundaki `DB_<mağazaId>`, `ACCOUNTS` ve `SERVER_HEARTBEAT` anahtarlarından okunur; hiçbir şey yazılmaz.

## Yayına alma (bir kez)
1. GitHub'da bu repo → **Settings → Pages**
2. *Build and deployment* → Source: **Deploy from a branch**, Branch: **main** / **(root)** → Save
3. 1-2 dakika sonra adres: `https://<kullanıcı>.github.io/sf-siparis/`

## Kullanım
- İlk açılışta Supabase URL, anon/publishable anahtar ve mağaza ID'leri girilir. Bunlar **yalnız o cihazın tarayıcısında** saklanır; repoda hiçbir anahtar yoktur.
- Telefonda tarayıcı menüsünden **Ana ekrana ekle** ile uygulama gibi açılır.
- Arama kutusunda `3 gün` → kargo durumu 3 gün ve daha uzun süredir aynı olanlar; `=3` → tam 3 gün.
- Sayfa açıkken dakikada bir kendiliğinden yenilenir.

Durum kuralları Sunucu Modu paneliyle (`sfadminlog/userscripts/sellerflash-panel.user.js`) aynı tutulmalıdır.
