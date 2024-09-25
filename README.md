# PRAKTIKUM 5 Job Control

## Nama : Yesi Paramita
## Kelas : SK3B
## NIM : 09011182328116


### Tugas

## **1. Eksekusi seluruh profile yang ada :**

a. Edit file profile /etc/profile dan tampilkan pesan sebagai berikut :
**echo “Profile dari /etc/profile”**

<img width="600" alt="Cuplikan layar 2024-09-25 202648" src="https://github.com/user-attachments/assets/16524576-eb98-4ccc-b138-eca65ac04bd1">

<img width="600" alt="Cuplikan layar 2024-09-25 202551" src="https://github.com/user-attachments/assets/cadbc734-a733-42b7-a82c-6aecd08b20c9">



b. Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :

/home/stD02001/.bash_profile

/home/. stD02001/.bash_login

/home/mahasiswa/.profile

/home/mahasiswa/.bashrc

Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap
file tersebut, cantumkan instruksi echo, misalnya pada /home/ mahasiswa/.bash_profile :
**echo “Profile dari .bash_profile”**
Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang
bersangkutan.

**/home/stD02001/.bash_profile**

<img width="600" alt="Cuplikan layar 2024-09-25 212745" src="https://github.com/user-attachments/assets/b480c6ed-ed9f-4405-98e8-87dfc89acc07">

<img width="600" alt="Cuplikan layar 2024-09-25 212639" src="https://github.com/user-attachments/assets/fb3bed77-9b20-475b-bc89-4c95134f85d7">

**/home/. stD02001/.bash_login**

<img width="600" alt="Cuplikan layar 2024-09-25 212753" src="https://github.com/user-attachments/assets/f63b579f-d57f-4c4d-bb82-591153fd6147">

<img width="600" alt="Cuplikan layar 2024-09-25 212816" src="https://github.com/user-attachments/assets/e5ad7653-cc16-4124-b574-9a41dddf4628">

**/home/mahasiswa/.profile**

<img width="600" alt="Cuplikan layar 2024-09-25 213100" src="https://github.com/user-attachments/assets/1a2c36df-eb01-4c9b-bac6-93c338081cb3">

<img width="600" alt="Cuplikan layar 2024-09-25 212943" src="https://github.com/user-attachments/assets/ae1e509b-a4f5-4c9e-ad39-ed2952e93866">

**/home/mahasiswa/.bashrc**

<img width="600" alt="Cuplikan layar 2024-09-25 213409" src="https://github.com/user-attachments/assets/6c4d4d35-2bb7-4af0-bfdd-954f2749ac29">

<img width="600" alt="Cuplikan layar 2024-09-25 213322" src="https://github.com/user-attachments/assets/aec732c2-5626-458a-9445-2c0a97092cd2">

c. Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:

**$ su mahasiswa**

**$ exit**

<img width="600" alt="Cuplikan layar 2024-09-25 213500" src="https://github.com/user-attachments/assets/7255e231-448a-4c41-8007-856f6474ac46">

kemudian gunakan opsi – sebagai berikut :

**$ su – mahasiswa**

**$ exit**

<img width="600" alt="Cuplikan layar 2024-09-25 213535" src="https://github.com/user-attachments/assets/a9779c15-e383-4ff7-90d9-c69fd78951c5">

Jelaskan perbedaan kedua utilitas tersebut.

= Perbedaannya adalah jika menggunakan perintah su mahasiswa, hanya identitas pengguna yang berubah sementara lingkungan (environment) dari pengguna sebelumnya tetap dipertahankan. Sebaliknya, perintah su - mahasiswa melakukan login baru sepenuhnya, termasuk memuat ulang seluruh lingkungan pengguna baru dari awal.


##**2. Prompt String (PS)**

a. Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell PS1=‟> „ export PS1

<img width="600" alt="Cuplikan layar 2024-09-25 214129" src="https://github.com/user-attachments/assets/83f63316-019b-4c60-8761-9086e9a06b06">

<img width="600" alt="Cuplikan layar 2024-09-25 214200" src="https://github.com/user-attachments/assets/ac0ceb5e-f2ca-42dc-a50c-49539364222d">

b. Eksperimen hasil PS1 : $ PS1=“! > “ 69 > PS1=”\d > “ Mon Sep 23 > PS1=”\t > “ 10:10:20 > PS1=”Saya=\u > “ Saya=mahasiswa > PS1=”\w >” ~ > PS1=\h >”

<img width="600" alt="Cuplikan layar 2024-09-25 215300" src="https://github.com/user-attachments/assets/75671317-6713-4319-b45d-87379146d974">

##**3. Logout**

Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout Echo “Terima kasih atas sesi yang diberikan” Sleep 5 clear

<img width="600" alt="Cuplikan layar 2024-09-25 225901" src="https://github.com/user-attachments/assets/6bf024eb-29fd-40f7-8d70-afa3bbaf3495">

<img width="600" alt="Cuplikan layar 2024-09-26 001744" src="https://github.com/user-attachments/assets/5850a2ac-15a6-4578-8e8d-769bcc308325">

<img width="600" alt="Cuplikan layar 2024-09-25 225901" src="https://github.com/user-attachments/assets/4c93c0f3-8326-46fb-a57c-93e4eb3f99df">

##**4. Bash script**

a. Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing :

p1.sh

#! /bin/bash

echo “Program p1”

ls –l

<img width="600" alt="Cuplikan layar 2024-09-25 230253" src="https://github.com/user-attachments/assets/94b29258-6f9c-4d9d-95c6-276e45018fca">

<img width="600" alt="Cuplikan layar 2024-09-25 230236" src="https://github.com/user-attachments/assets/f66cd50a-f6ac-4ef2-9416-374d6e53f72c">

p2.sh

#! /bin/bash

echo “Program p2”

who

<img width="600" alt="Cuplikan layar 2024-09-25 230316" src="https://github.com/user-attachments/assets/d3707366-b8ff-41d1-bdaf-0246610681c4">

<img width="600" alt="Cuplikan layar 2024-09-25 230404" src="https://github.com/user-attachments/assets/2705ca4f-0fb3-481d-bec7-f48a2e06dd4c">

p3.sh

#! /bin/bash

echo “Program p3”

ps x

<img width="600" alt="Cuplikan layar 2024-09-25 230501" src="https://github.com/user-attachments/assets/f594401b-9c0b-4014-aa13-3f7f112fdab8">

<img width="600" alt="Cuplikan layar 2024-09-25 230558" src="https://github.com/user-attachments/assets/a84f61af-de94-481f-bd50-9741389becf3">

b. Jalankan script tersebut sebagai berikut :

**$ ./p1.sh ; ./p3.sh ; ./p2.sh**

<img width="600" alt="Cuplikan layar 2024-09-25 230915" src="https://github.com/user-attachments/assets/ef602b8f-ff20-4155-9be7-98b256dbd421">

<img width="600" alt="Cuplikan layar 2024-09-25 230929" src="https://github.com/user-attachments/assets/a291a7ad-0e87-46f5-aaa7-a447d126a089">

<img width="600" alt="Cuplikan layar 2024-09-25 231104" src="https://github.com/user-attachments/assets/5960b060-6ba4-4f57-9d1d-f5e608b73dfa">

**$ ./p1.sh &**

<img width="600" alt="Cuplikan layar 2024-09-25 231202" src="https://github.com/user-attachments/assets/0e4a363d-0cef-4aac-a345-7f79ba90524d">

**$ ./p1.sh $ ./p2.sh & ./p3.sh &**

<img width="600" alt="Cuplikan layar 2024-09-25 231355" src="https://github.com/user-attachments/assets/58325625-fca9-4c55-a3fb-29c7dba91c78">

**$ ( ./p1.sh ; ./p3.sh ) &**

<img width="600" alt="Cuplikan layar 2024-09-25 231628" src="https://github.com/user-attachments/assets/87ea02a2-d0b0-43bf-9b16-0a5301c71182">

##**5. Jobs**

a. Buat shell-script yang melakukan loop dengan nama pwaktu.sh, setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil.

#!/bin/bash while [ true ]

do

date >> hasil

sleep 10

done

<img width="600" alt="Cuplikan layar 2024-09-25 231710" src="https://github.com/user-attachments/assets/d89a333c-edbe-4b92-a8fa-2b6a9162b90e">

<img width="600" alt="Cuplikan layar 2024-09-25 231820" src="https://github.com/user-attachments/assets/e3d8a107-af9a-43af-8195-04e6b0c585db">

b. Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background sebagai berikut :

$ jobs

$ find / -print > files 2>/dev/null &

$ jobs

<img width="600" alt="Cuplikan layar 2024-09-25 232032" src="https://github.com/user-attachments/assets/01abebf6-9246-4a57-83eb-6d6ef198ccd8">

c. Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background

$ fg %1

$ bg

<img width="600" alt="Cuplikan layar 2024-09-25 232122" src="https://github.com/user-attachments/assets/1469ed75-39f1-4a2b-a422-02a4850e9ba3">

d. Stop program background dengan utilitas kil

$ ps x

$ kill [Nomor PID]

<img width="600" alt="Cuplikan layar 2024-09-25 232402" src="https://github.com/user-attachments/assets/bf5577de-9921-4a96-b603-c34297313084">

##**6. History**

a. Ganti nilai HISTSIZE dari 1000 menjadi 20

$ HISTSIZE=20

$ h

<img width="600" alt="Cuplikan layar 2024-09-25 232633" src="https://github.com/user-attachments/assets/5348fd28-cc8c-4e68-b38e-fc10ef0be6ca">

b. Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir dilakukan

$ !-5

<img width="600" alt="Cuplikan layar 2024-09-25 232840" src="https://github.com/user-attachments/assets/4504a050-1e73-43e2-9ef9-41383760eac3">

c. Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer

$ !!

<img width="600" alt="Cuplikan layar 2024-09-25 232902" src="https://github.com/user-attachments/assets/20a45db5-8911-4db4-aa50-c656cb11a0f5">

d. Ulangi instruksi pada history bufer nomor 150

$ !150

<img width="600" alt="Cuplikan layar 2024-09-25 233240" src="https://github.com/user-attachments/assets/dbac7501-ff43-49ec-a657-480b047b5b59">

e. Ulangi instruksi dengan prefix “ls”

$ !ls

<img width="600" alt="Cuplikan layar 2024-09-25 233436" src="https://github.com/user-attachments/assets/c6327fdf-661a-4a3b-99ea-62faa9133d84">







