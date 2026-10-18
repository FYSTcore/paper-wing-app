# Paper Wing — Android uygulaması

Bu depo Paper Wing'in gerçek Android uygulamasını (Capacitor) derler. Oyunun kendisi `FYSTcore/paper-wing` deposunda durur.

- **Uygulama açılınca** internet varsa oyunun canlı sürümü siteden açılır: oyun güncellemeleri için yeni APK gerekmez.
- **İnternet yoksa** daha önce bir kez açıldıysa site çevrimdışı açılır; hiç açılmadıysa uygulamaya gömülü kopya açılır.
- Paket adı ve imza eski uygulamayla aynı (`io.github.fystcore.paperwing`), bu yüzden eski uygulamanın **üstüne güncelleme** olarak kurulur.

## Derleme
Actions → **Build Android** → Run workflow → sürüm adını yaz → Run. Bitince **Releases** sayfasında `paper-wing.apk` (telefon) ve `paper-wing.aab` (Play Store) olur.

Gerekli sırlar (Settings → Secrets and variables → Actions): `KEYSTORE_B64`, `KEYSTORE_PASSWORD`, `KEY_ALIAS`, `KEY_PASSWORD`.
İmza dosyası ve şifreler **asla** depoya yüklenmez.
