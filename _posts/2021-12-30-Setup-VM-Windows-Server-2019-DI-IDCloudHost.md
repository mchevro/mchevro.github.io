---
layout: post
title: Setup VM Windows Server 2019 Di IDCloudHost
---

## Introduction
Kali ini gw mau share cara setup VM dengan OS windows server 2019, yang dimana nanti berguna untuk di next tutorial ini✌️. 

Sebelumnya gw mau sedikit cerita, jadi tujuan gw setup VM ini untuk kuliah matkul *Sistem Manajemen Basis Data* yang mengharuskan gw install tools DBMS yaitu MS. SQL Server. 
Yang jadi permasalahanya adalah penyimpanan laptop gw udah gk cukup untuk install ini tools😪, jadi gw memutuskan untuk cari alternatifnya dengan cara membeli server dengan
harga yang sangat murah, atau bisa dibilang kita disini hanya sewa server pada saat diperlukan saja😲. Jadi langsung gass ke tutorialnya ⬇️

> Syarat untuk mengikuti tutorial ini anda harus sudah mempunyai akun IDCloudHost dan memiliki saldo minimal yaitu 50K. Saldo 50K ini syarat minimal Top Up di IDCloudHost dan nanti saldo ini tidak langsung habis tetapi untuk deposit agar bisa membuat VM dengan biaya perjam.


## Step 1 (Set Up VM)
[1]. Login ke Console [IDCloudHost](https://console.idcloudhost.com/hub/login).

[2]. Sekarang kita sudah berada di dashboard untuk nanti membuat VM.

![image](https://user-images.githubusercontent.com/67460437/147764905-0dd96d2a-36a7-478c-8b1a-37fdff742b55.png)

[3]. Klik Virtual Machine, seperti gambar dibawah ini ⬇️

![image](https://user-images.githubusercontent.com/67460437/147765143-1c4af356-a060-4155-b32c-27dcef8aedd5.png)

[4]. Pilih OS Windows Version 2019, seperti gambar dibawah ini ⬇️. Untuk spesifikasi sesuaikan dengan kebutuhan saja. Disini gw pake CPU 4 Core, Ram 8 GB, Disk 40 GB dengan **biaya sebesar 875K/Bulan**. Inget ini biaya **perbulanya, bukan biaya perjam**. Untuk biaya perjamnya dengan harga Rp 1.199 yang berarti gw biasa pake paling lama sekitar 5 Jam hanya mengeluarkan biaya sekitar Rp 5.995 saja😲. 

![image](https://user-images.githubusercontent.com/67460437/147765584-fac15f85-23bb-4aee-b5fd-a067c7b33b12.png)

[5]. Kita scrool kebawah untuk konfigurasi terakhir, seperti gambar dibawah ini ⬇️. Isi password untuk login VM nanti dan berikan label nama untuk ditampilkan di dashboard IDCloudhost.

![image](https://user-images.githubusercontent.com/67460437/147767673-6b9f7594-2b60-45c1-bcba-8e872778e4ef.png)

[6]. Jika semua konfigurasi diatas sudah terpenuhi, langkah selanjutnya adalah tekan button create yang berada di kanan bawah, seperti gambar dibawah ini ⬇️

![image](https://user-images.githubusercontent.com/67460437/147767897-79a456b0-62ac-4903-bf5b-517eddf32eca.png)

[7]. Tunggu beberapa saat sampai proses selesai☕.

![image](https://user-images.githubusercontent.com/67460437/147767969-d33d041e-2620-4d7f-b15e-08fb6bff9ecd.png)

## Step 2 (Akses VM Dengan Virtual Console)
[1]. Setelah proses selesai, klik VM yang telah dibuat, seperti gambar dibawah ini ⬇️

![image](https://user-images.githubusercontent.com/67460437/147768306-0c9f99d5-c8d1-457b-96cb-25fa5a53cf0f.png)

[2]. Sekarang saatnya akses VM dengan cara klik **Virtual Console**, seperti gambar dibawah ini ⬇️

![image](https://user-images.githubusercontent.com/67460437/147768585-7c546a5a-b3c1-4870-ae49-9537c4365953.png)

[3]. Klik **Ctrl+Alt+Delete**, seperti gambar dibawah ini ⬇️ untuk kita login ke windowsnya.

![image](https://user-images.githubusercontent.com/67460437/147768739-d12a20af-8fcd-4985-beda-3e197a65e4de.png)

[4]. Ketikan password yang dibuat sebelumnya, seperti gambar dibawah ini ⬇️, lalu tekan enter.

![image](https://user-images.githubusercontent.com/67460437/147768878-132fea52-85a5-4993-9a2a-94d068137224.png)

[5]. Sekarang anda sudah berhasil akses ke windows dengan sangat mudah 😎.

![image](https://user-images.githubusercontent.com/67460437/147768963-dc46c477-1967-44b1-9396-174c5c9a808a.png)

## Important ⚠️
Harga diatas dengan biaya sekitar Rp 1.199 yang gw bilang sebelumnya belum termasuk dengan biaya penyimpanan yang dikenakan sekitar **25K/Bulan**☹️. Jadi untuk menghemat pengeluaran gw sangat sarankan setelah digunakan hapus saja VM yang dibuat sebelumnya, agar tidak dikenakan biaya tambahan🥱. 

Untuk cara delete VM klik tab *VM-Kampus*, seperti gambar dibawah ini ⬇️

![image](https://user-images.githubusercontent.com/67460437/147770356-aee76096-0286-4d17-87d1-da388d1f477b.png)

Selanjutnya bisa klik tulisan **Delete**, seperti gambar dibawah ini ⬇️

![image](https://user-images.githubusercontent.com/67460437/147770449-58947a36-6f4d-4c93-bcfc-42f05c46c993.png)

Tunggu beberapa saat dan pastikan proses **Delete** telah berhasil dilakukan🙈.

## Closing


