# 🛡️ İMPERİEL Bot's

SENTRY Guard, sunucunuzu nuke, raid ve izinsiz yetki kullanımlarına karşı korumak için tasarlanmış, **V14 altyapılı** profesyonel bir koruma sistemidir.

## 👤 İletişim
Bu bot **.imperiel** tarafından geliştirilmiştir. Destek ve iletişim için Discord üzerinden arkadaşlık isteği gönderebilirsiniz.

---

## 🚀 Gelişmiş Koruma Özellikleri

* **Limit Sistemi (Token Koruması):** Whitelist'teki kişiler bile olsa, 1 dakika içinde 3'ten fazla işlem yapılması durumunda bot yetkileri dondurur ve sunucuyu kilitler.
* **Anti-Raid (Fake Hesap Koruması):** Kuruluş tarihi 7 günden yeni olan hesaplar sunucuya girdiği an otomatik olarak uzaklaştırılır.
* **Ses Koruması:** Seste toplu susturma, sağırlaştırma veya sesten atma eylemlerini anında engeller.
* **Otomatik Yedekleme:** Bot, her gece saat 04:00'da sunucunun rol, kanal ve kategori yedeğini otomatik olarak alır.
* **Panik Modu:** Saldırı anında tüm üye rollerinin yazma/konuşma izinlerini tek komutla kapatır.

---

## ⚙️ Kurulum Rehberi

1.  **Ayarlar:** `ayarlar.json` dosyasını açıp Token ve ID bilgilerini doldurun. `safeBots` kısmına diğer botlarınızı eklemeyi unutmayın.
2.  **Paketler:** Terminale sırasıyla yazın:
    ```bash
    npm init -y
    npm install discord.js croxydb node-cron
    ```
3.  **Başlatma:** Botu başlatmak için:
    ```bash
    node index.js
    ```

---

## 📋 Komut Listesi

| Komut | Açıklama |
| :--- | :--- |
| `.loglar` | Guard log kanallarını otomatik kurar. |
| `.panik [aç/kapat]` | Kayıtlı rollerin mesaj/ses yetkilerini kısıtlar/açar. |
| `.yedek-al` | Sunucunun tam yedeğini alır. |
| `.yedek-kur` | Son yedeği sunucuya yükler. |
| `.wl @kullanıcı/ID [kat]` | Belirtilen kişiyi seçilen kategoride whitelist'e alır. |
| `.ping` | Botun gecikme süresini gösterir. |

---

## ⚠️ Hayati Uyarılar

* **Rol Sıralaması:** Botun rolünü sunucu ayarlarından **en üst sıraya** (Kurucu rolünün hemen altına) taşıyın.
* **Yetkilendirme:** Botun rolüne **"Yönetici"** yetkisini verin.
* **Geliştirici İzinleri:** Discord Developer Portal'dan "Presence", "Server Members" ve "Message Content" (Intents) şalterlerini mutlaka açın.
