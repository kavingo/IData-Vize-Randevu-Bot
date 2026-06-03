

# iDATA Randevu Takip ve Otomasyon Botu

Python tabanlı, Discord üzerinden yönetilebilen gelişmiş iDATA randevu takip ve otomasyon botu kaynak kodu.

Bu proje; randevu uygunluğu takibi, çoklu kullanıcı yönetimi, şehir/ofis/kategori bazlı takip ve Discord üzerinden süreç yönetimi için geliştirilmiş profesyonel bir otomasyon altyapısıdır. Sistem hazır script mantığında değil, farklı senaryolara göre düzenlenebilir ve geliştirilebilir bir kaynak kod yapısına sahiptir.

> **Önemli Not:** Bu proje herhangi bir resmi kurum, konsolosluk, aracı kurum veya vize başvuru merkeziyle bağlantılı değildir. Yazılım kaynak kod olarak sunulmaktadır. Kullanım sorumluluğu tamamen alıcıya/kullanıcıya aittir.

---

## İçindekiler

- [Proje Hakkında](#proje-hakkında)
- [Öne Çıkan Özellikler](#öne-çıkan-özellikler)
- [Discord Yönetim Sistemi](#discord-yönetim-sistemi)
- [Çoklu Kullanıcı Yapısı](#çoklu-kullanıcı-yapısı)
- [Randevu Akışı](#randevu-akışı)
- [Bildirim Sistemi](#bildirim-sistemi)
- [Doğrulama Adımları](#doğrulama-adımları)
- [Teknik Yapı](#teknik-yapı)
- [Gereksinimler](#gereksinimler)
- [Teslimat İçeriği](#teslimat-i̇çeriği)
- [Kurulum Hakkında](#kurulum-hakkında)
- [Kullanım Alanları](#kullanım-alanları)
- [Demo ve Satış](#demo-ve-satış)
- [Yasal Uyarı](#yasal-uyarı)
- [Lisans](#lisans)

---

## Proje Hakkında

Bu bot, iDATA randevu süreçlerinde manuel kontrol yükünü azaltmak ve kullanıcı bazlı randevu takip işlemlerini Discord üzerinden yönetilebilir hale getirmek amacıyla geliştirilmiştir.

Sistem, kullanıcı tarafından belirlenen şehir, ofis, hizmet tipi, kategori, tarih aralığı ve randevu tercihlerine göre kontrol yapabilecek şekilde tasarlanmıştır. Randevu uygunluğu bulunduğunda Discord üzerinden bildirim gönderir ve yapılandırmaya bağlı olarak işlem akışını devam ettirebilecek altyapıya sahiptir.

Bot, birden fazla kullanıcı ve birden fazla şehir/ofis senaryosu için düzenlenebilir yapıdadır. Kaynak kod teslim edildiği için alıcı kendi ihtiyaçlarına göre akışları, ayarları ve komutları düzenleyebilir.

---

## Öne Çıkan Özellikler

- Python tabanlı tam kaynak kod
- Discord slash komutları ile yönetim
- Çoklu kullanıcı desteği
- Çoklu oturum mantığı
- Çoklu şehir ve ofis takibi
- Kullanıcı bazlı pasaport / üyelik bilgisi tanımlama
- Kullanıcı bazlı şehir, ofis, hizmet tipi ve kategori seçimi
- Tarih aralığı ve randevu tercihleri belirleme
- Kullanıcı bazlı başlatma, durdurma ve durum görüntüleme
- Manuel müdahale komutlarına uygun yapı
- Randevu uygunluğu kontrol sistemi
- Otomatik tarih ve saat seçimi altyapısı
- Uygun randevu bulunduğunda işlem akışını devam ettirebilme
- Paket / promosyon ekranlarına uyarlanabilir yapı
- Ek hizmet, kargo ve sözleşme adımlarına uygun akış mantığı
- Ödeme sayfasına kadar ilerleyebilen işlem yapısı
- Slot dolduğunda yeniden deneme mantığı
- Farklı tarih seçmeye devam edebilen retry sistemi
- Hata yakalama, sayfa yenileme ve tekrar deneme yapısı
- Detaylı Discord bildirimleri
- VPS veya lokal bilgisayarda çalıştırılabilir altyapı
- Modüler ve geliştirilebilir dosya yapısı

---

## Discord Yönetim Sistemi

Bot Discord üzerinden yönetilebilecek şekilde hazırlanmıştır. Kullanıcı bazlı işlemler slash komutları ile kontrol edilebilir.

Örnek yönetim mantığı:

- Kullanıcı ekleme
- Kullanıcı bilgilerini düzenleme
- Randevu kriterlerini belirleme
- Belirli kullanıcı için botu başlatma
- Belirli kullanıcı için botu durdurma
- Mevcut işlem durumunu görüntüleme
- Manuel müdahale gereken durumlarda komutla devam ettirme
- İşlem hatalarını ve bildirimleri Discord üzerinden takip etme

Bu yapı sayesinde bot sunucuda veya lokal bilgisayarda çalışırken kontrol süreci Discord üzerinden yönetilebilir.

---

## Çoklu Kullanıcı Yapısı

Sistem, birden fazla kullanıcıyı ayrı ayrı takip edebilecek şekilde tasarlanmıştır.

Her kullanıcı için farklı bilgiler tanımlanabilir:

- Kullanıcı adı
- Pasaport / üyelik bilgileri
- Şehir tercihi
- Ofis tercihi
- Hizmet tipi
- Kategori
- Tarih aralığı
- Randevu tercihleri
- Bildirim ayarları
- Oturum durumu

Bu yapı sayesinde tek bot üzerinden farklı kullanıcılar, farklı şehirler ve farklı başvuru senaryoları yönetilebilir.

---

## Randevu Akışı

Sistem, uygun randevu bulunduğunda işlem akışını devam ettirebilecek altyapıya sahiptir.

Desteklenen akış mantıkları:

- Randevu uygunluğu kontrolü
- Tarih seçimi
- Saat seçimi
- Paket / promosyon ekranlarına uyarlanabilir akış
- Ek hizmet adımlarına uyarlanabilir yapı
- Kargo bilgileri
- Sözleşme onayları
- Ödeme sayfasına ilerleme
- Slot dolduğunda yeniden deneme
- Gerekirse farklı tarih seçmeye devam etme
- Manuel müdahale gereken durumlarda Discord üzerinden bilgi verme

Akış yapısı modüler olduğu için alıcı kendi kullanım senaryosuna göre şehir, kategori, ofis veya işlem adımlarını düzenleyebilir.

---

## Bildirim Sistemi

Botun hangi aşamada olduğu Discord üzerinden takip edilebilir.

Bildirim örnekleri:

- Bot başlatıldı
- Kullanıcı oturumu açılıyor
- Kontrol ekranı geçiliyor
- Randevu kontrol ediliyor
- Randevu uygunluğu bulundu
- Tarih seçildi
- Saat seçildi
- Slot doldu
- Yeniden deneniyor
- Ödeme ekranına gelindi
- Hata oluştu
- Manuel müdahale gerekiyor
- İşlem tamamlandı

Bu yapı sayesinde bot arka planda çalışırken süreç anlık olarak izlenebilir.

---

## Doğrulama Adımları

Bot, SMS veya e-posta doğrulama gibi kullanıcı müdahalesi gerektiren adımlara uyarlanabilecek yapıdadır.

Desteklenebilecek senaryolar:

- Kullanıcıya Discord üzerinden doğrulama bildirimi gönderme
- Manuel kod girme akışı
- İşlemi duraklatma ve devam ettirme mantığı
- Özel doğrulama entegrasyonlarına uygun genişletilebilir yapı

Doğrulama gerektiren akışlarda sistemin nasıl kullanılacağı, alıcının kendi kullanım senaryosuna ve ilgili platform kurallarına göre belirlenmelidir.

---

## Teknik Yapı

Proje Python ile geliştirilmiştir. Dosya yapısı modüler ve genişletilebilir olacak şekilde hazırlanmıştır.

Örnek proje yapısı:

```bash
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
```

> Gerçek dosya yapısı teslim edilen sürüme göre değişebilir.

---

## Gereksinimler

Temel kullanım için gerekli olabilecek araçlar:

- Python 3.x
- Discord bot token
- Gerekli Python kütüphaneleri
- VPS veya lokal bilgisayar
- Temel terminal bilgisi
- Kullanıcı ayar dosyalarının düzenlenmesi

Gerekli kütüphaneler `requirements.txt` dosyasıyla birlikte teslim edilir.

---

## Teslimat İçeriği

Satış kapsamında teslim edilecek içerikler:

- Tam kaynak kod dosyaları
- `requirements.txt`
- Örnek ayar dosyaları
- Kullanıcı yapılandırma örnekleri
- Temel kurulum açıklaması
- Çalışma mantığı açıklaması
- Discord komut kullanım mantığı
- Gerekli teknik notlar

Ek ücret karşılığında sağlanabilecek hizmetler:

- VPS kurulumu
- Bot kurulumu
- Ortam ayarlarının yapılması
- Özel komut ekleme
- Yeni şehir / kategori uyarlaması
- Yeni özellik geliştirme
- Teknik destek

---

## Kurulum Hakkında

Kurulum için temel Python ve terminal bilgisi yeterlidir. Proje, alıcının kendi ortamına göre yapılandırılabilir.

Genel kurulum mantığı:

1. Proje dosyaları alınır.
2. Python ortamı hazırlanır.
3. Gerekli paketler yüklenir.
4. Discord bot token ve ayar dosyaları düzenlenir.
5. Kullanıcı bilgileri ve randevu tercihleri tanımlanır.
6. Bot başlatılır.
7. Discord üzerinden yönetim komutları kullanılır.

Detaylı kurulum bilgisi satış sonrası teslim edilen teknik açıklamalarda yer alır.

---

## Kullanım Alanları

Bu kaynak kod şu kişiler için uygundur:

- Vize randevu süreçleriyle ilgili otomasyon altyapısı kurmak isteyenler
- Kendi randevu takip sistemini geliştirmek isteyen yazılımcılar
- Discord üzerinden yönetilebilen otomasyon botu arayanlar
- Çoklu kullanıcı destekli bir sistem kurmak isteyenler
- Kaynak kodu alıp kendi ihtiyaçlarına göre geliştirmek isteyenler
- White-label yazılım altyapısı arayanlar
- Otomasyon ve takip sistemi geliştirmek isteyen kişiler

---

## Demo ve Satış

Kaynak kod ciddi alıcılara özel olarak satılmaktadır.

Demo, detaylı özellik listesi ve teknik bilgiler yalnızca ciddi alıcılarla paylaşılır. Kaynak kod tamamen düzenlenebilir şekilde teslim edilir.

Satış modeli:

- Tek seferlik kaynak kod satışı
- Özel kurulum desteği
- İsteğe bağlı geliştirme desteği
- White-label kullanım imkanı

---

## Yasal Uyarı

Bu yazılım herhangi bir resmi kurum, konsolosluk, aracı kurum veya vize başvuru merkeziyle bağlantılı değildir.

Yazılım yalnızca kaynak kod ve otomasyon altyapısı olarak sunulmaktadır. Randevu garantisi vermez. Alıcı, yazılımı kullanırken ilgili platformların kullanım şartlarına, yürürlükteki yasalara ve resmi başvuru kurallarına uygun hareket etmekten kendisi sorumludur.

Satıcı, yazılımın kötüye kullanımı, platform kurallarına aykırı kullanımı veya üçüncü taraf sistemlerde doğabilecek sonuçlardan sorumlu değildir.

---

## Lisans

Bu proje özel kaynak kod satışı kapsamında değerlendirilir.

Kodun yeniden satışı, paylaşılması veya üçüncü kişilere dağıtılması satış şartlarına göre ayrıca belirlenir.

Detaylı lisans ve kullanım şartları satış öncesinde alıcıyla netleştirilir.

## İletişim : 
Discord : @mebya
Telegram : @kavingo
