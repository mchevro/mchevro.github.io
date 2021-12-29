---
layout: post
title: Cara Jalankan C++ Di VsCode
---

## Introduction
Mau running c++ di vscode kok gk bisa ya?😕, padahal udah ikutin tutorial di YT pake keyword "Cara jalankan c++ di vscode" tetep aja gk bisa😒. 
dah lah pasrah gk mau ngoding😜...

Tunggu dulu brother mungkin aja lu salah pada saat installasi atau lu cuman next next aja pas install tanpa ngeliat installasi itu berhasil atau enggak🤭. 

Disni gw mau share sedikit cara jalankan C++ menggunakan Visual Studio Code atau disingkat VsCode😎. Langsung aja gass ke tutornya⬇️

## Step 1 (VsCode & Extension)🔥
> **Visual Studio Code** adalah text editor yang berguna untuk menulis code dengan beberapa fitur seperti highlight sintaks, autocomplate code dan beberapa fitur lain bisa didapatkan dengan cara install **Extension** tertentu.

[1]. Download VsCode melalui link ini brother [Visual Studio Code](https://code.visualstudio.com/download).

[2]. Install VsCodenya, tinggal di next next aja kalo ini✌️.

[3]. Setelah install berhasil, buka VsCodenya dan ke menu **Extensions** dibagian sebelah kiri, atau bisa tekan **ctrl+shift+x**.

[4]. Cari extension **C/C++** dan klik install extensionya, seperti gambar dibawah ini ⬇️

![image](https://user-images.githubusercontent.com/67460437/147690736-c4910089-ad50-4809-8eb3-f2079178e3cd.png)

[5]. Cari extension **Code Runner** dan klik install extensionya, seperti gambar dibawah ini ⬇️

![image](https://user-images.githubusercontent.com/67460437/147690927-e35ca9a2-173a-44e0-b992-007b76f37f2e.png)

## Step 2 (MSYS2 For Windows)
> **MSYS2** adalah tools instalasi paket yang berguna untuk menginstall GCC++ atau disebut dengan compiler, yang berguna untuk mengubah source code C++ ke bahasa mesin agar dapat dijalankan dikomputer

[1]. Download MSYS2 [disini](https://github.com/msys2/msys2-installer/releases/download/2021-11-30/msys2-x86_64-20211130.exe).

[2]. Setelah download selesai, jalankan **MSYS2** untuk melakukan installasi. Wajib 64 Bit Windows 7 atau Windows terbaru.

[3]. Lokasi installasi disarankan di C:\msys64. seperti gambar dibawah ini ⬇️

![image](https://user-images.githubusercontent.com/67460437/147695232-c0cc7499-e78c-4344-a495-c9373cee57e1.png)

[4]. Jika sudah selesai, jalankan **MSYS2**.

[5]. Pastikan sudah terbuka terminalnya, dan ketikan *pacman -Syu*, seperti gambar dibawah ini ⬇️, dan ketikan Y

![image](https://user-images.githubusercontent.com/67460437/147695670-ba119409-9695-47cd-b35d-3e9797be5b60.png)

[6]. Jika update package sudah berhasil, ketikan Y, seperti gambar dibawah ini ⬇️, nanti akan tertutup terminalnya.

![image](https://user-images.githubusercontent.com/67460437/147695911-a6e70ef6-492c-4840-b184-58f1c59fb52a.png)

[7]. Jalankan kembali **MSYS2 MSYS** di menu start windows, seperti gambar dibawah ini ⬇️

![image](https://user-images.githubusercontent.com/67460437/147696124-e16e3e94-2ffe-4256-9185-0284706b004f.png)

[8]. Jika terminal sudah terbuka, ketikan *pacman -Su* untuk perbarui sisa paket dasar, seperti gambar dibawah ini ⬇️, dan ketikan Y

![image](https://user-images.githubusercontent.com/67460437/147696317-be5771c8-e8d6-4ba5-aa5e-64cb0e55ae7e.png)

[9]. Langkah selanjutnya install beberapa tools dan mingw-w64 GCC untuk compilernya. Ketikan *pacman -S --needed base-devel mingw-w64-x86_64-toolchain*, jika ada pertanyaan **Enter a selection (default=all)** di enter saja, lalu ketik Y, seperti gambar dibawah ini ⬇️ 

![image](https://user-images.githubusercontent.com/67460437/147697424-d516d9c7-50fc-468f-bf74-e6d7f0193c05.png)

[10]. Jika cara diatas sudah berhasil dilakukan, silahkan tutup terminalnya dan buka **MSYS2 MinGW 64-bit**, seperti gambar dibawah ini ⬇️

![image](https://user-images.githubusercontent.com/67460437/147697704-7d9150cc-774c-4b7f-bb07-cb0d129aa92f.png)

[11]. Sekarang sudah berhasil nihh brother installasi compilernya. Untuk test coba ketikan gcc, seperti gambar dibawah ini ⬇️. Disini error karena tidak ada file yang mau dicompile, tetapi sampai disini membuktikan bahawa gcc berhasil diinstall😲.

![image](https://user-images.githubusercontent.com/67460437/147697792-702078e8-bdb7-4449-90e3-fae4bfe1e607.png)

## Step 3 (Setting Environment Windows)
> **Edit the system environment variables** berguna untuk command prompt mengenal perintah *gcc* untuk compile file C/C++

[1]. Ketik dipencarian windows **Edit the system environment variables**, seperti gambar dibawah ini ⬇️

![image](https://user-images.githubusercontent.com/67460437/147698178-961e5c8f-bc7e-4e02-ba67-921d19cc1795.png)

[2]. Klik **Environment Variables**, seperti gambar dibawah ini ⬇️

![image](https://user-images.githubusercontent.com/67460437/147698322-6308a5c5-857a-4621-80fa-9287b7f48cc3.png)

[3]. Edit Path, seperti gambar dibawah ini ⬇️

![image](https://user-images.githubusercontent.com/67460437/147698450-1168686f-5dce-4102-a7ff-c24004c042eb.png)

[4]. Klik New dan tambahkan directory **C:\msys64\mingw64\bin** seperti gambar dibawah ini ⬇️ jika memang anda mengikuti tutorial dari awal🤪

![image](https://user-images.githubusercontent.com/67460437/147698705-b51be7d7-d906-4ab7-aecd-01932b114209.png)


