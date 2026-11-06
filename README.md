# Oz Zeka

Kişisel asistan. Bu depoda Oz Zeka'nın `.py` dosyaları durur.

## GitHub'dan güncelleme

Oz Zeka bu deponun ana dalındaki (`main`) `.py` dosyalarını kendi `uygulama` klasörüne indirir:

- **Açılışta:** Ayarlar > Güncelleme'de "Açılışta kendiliğinden güncelle" işaretliyse, açıldıktan birkaç saniye sonra bakar.
- **Elle:** Ayarlar > Güncelleme > **Güncelle**, ardından **Yeniden başlat**.
- **Telegram:** bota `güncelle` yaz. İndirir, yeniden başlar ve "yeniden açıldım" der.

Güvenlik önlemleri:

- Sadece değişen dosyalar indirilir. İndirilen dosya bozuksa hiçbir şey değişmez.
- Eski dosyalar `veriler\guncelleme_yedek` klasörüne yedeklenir (son 10 güncelleme).
- Yeni sürüm açılmazsa eski hali kendiliğinden geri konur.
- `veriler` klasörü (anahtarlar, `veriler.json`) **depoya konmaz** ve güncellemeden etkilenmez.
