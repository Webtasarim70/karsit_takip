# e-Karşıt Takip

Bağımsız, tek HTML dosyalı e-Karşıt Takip uygulaması. CSS, uygulama JavaScript'i ve ExcelJS kütüphanesi `index.html` içine gömülüdür.

## Kullanım
- GitHub Pages üzerinden `index.html` sayfasını açın.
- Kayıtlar bu tarayıcının `localStorage` alanında saklanır. Tarayıcı verileri temizlenirse yedek alınmamış kayıtlar silinebilir.
- Excel içe/dışa aktarma ve kayıt bazında Not alanı korunur.
- GİB'den senkronizasyon için aşağıdaki eklentiyi kurup GİB portalına giriş yapın.

## Tarayıcı eklentisi
Chrome/Edge'de `extension/` klasörünü ayrı bir eklenti olarak yükleyin: Eklentiler sayfası → Geliştirici modu → Paketlenmemiş öğe yükle → `extension` klasörü.

Eklenti, GİB oturumunu tarayıcıda kullanır. GİB kullanıcı adı, parola, çerez veya erişim belirteci bu uygulama tarafından kaydedilmez.

## Veri eşleştirme
Senkronizasyon `İşlem ID` alanına göre yeni kayıt ekler ve mevcut kayıtları günceller; mevcut kaydın `Not` alanı korunur.
