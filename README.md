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

## Veri eşleştirme ve değişiklik geçmişi
- GİB kayıtları `İşlem ID` alanına göre eşleştirilir.
- Yeni kayıtlar eklenir; mevcut kayıtlarda yalnızca değişen GİB alanları güncellenir.
- `Son Düzenleme Tarihi` karşılaştırmada kullanılır; aynı tarih olsa bile alanlar ve özellikle `Durum` ayrıca karşılaştırılır.
- Her alan değişikliği eski değer, yeni değer, GİB düzenleme tarihi ve tespit zamanı ile değişiklik geçmişine kaydedilir.
- Değişiklik geçmişi kayıtlarla aynı tarayıcı deposunda saklanır. Kullanıcı tarafından girilen `Not` alanı senkronizasyonda korunur.
- Senkronizasyon sonunda yeni, değişen, değişmeyen kayıt ve kaydedilen alan değişikliği sayıları gösterilir.
- Excel yedeği ayrı bir `Değişiklik Geçmişi` sayfası da içerir; bu sayfa içe aktarıldığında geçmiş kayıtlar birleştirilerek geri yüklenir.
