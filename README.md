# YANSIMA TV — Android projesi

Dört ön tanımlı kanal, siyah tema, M3U URL/dosya desteği, Xtream canlı kanal yükleme ve Media3 oynatıcı içerir.

## Telefon üzerinden ücretsiz APK derleme (GitHub Actions)

1. https://github.com adresinde ücretsiz hesap oluşturun/giriş yapın.
2. Yeni bir **public** repository oluşturun (ör. `yansima-tv`).
3. Bu klasördeki proje dosyalarını repository köküne yükleyin. `.github/workflows/build-apk.yml` dosyasının bu tam yol ile yüklendiğinden emin olun.
4. Repository'de **Actions** sekmesine girin ve `Build YANSIMA TV APK` iş akışını seçin. `Run workflow` düğmesine basın (ilk push da derlemeyi başlatır).
5. İş akışı yeşil tikle bittiğinde çalıştırma sayfasının altındaki **Artifacts** bölümünden `YANSIMA-TV-debug-APK` dosyasını indirin.
6. ZIP içinden `app-debug.apk` dosyasını çıkarıp Android telefona kurun.

Standart GitHub-hosted runner'larda public depolar için Actions kullanımı ücretsizdir. Repository public olacağından kaynak kodu ve yayın URL'leri herkesçe görülebilir; özel liste/şifre eklemeyin.

## Bilinen sınırlamalar
- Bu arşiv kaynak projedir; APK, GitHub Actions başarılı tamamlandıktan sonra oluşur.
- Yayınların çalışması sunucu erişimine bağlıdır. HTTP yayınlar güvenli olmayan bağlantı kullanabilir.
- Xtream sunucularının cevap biçimleri değişebilir. EPG, VOD, kalıcı favoriler ve güvenli hesap saklama bu MVP'de yoktur.
- Yalnızca kullanma izniniz olan yayınları kullanın.
