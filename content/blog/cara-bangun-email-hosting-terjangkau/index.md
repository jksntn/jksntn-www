---
title: Cara Membangun Email Hosting dengan Harga Terjangkau
date: 2023-05-28
featured_image: images/email2.png
featured: false
draft: false
blog/tags:
  - e-mail
  - web development
---
Sebelum menjelaskan ini, perlu kalian ketahui dulu kalau email hosting itu cukup mahal, bahkan yang gratisan seperti zoho dan Yandex membatasi fitur gratisnya, sehingga ada hal yang menyebalkan seperti email engga kekirim dan banyak hal lainnya.

## Perbandingan Harga

Email hosting berbayar yang bagus dan paling murahpun sebenernya masih mahal, untuk Google sendiri seharga $4.20, yang termurah mungkin adalah Zoho lite, itu seharga $1. Dan yang untuk lokal sendiri (Niagahoster) seharga Rp80.000. Kalau kalian concern sekali dengan service lainnya seperti google workplace yang banyak sekali fiturnya seperti google docs, meet, dll. mending pilih Google aja, tapi perhatikan itu $4.20 hanya untuk 1 orang/alamat email ya, kalau usernya ada 20 orang tinggal dihitung saja 😅.

![Perbandingan Harga](images/email2.png)

Tapi kalau kalian hanya butuh email yang bisa digunakan untuk bisnis/ menggunakan domain kalian sendiri, saya menyarankan hal ini.

Supaya email hosting biayanya bisa saya tekan lebih murah lagi, saya menggunakan: 

1.  Domain (my.id seharga Ro10.000/tahun) 
2.  DNS/Domain manager menggunakan [Netlify](https://www.netlify.com/) (gratis) 
3.  Shared hosting (gratis, saya numpang addon domain doang ke temen 😅) 
4.  Email gratisan dari google sebagai storagenya.

{{< announcement content="<p class='title'>Catatan</p>Sebenarnya untuk DNS manager ga perlu menggunakan Netlify, bisa menggunakan dns manager bawaan dari penyedia domain, atau menggunakan yang gratisan lainnya yang bagus seperti Cloudflare. Kebetulan saat ini saya sudah menggunakan Netlify yang juga untuk kebutuhan deploy web Static." >}}

![Infrastruktur Email](images/email1.png)

Kalau melihat di gambar di atas, ada 3 infrastruktur, yaitu:  

-   DNS manager (Netlify)
-   Shared hosting (sebagai server email)
-   Email google gratisan (Storage dan email alias).

## Setup DNS

Di Netlify saya menambahkan mx record yang diarahkan ke ip server shared hosting saya. Dengan catatan, di shared hosting tadi harus sudah menambah addon domain jksntn.my.id saya. Sisanya seperti SPF dan DKIM nya saya tambahkan record txt nya di DNS manager (di Netlify).

Supaya tidak ada masalah, pastikan IPnya mengarah ke shared hosting, karena kalau salah atau IP Shared hostingnya berubah, servernya bakal error engga bisa menerima dan mengirim email.

![](images/email3.png)

## Setup di Server Shared Hosting

Di shared hostingnya, hal yang perlu dilakukan adalah menambahkan (addon) domain di shared hostingnya (kalau yang saya pake cpanel). Kalau sudah, langsung cek aja Deliverability (seperti di gambar), pastikan alamat IP servernya sudah ditambah di mx record DNS managementnya.

Kalau masih ada error, tambahkan/pastikan SPF dan DKIM record sudah ditambah recordnya di DNS management.

![](images/email4.png)

Setelah itu tinggal ditambah alamat emailnya di Shared hosting ini, nanti akan ada email awal yang masuk berisikan instruksi setup/credential apabila mau dipasang di Client Email (smtp,pop3, port, dll).

![](images/email5.png)

## Setup di Email Google gratisan

Nah fungsi Email Google gratisan adalah supaya memudahkan mengecek email yang masuk, dan yang terpenting sebagai pengganti email storage yang masuk (pastiin setup pop3nya jangan save copy email ke server, supaya hanya masuk ke email gratisan google kita).

![](images/email6.png)

![](images/email7.png)

## Final Verdict

Nah gaes, dengan cara ini saya bisa hemat banget pengeluaran untuk membangun email hosting. Ini juga bisa digunakan untuk membangun email bisnis awal-awal apabila kalian membangun bisnis sendiri.

Semoga bermanfaat. 👌
