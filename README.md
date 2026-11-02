# Zombi Uygulama İncelemesi: FeedDemon 4.5

Bu çalışma, geliştiricisi tarafından bırakıldığı hâlde kullanılmaya devam eden bir uygulamayı inceleyen ders ödevidir. Bu aşamada kod yazılmamıştır.

> **Durum:** Kaynak araştırması tamamlandı. Gerçek kullanıcıyla beş dakikalık görüşme ve üç örtük kuralın doğrulanması henüz tamamlanmadı. İnternet yorumu kişisel görüşme olarak sunulmamaktadır.

## 1. Kimlik

**Uygulama:** FeedDemon 4.5  
**Geliştirici:** Nick Bradbury

FeedDemon, Windows üzerinde haber sitelerinin ve blogların RSS akışlarını tek ekranda takip etmeyi sağlar. Kullanıcı, siteleri ayrı ayrı açmadan yeni içerikleri okuyabilir. İnternette belirlenen kullanıcı, geliştiricinin bloguna “Ron” adıyla yorum bırakan kişidir.

## 2. Ölüm kanıtı

Nick Bradbury, **20 Haziran 2013** tarihli yazısında FeedDemon'un son sürümünü yayımladığını ve ücretsiz sunduğunu duyurmuştur. Bu sürümde Google Reader eşitlemesi kaldırılmıştır. [Son sürüm duyurusu](https://nickbradbury.com/2013/06/20/the-last-version-of-feeddemon-is-here-and-its-free/)

Geliştirici, **10 Mart 2016** tarihli “FeedDemon Support Group is Pining for the Fjords” yazısında destek grubunu kapatmaya karar verdiğini ve mevcut bilgilerden yararlanılabilmesi için grubu salt okunur hâle getirdiğini açıklamıştır. [Geliştiricinin FeedDemon yazıları](https://nickbradbury.com/category/feeddemon/)

Zombi değerlendirmesi, uygulamanın eski görünmesine değil, geliştiricinin açık bırakılma duyurularına dayanır.

## 3. Yaşam kanıtı

Geliştiricinin “Tic Tac Troll” yazısına **29 Eylül 2026** tarihinde yorum yapan Ron şöyle demiştir:

> “I still use FeedDemon every day.”

Türkçesi: “FeedDemon'u hâlâ her gün kullanıyorum.”

Aynı yorumda daha iyi bir RSS toplayıcısı bulamadığını belirtmiştir. Geliştirici de aynı gün yoruma yanıt vermiştir. Bu, güncel kullanıma ilişkin kamuya açık bir kullanıcı beyanıdır; benim yaptığım görüşme değildir. [Yorumun bulunduğu yazı](https://nickbradbury.com/2026/09/28/tic-tac-troll/)

**Tamamlanacak görüşme kaydı:**

- Kullanıcı adı veya izinli takma adı: Henüz kaydedilmedi.
- Görüşme tarihi ve paylaşım izni: Henüz alınmadı.
- Kullanım sıklığı ve amacı: Görüşmede sorulacak.
- Kullanıcının gerçek cümlesi: Görüşme sonrasında eklenecek.

## 4. Neden ölmüyor?

Savunduğum en güçlü neden, **kullanıcının alternatifleri mevcut program kadar iyi bulmamasıdır**. Ron'un yorumu bu gerekçeyi desteklemektedir. Kullanıcı, günlük RSS takip ihtiyacını karşılayan aracı kullanmayı sürdürmektedir.

Alışkanlık, arşiv veya kullanım kolaylığı gibi başka etkenler araştırılabilir; görüşme yapılmadan bunlar doğrulanmış kullanıcı gerekçeleri sayılmamalıdır.

## 5. Ne zaman düşer?

Olası kırılma noktası, yeni Windows sürümleri veya haber sitelerinin bağlantı ve güvenlik yöntemleriyle uyumsuz hâle gelmesidir. Geliştirilmesi bırakıldığı için gelecekteki uyumsuzlukların giderileceği varsayılamaz.

Bu bir risk değerlendirmesidir; uygulamanın bugün bütün sistemlerde çalışmadığı iddiası değildir.

## 6. Örtük bağlam

Aşağıdaki üç madde **görüşmede sınanacak kural adaylarıdır**. FeedDemon'un doğrulanmış davranışı veya gerçek bir kullanıcının gözlemlenmiş kuralları olarak sunulmamaktadır.

| Doğrulanacak kural adayı | Ruby ile yeniden yazan ajana söylenmezse olası sonuç |
| --- | --- |
| Aynı haber tekrar geldiğinde ikinci kayıt açılmamalı ve okundu durumu korunmalı. | Yinelenen haberler oluşabilir; okunmuş içerik yeniden okunmamış görünebilir. |
| Kullanıcının favoriye aldığı içerikler normal temizlik işleminde silinmemeli. | Kullanıcının saklamak istediği kayıtlar kaybolabilir. |
| Bir RSS kaynağı geçici olarak erişilemez olduğunda mevcut kayıtlar korunmalı ve diğer kaynakların güncellenmesi sürmeli. | Geçici bağlantı hatası veri kaybına veya bütün güncellemenin durmasına yol açabilir. |

Her aday kullanıcıya doğrulatılmalı; uygun değilse kullanıcının gerçek kuralıyla değiştirilmelidir. Haber kimliği, saklama süresi ve favorilerde tam metin mi bağlantı mı tutulacağı ayrıca netleştirilmelidir.

## 7. Yapay zekâ izi

Çalışmanın başlangıcında ChatGPT'nin “Bana zombi uygulama örnekleri ver” sorusu için kaydettiği ilk üç aday:

1. Picasa
2. Windows Movie Maker
3. Microsoft Money

Bunlar araştırılması gereken adaylardır; yalnızca yapay zekânın önermesi zombi olduklarını kanıtlamaz.

İlk araştırmada SyncToy değerlendirilmiş, sınıftaki mevcut seçimlerden farklı bir aday arandığında FeedDemon'a geçilmiştir. FeedDemon'un tercih edilme nedeni, bırakılma duyurularının ve güncel bir kullanım beyanının bulunması; temel işlevinin sınırlı bir RSS okuyucu projesine indirgenebilmesidir.

Araştırmanın düzenlenmesinde ve metnin hazırlanmasında ChatGPT kullanılmıştır. Kaynaklar geliştiricinin kamuya açık yazıları ve yorumudur. Kullanıcı görüşmesi uydurulmamıştır.

## Ruby ile olası yeniden yazım kapsamı

Sonraki haftalarda seçilmesi hâlinde temel kapsam:

- RSS adresi ekleme.
- Haberleri listeleme.
- Okundu bilgisini tutma.
- Favorilere ekleme.

Bu liste bir proje önerisidir. Henüz Ruby uygulaması geliştirilmemiştir.

## Sınıfta kısa savunma

“FeedDemon'u zombi uygulama adayı olarak seçtim. Geliştiricisi 2013'te son sürümü duyurmuş, 2016'da destek grubunu salt okunur hâle getirmiş. Buna rağmen 2026 tarihli bir kullanıcı yorumunda programın her gün kullanıldığı belirtiliyor. Bu nedenle üreticisi tarafından bırakılmış ama kullanıcı tarafında yaşamaya devam eden bir uygulama örneği. Kullanıcının alternatifleri yeterli bulmaması, uygulamanın neden yaşadığını açıklıyor. Ruby ile yeniden yazımda RSS adresi ekleme, haberleri listeleme, okundu bilgisi ve favorilerle sınırlı bir kapsam seçilebilir. Gerçek kullanıcı görüşmesi ve üç örtük kuralın doğrulanması ise henüz tamamlanmadı.”

## Teslim öncesi kalanlar

- [ ] Sınıf yorumlarında FeedDemon adının başka biri tarafından alınmadığını kontrol et.
- [ ] İzin veren gerçek bir kullanıcıyla beş dakika görüş.
- [ ] Görüşme tarihi, kullanım amacı, sıklığı ve gerçek alıntıyı ekle.
- [ ] Üç örtük kuralı kullanıcı gözlemleriyle doğrula veya değiştir.
- [ ] Eklenecek ekran görüntülerindeki kişisel verileri karart.

## Kaynaklar

1. Nick Bradbury, [The Last Version of FeedDemon is Here, and it's Free](https://nickbradbury.com/2013/06/20/the-last-version-of-feeddemon-is-here-and-its-free/), 20 Haziran 2013.
2. Nick Bradbury, [FeedDemon kategorisi — destek grubunun kapanış duyurusu](https://nickbradbury.com/category/feeddemon/), 10 Mart 2016.
3. Nick Bradbury, [Tic Tac Troll](https://nickbradbury.com/2026/09/28/tic-tac-troll/), 28 Eylül 2026; Ron'un yorumu, 29 Eylül 2026.

Kaynak kontrol tarihi: 2 Kasım 2026.
