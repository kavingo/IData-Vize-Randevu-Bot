iDATA Randevu Takip ve Otomasyon Botu Kaynak Kodu

Python tabanlı, Discord üzerinden yönetilebilen gelişmiş iDATA randevu takip ve otomasyon botu kaynak kodu satılıktır.

Bu proje, manuel randevu kontrol sürecini azaltmak ve kullanıcı bazlı randevu takip işlemlerini daha düzenli yönetmek amacıyla geliştirilmiş profesyonel bir otomasyon altyapısıdır. Sistem basit bir hazır script mantığında değil; çoklu kullanıcı, çoklu şehir, farklı ofis, farklı kategori ve farklı başvuru senaryolarına uyarlanabilecek şekilde hazırlanmıştır.

Not: Bu proje herhangi bir resmi kurumla bağlantılı değildir. Yazılım kaynak kod olarak satılmaktadır. Kullanım sorumluluğu tamamen alıcıya aittir.

⸻

Proje Hakkında

Bot, Discord slash komutları üzerinden yönetilir. Her kullanıcı için farklı bilgiler ve randevu tercihleri tanımlanabilir. Sistem, belirlenen kriterlere göre randevu uygunluğunu kontrol eder ve uygunluk bulunduğunda işlem akışını devam ettirebilecek altyapıya sahiptir.

Kullanıcı bazlı başlatma, durdurma, durum görüntüleme ve manuel müdahale komutları Discord üzerinden yönetilebilir. Botun hangi aşamada olduğu anlık olarak Discord bildirimleriyle takip edilebilir.

⸻

Öne Çıkan Özellikler

* Python tabanlı tam kaynak kod
* Discord slash komut sistemi
* Çoklu kullanıcı desteği
* Çoklu oturum mantığı
* Çoklu şehir ve ofis takibi
* Kullanıcı bazlı randevu tercihleri
* Kullanıcı bazlı şehir, ofis, hizmet tipi ve kategori seçimi
* Tarih aralığına göre randevu kontrol mantığı
* Otomatik tarih ve saat seçimi altyapısı
* Uygun randevu bulunduğunda işlem akışını devam ettirebilme
* Paket / promosyon ekranlarına uyarlanabilir yapı
* Ek hizmet, kargo ve sözleşme adımlarına uygun akış mantığı
* Ödeme sayfasına kadar ilerleyebilen işlem yapısı
* Slot dolduğunda yeniden deneme mantığı
* Farklı tarih seçmeye devam edebilen retry sistemi
* Manuel müdahale komutlarına uygun yapı
* SMS / e-posta doğrulama adımlarına uyarlanabilir sistem
* Doğrulama gerektiğinde kullanıcıya bildirim gönderme mantığı
* Hata yakalama, sayfa yenileme ve tekrar deneme yapısı
* Detaylı Discord bildirim sistemi
* VPS veya lokal bilgisayarda çalıştırılabilir altyapı
* Modüler ve geliştirilebilir dosya yapısı

⸻

Discord Bildirimleri

Sistem çalışırken botun bulunduğu aşama Discord üzerinden takip edilebilir.

Bildirim örnekleri:

* Bot başlatıldı
* Kullanıcı oturumu açılıyor
* Randevu kontrol ediliyor
* Randevu uygunluğu bulundu
* Tarih seçildi
* Saat seçildi
* Slot doldu
* Yeniden deneniyor
* Ödeme ekranına gelindi
* Hata oluştu
* İşlem tamamlandı
* Manuel müdahale gerekiyor

Bu yapı sayesinde bot arka planda çalışırken işlem süreci anlık olarak izlenebilir.

⸻

Çoklu Kullanıcı Yapısı

Sistem birden fazla kullanıcıyı ayrı ayrı takip edebilecek şekilde tasarlanmıştır.

Her kullanıcı için farklı bilgiler tanımlanabilir:

* Kullanıcı adı
* Pasaport / üyelik bilgileri
* Şehir tercihi
* Ofis tercihi
* Hizmet tipi
* Kategori
* Tarih aralığı
* Randevu tercihleri
* Bildirim ayarları
* Oturum durumu

Bu yapı sayesinde tek sistem üzerinden birden fazla kullanıcı ve farklı başvuru senaryosu yönetilebilir.

⸻

Randevu Akışı

Sistem, uygun randevu bulunduğunda işlem akışını devam ettirebilecek şekilde hazırlanmıştır.

Desteklenen akış yapıları:

* Uygunluk kontrolü
* Tarih seçimi
* Saat seçimi
* Paket / promosyon ekranları
* Ek hizmet adımları
* Kargo bilgileri
* Sözleşme onayları
* Ödeme sayfasına ilerleme
* Slot dolduğunda tekrar deneme
* Gerekirse farklı tarih seçmeye devam etme

Akış yapısı modüler olduğu için alıcı kendi kullanım senaryosuna göre şehir, kategori, ofis veya işlem adımlarını düzenleyebilir.

⸻

Doğrulama Adımları

Bot, SMS veya e-posta doğrulama gibi kullanıcı müdahalesi gerektiren adımlara uyarlanabilecek yapıdadır.

Desteklenebilecek senaryolar:

* Kullanıcıya Discord üzerinden doğrulama bildirimi gönderme
* Manuel kod girme akışı
* Özel doğrulama entegrasyonlarına uygun genişletilebilir yapı
* İşlem duraklatma ve devam ettirme mantığı

⸻

Teknik Yapı

Proje Python ile geliştirilmiştir. Dosya yapısı düzenlenebilir ve genişletilebilir şekilde hazırlanmıştır.

Genel teknik yapı:

project/
│
├── bot/
│   ├── commands/
│   ├── handlers/
│   └── notifications/
│
├── automation/
│   ├── browser/
│   ├── flow/
│   ├── retry/
│   └── user_sessions/
│
├── config/
│   ├── users.json
│   └── settings.example.json
│
├── requirements.txt
└── README.md

Gerçek dosya yapısı teslim edilen sürüme göre değişebilir.

⸻

Gereksinimler

Temel kurulum için gerekli bilgiler:

* Python 3.x
* Discord bot token
* Gerekli Python kütüphaneleri
* VPS veya lokal bilgisayar
* Temel terminal bilgisi
* Kullanıcı ayar dosyalarının düzenlenmesi

Gerekli kütüphaneler requirements.txt dosyasıyla birlikte teslim edilir.

⸻

Teslimat İçeriği

Satış kapsamında teslim edilecek içerikler:

* Tam kaynak kod dosyaları
* requirements.txt
* Örnek ayar dosyaları
* Kullanıcı yapılandırma örnekleri
* Temel kurulum açıklaması
* Çalışma mantığı açıklaması
* Discord komut kullanım mantığı
* Gerekli teknik notlar

İsteğe bağlı olarak ek ücretle şu hizmetler sağlanabilir:

* VPS kurulumu
* Bot kurulumu
* Ortam ayarlarının yapılması
* Özel komut ekleme
* Yeni şehir / kategori uyarlaması
* Yeni özellik geliştirme
* Teknik destek

⸻

Kimler İçin Uygun?

Bu kaynak kod şu kişiler için uygundur:

* Vize randevu süreçleriyle ilgili otomasyon altyapısı kurmak isteyenler
* Kendi randevu takip sistemini geliştirmek isteyen yazılımcılar
* Discord üzerinden yönetilebilen otomasyon botu arayanlar
* Çoklu kullanıcı destekli bir sistem kurmak isteyenler
* Kaynak kodu alıp kendi ihtiyaçlarına göre geliştirmek isteyenler
* White-label yazılım altyapısı arayanlar

⸻

Satış ve Demo

Kaynak kod ciddi alıcılara özel olarak satılmaktadır.

Demo, özellik listesi ve teknik detaylar yalnızca ciddi alıcılarla paylaşılır. Kaynak kod tamamen düzenlenebilir şekilde teslim edilir.

Satış modeli:

* Tek seferlik kaynak kod satışı
* Özel kurulum desteği
* İsteğe bağlı geliştirme desteği
* White-label kullanım imkanı

⸻

Önemli Not

Bu yazılım herhangi bir resmi kurum, konsolosluk, aracı kurum veya vize başvuru merkeziyle bağlantılı değildir.

Yazılım yalnızca kaynak kod ve otomasyon altyapısı olarak sunulmaktadır. Randevu garantisi vermez. Alıcı, yazılımı kullanırken ilgili platformların kullanım şartlarına, yürürlükteki yasalara ve resmi başvuru kurallarına uygun hareket etmekten kendisi sorumludur.

Satıcı, yazılımın kötüye kullanımı, platform kurallarına aykırı kullanımı veya üçüncü taraf sistemlerde doğabilecek sonuçlardan sorumlu değildir.

⸻

Lisans

Bu proje özel kaynak kod satışı kapsamında değerlendirilir.

Kodun yeniden satışı, paylaşılması veya üçüncü kişilere dağıtılması satış şartlarına göre ayrıca belirlenir.

Detaylı lisans ve kullanım şartları satış öncesinde alıcıyla netleştirilir.

İletişim : 
Discord : @mebya
Telegram : @kavingo
