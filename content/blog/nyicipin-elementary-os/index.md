---
title : Nyicipin Elementary OS
date : 2023-04-28
featured_image: images/01.jpeg
featured: false
draft: false
"blog/tags": [ linux, ubuntu ]
---

Buat yang belum tau, [elementaryOS 7](https://en.wikipedia.org/wiki/Elementary_OS) ini Linux/GNU. Elementary OS termasuk turunan dari Ubuntu LTS. Makanya package managernya pake APT, dan Desktop Environtmentnya (DE) masih setia menggunakan [Pantheon](https://en.wikipedia.org/wiki/Elementary_OS#Pantheon_desktop_environment), bukan gnome atau KDE gitu.

Jadi ceritanya saya lagi kangen sama Linux, dan pengen cobain kembali menggunakan Linux setelah sebelumnya pake hackintosh di Thinkpad X250 saya ini. 

![Elementary OS 7](images/1.jpeg)

Sebelumnya saya pernah juga install linux selain elementaryOS di Thinkpad X250 saya ini, seperti: Pop\_OS, Garuda Linux, dan Arch Linux. Dan yang paling oke untuk thinkpad x250 saya ini kebetulan ya elementaryOS 7 ini. Walaupun DE nya simpel engga bisa dikastem dengan leluasa seperti gnome ataupun kde, tapi yang penting stabil dan tetap bisa digunakan menurut saya udah bagus sih.

Soalnya pengalaman saya ketika menggunakan PopOS/Garuda Linux/Arch Linux, ada beberapa bug yang ngeselin dan entah gimana caranya lagi buat benerin. Akhirnya balik lagi ke Windows.

Oiya saya pake dualboot Windows 10 dengan elementaryOS 7 ini biar kalo sewaktu-waktu butuh aplikasi khusus win 10, saya tinggal boot ke windows. Misalnya pas lagi butuh pake [3tools](http://www.3u.com/), aplikasi khusus management iOS (Backup, restore, maintenance, dll). Atau misalnya saya butuh bikin instalasi win10 yang cuman bisa pake Rufus. Saya pernah coba burning flashdisk pake apps di linux tapi ga ada yang jalan (untuk saat ini).

## First Impression

elementaryOS 7 ini feelnya sekilas mirip banget sama macOS. seperti dock, taskbar dan ui beberapa aplikasi bawaannya. Tapi ketika makin mendalami elementaryOS, bakal tau bedanya gimana 😅.

Mungkin impression ini beda tiap pengguna laptop/PC, tapi di Thinkpad X250 saya ini bener-bener flawless, maksudnya dari driver semuanya kebaca. Beda ketika saya menggunakan Pop\_OS. Ada bug pada driver vganya, jadi setiap boot selalu kepilih hi-DPI yang bikin tampilan jadi kecil resolusinya. Dan gamepad wireless 8bitdo zero saya juga ga kebaca di Pop\_OS 😭. 

Tapi masalah di OS sebelumnya itu engga saya temuin di elementaryOS, kecuali mungkin masalah management ram. 😅

## Aplikasi Alternatif

Perlu saya jelaskan juga kalau saya mengunakan Linux sebenernya udah cukup lama, kalau bisa dihitung mungkin dari tahun 2008. Tapi mulai agak intens dan pake buat gantiin Windows itu mungkin sekitar tahun 2017-2018. 

Jadi sebenernya saya bukan fulltimer pengguna Linux juga. Hanya sesekali aja ketika penasaran dengan OS tersebut.

Nah, mungkin banyak yang penasaran bagaimana cara beradaptasi dari yang sebelumnya pake Windows kemudian tiba-tiba menggunakan Linux? Saya akan jelasin beberapa aplikasi alternatif yang saya gunakan di Linux sebagai pengganti aplikasi yang biasa saya gunakan di Windows.

- **Office.** Kalau di Windows tentunya saya menggunakan Microsoft Office, di Linux saya menggunakan LibreOffice 7.5 yang udah lebih baik lagi. Tapi tentu saja format kedua aplikasi ini masih tidak flawless, maksudnya ketika dipindah edit, ada saja format tulisan yang berubah. Dan untuk spreadsheet tentu saja ada formula yang di excel jalan, di Libre office ga jalan. Tapi karena saya kebanyakan pake Google Docs buat kerjaan, jadi engga ada masalah formatting 😁.

- **Vector Editing.** Di Linux saya menggunakan [Figma for Linux](https://github.com/Figma-Linux/figma-linux) (karena figma ga ada aplikasi resmi untuk linux), dan inkscape. Bahkan fitur inkscape labih banyak kepake buat saya semisal butuh tracing gambar jpeg ke vector. Sisanya buat bikin poster atau apapun saya malah seringnya bikin di Figma atau di Canva.

- **Image Editing.** Kalau di Windows kan biasanya pake Photoshop atau Affinity Photos, di Linux saya pake Gimp, dan ringannya luar biasa untuk editing kecil semacam hapus bg, manipulasi, dan editing simpel yang biasa saya lakukan, di gimp udah cukup banget. 

- **Video Editing.** Kalau di windows saya biasa pake Adobe Premiere dan Capcut, di Linux ada Kdenlive yang mirip banget workflow nya sama Premiere pro. Dan untuk animasi pendek saya malah pake Canva 🫣

-  **Gaming.** Karena saya terbiasa gaming di windows pake steam, jadi pake steam di Linux juga udah cukup kok, apalagi karena ada project proton steam yang bikin game windows bisa dimainin dengan lancar di Steam Linux.

- **XAMPP.** Kok dimasukin? Soalnya biar kamu tau aja, kalo pake xampp di Linux itu engga seenak pake di Windows. Sebenernya sih di linux udah bisa install satu-satu php, mysql, dan apache, tapi buat yang sering ganti-ganti php gitu dan ga mau mengubah/mempengaruhi sistem, kamu bisa pake [LocalWP](https://localwp.com/). Dan saya baru tau ini pas pindah ke elementaryOS 😅. 

- **Screenshots.** Nah ini soalnya kerjaan saya itu banyak membutuhkan screenshot. Kalau di Windows saya biasa pake [ShareX](https://getsharex.com/), kalo di elementaryOS saya pake bawaan OS nya aja, udah cukup fiturnya buat saya.

- **Clipboard Manager.** Nah ini kalo di windows kan bisa pake Win+V, kalo di linux itu ada banyak, dan biasanya di tiap DE udah ada fiturnya masing-masing. Kalau saya sendiri pake [CopyQ](https://hluk.github.io/CopyQ/). Udah sangat membantu karena kerjaan banyak fungsi copas-copas.

- **PDF Reader.** Saya pake bawaan, dan enakan di Linux ketimbang di Windows. Windows sendiri ga punya pdf bawaan (malah pake Edge buat baca pdf), kalo di windows saya malah install SumatraPDF yang ringan. Kalo di Linux bawaannya udah enak banget.

- **Ebook Management.** Untungya Calibre udah terenak dan terlengkap yang multiplatform juga. Jadi ga perlu cari alternatifnya lagi.

- **Note Taking.** The One and only yang saya pake yaitu Obsidian udah multiplatform, dan saya tinggal pake Github buat sync tulisan saya dari windows ke Linux. Jadi ga perlu cari alternatifnya lagi.

---

Untuk beberapa aplikasi yang sudah multiplatform sebenernya udah banyak yang udah support Linux. Seperti Zoom, VSCode, Steam, VLC, Calibre, Chrome/Brave, Spotify, Anydesk, Obsidian, dan banyak lagi. Jadi ga perlu cari alternatifnya lagi.

## Apakah elementaryOS 7 cocok buatmu?

Tentu saja belum tentu. 🫣

Dan Linux itu bukan untuk semua orang.

Karena masih banyak aplikasi windows yang belum disupport walaupun pakai aplikasi container seperti wine. Kalaupun pakai virtual machine, tentu beda rasanya ketika dibuka menggunakan OS Windows sendiri. 

Misalnya saja yang terbiasa bekerja dengan adobe family, tentu ga bisa pake linux. Bahkan file Office saja masih banyak perubahan format ketika menggunakan beda aplikasi Windows dan Linux. 

Udah gitu install aplikasi di Linux itu engga semudah di Windows yang download tinggal install, masih ada saja pengaturan biar si aplikasi itu berjalan dengan mulus. Ya walaupun sudah ada Store dan Flathub yang memudahkan kamu install aplikasi Linux. 

Tapi learning curve dari Windows ke Linux itu cukup sulit buat yang agak males belajar OS lagi 😅. Beda dengan macOS yang learning curve nya masih mudah.

Tapi coba pikirkan ini.

Ketika saya install linux itu semua driver hardware thinkpad x250 saya itu keinstall dengan sendirinya. Beda ketika saya harus download-download lagi driver yang cocok buat thinkpad x250 di windows 😅. 

Bahkan windows itu sendiri engga gratis, kecuali laptopnya sudah terinstall windows. Kamu secara legal harus beli OS windows yang engga murah juga. 

Kecuali kamu ada email sekolah, kamu bisa dapet license windows gratis. 

Tapi kalo engga? 

Udah bener sih Linux ini solusi murah apabila OS nya kebanyakan digunakan untuk membuka aplikasi Web. 👌
