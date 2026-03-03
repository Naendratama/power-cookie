# power-cookie

![ss](https://github.com/Naendratama/power-cookie/blob/main/Screenshot%202026-03-03%20190004.png)

Category: Web Exploitation

Difficulty: Medium

Description: Can you get the flag?

Hint: Do you know how to modify cookies?



![ss](https://github.com/Naendratama/power-cookie/blob/main/Screenshot%202026-03-03%20190102.png)

Coba kita tekan continue as guest

![ss](https://github.com/Naendratama/power-cookie/blob/main/Screenshot%202026-03-03%20190122.png)

Bisa dilihat, mungkin ini ada kaitannya dengan cookie, ayo kita lihat menggunakan developer tool, dann ke bagiannn aplication laluu cookie

![ss](https://github.com/Naendratama/power-cookie/blob/main/Screenshot%202026-03-03%20190156.png)

Bisa dilihat terdapat "isAdmin" dengan value 0, coba kita ubah valuenya menjadi 1

![ss](https://github.com/Naendratama/power-cookie/blob/main/Screenshot%202026-03-03%20190210.png)

sudah diubah, tetapi masih tidak bisa

Ayo kita coba menggunakan burp suite, kita intercept requestnya lalu kirim ke repeater.

![ss](https://github.com/Naendratama/power-cookie/blob/main/Screenshot%202026-03-03%20190304.png)

Bisa dilihat, terdapat "isAdmin" dengan value 0, ayo kita ubah  menjadi valuenya menjadi 1, lalu kita send request

![ss](https://github.com/Naendratama/power-cookie/blob/main/Screenshot%202026-03-03%20190353.png)

And yapp, kita berhasil mendapatkan flagnya

Flag : picoCTF{gr4d3_A_c00k13_0d351e23}


