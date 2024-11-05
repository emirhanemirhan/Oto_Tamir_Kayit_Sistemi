# Oto_Tamir_Kayit_Sistemi

•Emirhan Erdem-230260199

•Emirhan Alişan-220260081

•Alper Nas-220260039

Oto tamir ve kayıt sistemi,araçların bakım ve onarım süreçlerini yönetmek için geliştirilmiştir.Araç bilgileri, ruhsat bilgileri, müşteri iletişim bilgileri, tamir çeşitleri, tamir başlangıç ve bitiş tarihi, fiyatlandırma ana varlıkları oluşturur. Her araç, bakım kayıtlarıyla ilişkilidir ve kullanıcılar, araçlarının bakım geçmişini izleyebilir.Bu sistem, bakım süreçlerini optimize ederek verimlilik ve şeffaflık sağlar.Aşağıda bu varlıkların sahip olduğu nitelikler ve aralarındaki ilişkiler belirtilmiştir.

Kullanıcı Profilleri Tablosu:

| Kullanıcı Profilleri | Açıklama        | 
|----------------------|-----------------------|
| Müşteri Girişi | Sanayiye gelip araç tamiri isteyen birey yada şirket  |
| Personel Girişi | Veri tabanına erişimi kısıtlı personel |
| Yönetici Girişi | Veri tabanını yöneten müdür  |


Varlık-Özellik Tablosu:

| Varlıklar | Özellikler |
|-----------------|----------|
| Araç Bilgileri | Araç ID,Araç Markası , Araç Modeli , Araç Tipi , Yıl ,Renk,Şase Numarası,Motor Numarası,Plaka Numarası,Kilometre,Yakıt Tipi,Vites Tipi,Garanti Durumu|
| Ruhsat Bilgileri | Ruhsat Numarası, Ruhsat Sahibi ,Verildiği İl İlçe, Tescil Tarihi ,Tescil Sıra No,Geçerlilik Süresi|
| Personel Bilgileri  | Personel ID,Ad Soyad  , TC Numarası , Telefon Numarası , E posta ,Adres  , Görev/Ünvan , Çalışma Tarihleri , Eğitim Durumu ,İzin Durumu,Maaşı|
| Müşteri Bilgileri | Müşteri ID,Müşteri Adı ,Telefon Numarası,E-posta Adresi,Adres,Müşteri Tipi,İletişim Tercihi|
| Tamir Çeşitleri  | Tamir ID,Sigorta ,Kasko , Bireysel |
| Tamir Başlangıç ve Bitiş tarihi |Başlangıç Tarihi,Bitiş Tarihi,Tamir Süresi,Gecikme Sebepleri(Varsa)|
| Fiyatlandırma  | Tamir Türü Fiyatı , Parça Fiyatları, İşçilik Ücreti, Vergilendirme, İskonto, Toplam Fiyat,Ödeme Tipi, Ödenme Durumu|


Varlık-İlişki Tablosu:


| Varlık 1 | Varlık 2  | İlişki| 
|----------------------|-----------------------|----------------------|
| Müşteri | Araç |Sahibi(1-N)|
| Müşteri | Fiyat|Öder(1-N)|
| Araç | Ruhsat |Vardır(1-1)|
| Araç | Fiyat |Etkiler(1-N)|
| Personel| Tarih |Belirler(N-N)|
| Personel | Fiyat |Belirler(N-N)|
| Tamir | Fiyat |Etkiler(1-N)|







Projenin E-R diyagraımı aşağıda gösterilmiştir:

![image](https://github.com/user-attachments/assets/c86d9d5e-64db-4c70-a123-00bbb42522e8)



