---
layout: post
title: References
permalink: /References/
date:   2016-05-17 14:51:20 +0300
backcolor: 43b02a
fontcolor: fff
---

## Mobiliz NG(Next Generation) Web Uygulama Arayüzü
Bu repo; araç takip ve filo yönetimi uygulaması için geliştirilen web arayüzü kaynak kodlarını içerir.


[Canlı Ortam](https://ng.mobiliz.com.tr) | [Geliştirme Ortamı](https://ngtest.mobiliz.com.tr)

## Kurulum
* İlgili branch geliştiricinin bilgisayarına clone'lanır; <br />
`git clone -b {branch} https://{kullanıcı}:{şifre}@github.com/MobilizIT/ng-ui.git`

## Çalıştırma
* Uygulamayı çalıştırmak için 3 adet `task` bulunmaktadır.
    * `default` : `gulp` konfigürasyonunda tanımlı `local` api'de tanımlı olan adrese bağlanmaya çalışır. Dosyalardaki değişimleri izler, `8888` portunda çalışmaya başlar.
    * `local` : `default` taskındaki aynı işlemler geçerlidir.
    * `integration` : Dosya değişimlerini izlemez, ayrıca web sunucusu ayağa kaldırmaz. Sadece dosyaları başka bir sunucuda çalıştırmak için `dist` dizinine hazırlar. Kaynak kod analizi için `plato` taskını çalıştırır ve `dist/report` dizini altına dosyaları hazırlar.
    * `release` : Dosya değişimlerini izlemez, ayrıca web sunucusu ayağa kaldırmaz. Dosyaları gerçek ortama göndermek için `dist` dizini altına hazırlar.

Örnek çalıştırma parametreleri aşağıdaki gibidir:
* `gulp` : `default` task ile işlem yapar.
* `gulp local` : `gulp` ile aynı task'ı çalıştırır.
* `gulp integration` : gulp konfigürasyonu içerisindeki `environmentConstants` task'ında belirtilen `integration` parametresine göre işlemleri başlatır. Uygulama `https://ngtest.mobiliz.com.tr/service1` adresinden veri alacak şekilde ayağa kalkar.
* `gulp local --api=integration --vendor=globefleet --appversion=2.04.0` :
* `api`, `vendor`, `appversion` parametreleri tanımlanmadan çalıştırılırsa default değerlerine göre dosyalar oluşturulur.

## Vendor Listesi
Arayüzün hangi müşteriler için özelleştirileceğini belirtir listedir. Bu listedeki verilere göre API, logo ve sayfa başlık değerleri değiştir.

Listenin mevcut hali: `var applicationVendor = [{vendor: 'filoturk', title: 'FiloTürk'}, {vendor: 'globefleet', title: 'GlobeFleet'},
                         {vendor: 'elcobil', title: 'Elcobil'}, {vendor: 'aplusa', title: 'CarTrack'},
                         {vendor: 'etit', title: 'ETIT'}, {vendor: 'castrol', title: 'Castrol Filozof'}];`

## Notlar
* Geliştirmeleri ve commitlerimizi `develop` şimdilik branch'ine yapıyoruz.
* Kodun mevcut halinde minify ya da obfuscate işlemleri yapmıyor.

## Versiyonlar
* v2.03.1
* v2.02.0
* v2.01.1
* v2.01.0
* v2.00.4.2
* v2.00.2


## Lisans
Tüm hakları Mobiliz A.Ş.'ne aittir. &copy; 2016
