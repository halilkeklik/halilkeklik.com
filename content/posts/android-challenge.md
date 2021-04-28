---
title: "Arabam.com stajyer android challenge"
slug: "android-challenge"
description: "Android challenge"
date: 2021-04-28T15:50:00+02:00
draft: false
---
# Arabam.com stajyer android challenge
 Merhabalar,
 
Burada size Arabam.com staj başvurum sonucu bana verilen challenge nasıl yaptığımdan bahsedeceğim.

Başvurama olumlu dönüş aldığım zaman bize android bilgimizi ölçmek için 2 hafta içinde istedikleri projeyi bitirmemizi istiyorlardı.Proje kısaca 2 sayfadan oluşan bir uygulamaydı.Bu iki sayfa birinde araçların listesi gözükmesi diğerinde ise listeden seçilen bir aracın detay sayfası olması gerekiyordu.Proje detayını [buradan](https://github.com/halilkeklik/android-assignment/blob/main/CHALLENGE_README.md) bulabilirsiniz.

Şunu belirtmeliyim ki bu challengedan önce sadece basit bir kaç android projesi ve birkaç temel android tutorial videosu dışında bir bilgim yoktu.Bu yüzden challengeda bizden istenen birçok şeyi bilmiyordum bundan dolayı ilk 2 günümü araştırma yaparak geçirdim.Araştırma sürecim bittiğinde projeye başlama zamanım gelmişti.

Proje başlarken neresinden başlamam gerektiğine emin olmamıyordum.O yüzden tanıdığım birkaç insana danıştıktan sonra ilk önce ui kısımlarını halletmeye karar verdim.Çünkü daha önce android üzerinde ui ile ilgili işler yapmıştım ne kadar basit olsalarda.Ui kısımlarını hallederken bir yandan da API ve Pagination ile ilgili araştırmalar yapmanın bana zaman kazandıracağını düşünmüştüm.

Projede 1 adet activity kullandım. Uygulama içindeki ekranlar için fragmentları kullandım. Fragmentların hepsini activityde yönettim.

Fragmentleri yapmadan önce API işlerini sonraya bıraktığım için kendim bir static bir liste oluşturdum.Bu listeyi API uygun bir şekilde oluşturdum.Herhangi bir deneme yapacağım zaman bu oluşturduğum liste üzerinden yaptım.Bu listeyide Repository aldı dosya altında classın içinde oluşturdum böylelikle herhangi bir değişiklik yaptığım zaman class içini değiştirmem yetecekti.

Elimde bir liste vardı artık o yüzden ilk ekranımı oluşturmam gerekiyordu.İlk önce listeleme ekranını oluşturdum.Bu ekranda arbaları listelmek için recyclerview kullandım.İlk 2 günü araştırma yaptığımı söylemiştim, bu araştırmalar sonucunda liste oluşturmak için en verimlisi recyclerview olduğuna kanaat getirdim.Seçilen aracın detay sayfası görünmesi için arabaların id bir yerde tutmam gerekiyordu bunun için bundle kullandım. 

Artık liste ekranım olduğuna göre artık geriye detay ekranım kalmıştı.Detay ekranında API baktığımda bazı verilerin sabit olarak geldiğini bazılarının liste halinde geldiğini farkettim.Bu yüzden liste halinde gelen veriler için ayrı bir recyclerview oluşturdum.Arabanın fotografları göstermek için viewpager kullandım. Birden fazla image göstermek için kullanışlı olduğunu düşünüyorum.

Artık ekranlarım hazır olduğuna göre kendi oluturduğum liste yerince API dan gelen liste göstermem gerekiyordu.HTTP isteklerini verilen API'den data alabilmek için retrofit kullandım.Bize verilen API retrofit kullanarak erişmiştim geriye repository oluşturdupum classı buna uygun bir şekilde modifiye etmek kalmıştı.

Artık listeleme ekranımda API dan gelen liste gözüküyordu.Ama sabit bir liste geliyordu.Pagination için "androidx.paging:paging" kütüphanesini kullandım. Çünkü bu kütüphane paginationın büyük kısmını kendisi hallediyor ve bu benim işimi kolaylaştırdı.

Size bana gelen android challenge yaparken neler düşündüğümü, nasıl yaptığımı, hangi adımları takip ettiğimi kabaca anlattım.Projenin tüm detaylarını bu [github reposunda](https://github.com/halilkeklik/android-assignment) bulabilirsiniz.


