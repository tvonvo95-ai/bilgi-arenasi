# Bilgi Arenası — ilk sürüm

## GitHub Pages kurulumu
1. `index.html` dosyasını GitHub deposunun **kök dizinine** yükleyin (ZIP dosyasını değil).
2. GitHub deposunda **Settings > Pages > Build and deployment > Deploy from a branch > main / (root) > Save** seçin.
3. Birkaç dakika sonra GitHub Pages adresinizi açın.

## Firebase kurulumu
1. Firebase Authentication bölümünde **Email/Password** ve isteğe bağlı **Google** etkinleştirin.
2. Firebase Project settings > Your apps > Web app > SDK setup and configuration alanından **apiKey** değerini alın; `index.html` içindeki `BURAYA_API_KEY` ile değiştirin. Diğer alanları da kendi projenizle karşılaştırın.
3. Authentication > Settings > Authorized domains bölümüne `tvonvo95-ai.github.io` alan adını ekleyin.
4. Firestore > Rules bölümüne `firestore.rules` içeriğini yapıştırıp yayımlayın.
5. Online mod için iki farklı hesap ve iki cihazla test edin.

## Sınırlar ve güvenlik
- Tek kişilik mod Firebase olmadan çalışır.
- Online mod temel oda oluşturma/katılma ve eşzamanlı soru gösterimini sağlar. **Puanlar istemci tarafından hesaplanır; hileye karşı güvenli değildir.** Ödüllü veya para kazandıran yarışmalarda kullanılmamalıdır.
- Google popup girişi bazı mobil tarayıcılarda engellenebilir.
- GitHub Pages statik barındırmadır. Gerçek reklam geliri için reklam ağı onayı ve politika uyumu gerekir.
- Firebase web `apiKey` gizli anahtar değildir; **servis hesabı özel anahtarlarını asla depoya koymayın**.
