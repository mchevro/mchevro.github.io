---
layout: post
title: Cara Fix Masalah Koneksi Ke VPN L2TP Windows 10
---

## Introduction
Beberapa hari lalu gw mencoba membuat akun VPN di [Tunnel Lapan Tech](https://tunnel.lapan-tech.com/), Tapi pas gw coba koneksikan ke pc gw yang menggunakan windows 10 tidak bisa terkoneksi😔. 

Pada saat itu gw buat menggunakan jenis VPN L2TP, sementara itu pas gw coba terkoneksi dengan jenis PPTP itu bisa terkoneksi dengan lancar di pc gw. Hmm keliatanya ada yg aneh disini🤔, gw sempat berpikir mungkin ini masalah dari server [Tunnel Lapan Tech](https://tunnel.lapan-tech.com/)🙄. 

Setelah gw mencoba terkoneksi menggunakan HP ternyata bisa jalan dengan jenis L2TP, berarti permasalahnya bukan di servernya, tetapi di pc gw🙈. Sekarang gw mau coba share cara gw memperbaiki permasalahan ini dengan sangat mudah😎. Cek dibawah ini ⬇️


## Error Yang Gw Alami
> seperti gambar dibawah ini ⬇️ lah error yang gw alami.

![image](https://user-images.githubusercontent.com/67460437/147941997-0ccdafcc-83f5-44dd-b950-0047698efb75.png)

## Step 1 (Bypass Koneksi)
> Secara bawaan windows gk mendukung koneksi jenis VPN L2TP/IPsec kalo server VPN berada di belakang NAT. Jadi untuk handle masalah ini kita bisa ubah *registry*.

[1]. Buka *registry* editor, seperti gambar dibawah ini ⬇️.

![image](https://user-images.githubusercontent.com/67460437/147961138-f71b15da-53b1-4a6c-a51e-abe5b9086476.png)

[2]. kita akan menambahkan *key* dengan cara klik panel dikiri dan buka directory **HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Sevices\PolicyAgent**, seperti gambar dibawah ini ⬇️.

![image](https://user-images.githubusercontent.com/67460437/147961805-e2e8d85f-ce74-47e5-a825-50b725a338a4.png)

[3]. Klik kanan di space kosong lalu klik **New > DWORD (32 bit) Value**. Lalu isikan *key* baru ini dengan nama **AssumeUDPEncapsulationContextOnSendRule** dan enter, seperti gambar dibawah ini ⬇️

![image](https://user-images.githubusercontent.com/67460437/147962263-6773cd12-f6bb-4e00-8038-120c0c4d7b7e.png)

[4]. Jika sudah dibuat kemudia klik kanan pilih **modify** dan isikan Value data **2**, seperti gambar dibawah ini ⬇️. lalu Ok 

![image](https://user-images.githubusercontent.com/67460437/147962379-8fc6cada-e8cb-4382-84cd-6a3f14b0a0e9.png)

## Step 2 (Restart PC)
Setelah langkah diatas dilakukan, laptop/pc kita harus wajib direstart agar perubahan yang kita lakukan bisa berjalan dengan lancar😎.

## Closing
Langkah diatas kemungkinan berhasilnya sangat besar. Jadi jika permasalahan ini belum bisa juga silahkan anda hubungi pihak penyedia VPN atau ISP anda, Karena ada beberapa ISP yang membelokir trafic VPN karena dianggap berbahaya😲.

Sekian sharing gw kali ini, mohon maaf bila ada kekurangan penulisan✌️. Terima kasih banyak semuanya👋.

## Referensi 
- https://www.wintips.org/fix-cannot-connect-to-l2tp-vpn-in-windows-10-solved/
