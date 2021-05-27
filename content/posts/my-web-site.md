---
title: "Hugo ile oluşturduğum web sitesi"
slug: "my-web-site"
description: "Web Sitesi"
date: 2021-04-22T20:25:38+02:00
weight: 2
draft: false
---
Hugo ile nasıl static web sitesi nasıl oluştuduğumdan anlatıcağım.<!--more-->

İlk olarak google domainsten bir domain adresi aldım. Bu domain adresinin DNS ayarlarını kontrol etmek için [cloudflare](https://www.cloudflare.com/) yönlendirdim.

Domain işlerimi hallettikten sonra site oluşturma kısmı halletmem gerekiryordu. Bunun için [Hugodan](https://themes.gohugo.io/) bir tema seçmem gerekti. Tema işini hallettikten sonra [Hugonun](https://gohugo.io/getting-started/quick-start/) kendi sitesinde ki tutorial kısmını takip ederek bir static site oluturmuş oldum.

Oluturmuş olduğum bu site local bilgisayarımda çalışıyordu.Burada github pages devreye giricek.

[Github pages](https://pages.github.com/), github repository bulunan web sitemi domainme yönlendirmekle kalmayıp bir ubuntu cihaz üzerinde otomatik oluşturup bir hata olup olmadığınıda sana geri bildiriyor. Böylelikle yeni bir post paylaştığınızda kendinizin test etmesine gerek kalmıyor. 

Son olarakta githup pagesı cloudflare yöneldirmek kaldı. Burada da [github docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site) bulucağınız A tipi kayıtları DNS ayarlarnıza girerseniz halletmiş oluyorsunuz. 



